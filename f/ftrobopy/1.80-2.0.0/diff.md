# Comparing `tmp/ftrobopy-1.80.tar.gz` & `tmp/ftrobopy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ftrobopy-1.80.tar", last modified: Sat Jun 10 08:54:34 2017, max compression
+gzip compressed data, was "dist/ftrobopy-2.0.0.tar", last modified: Fri Jul  7 08:13:22 2023, max compression
```

## Comparing `ftrobopy-1.80.tar` & `ftrobopy-2.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxr-xr-x   0 stuehn     (501) staff       (20)        0 2017-06-10 08:54:34.000000 ftrobopy-1.80/
--rwxr-xr-x   0 stuehn     (501) staff       (20)   105621 2017-06-10 08:36:25.000000 ftrobopy-1.80/ftrobopy.py
--rw-r--r--   0 stuehn     (501) staff       (20)      343 2017-06-10 08:54:34.000000 ftrobopy-1.80/PKG-INFO
--rw-r--r--   0 stuehn     (501) staff       (20)      144 2017-06-10 08:33:16.000000 ftrobopy-1.80/README.txt
--rw-r--r--   0 stuehn     (501) staff       (20)      416 2017-06-10 08:50:24.000000 ftrobopy-1.80/setup.py
+drwxrwxr-x   0 stuehn    (1000) stuehn    (1000)        0 2023-07-07 08:13:22.000000 ftrobopy-2.0.0/
+-rw-rw-r--   0 stuehn    (1000) stuehn    (1000)      349 2023-07-07 08:13:22.000000 ftrobopy-2.0.0/PKG-INFO
+-rw-rw-r--   0 stuehn    (1000) stuehn    (1000)      422 2023-07-06 17:44:58.000000 ftrobopy-2.0.0/setup.py
+-rw-rw-r--   0 stuehn    (1000) stuehn    (1000)   143976 2023-07-06 17:39:09.000000 ftrobopy-2.0.0/ftrobopy.py
+-rw-rw-r--   0 stuehn    (1000) stuehn    (1000)      144 2023-07-06 17:39:09.000000 ftrobopy-2.0.0/README.txt
```

### Comparing `ftrobopy-1.80/ftrobopy.py` & `ftrobopy-2.0.0/ftrobopy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 """
-***********************************************************************
+**************************************************************************
 **ftrobopy** - Ansteuerung des fischertechnik TXT Controllers in Python
-***********************************************************************
-(c) 2015, 2016, 2017 by Torsten Stuehn
+**************************************************************************
+(c) 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023 by Torsten Stuehn
 """
 
 from __future__ import print_function
 from os import system
 import os
 import platform
 import sys
 import socket
 import threading
 import struct
 import time
-from math import sqrt
+from math import sqrt, log
+
+try:
+  import ftTA2py
+except:
+  pass
 
 __author__      = "Torsten Stuehn"
-__copyright__   = "Copyright 2015, 2016, 2017 by Torsten Stuehn"
+__copyright__   = "Copyright 2015 - 2023 by Torsten Stuehn"
 __credits__     = "fischertechnik GmbH"
 __license__     = "MIT License"
-__version__     = "1.8"
+__version__     = "2.0.0"
 __maintainer__  = "Torsten Stuehn"
 __email__       = "stuehn@mailbox.org"
-__status__      = "release"
-__date__        = "06/10/2017"
+__status__      = "stable"
+__date__        = "06/15/2023"
 
 try:
   xrange
 except NameError:
   xrange = range
 
 def version():
@@ -37,15 +42,15 @@
 
      :return: Versionsnummer (float)
 
      Anwendungsbeispiel:
 
      >>> print("ftrobopy Version ", ftrobopy.ftrobopy.version())
   """
-  return __version__
+  return __version__ + " " + __status__
 
 
 def default_error_handler(message, exception):
   print(message)
   return False
 
 def default_data_handler(ftTXT):
@@ -86,14 +91,17 @@
   # input configuration codes for TXT motor shield
   C_MOT_INPUT_DIGITAL_VOLTAGE  = 0
   C_MOT_INPUT_DIGITAL_5K       = 1
   C_MOT_INPUT_ANALOG_VOLTAGE   = 2
   C_MOT_INPUT_ANALOG_5K        = 3
   C_MOT_INPUT_ULTRASONIC       = 4
   
+  C_EXT_MASTER                 = 0 # use TXT master
+  C_EXT_SLAVE                  = 1 # use TXT slave extension
+  
   # sound commands and messages for spi communication to motor shield (only needed in direct mode)
   C_SND_CMD_STATUS             = 0x80
   C_SND_CMD_DATA               = 0x81
   C_SND_CMD_RESET              = 0x90
   C_SND_MSG_RX_CMD             = 0xBB  # return if in CMD mode
   C_SND_MSG_RX_DATA            = 0x55  # return if in DATA mode
   C_SND_MSG_RX_COMPLETE        = 0xAA  # return after all data has been transfered
@@ -104,15 +112,15 @@
   C_SND_STATE_IDLE             = 0x00
   C_SND_STATE_START            = 0x01
   C_SND_STATE_STOP             = 0x02
   C_SND_STATE_RUNNING          = 0x03
   C_SND_STATE_DATA             = 0x04
 
 
-  def __init__(self, host='127.0.0.1', port=65000, serport='/dev/ttyO2' , on_error=default_error_handler, on_data=default_data_handler, directmode=False):
+  def __init__(self, host='127.0.0.1', port=65000, serport='/dev/ttyO2' , on_error=default_error_handler, on_data=default_data_handler, directmode=False, use_extension=False, use_TransferAreaMode=False):
     """
       Initialisierung der ftTXT Klasse:
 
       * Alle Ausgaenge werden per default auf 1 (=Motor) gesetzt
       * Alle Eingaenge werden per default auf 1, 0 (=Taster, digital) gesetzt
       * Alle Zaehler werden auf 0 gesetzt
 
@@ -129,14 +137,23 @@
       
       :param serport: Serieller Port zur direkten Ansteuerung der Motorplatine des TXT
       :type serport: string
 
       :param on_error: Errorhandler fuer Fehler bei der Kommunikation mit dem Controller (optional)
       :type port: function(str, Exception) -> bool
 
+      :param directmode: Default: False. Direkte serielle Kommunikation zwischen TXT Linux-Platine und Motorplatine unter Umgehung der Socket-Schnittstelle (nur sinnvoll in der CFW im offline Modus)
+      :type boolean:
+
+      :param use_extension: Default: False. Erlaubt einen zweiten TXT-Kontroller am Extension Port.
+      :type boolean:
+
+      :param use_TransferAreaMode: Default False. Verwendet eine shared-Memory Methode (TransferAreaMode) zum Datenaustausch mit der Motorplatine (nur sinnvoll im Offline Modus)
+      :type boolean:
+
 
       :return: Leer
 
       Anwedungsbeispiel:
 
       >>> import ftrobopy
       >>> txt = ftrobopy.ftTXT('192.168.7.2', 65000)
@@ -145,23 +162,35 @@
     self._m_version            = 0
     self._host                 = host
     self._port                 = port
     self._ser_port             = serport
     self.handle_error          = on_error
     self.handle_data           = on_data
     self._directmode           = directmode
+    self._use_extension        = use_extension
+    self._use_TransferAreaMode = use_TransferAreaMode
     self._spi                  = None
     self._SoundFilesDir        = ''
     self._SoundFilesList       = []
     self._sound_state          = 0  # current state of sound-communication state-machine in 'direct'-mode
     self._sound_data           = [] # curent buffer for sound data (wav-file[44:])
     self._sound_data_idx       = 0
     self._sound_current_rep    = 0
     self._sound_current_volume = 100
-    if self._directmode:
+    self._TransferArea_isInitialized = False
+    if self._use_TransferAreaMode:
+      if (ftTA2py.initTA()) == 1:
+        self._TransferArea_isInitialized = True
+      else:
+        print("Error: Transfer Area could not be initialized! Please check if ftTA2py.so exists.")
+        sys.exit(-1)
+    elif self._directmode:
+      if use_extension:
+        print("Error: direct-mode does currently not support TXT slave extensions.")
+        sys.exit(-1)
       import serial
       self._ser_ms     = serial.Serial(self._ser_port, 230000, timeout=1)
       self._sock       = None
       import spidev
       try:
         self._spi      = spidev.SpiDev(1,0) # /dev/spidev1.0
       except error:
@@ -189,96 +218,136 @@
     else:
       self._sock=socket.socket()
       self._sock.settimeout(5)
       self._sock.connect((self._host, self._port))
       self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
       self._sock.setblocking(1)
       self._ser_ms            = None
+      self._i2c_sock=socket.socket()
+      self._i2c_sock.settimeout(5)
+
     self._txt_stop_event      = threading.Event()
     self._camera_stop_event   = threading.Event()
+    self._bt_joystick_stop_event = threading.Event()
     self._txt_stop_event.set()
     self._camera_stop_event.set()
+    self._bt_joystick_stop_event.set()
     self._exchange_data_lock  = threading.RLock()
     self._camera_data_lock    = threading.Lock()
+    self._bt_joystick_lock    = threading.RLock()
     self._socket_lock         = threading.Lock()
     self._txt_thread          = None
     self._camera_thread       = None
+    self._bt_joystick_thread  = None
     self._update_status       = 0
     self._update_timer        = time.time()
     self._cycle_count         = 0
     self._sound_timer         = self._update_timer
     self._sound_length        = 0
-    self._config_id           = 0
-    self._config_id_old       = 0
-    self._m_extension_id      = 0
+    self._config_id           = [0,0] # [0]:master [1]:slave
+    self._config_id_old       = 0 # only used in direct mode
+    self._TransferDataChanged = False
     self._ftX1_pgm_state_req  = 0
     self._ftX1_old_FtTransfer = 0
     self._ftX1_dummy          = b'\x00\x00'
-    self._ftX1_motor          = [1,1,1,1]
+    self._ftX1_motor          = [1,1,1,1,1,1,1,1]
     self._ftX1_uni            = [1,1,b'\x00\x00',
                                  1,1,b'\x00\x00',
                                  1,1,b'\x00\x00',
                                  1,1,b'\x00\x00',
                                  1,1,b'\x00\x00',
                                  1,1,b'\x00\x00',
                                  1,1,b'\x00\x00',
+                                 1,1,b'\x00\x00',
+                                 1,1,b'\x00\x00',
+                                 1,1,b'\x00\x00',
+                                 1,1,b'\x00\x00',
+                                 1,1,b'\x00\x00',
+                                 1,1,b'\x00\x00',
+                                 1,1,b'\x00\x00',
+                                 1,1,b'\x00\x00',
                                  1,1,b'\x00\x00']
     self._ftX1_cnt            = [1,b'\x00\x00\x00',
                                  1,b'\x00\x00\x00',
                                  1,b'\x00\x00\x00',
+                                 1,b'\x00\x00\x00',
+                                 1,b'\x00\x00\x00',
+                                 1,b'\x00\x00\x00',
+                                 1,b'\x00\x00\x00',
                                  1,b'\x00\x00\x00']
-    self._ftX1_motor_config   = [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0]
+    self._ftX1_motor_config   = [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0]
     self._exchange_data_lock.acquire()
-    self._pwm          = [0,0,0,0,0,0,0,0]
-    self._motor_sync   = [0,0,0,0]
-    self._motor_dist   = [0,0,0,0]
-    self._motor_cmd_id = [0,0,0,0]
-    self._counter      = [0,0,0,0]
-    self._sound        = 0
-    self._sound_index  = 0
-    self._sound_repeat = 0
-    self._current_input           = [0,0,0,0,0,0,0,0]
-    self._current_counter         = [0,0,0,0]
-    self._current_counter_value   = [0,0,0,0]
-    self._current_counter_cmd_id  = [0,0,0,0]
-    self._current_motor_cmd_id    = [0,0,0,0]
-    self._current_sound_cmd_id    = 0
-    self._current_ir              = range(26)
+    self._pwm          = [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0]
+    self._motor_sync   = [0,0,0,0,0,0,0,0]
+    self._motor_dist   = [0,0,0,0,0,0,0,0]
+    self._motor_cmd_id = [0,0,0,0,0,0,0,0]
+    self._counter      = [0,0,0,0,0,0,0,0]
+    self._sound        = [0,0]
+    self._sound_index  = [0,0]
+    self._sound_repeat = [0,0]
+    self._current_input           = [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0]
+    self._current_counter         = [0,0,0,0,0,0,0,0]
+    self._current_counter_value   = [0,0,0,0,0,0,0,0]
+    self._current_counter_cmd_id  = [0,0,0,0,0,0,0,0]
+    self._current_motor_cmd_id    = [0,0,0,0,0,0,0,0]
+    self._current_sound_cmd_id    = [0,0]
+    self._current_ir              = [0 for i in range(26)]
     self._ir_current_ljoy_left_right = [0,0,0,0,0] # -15 ... 15
     self._ir_current_ljoy_up_down    = [0,0,0,0,0] # -15 ... 15
     self._ir_current_rjoy_left_right = [0,0,0,0,0] # -15 ... 15
     self._ir_current_rjoy_up_down    = [0,0,0,0,0] # -15 ... 15
     self._ir_current_buttons         = [0,0,0,0,0] # 0:OFF 1:ON
     self._ir_current_dip_switch      = [0,0,0,0,0] # 0:all 1:0-0 2:1-0 3:0-1 4:1-1
+    self._bt_ljoy_left_right         = 0 # -32767 ... 32512
+    self._bt_ljoy_up_down            = 0 # -32767 ... 32512
+    self._bt_rjoy_left_right         = 0 # -32767 ... 32512
+    self._bt_rjoy_up_down            = 0 # -32767 ... 32512
+    #self._bt_buttons                 = 0 # the bluetooth remote has no detectable buttons
+    #self._bt_dip_switch              = 0 # and no dip switches; currently only one bt remote can be connected
     self._current_power           = 0 # voltage of battery or power supply
     self._current_temperature     = 0 # temperature of ARM CPU
     self._current_reference_power = 0
     self._current_extension_power = 0
     self._debug                   = []
+    self._firstUpdateConfig       = [True, True]
     self._exchange_data_lock.release() 
 
+  def stopTransferArea(self):
+    if self._TransferArea_isInitialized:
+      ftTA2py.stopTA()
+    
   def isOnline(self):
-    return (not self._txt_stop_event.isSet()) and (self._txt_thread is not None)
+    if self._use_TransferAreaMode:
+      return self._TransferArea_isInitialized
+    else:
+      return (not self._txt_stop_event.is_set()) and (self._txt_thread is not None)
   
   def cameraIsOnline(self):
-    return (not self._camera_stop_event.isSet()) and (self._camera_thread is not None)
-  
+    return (not self._camera_stop_event.is_set()) and (self._camera_thread is not None)
+
   def queryStatus(self):
     """
        Abfrage des Geraetenamens und der Firmware Versionsnummer des TXT
        Nach dem Umwandeln der Versionsnummer in einen Hexadezimalwert, kann
        die Version direkt abgelesen werden.
 
        :return: Geraetename (string), Versionsnummer (integer)
 
        Anwendungsbeispiel:
 
        >>> name, version = txt.queryStatus()
     """
-    if self._directmode:
+    if self._use_TransferAreaMode:
+      # TODO
+      # not sure how to detect version yet, just set standard value
+      self._m_devicename = 'TXT TransferAreaMode'
+      self._m_version    = 0x4060600
+      self._m_firmware   = 'firmware version not detected'
+      return self._m_devicename, self._m_version
+    elif self._directmode:
       # not sure how to detect version yet, just set standard value
       self._m_devicename = 'TXT direct'
       self._m_version    =  0x4010500
       self._m_firmware   = 'firmware version not detected'
       return self._m_devicename, self._m_version
     m_id         = 0xDC21219A
     m_resp_id    = 0xBAC9723E
@@ -300,14 +369,164 @@
     self._m_version    = m_version
     v1                 = int(hex(m_version)[2])
     v2                 = int(hex(m_version)[3:5])
     v3                 = int(hex(m_version)[5:7])
     self._m_firmware   = 'firmware version '+str(v1)+'.'+str(v2)+'.'+str(v3)
     return m_devicename, m_version
 
+  def i2c_read(self, dev, reg, reg_len=1, data_len=1, debug=False):
+    """
+      I2C lesen
+      
+      :param dev: Die I2C Geraeteadresse
+      :type dev: integer
+
+      :param reg: Das Register, das ausgelesen werden soll (Untergeraeteadresse)
+      :type reg: integer
+
+      :param reg_len: Die Laenge des Registers in Byte (default=1)
+      :type reg_len: integer
+
+      :param data_len: Die Laenge der Datenantwort (default=1)
+      :type data_len: integer
+
+      :return: Die Datenantwort des I2C Geraetes (string)
+
+      Anwendungsbeispiel:
+
+      >>> res=txt.i2c_read(0x18, 0x3f, data_len=6)
+      >>> x,y,z=struct.unpack('<hhh', res)                    
+      >>> print("Beschleunigung des BMX055 Kombisensors in x-, y- und z-Richtung = ", x >> 4 , y >> 4, z >> 4)
+    """
+    m_id         = 0xB9DB3B39
+    m_resp_id    = 0x87FD0D90
+    m_command    = 0x01
+    buf          = struct.pack('>IBIIHH', m_id, m_command, dev, reg_len, data_len, reg)
+    if debug:
+      print("i2c_read, sendbuffer: ", end='')
+      for k in buf: print(format(int(k), '02X'), end=' ')
+      print()
+    res          = self._i2c_sock.send(buf)
+    data         = self._i2c_sock.recv(512)
+    if debug:
+      print("i2c_read, receivebuffer: ", end='')
+      for k in data: print(format(int(k), '02X'), end=' ')
+      print()
+    fstr = '>IBIHB'
+    for k in range(data_len): fstr+='B'
+    response_id = 0
+    if len(data) == struct.calcsize(fstr):
+      response_id=struct.unpack(fstr, data)[0]
+    if response_id != m_resp_id:
+      self.handle_error('WARNING: ResponseID %s of I2C read command does not match' % hex(response_id), None)
+      return None
+    return data[-data_len:]
+
+  def i2c_write(self, dev, reg, value, debug=False):                                             
+    """
+      I2C schreiben
+      
+      :param dev: Die I2C Geraeteadresse
+      :type dev: integer
+
+      :param reg: Das Register, das beschrieben werden soll (Untergeraeteadresse)
+      :type reg: integer
+
+      :param value: Der in das Register zu schreibende Wert
+      :type value: integer (0-255)
+
+      :return: True (boolean) bei fehlerfreier Ausfuehrung, sonst "None"
+
+      Anwendungsbeispiel:
+
+      >>> # Settings for BMX055 acceleration
+      >>> txt.i2c_write(0x18, 0x3e, 0x80)                                           
+      >>> txt.i2c_write(0x18, 0x0f, 0x0c)                             
+      >>> txt.i2c_write(0x18, 0x10, 0x0f)                             
+    """
+    m_id         = 0xB9DB3B39                                                 
+    m_resp_id    = 0x87FD0D90                                                 
+    m_command    = 0x02                                                       
+    buf = struct.pack('>IBIIIB',m_id, m_command, dev, 0x02, reg, value)      
+    if debug:
+      print("i2c_write, sendbuffer: ", end='')
+      for k in buf: print(format(int(k), '02X'), end=' ')
+      print()
+    res          = self._i2c_sock.send(buf)
+    data         = self._i2c_sock.recv(512)
+    if debug:
+      print("i2c_write, receivebuffer: ", end='')
+      for k in data: print(format(int(k), '02X'), end=' ')
+      print()
+    fstr = '>III'
+    response_id = 0
+    if len(data) == struct.calcsize(fstr):
+      response_id =struct.unpack(fstr, data)[0]
+    if response_id != m_resp_id:
+      self.handle_error('WARNING: ResponseID %s of I2C write command does not match' % hex(response_id), None)
+      return None
+    return True
+
+  def i2c_write_bytes(self, dev, *argv):
+    m_id = 0xB9DB3B39
+    m_resp_id = 0x87FD0D90
+
+    m_lenth = 0
+    for i in argv:
+      m_lenth += 1
+    buf = struct.pack('>IBIIBBB', m_id, m_lenth, dev, m_lenth, 0x00, 0x00, 0x00)
+    for i in argv:
+      buf += struct.pack('B', i)
+
+    if debug:
+      print("i2c_write, sendbuffer: ", end='')
+      for k in buf: print(format(int(k), '02X'), end=' ')
+      print()
+    res = self._i2c_sock.send(buf)
+    data = self._i2c_sock.recv(512)
+
+    if debug:
+      print("i2c_write, receivebuffer: ", end='')
+      for k in data: print(format(int(k), '02X'), end=' ')
+      print()
+    fstr = '>III'
+    response_id = 0
+    if len(data) == struct.calcsize(fstr):
+      response_id = struct.unpack(fstr, data)[0]
+    if response_id != m_resp_id:
+      self.handle_error('WARNING: ResponseID %s of I2C write command does not match' % hex(response_id), None)
+      return None
+
+    return True
+
+  def i2c_write_buffer(self, dev, buffer, m_length,  debug = False):
+    m_id = 0xB9DB3B39
+    buf = struct.pack('>IBIIBBB', m_id, m_length, dev, m_length, 0x00, 0x00, 0x00) + buffer
+
+    if debug:
+      print("i2c_write, sendbuffer: ", end='')
+      for k in buf: print(format(int(k), '02X'), end=' ')
+      print()
+    res = self._i2c_sock.send(buf)
+    data = self._i2c_sock.recv(512)
+
+    if debug:
+      print("i2c_write, receivebuffer: ", end='')
+      for k in data: print(format(int(k), '02X'), end=' ')
+      print()
+    fstr = '>III'
+    response_id = 0
+    if len(data) == struct.calcsize(fstr):
+      response_id = struct.unpack(fstr, data)[0]
+    if response_id != 0x87FD0D90:
+      self.handle_error('WARNING: ResponseID %s of I2C write command does not match' % hex(response_id), None)
+      return None
+
+    return True
+
   def getDevicename(self):
     """
        Liefert den zuvor mit queryStatus() ausgelesenen Namen des TXT zurueck
 
        :return: Geraetename (string)
 
        Anwendungsbeispiel:
@@ -349,28 +568,30 @@
 
        :return: Leer
 
        Anwendungsbeispiel:
 
        >>> txt.startOnline()
     """
+    if self._TransferArea_isInitialized:
+      return
     if self._directmode == True:
-      if self._txt_stop_event.isSet():
+      if self._txt_stop_event.is_set():
         self._txt_stop_event.clear()
       if self._txt_thread is None:
         self._txt_thread = ftTXTexchange(txt=self, sleep_between_updates=update_interval, stop_event=self._txt_stop_event)
         self._txt_thread.setDaemon(True)
         self._txt_thread.start()
-        # keep_connection_thread is needed when using SyncDataBegin/End in interactive python mode
+        # keep_connection_thread is only needed when using SyncDataBegin/End in interactive python mode
         #self._txt_keep_connection_stop_event = threading.Event()
         #self._txt_keep_connection_thread = ftTXTKeepConnection(self, 1.0, self._txt_keep_connection_stop_event)
         #self._txt_keep_connection_thread.setDaemon(True)
         #self._txt_keep_connection_thread.start()
       return None
-    if self._txt_stop_event.isSet():
+    if self._txt_stop_event.is_set():
       self._txt_stop_event.clear()
     else:
       return
     if self._txt_thread is None:
       m_id       = 0x163FF61D
       m_resp_id  = 0xCA689F75
       buf        = struct.pack('<I64s', m_id,b'')
@@ -381,34 +602,44 @@
       fstr       = '<I'
       response_id = 0
       if len(data) == struct.calcsize(fstr):
         response_id, = struct.unpack(fstr, data)
       if response_id != m_resp_id:
         self.handle_error('WARNING: ResponseID %s of startOnline command does not match' % hex(response_id), None)
       else:
+        self.updateConfig(self.C_EXT_MASTER)
+        if self._use_extension:
+          self.updateConfig(self.C_EXT_SLAVE)
         self._txt_thread = ftTXTexchange(txt=self, sleep_between_updates=update_interval, stop_event=self._txt_stop_event)
         self._txt_thread.setDaemon(True)
         self._txt_thread.start()
         # keep_connection_thread is needed when using SyncDataBegin/End in interactive python mode
         self._txt_keep_connection_stop_event = threading.Event()
         self._txt_keep_connection_thread = ftTXTKeepConnection(self, 1.0, self._txt_keep_connection_stop_event)
         self._txt_keep_connection_thread.setDaemon(True)
         self._txt_keep_connection_thread.start()
+        time.sleep(0.1)
+        self._i2c_sock.connect((self._host, self._port+2))
+        self._i2c_sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        self._i2c_sock.setblocking(1)
     return None
 
   def stopOnline(self):
     """
        Beendet den Onlinebetrieb des TXT und beendet den Python-Thread der fuer den Datenaustausch mit dem TXT verantwortlich war.
 
        :return: Leer
 
        Anwendungsbeispiel:
 
        >>> txt.stopOnline()
     """
+    if self._TransferArea_isInitialized:
+      self.stopTransferArea()
+      return None
     if self._directmode:
       self._txt_stop_event.set()
       self._txt_thread = None
       if self._spi:
         self._spi.close()
       return None
     if not self.isOnline():
@@ -427,15 +658,15 @@
     if len(data) == struct.calcsize(fstr):
       response_id, = struct.unpack(fstr, data)
     if response_id != m_resp_id:
       self.handle_error('WARNING: ResponseID %s of stopOnline command does not match' % hex(response_id), None)
     self._txt_thread = None
     return None
 
-  def setConfig(self, M, I):
+  def setConfig(self, M, I, ext=C_EXT_MASTER):
     """
        Einstellung der Konfiguration der Ein- und Ausgaenge des TXT.
        Diese Funktion setzt nur die entsprechenden Werte in der ftTXT-Klasse.
        Zur Uebermittlung der Werte an den TXT wird die updateConfig-Methode verwendet.
 
        :param M: Konfiguration der 4 Motorausgaenge (0=einfacher Ausgang, 1=Motorausgang)
        :type M: int[4]
@@ -467,38 +698,38 @@
                 (txt.C_RESISTOR,   txt.C_ANALOG),
                 (txt.C_SWITCH,     txt.C_DIGITAL),
                 (txt.C_SWITCH,     txt.C_DIGITAL),
                 (txt.C_SWITCH,     txt.C_DIGITAL)]
        >>> txt.setConfig(M, I)
        >>> txt.updateConfig()
     """
-    self._config_id += 1
+    self._config_id[ext] += 1
     # Configuration of motors
     # 0=single output O1/O2
     # 1=motor output M1
     # self.ftX1_motor          = [M[0],M[1],M[2],M[3]]  # BOOL8[4]
-    self._ftX1_motor            = M
+    self._ftX1_motor[4*ext:4*ext+4] = M
     # Universal input mode, see enum InputMode:
     # MODE_U=0
     # MODE_R=1
     # MODE_R2=2
     # MODE_ULTRASONIC=3
     # MODE_INVALID=4
     # print("setConfig I=", I)
-    self._ftX1_uni           = [I[0][0],I[0][1],b'\x00\x00',
-                                I[1][0],I[1][1],b'\x00\x00',
-                                I[2][0],I[2][1],b'\x00\x00',
-                                I[3][0],I[3][1],b'\x00\x00',
-                                I[4][0],I[4][1],b'\x00\x00',
-                                I[5][0],I[5][1],b'\x00\x00',
-                                I[6][0],I[6][1],b'\x00\x00',
-                                I[7][0],I[7][1],b'\x00\x00'] 
+    self._ftX1_uni[24*ext:24*ext+24] = [I[0][0],I[0][1],b'\x00\x00',
+                                        I[1][0],I[1][1],b'\x00\x00',
+                                        I[2][0],I[2][1],b'\x00\x00',
+                                        I[3][0],I[3][1],b'\x00\x00',
+                                        I[4][0],I[4][1],b'\x00\x00',
+                                        I[5][0],I[5][1],b'\x00\x00',
+                                        I[6][0],I[6][1],b'\x00\x00',
+                                        I[7][0],I[7][1],b'\x00\x00']
     return None
 
-  def getConfig(self):
+  def getConfig(self, ext=C_EXT_MASTER):
     """
        Abfrage der aktuellen Konfiguration des TXT
 
        :return: M[4], I[8][2]
        :rtype: M:int[4], I:int[8][2]
 
        Anwendungsbeispiel: Aenderung des Eingangs I2 auf analoge Ultraschall Distanzmessung
@@ -507,47 +738,52 @@
        - Der Eingang I2 des TXT wird in diesem Beispiel ueber das Feldelement I[1] angesprochen
 
        >>> M, I = txt.getConfig()
        >>> I[1] = (txt.C_ULTRASONIC, txt.C_ANALOG)
        >>> txt.setConfig(M, I)
        >>> txt.updateConfig()
     """
-    m  = self._ftX1_motor
-    i  = self._ftX1_uni
+    m  = self._ftX1_motor[4*ext:4*ext+4]
+    i  = self._ftX1_uni[24*ext:24*ext+24]
     ii = [(i[0], i[1]), (i[3], i[4]),(i[6], i[7]),(i[9], i[10]),(i[12], i[13]),(i[15], i[16]),(i[18], i[19]),(i[21], i[22]) ]
     return m, ii 
 
-  def updateConfig(self):
+  def updateConfig(self, ext=C_EXT_MASTER):
     """
        Uebertragung der Konfigurationsdaten fuer die Ein- und Ausgaenge zum TXT
 
        :return: Leer
 
        Anwendungsbeispiel:
 
        >>> txt.setConfig(M, I)
        >>> txt.updateConfig()
     """
+    if self._use_TransferAreaMode:
+      # in TransferAreaMode the configuration is automatically updated
+      return
     if self._directmode:
       # in direct mode i/o port configuration is performed automatically in exchangeData thread
       return
-    if not self.isOnline():
-      self.handle_error("Controller must be online before updateConfig() is called", None)
-      return
+    if not self._firstUpdateConfig[ext]:
+      if not self.isOnline():
+        self.handle_error("Controller must be online before updateConfig() is called", None)
+        return
+      self._firstUpdateConfig[ext] = False
     m_id       = 0x060EF27E
     m_resp_id  = 0x9689A68C
-    self._config_id += 1
-    fields = [m_id, self._config_id, self._m_extension_id]
+    self._config_id[ext] += 1
+    fields = [m_id, self._config_id[ext], ext]
     fields.append(self._ftX1_pgm_state_req)
     fields.append(self._ftX1_old_FtTransfer)
     fields.append(self._ftX1_dummy)
-    fields += self._ftX1_motor
-    fields += self._ftX1_uni
-    fields += self._ftX1_cnt
-    fields += self._ftX1_motor_config
+    fields += self._ftX1_motor[4*ext:4*ext+4]
+    fields += self._ftX1_uni[24*ext:24*ext+24]
+    fields += self._ftX1_cnt[8*ext:8*ext+8]
+    fields += self._ftX1_motor_config[16*ext:16*ext+16]
     buf = struct.pack('<Ihh B B 2s BBBB BB2s BB2s BB2s BB2s BB2s BB2s BB2s BB2s B3s B3s B3s B3s 16h', *fields)
     self._socket_lock.acquire()
     res = self._sock.send(buf)
     data = self._sock.recv(512)
     self._socket_lock.release()
     fstr    = '<I'
     response_id = 0
@@ -556,45 +792,49 @@
     if response_id != m_resp_id:
       self.handle_error('WARNING: ResponseID %s of updateConfig command does not match' % hex(response_id), None)
       # Stop the data exchange thread and the keep connection thread if we were online
       self._txt_stop_event.set()
       self._txt_keep_connection_stop_event.set()
     return None
 
-  def startCameraOnline(self):
+  def startCameraOnline(self, width=320, height=240, fps=15):
     """
       Startet den Prozess auf dem TXT, der das aktuelle Camerabild ueber Port 65001 ausgibt und startet einen Python-Thread,
       der die Cameraframes kontinuierlich vom TXT abholt. Die Frames werden vom TXT im jpeg-Format angeliefert.
       Es wird nur das jeweils neueste Bild aufgehoben.
 
       Nach dem Starten des Cameraprozesses auf dem TXT vergehen bis zu 2 Sekunden, bis des erste Bild vom TXT gesendet wird.
 
+      *Anmerkung:* Falls diese Funktion im Offline-Modus auf dem TXT unter der CFW (Community Firmware Version >0.9) verwendet werden soll,
+      muss zuvor die ftGUI-App auf dem TXT gestartet werden. Im 'direct'-Modus stehen die Camera-Funktionen von ftrobopy nicht zur Verfuegung.
+      In diesem Fall sollte die openCV-Bibliothek oder ftrobopylib.so verwendet werden.
+
       Anwendungsbeispiel:
 
       Startet den Cameraprozess, wartet 2.5 Sekunden und speichert das eingelesene Bild als Datei 'txtimg.jpg' ab.
 
       >>> txt.startCameraOnline()
       >>> time.sleep(2.5)
       >>> pic = txt.getCameraFrame()
       >>> with open('txtimg.jpg','wb') as f:
       >>>   f.write(bytearray(pic))
     """
     if self._directmode:
       # ftrobopy.py does not support camera in direct mode, please use native camera support (e.g. ftrobopylib.so or opencv)
       return
-    if self._camera_stop_event.isSet():
+    if self._camera_stop_event.is_set():
       self._camera_stop_event.clear()
     else:
       return
     if self._camera_thread is None:
       m_id                  = 0x882A40A6
       m_resp_id             = 0xCF41B24E
-      self._m_width         = 320
-      self._m_height        = 240
-      self._m_framerate     = 15
+      self._m_width         = width
+      self._m_height        = height
+      self._m_framerate     = fps
       self._m_powerlinefreq = 0 # 0=auto, 1=50Hz, 2=60Hz
       buf        = struct.pack('<I4i', m_id,
                                      self._m_width,
                                      self._m_height,
                                      self._m_framerate,
                                      self._m_powerlinefreq)
       self._socket_lock.acquire()
@@ -644,14 +884,18 @@
     return
 
   def getCameraFrame(self):
     """
       Diese Funktion liefert das aktuelle Camerabild des TXT zurueck (im jpeg-Format).
       Der Camera-Prozess auf dem TXT muss dafuer vorher gestartet worden sein.
 
+      *Anmerkung:* Falls diese Funktion im Offline-Modus auf dem TXT unter der CFW (Community Firmware Version >0.9) verwendet werden soll,
+      muss zuvor die ftGUI-App auf dem TXT gestartet werden. Im 'direct'-Modus stehen die Camera-Funktionen von ftrobopy nicht zur Verfuegung.
+      In diesem Fall sollte die openCV-Bibliothek oder ftrobopylib.so verwendet werden.
+
       Anwendungsbeispiel:
 
       >>>   pic = txt.getCameraFrame()
 
       :return: jpeg Bild
     """
     if self._directmode:
@@ -661,23 +905,23 @@
       frame = None
       while frame == None:
         frame = self._camera_thread.getCameraFrame()
         count += 1
         if frame != None:
           if len(frame) == 0:
             frame = None
-        if count > 20:
+        if count > 100:
           print('Timeout while getting new frame from camera')
           return None
         time.sleep(0.01)
       return frame
     else:
       return None
 
-  def incrMotorCmdId(self, idx):
+  def incrMotorCmdId(self, idx, ext=C_EXT_MASTER):
     """
       Erhoehung der sog. Motor Command ID um 1.
 
       Diese Methode muss immer dann aufgerufen werden, wenn die Distanzeinstellung eines Motors (gemessen ueber die 4 schnellen Counter-Eingaenge)
       geaendert wurde oder wenn ein Motor mit einem anderen Motor synchronisiert werden soll. Falls nur die Motorgeschwindigkeit veraendert wurde,
       ist der Aufruf der incrMotorCmdId()-Methode nicht notwendig.
 
@@ -691,63 +935,73 @@
       Anwendungsbeispiel:
 
       Der Motor, der am TXT-Anschluss M2 angeschlossen ist, soll eine Distanz von 200 (Counterzaehlungen) zuruecklegen.
 
       >>> txt.setMotorDistance(1, 200)
       >>> txt.incrMotorCmdId(1)
     """
-    self._exchange_data_lock.acquire()
-    self._motor_cmd_id[idx] += 1
-    self._motor_cmd_id[idx] &= 0x07
-    self._exchange_data_lock.release()
+    if self._use_TransferAreaMode:
+      ftTA2py.fX1out_incr_motor_cmd_id(ext,idx)
+    else:
+      self._exchange_data_lock.acquire()
+      self._motor_cmd_id[4*ext+idx] += 1
+      self._motor_cmd_id[4*ext+idx] &= 0x07
+      self._exchange_data_lock.release()
+      self._TransferDataChanged = True
     return None
 
-  def getMotorCmdId(self, idx=None):
+  def getMotorCmdId(self, idx=None, ext=C_EXT_MASTER):
     """
       Liefert die letzte Motor Command ID eines Motorausgangs (oder aller Motorausgaenge als array) zurueck.
 
       :param idx: Nummer des Motorausgangs. Falls dieser Parameter nicht angeben wird, wird die Motor Command ID aller Motorausgaenge als Array[4] zurueckgeliefert.
       :type idx: integer
 
       :return: Die Motor Command ID eines oder aller Motorausgaenge
       :rtype: integer oder integer[4] array
 
       Anwendungsbeispiel:
 
       >>> letzte_cmd_id = txt.getMotorCmdId(4)
     """
-    if idx != None:
-      ret=self._motor_cmd_id[idx]
+    if self._use_TransferAreaMode:
+      if idx != None:
+        ret=ftTA2py.fX1in_motor_ex_cmd_id(ext,idx)
+      else:
+        ret=[ftTA2py.fX1in_motor_ex_cmd_id(ext,0), ftTA2py.fX1in_motor_ex_cmd_id(ext,1), ftTA2py.fX1in_motor_ex_cmd_id(ext,2), ftTA2py.fX1in_motor_ex_cmd_id(ext,3)]
     else:
-      ret=self._motor_cmd_id
+      if idx != None:
+        ret=self._motor_cmd_id[4*ext+idx]
+      else:
+        ret=self._motor_cmd_id[4*ext:4*ext+4]
     return ret
 
   def cameraOnline(self):
     """
       Mit diesem Befehl kann abgefragt werden, ob der Camera-Prozess gestartet wurde
 
       :return:
       :rtype: boolean
     """
     return self._camera_online
 
-  def getSoundCmdId(self):
+  def getSoundCmdId(self, ext=C_EXT_MASTER):
     """
       Liefert die letzte Sound Command ID zurueck.
 
       :return: Letzte Sound Command ID
       :rtype: integer
 
       Anwendungsbeispiel:
 
       >>> last_sound_cmd_id = txt.getSoundCmdId()
     """
-    return self._sound
+    return self._sound[ext]
 
-  def incrCounterCmdId(self, idx):
+  def incrCounterCmdId(self, idx, ext=C_EXT_MASTER):
     """
       Erhoehung der Counter Command ID um eins.
       Falls die Counter Command ID eines Counters um eins erhoeht wird, wird der entsprechende Counter zurueck auf 0 gesetzt.
 
       :param idx: Nummer des schnellen Countereingangs, dessen Command ID erhoeht werden soll. (Hinweis: die Zaehlung erfolgt hier von 0 bis 3 fuer die Counter C1 bis C4)
       :type idx: integer
 
@@ -755,40 +1009,45 @@
 
       Anwendungsbeispiel:
 
       Erhoehung der Counter Command ID des Counters C4 um eins.
 
       >>> txt.incrCounterCmdId(3)
     """
+    if self._use_TransferAreaMode:
+      # not used
+      return
     self._exchange_data_lock.acquire()
-    self._counter[idx] += 1
-    self._counter[idx] &= 0x07
+    self._counter[4*ext+idx] += 1
+    self._counter[4*ext+idx] &= 0x07
     self._exchange_data_lock.release()
+    self._TransferDataChanged = True
     return None
 
-  def incrSoundCmdId(self):
+  def incrSoundCmdId(self, ext=C_EXT_MASTER):
     """
       Erhoehung der Sound Command ID um eins.
       Die Sound Command ID muss immer dann um eins erhoeht werden, falls ein neuer Sound gespielt werden soll oder
       wenn die Wiederholungsanzahl eines Sounds veraendert wurde. Falls kein neuer Sound index gewaehlt wurde und auch
       die Wiederholungsrate nicht veraendert wurde, wird der aktuelle Sound erneut abgespielt.
 
       :return: Leer
 
       Anwendungsbeispiel:
 
       >>> txt.incrSoundCmdId()
     """
     self._exchange_data_lock.acquire()
-    self._sound += 1
-    self._sound &= 0x0F
+    self._sound[ext] += 1
+    self._sound[ext] &= 0x0F
     self._exchange_data_lock.release()
+    self._TransferDataChanged = True
     return None
 
-  def setSoundIndex(self, idx):
+  def setSoundIndex(self, idx, ext=C_EXT_MASTER):
     """
       Einstellen eines neuen Sounds.
 
       :param idx: Nummer des neuen Sounds (0=Kein Sound, 1-29 Sounds des TXT)
       :type idx: integer
 
       :return: Leer
@@ -798,15 +1057,15 @@
       Sound "Augenzwinkern" einstellen und 2 mal abspielen.
 
       >>> txt.setSoundIndex(26)
       >>> txt.setSoundRepeat(2)
       >>> txt.incrSoundCmdId()
     """
     self._exchange_data_lock.acquire()
-    self._sound_index = idx
+    self._sound_index[ext] = idx
     self._exchange_data_lock.release()
     if self._directmode and self._spi:
       self._exchange_data_lock.acquire()
       self._sound_data     = []
       self._sound_data_idx = 0
       self._exchange_data_lock.release()
       if idx > 0:
@@ -817,60 +1076,62 @@
           self._exchange_data_lock.acquire()
           self._sound_data     = list(bytearray(buf[44:]))
           filler = [0x80 for i in range(self.C_SND_FRAME_SIZE - (len(self._sound_data) % self.C_SND_FRAME_SIZE))]
           self._sound_data += filler
           self._sound_data_idx = 0
           self._exchange_data_lock.release()
           self._sound_current_volume = 100
+    self._TransferDataChanged = True
     return None
 
-  def getSoundIndex(self):
+  def getSoundIndex(self, ext=C_EXT_MASTER):
     """
       Liefert die Nummer des aktuell eingestellten Sounds zurueck.
 
       :return: Nummer des aktuell eingestellten Sounds
       :rtype: integer
 
       Anwendungsbeispiel:
 
       >>> aktueller_sound = txt.getSoundIndex()
     """
-    return self._sound_index
+    return self._sound_index[ext]
 
-  def setSoundRepeat(self, rep):
+  def setSoundRepeat(self, rep, ext=C_EXT_MASTER):
     """
       Einstellen der Anzahl der Wiederholungen eines Sounds.
 
       :param rep: Anzahl der Wiederholungen (0=unendlich oft wiederholen)
       :type rep: integer
 
       Anwendungsbeispiel:
 
       "Motor-Sound" unendlich oft (d.h. bis zum Ende des Programmes oder bis zur naechsten Aenderung der Anzahl der Wiederholungen) abspielen.
 
       >>> txt.setSound(19) # 19=Motor-Sound
       >>> txt.setSoundRepeat(0)
     """
     self._exchange_data_lock.acquire()
-    self._sound_repeat = rep
+    self._sound_repeat[ext] = rep
     self._exchange_data_lock.release()
+    self._TransferDataChanged = True
     return None
 
-  def getSoundRepeat(self):
+  def getSoundRepeat(self, ext=C_EXT_MASTER):
     """
       Liefert die aktuell eingestellte Wiederholungs-Anzahl des Sounds zurueck.
 
       :return: Aktuell eingestellte Wiederholungs-Anzahl des Sounds.
       :rtype: integer
 
       Anwendungsbeispiel:
 
       >>> repeat_rate = txt.getSoundRepeat()
     """
-    return self._sound_repeat
+    return self._sound_repeat[ext]
 
   def setSoundVolume(self, volume):
     """
       Setzt die Lautstaerke, mit der Sounds abgespielt werden.
 
       :param volume: 0=nicht hoehrbar bis 100=maximale Lautstaerke (Default=100).
       :type idx: integer
@@ -917,33 +1178,36 @@
     """
     if self._directmode:
       return self._sound_current_volume
     else:
       print("getSoundVolume() steht nur im 'direct'-Modus zur Verfuegung.")
       return None
 
-  def getCounterCmdId(self, idx=None):
+  def getCounterCmdId(self, idx=None, ext=C_EXT_MASTER):
     """
       Liefert die letzte Counter Command ID eines (schnellen) Counters zurueck
 
       :param idx: Nummer des Counters. (Hinweis: die Zaehlung erfolgt hier von 0 bis 3 fuer die Counter C1 bis C4)
 
       Anwendungsbeispiel:
 
       Counter Command ID des schnellen Counters C3 in Variable num einlesen.
 
       >>> num = txt.getCounterCmdId(2)
     """
+    if self._use_TransferAreaMode:
+      # not used
+      return
     if idx != None:
-      ret=self._counter[idx]
+      ret=self._counter[4*ext+idx]
     else:
-      ret=self._counter
+      ret=self._counter[4*ext:4*ext+4]
     return ret
 
-  def setPwm(self, idx, value):
+  def setPwm(self, idx, value, ext=C_EXT_MASTER):
     """
       Einstellen des Ausgangswertes fuer einen Motor- oder Output-Ausgang. Typischerweise wird diese Funktion nicht direkt aufgerufen,
       sondern von abgeleiteten Klassen zum setzen der Ausgangswerte verwendet.
       Ausnahme: mit Hilfe dieser Funktionen koennen Ausgaenge schnell auf 0 gesetzt werden um z.B. einen Notaus zu realisieren (siehe auch stopAll)
 
       :param idx: Nummer des Ausgangs. (Hinweis: die Zaehlung erfolgt hier von 0 bis 7 fuer die Ausgaenge O1-O8)
       :type idx: integer (0-7)
@@ -958,30 +1222,42 @@
       * Motor am Anschluss M1 soll mit voller Geschwindigkeit Rueckwaerts laufen.
       * Lampe am Anschluss O3 soll mit halber Leuchtkraft leuchten.
 
       >>> txt.setPwm(0,0)
       >>> txt.setPwm(1,512)
       >>> txt.setPwm(2,256)
     """
+    if value == 1:
+      value = 0
+    if self._use_TransferAreaMode:
+      ftTA2py.fX1out_duty(0, idx, value)
+      self._pwm[8*ext+idx]=value
+      return
     self._exchange_data_lock.acquire()
-    self._pwm[idx]=value
+    self._pwm[8*ext+idx]=value
     self._exchange_data_lock.release()
+    self._TransferDataChanged = True
     return None
 
   def stopAll(self):
     """
     Setzt alle Ausgaenge auf 0 und stoppt damit alle Motoren und schaltet alle Lampen aus.
 
     :return:
     """
-    for i in range(8):
+    if self._use_extension:
+      n=16
+    else:
+      n=8
+    for i in range(n):
       self.setPwm(i, 0)
+    self._TransferDataChanged = True
     return
 
-  def getPwm(self, idx=None):
+  def getPwm(self, idx=None, ext=C_EXT_MASTER):
     """
       Liefert die zuletzt eingestellten Werte der Ausgaenge O1-O8 (als array[8]) oder den Wert eines Ausgangs.
 
       :param idx:
       :type idx: integer oder None, bzw. leer
 
       - Wenn kein idx-Parameter angegeben wurde, werden alle Pwm-Einstellungen als array[8] zurueckgeliefert.
@@ -1001,20 +1277,20 @@
       >>> if M1_a > 0 and M1_b == 0:
             print("Geschwindigkeit Motor M1: ", M1_a, " (vorwaerts).")
           else:
             if M1_a == and M1_b > 0:
               print("Geschwindigkeit Motor M1: ", M1_b, " (rueckwaerts).")
     """
     if idx != None:
-      ret=self._pwm[idx]
+      ret=self._pwm[8*ext+idx]
     else:
-      ret=self._pwm
+      ret=self._pwm[8*ext:8*ext+8]
     return ret
 
-  def setMotorSyncMaster(self, idx, value):
+  def setMotorSyncMaster(self, idx, value, ext=C_EXT_MASTER):
     """
       Hiermit koennen zwei Motoren miteinander synchronisiert werden, z.B. fuer perfekten Geradeauslauf.
 
       :param idx: Der Motorausgang, der synchronisiert werden soll
       :type idx: integer
 
       :param value: Die Numer des Motorausgangs, mit dem synchronisiert werden soll.
@@ -1033,20 +1309,25 @@
       Um die Synchronisations-Befehle abzuschliessen, muss ausserdem die MotorCmdId der Motoren erhoeht werden.
 
       >>> txt.setMotorSyncMaster(0, 2)
       >>> txt.setMotorSyncMaster(1, 1)
       >>> txt.incrMotorCmdId(0)
       >>> txt.incrMotorCmdId(1)
     """
+    if self._use_TransferAreaMode:
+      ftTA2py.fX1out_master(ext, idx, value)
+      self._motor_sync[4*ext+idx]=value
+      return
     self._exchange_data_lock.acquire()
-    self._motor_sync[idx]=value
+    self._motor_sync[4*ext+idx]=value
     self._exchange_data_lock.release()
+    self._TransferDataChanged = True
     return None
 
-  def getMotorSyncMaster(self, idx=None):
+  def getMotorSyncMaster(self, idx=None, ext=C_EXT_MASTER):
     """
       Liefert die zuletzt eingestellte Konfiguration der Motorsynchronisation fuer einen oder alle Motoren zurueck.
 
       :param idx: Die Nummer des Motors, dessen Synchronisation geliefert werden soll oder None oder <leer> fuer alle Ausgaenge.
       :type idx: integer
 
       :return: Leer
@@ -1058,20 +1339,20 @@
 
       Anwendungsbeispiel:
 
       >>> xm = txt.getMotorSyncMaster()
       >>> print("Aktuelle Konfiguration aller Motorsynchronisationen: ", xm)
     """
     if idx != None:
-      ret=self._motor_sync[idx]
+      ret=self._motor_sync[4*ext+idx]
     else:
-      ret=self._motor_sync
+      ret=self._motor_sync[4*ext:ext+4]
     return ret
 
-  def setMotorDistance(self, idx, value):
+  def setMotorDistance(self, idx, value, ext=C_EXT_MASTER):
     """
       Hiermit kann die Distanz (als Anzahl von schnellen Counter-Zaehlungen) fuer einen Motor eingestellt werden.
 
       :param idx: Nummer des Motorausgangs
       :type idx: integer
 
       :return: Leer
@@ -1084,20 +1365,25 @@
 
       Der Motor an Ausgang M3 soll 100 Counter-Zaehlungen lang drehen.
       Um den Distanz-Befehl abzuschliessen, muss ausserdem die MotorCmdId des Motors erhoeht werden.
 
       >>> txt.setMotorDistance(2, 100)
       >>> txt.incrMotorCmdId(2)
     """
+    if self._use_TransferAreaMode:
+      ftTA2py.fX1out_distance(ext, idx, value)
+      self._motor_dist[4*ext+idx]=value
+      return
     self._exchange_data_lock.acquire()
-    self._motor_dist[idx]=value
+    self._motor_dist[4*ext+idx]=value
     self._exchange_data_lock.release()
+    self._TransferDataChanged = True
     return None
 
-  def getMotorDistance(self, idx=None):
+  def getMotorDistance(self, idx=None, ext=C_EXT_MASTER):
     """
       Liefert die zuletzt eingestellte Motordistanz fuer einen oder alle Motorausgaenge zurueck.
 
       :param idx: Nummer des Motorausgangs
       :type idx: integer
 
       :return: Letzte eingestellte Distanz eines Motors (idx=0-3) oder alle zuletzt eingestellten Distanzen (idx=None oder kein idx-Parameter angegeben)
@@ -1108,20 +1394,20 @@
 
       Anwendungsbeispiel:
 
       >>> md = txt.getMotorDistance(1)
       >>> print("Mit setMotorDistance() eingestellte Distanz fuer M2: ", md)
     """
     if idx != None:
-      ret=self._motor_dist[idx]
+      ret=self._motor_dist[4*ext+idx]
     else:
-      ret=self._motor_dist
+      ret=self._motor_dist[4*ext:4*ext+4]
     return ret
 
-  def getCurrentInput(self, idx=None):
+  def getCurrentInput(self, idx=None, ext=C_EXT_MASTER):
     """
        Liefert den aktuellen vom TXT zurueckgelieferten Wert eines Eingangs oder aller Eingaenge als Array
 
        :param idx: Nummer des Eingangs
        :type idx: integer
 
        :return: Aktueller Wert eines Eingangs (idx=0-7) oder alle aktuellen Eingangswerte des TXT-Controllers als Array[8] (idx=None oder kein idx angegeben)
@@ -1130,21 +1416,27 @@
 
        - der idx-Parameter wird angeben von 0 bis 7 fuer die Eingaenge I1 bis I8.
 
        Anwendungsbeispiel:
 
        >>> print("Der aktuelle Wert des Eingangs I4 ist: ", txt.getCurrentInput(3))
     """
-    if idx != None:
-      ret=self._current_input[idx]
+    if self._use_TransferAreaMode:
+      if idx != None:
+        ret = ftTA2py.fX1in_uni(ext, idx)
+      else:
+        ret = [ftTA2py.fX1in_uni(ext, 0), ftTA2py.fX1in_uni(ext, 1), ftTA2py.fX1in_uni(ext, 2), ftTA2py.fX1in_uni(ext, 3), ftTA2py.fX1in_uni(ext, 4), ftTA2py.fX1in_uni(ext, 5), ftTA2py.fX1in_uni(ext, 6), ftTA2py.fX1in_uni(ext, 7) ]
     else:
-      ret=self._current_input
+      if idx != None:
+        ret=self._current_input[8*ext+idx]
+      else:
+        ret=self._current_input[8*ext:8*ext+8]
     return ret
 
-  def getCurrentCounterInput(self, idx=None):
+  def getCurrentCounterInput(self, idx=None, ext=C_EXT_MASTER):
     """
       Zeigt an, ob ein Counter oder alle Counter (als Array[4]) sich seit der letzten Abfrage veraendert haben.
 
       :param idx: Nummer des Counters
       :type idx: integer
 
       :return: Aktueller Status-Wert eines Counters (idx=0-3) oder aller schnellen Counter des TXT-Controllers als Array[4] (idx=None oder kein idx angegeben)
@@ -1157,21 +1449,27 @@
 
       >>> c = txt.getCurrentCounterInput(0)
       >>> if c==0:
       >>>   print("Counter C1 hat sich seit der letzten Abfrage nicht veraendert")
       >>> else:
       >>>   print("Counter C1 hat sich seit der letzten Abfrage veraendert")
     """
-    if idx != None:
-      ret=self._current_counter[idx]
+    if self._use_TransferAreaMode:
+      if idx != None:
+        ret = ftTA2py.fX1in_cnt_in(ext, idx)
+      else:
+        ret = [ftTA2py.fX1in_cnt_in(ext, 0), ftTA2py.fX1in_cnt_in(ext, 1), ftTA2py.fX1in_cnt_in(ext, 2),ftTA2py.fX1in_cnt_in(ext, 3)]
     else:
-      ret=self._current_counter
+      if idx != None:
+        ret=self._current_counter[4*ext+idx]
+      else:
+        ret=self._current_counter[4*ext:4*ext+4]
     return ret
 
-  def getCurrentCounterValue(self, idx=None):
+  def getCurrentCounterValue(self, idx=None, ext=C_EXT_MASTER):
     """
       Liefert den aktuellen Wert eines oder aller schnellen Counter Eingaenge zurueck.
       Damit kann z.B. nachgeschaut werden, wie weit ein Motor schon gefahren ist.
 
       :param idx: Nummer des Counters
       :type idx: integer
 
@@ -1181,21 +1479,27 @@
 
       - der idx-Parameter wird angegeben von 0 bis 3 fuer die Counter C1 bis C4.
 
       Anwendungsbeispiel:
 
       >>> print("Aktueller Wert von C1: ", txt.getCurrentCounterValue(0)
     """
-    if idx != None:
-      ret=self._current_counter_value[idx]
+    if self._use_TransferAreaMode:
+      if idx != None:
+        ret = ftTA2py.fX1in_counter(ext, idx)
+      else:
+        ret = [ftTA2py.fX1in_counter(ext, 0), ftTA2py.fX1in_counter(ext, 1), ftTA2py.fX1in_counter(ext, 2),ftTA2py.fX1in_counter(ext, 3)]
     else:
-      ret=self._current_counter_value
+      if idx != None:
+        ret=self._current_counter_value[4*ext+idx]
+      else:
+        ret=self._current_counter_value[4*ext:4*ext+4]
     return ret
 
-  def getCurrentCounterCmdId(self, idx=None):
+  def getCurrentCounterCmdId(self, idx=None, ext=C_EXT_MASTER):
     """
       Liefert die aktuelle Counter Command ID eines oder aller Counter zurueck.
 
       :param idx: Nummer des Counters
       :type idx: integer
 
       :return: Aktuelle Commmand ID eines Counters (idx=0-3) oder aller Counter des TXT-Controllers als Array[4] (idx=None oder kein idx angegeben)
@@ -1205,21 +1509,27 @@
       - der idx-Parameter wird angeben von 0 bis 3 fuer die Counter C1 bis C4.
 
       Anwendungsbeispiel:
 
       >>> cid = txt.getCurrentCounterCmdId(3)
       >>> print("Aktuelle Counter Command ID von C4: ", cid)
     """
-    if idx != None:
-      ret=self._current_counter_cmd_id[idx]
+    if self._use_TransferAreaMode:
+      if idx != None:
+        ret = ftTA2py.fX1in_cnt_reset_cmd_id(ext, idx)
+      else:
+        ret = [ftTA2py.fX1in_cnt_reset_cmd_id(ext, 0), ftTA2py.fX1in_cnt_reset_cmd_id(ext, 1), ftTA2py.fX1in_cnt_reset_cmd_id(ext, 2),ftTA2py.fX1in_cnt_reset_cmd_id(ext, 3)]
     else:
-      ret=self._current_counter_cmd_id
+      if idx != None:
+        ret=self._current_counter_cmd_id[4*ext+idx]
+      else:
+        ret=self._current_counter_cmd_id[4*ext:4*ext+4]
     return ret
 
-  def getCurrentMotorCmdId(self, idx=None):
+  def getCurrentMotorCmdId(self, idx=None, ext=C_EXT_MASTER):
     """
       Liefert die aktuelle Motor Command ID eines oder aller Motoren zurueck.
 
       :param idx: Nummer des Motors
       :type idx: integer
 
       :return: Aktuelle Commmand ID eines Motors (idx=0-3) oder aller Motoren des TXT-Controllers als Array[4] (idx=None oder kein idx angegeben)
@@ -1228,32 +1538,38 @@
 
       - der idx-Parameter wird angeben von 0 bis 3 fuer die Motoren M1 bis M4.
 
       Anwendungsbeispiel:
 
       >>> print("Aktuelle Motor Command ID von M4: ", txt.getCurrentMotorCmdId(3))
     """
-    if idx != None:
-      ret=self._current_motor_cmd_id[idx]
+    if self._use_TransferAreaMode:
+      if idx != None:
+        ret = ftTA2py.fX1in_motor_ex_cmd_id(ext, idx)
+      else:
+        ret = [ftTA2py.fX1in_motor_ex_cmd_id(ext, 0), ftTA2py.fX1in_motor_ex_cmd_id(ext, 1), ftTA2py.fX1in_motor_ex_cmd_id(ext, 2),ftTA2py.fX1in_motor_ex_cmd_id(ext, 3)]
     else:
-      ret=self._current_motor_cmd_id
+      if idx != None:
+        ret=self._current_motor_cmd_id[4*ext+idx]
+      else:
+        ret=self._current_motor_cmd_id[4*ext:4*ext+4]
     return ret
 
-  def getCurrentSoundCmdId(self):
+  def getCurrentSoundCmdId(self, ext=C_EXT_MASTER):
     """
       Liefert die aktuelle Sound Command ID zurueck.
 
       :return: Die aktuelle Sound Command ID
       :rtype: integer
 
       Anwendungsbeispiel:
 
       >>> print("Die aktuelle Sound Command ID ist: ", txt.getCurrentSoundCmdId())
     """
-    ret=self._current_sound_cmd_id
+    ret=self._current_sound_cmd_id[ext]
     return ret
 
   def getCurrentIr(self):
     """
     Liefert eine Liste mit den aktuellen Werten der IR-Fernbedienung zurueck (keine direct-Mode Unterstuetzung).
     Diese Funktion ist obsolet und sollte nicht mehr verwendet werden.
     """
@@ -1274,45 +1590,49 @@
     """
     Liefert die den aktuellen Netzwerkport zum TXT zurueck (normalerweise 65000).
     :return: Netzwerkport
     :rtype: int
     """
     return self._port
   
-  def getPower(self):
+  def getPower(self, ext=C_EXT_MASTER):
     """
     Liefert die aktuelle Spannung der angeschlossenen Stromversorgung des TXT in mV (Netzteil- oder Batterie-Spannung).
     
     Diese Funktion steht nur im 'direct'-Modus zur Verfuegung.
     
     Anwendungsbeispiel:
     
     >>> Spannung = txt.getPower()
     >>> if Spannung < 7900:
     >>>   print("Warnung: die Batteriespannung des TXT ist schwach. Bitte die Batterie umgehend austauschen !")
     
     """
-    if self._directmode:
+    if self._use_TransferAreaMode:
+      return ftTA2py.TxtPowerSupply(ext)
+    elif self._directmode:
       return self._current_power
     else:
       print("Diese Funktion steht nur im 'direct'-Modus zur Verfuegung.")
       return None
 
-  def getTemperature(self):
+  def getTemperature(self, ext=C_EXT_MASTER):
     """
     Liefert die aktuelle Temperatur der CPU des TXT (Einheit: ?) zurueck.
     
     Diese Funktion steht nur im 'direct'-Modus zur Verfuegung.
     
     Anwendungsbeispiel:
     
     >>> Temperatur = txt.getTemperature()
     >>> print("Die Temperatur im innern des TXT betraegt: ", Temperatur, " (Einheit unbekannt)")
     
     """
+    if self._use_TransferAreaMode:
+      return ftTA2py.TxtCPUTemperature(ext)
     if self._directmode:
       return self._current_temperature
     else:
       print("Diese Funktion steht nur im 'direct'-Modus zur Verfuegung.")
       return None
 
   def getReferencePower(self):
@@ -1359,22 +1679,26 @@
 
       >>> SyncDataBegin()
       >>> motor1.setSpeed(512)
       >>> motor2.setSpeed(512)
       >>> lampe1.setLevel(512)
       >>> SyncDataEnd()
     """
+    if self._use_TransferAreaMode:
+      return
     self._exchange_data_lock.acquire()
 
   def SyncDataEnd(self):
     """
       Die Funktionen SyncDataBegin() und SyncDataEnd()  werden verwendet um eine ganze Gruppe von Befehlen gleichzeitig ausfuehren zu koennen.
 
       Anwendungsbeispiel siehe SyncDataBegin()
     """
+    if self._use_TransferAreaMode:
+      return
     self._exchange_data_lock.release()
 
   def updateWait(self, minimum_time=0.001):
     """
       Wartet so lange, bis der naechste Datenaustausch-Zyklus mit dem TXT erfolgreich abgeschlossen wurde.
       
       Anwendungsbeispiel:
@@ -1383,14 +1707,16 @@
       >>> motor1.setDistance(100)
       >>> while not motor1.finished():
       >>>   txt.updateWait()
       
       Ein einfaches "pass" anstelle des "updateWait()" wuerde zu einer deutlich hoeheren CPU-Last fuehren.
       
     """
+    if self._use_TransferAreaMode:
+      return
     self._exchange_data_lock.acquire()
     self._update_status = 0
     self._exchange_data_lock.release()
     while self._update_status == 0:
       time.sleep(minimum_time)
 
 class ftTXTKeepConnection(threading.Thread):
@@ -1432,44 +1758,250 @@
             print('ResponseID ', hex(response_id),'of keep connection queryStatus command does not match')
             self._txt_stop_event.set()
         time.sleep(1.0)
       except:
         return
     return
 
+class CRC32(object):
+  def __init__(self):
+    self.Reset()
+    self.m_table = [0 for i in range(256)]
+    for dividend in range(256):
+      #remainder = (dividend << 24) & 0xffffffff
+      remainder = dividend << 24
+      for bit in range(8,0,-1):
+        if remainder & 0x80000000:
+          remainder = (remainder << 1) ^ 0x04C11DB7
+        else:
+          remainder = (remainder << 1)
+        #remainder &= 0xffffffff
+      self.m_table[dividend] = remainder & 0xffffffff
+    return
+
+  def Reset(self):
+    self.m_crc = 0xffffffff
+    self.c = 0
+    return
+
+  def Add16bit(self, val):
+    self.c += 1
+    val &= 0xffff
+    data = (self.m_crc >> 24) ^ (val >> 8)
+    data &= 0xff
+    self.m_crc = (self.m_crc << 8) ^ self.m_table[data]
+    self.m_crc &= 0xffffffff
+    data = (self.m_crc >> 24) ^ (val & 0xff)
+    data &= 0xff
+    self.m_crc = ((self.m_crc << 8) & 0xffffffff) ^ self.m_table[data]
+    self.m_crc &= 0xffffffff
+    return
+
+class compBuffer(object):
+  def __init__(self):
+    self.m_crc = CRC32()
+    self.Reset()
+    return
+
+  def Reset(self):
+    self.Rewind()
+    self.m_compressed               = []
+    self.m_nochange_count           = 0
+    return
+
+  def Rewind(self):
+    self.m_bitbuffer                = 0
+    self.m_bitcount                 = 0
+    self.m_nochange_count           = 0
+    self.m_previous_word            = 0
+    self.m_crc.Reset()
+    return
+
+  def GetBits(self, count):
+    # byte      |2 2 2 2 2 2 2 2|1 1 1 1 1 1 1 1|
+    # fragment  |7 7|6 6|5 5|4 4 4 4|3 3|2 2|1 1|
+    while(self.m_bitcount<count):
+      cp = self.m_compressed[0]
+      if isinstance(cp, str):
+        self.m_bitbuffer |= ord(cp) << self.m_bitcount
+      else:
+        self.m_bitbuffer |= cp << self.m_bitcount
+      self.m_compressed = self.m_compressed[1:]
+      self.m_bitcount += 8
+    res = self.m_bitbuffer & (0xffffffff >> (32-count) )
+    self.m_bitbuffer >>= count
+    self.m_bitcount -= count
+    #print("m_bitcount=", self.m_bitcount, " m_bitbuffer=",format(self.m_bitbuffer, '016b'), " m_compressed=",' '.join(format(ord(x),'08b') for x in self.m_compressed))
+    return res
+
+  def GetWord(self):
+    word = 0
+    if self.m_nochange_count > 0:
+      self.m_nochange_count -= 1
+      word = self.m_previous_word
+    else:
+      head = self.GetBits(2)
+      if head == 0:
+        # 00 NoChange 1x16 bit
+        word = self.m_previous_word
+      elif head == 1:
+        # 01 00 NoChange 2x16 bit
+        # 01 01 NoChange 3x16 bit
+        # 01 10 NoChange 4x16 bit
+        # 01 11 xxxx NoChange 5..19x16 bit
+        # 01 11 1111 xxxxxxxx NoChange 20..274 x16 bit
+        # 01 11 1111 11111111 xxxxxxxx-xxxxxxxx NoChange 275... x16 bit
+        word = self.m_previous_word
+        count = self.GetBits(2)
+        if count<3:
+          self.m_nochange_count = count+2-1
+        else:
+          count = self.GetBits(4)
+          if count<15:
+            self.m_nochange_count = count+5-1
+          else:
+            count = self.GetBits(8)
+            if count<255:
+              self.m_nochange_count = count+20-1
+            else:
+              count = self.GetBits(16)
+              self.m_nochange_count = count+275-1
+      elif head == 2:
+        if self.m_previous_word > 0:
+          word = 0
+        else:
+          word = 1
+      elif head == 3:
+        word = self.GetBits(16)
+    self.m_previous_word=0
+    #self.m_crc.Add16bit(word)
+    return(word)
+  
+  def PushBits(self, count, bits):
+    self.m_bitbuffer |= (bits << self.m_bitcount)
+    self.m_bitbuffer &= 0xffffffff
+    self.m_bitcount += count
+    while (self.m_bitcount >=8):
+      self.m_bitcount -= 8
+      self.m_compressed.append(self.m_bitbuffer & 0xff)
+      self.m_bitbuffer >>= 8
+    #print("m_bitcount=", self.m_bitcount, " m_bitbuffer=",format(self.m_bitbuffer, '016b'), " m_compressed=",' '.join(format(ord(x),'08b') for x in self.m_compressed))
+    return
+  
+  def EncodeNoChangeCount(self):
+    # 00 NoChange 1x16 bit
+    # 01 00 NoChange 2x16 bit
+    # 01 01 NoChange 3x16 bit
+    # 01 10 NoChange 4x16 bit
+    # 01 11 xxxx NoChange 5..19x16 bit
+    # 01 11 1111 xxxxxxxx NoChange 20..274 x16 bit
+    # 01 11 1111 11111111 xxxxxxxx-xxxxxxxx NoChange 275... bit
+    while(self.m_nochange_count>0):
+      if (self.m_nochange_count==1):
+        self.PushBits(2,0)
+        break
+      elif (self.m_nochange_count<=4):
+        self.PushBits(2,1)
+        self.PushBits(2,self.m_nochange_count-2)
+        break
+      elif (self.m_nochange_count<=4+15):
+        self.PushBits(2,1)
+        self.PushBits(2,3)
+        self.PushBits(4,self.m_nochange_count-4-1)
+        break
+      elif (self.m_nochange_count<=4+15+255):
+        self.PushBits(2,1)
+        self.PushBits(2,3)
+        self.PushBits(4,15)
+        self.PushBits(8,self.m_nochange_count-4-15-1)
+        break
+      elif (self.m_nochange_count<=4+15+255+4096):
+        self.PushBits(2,1)
+        self.PushBits(2,3)
+        self.PushBits(4,15)
+        self.PushBits(8,255)
+        self.PushBits(16,self.m_nochange_count-4-15-255-1)
+        break
+      else:
+        self.PushBits(2,1)
+        self.PushBits(2,3)
+        self.PushBits(4,15)
+        self.PushBits(8,255)
+        self.PushBits(16,4095)
+        self.m_nochange_count += -4-15-255-4096
+    self.m_nochange_count = 0
+    return
+  
+  def AddWord(self, word, word_for_crc=None):
+    if word_for_crc==None:
+      self.m_crc.Add16bit(word)
+    else:
+      self.m_crc.Add16bit(word_for_crc)
+
+    if word == self.m_previous_word:
+      self.m_nochange_count += 1
+    else:
+      self.EncodeNoChangeCount()
+      if (word == 1 and self.m_previous_word == 0) or (word == 0 and self.m_previous_word != 0):
+        # 10 Toggle (0 to 1, everything else to 0)
+        self.PushBits(2,2)
+      else:
+        # 11 16 bit follow immediately
+        self.PushBits(2,3)
+        self.PushBits(16,word)
+    self.m_previous_word = 0
+
+  def Finish(self):
+    self.EncodeNoChangeCount()
+    if self.m_bitcount > 0:
+      self.PushBits(8-self.m_bitcount,0)
+
+  def GetCompBuffer(self):
+    return self.m_compressed
+
 class ftTXTexchange(threading.Thread):
   """
   Thread zum kontinuierlichen Datenaustausch zwischen TXT und einem Computer, bzw. zwischen 
   der TXT Linux Platine und der TXT Motorplatine (im Direktmodus).
   sleep_between_updates ist die Zeit, die zwischen zwei Datenaustauschprozessen gewartet wird.
   Der TXT kann im schnellsten Falle alle 10 ms Daten austauschen.
   Typischerweise wird diese Thread-Klasse vom Endanwender nicht direkt verwendet.
   """
   def __init__(self, txt, sleep_between_updates, stop_event):
     threading.Thread.__init__(self)
     self._txt                       = txt
     self._txt_sleep_between_updates = sleep_between_updates
     self._txt_stop_event            = stop_event
     self._txt_interval_timer        = time.time()
+    if (self._txt._use_extension):
+      self.compBuffer = compBuffer()
+    self._crc0 = 809550095
+    self._cmpbuf0 = [253,34] #'\xfd"' # chr(253),chr(34)
+    self._previous_uncbuf = [0 for i in range(54)]
+    self._previous_response = [0 for i in range(84)]
+    self._previous_crc = self._crc0
+    self._recv_crc0 = 0x628ebb05
+    self._recv_crc = self._recv_crc0
+    self._prev_recv_crc = self._recv_crc
     return
   
   def run(self):
     while not self._txt_stop_event.is_set():
       if self._txt._directmode :
         if (self._txt_sleep_between_updates > 0):
           time.sleep(self._txt_sleep_between_updates)
 
         self._txt._cycle_count += 1
         if self._txt._cycle_count > 15:
           self._txt._cycle_count = 0
 
         self._txt._exchange_data_lock.acquire()
 
-        if self._txt._config_id != self._txt._config_id_old:
-          self._txt._config_id_old = self._txt._config_id
+        if self._txt._config_id[0] != self._txt._config_id_old:
+          self._txt._config_id_old = self._txt._config_id[0]
           #
           # at first, transfer i/o config data from TXT to motor shield
           # (this is only necessary, if config data has been changed, e.g. the config_id number has been increased)
           #
           fields = []
           fmtstr = '<BBB BBBB H BBBBBB'
           #fmtstr = '<' # little endian
@@ -1621,17 +2153,17 @@
         #fmtstr  = '<'
         #fmtstr += 'B'    # [0]     command code
         #fmtstr += 'B'    # [1]     length of data block
         #fmtstr += 'B'    # [2]     cycle counter
         #fmtstr += 'B'    # [3]     bit pattern of connected txt extension modules, 0 = only master
         #fmtstr += 'B'    # [4]     digital input bits
         #fmtstr += 'BBBB' # [5:9]   analog inputs I1-I4 bits 0-7
-        #fmtstr += 'BBB'  # [9:12]  analog inputs I1-I4 bits 8-12 : 22111111 33332222 44444433
+        #fmtstr += 'BBB'  # [9:12]  analog inputs I1-I4 bits 8-13 : 22111111 33332222 44444433  |  44444433 33332222 22111111
         #fmtstr += 'BBBB' # [12:16] analog inputs I5-I8 bits 0-7
-        #fmtstr += 'BBB'  # [16:19] analog inputs I5-I8 bits 8-12 : 66555555 77776666 88888877
+        #fmtstr += 'BBB'  # [16:19] analog inputs I5-I8 bits 8-13 : 66555555 77776666 88888877  |  88888877 77776666 66555555
         #fmtstr += 'B'    # [19]    voltage power supply analog bits 0-7
         #fmtstr += 'B'    # [20]    temperature analog bits 0-7
         #fmtstr += 'B'    # [21]    pwr and temp bits 8-12: ttpp pppp
         #fmtstr += 'B'    # [22]    reference voltage analog bits 0-7
         #fmtstr += 'B'    # [23]    extension voltage VBUS analog bits 0-7
         #fmtstr += 'B'    # [24]    ref and ext analog bits 8-12 : eeee rrrr
         #fmtstr += 'B'    # [25]    bit pattern of fast counters (bit0=C1 .. bit3=C2, bit4-7 not used)
@@ -1670,25 +2202,25 @@
               self._txt._current_input[k] = 1
             else:
               self._txt._current_input[k] = 0
           else:
             if k == 0:
               self._txt._current_input[k] = response[5]  + 256 * (response[9] & 0x3F)
             elif k == 1:
-              self._txt._current_input[k] = response[6]  + 256 * (((response[9]  >> 6) & 0x03) + (response[10] << 2) & 0x3C)
+              self._txt._current_input[k] = response[6]  + 256 * (((response[9]  >> 6) & 0x03) + ((response[10] << 2) & 0x3C))
             elif k == 2:
-              self._txt._current_input[k] = response[7]  + 256 * (((response[10] >> 4) & 0x0F) + (response[11] << 4) & 0x30)
+              self._txt._current_input[k] = response[7]  + 256 * (((response[10] >> 4) & 0x0F) + ((response[11] << 4) & 0x30))
             elif k == 3:
               self._txt._current_input[k] = response[8]  + 256 * ((response[11]  >> 2) & 0x3F)
             elif k == 4:
               self._txt._current_input[k] = response[12] + 256 * (response[16] & 0x3F)
             elif k == 5:
-              self._txt._current_input[k] = response[13] + 256 * (((response[16] >> 6) & 0x03) + (response[17] << 2) & 0x3C)
+              self._txt._current_input[k] = response[13] + 256 * (((response[16] >> 6) & 0x03) + ((response[17] << 2) & 0x3C))
             elif k == 6:
-              self._txt._current_input[k] = response[14] + 256 * (((response[17] >> 4) & 0x0F) + (response[18] << 4) & 0x30)
+              self._txt._current_input[k] = response[14] + 256 * (((response[17] >> 4) & 0x0F) + ((response[18] << 4) & 0x30))
             elif k == 7:
               self._txt._current_input[k] = response[15] + 256 * ((response[18]  >> 2) & 0x3F)
         
         # power (of battery and/or main power supply) in volt and internal TXT temperature
         #
         self._txt._current_power       = response[19] + 256 * (response[21] & 0x3F )
         self._txt._current_temperature = response[20] + 256 * ((response[21] >> 6 ) & 0x03)
@@ -1794,63 +2326,192 @@
                   self._txt._sound_current_rep += 1
                   if self._txt._sound_current_rep < self._txt.getSoundRepeat():
                     self._txt._sound_data_idx = 0
                   else:
                     res=self._txt._spi.xfer([self._txt.C_SND_CMD_STATUS, self._txt.getSoundCmdId(), 0])
                     nFreeBuffers = res[1]
                     self._txt._sound_state = self._txt.C_SND_STATE_IDLE
-                    self._txt._current_sound_cmd_id = self._txt.getSoundCmdId()
+                    self._txt._current_sound_cmd_id[0] = self._txt.getSoundCmdId()
                     break
       else:
        try:
         if (self._txt_sleep_between_updates > 0):
           time.sleep(self._txt_sleep_between_updates)
-        exchange_ok = False
-        m_id          = 0xCC3597BA
-        m_resp_id     = 0x4EEFAC41
-        self._txt._exchange_data_lock.acquire()
-        fields  = [m_id]
-        fields += self._txt._pwm
-        fields += self._txt._motor_sync
-        fields += self._txt._motor_dist
-        fields += self._txt._motor_cmd_id
-        fields += self._txt._counter
-        fields += [self._txt._sound, self._txt._sound_index, self._txt._sound_repeat,0,0]
-        self._txt._exchange_data_lock.release()
-        buf = struct.pack('<I8h4h4h4h4hHHHbb', *fields)
-        self._txt._socket_lock.acquire()
-        res = self._txt._sock.send(buf)
-        data = self._txt._sock.recv(512)
-        self._txt._update_timer = time.time()
-        self._txt._socket_lock.release()
-        fstr    = '<I8h4h4h4h4hH4bB4bB4bB4bB4bBb'
-        response_id = 0
-        if len(data) == struct.calcsize(fstr):
-          response = struct.unpack(fstr, data)
+
+        if self._txt._use_extension:
+          #start_time=time.time()
+          m_id          = 0xFBC56F98
+          m_resp_id     = 0x6F3B54E6
+          m_extrasize   = 0
+          self._txt._exchange_data_lock.acquire()
+          fields  = [m_id] # commad id
+          fields += [m_extrasize] # will be calculated below
+          fields += [0]      # CRC, set below
+          fields += [1]      # number of active extensions
+          fields += [0]      # 16 bit dummy align
+          fstr = '<IIIHH'
+          self._txt._exchange_data_lock.release()
+          if self._txt._TransferDataChanged:
+            uncbuf = []
+            # add MASTER fields
+            self._txt._exchange_data_lock.acquire()
+            uncbuf += self._txt._pwm[:8]
+            uncbuf += self._txt._motor_sync[:4]
+            uncbuf += self._txt._motor_dist[:4]
+            uncbuf += self._txt._motor_cmd_id[:4]
+            uncbuf += self._txt._counter[:4]
+            uncbuf += [self._txt._sound[0], self._txt._sound_index[0], self._txt._sound_repeat[0]]
+            # add SLAVE flieds
+            uncbuf += self._txt._pwm[8:]
+            uncbuf += self._txt._motor_sync[4:]
+            uncbuf += self._txt._motor_dist[4:]
+            uncbuf += self._txt._motor_cmd_id[4:]
+            uncbuf += self._txt._counter[4:]
+            # for now use same sound as for MASTER
+            uncbuf += [self._txt._sound[1], self._txt._sound_index[1], self._txt._sound_repeat[1]]
+            self._txt._exchange_data_lock.release()
+            #print(uncbuf)
+            # compress buffer
+            self.compBuffer.Reset()
+            for i in range(len(uncbuf)):
+              if uncbuf[i] == self._previous_uncbuf[i]:
+                self.compBuffer.AddWord(0, word_for_crc=uncbuf[i])
+              else:
+                if uncbuf[i] == 0:
+                  self.compBuffer.AddWord(1, word_for_crc=0)
+                else:
+                  self.compBuffer.AddWord(uncbuf[i])
+            self.compBuffer.Finish()
+            self._previous_uncbuf = uncbuf[:]
+            crc = self.compBuffer.m_crc.m_crc & 0xffffffff
+            cmpbuf = self.compBuffer.m_compressed
+            self._txt._TransferDataChanged = False
+            self._previous_crc = crc
+          else:
+            crc = self._previous_crc
+            cmpbuf = self._cmpbuf0
+          
+          m_extrasize = len(cmpbuf)
+          fields += cmpbuf
+          fstr   += str(m_extrasize)+'B'
+          #fields += [0] # dummy byte UINT8
+          #fstr   += 'B'
+          fields[1] = m_extrasize
+          fields[2] = crc
+          #print("fields=", fields)
+          #print("crc=",hex(crc)," : ", format((crc >>24) & 255, '3d'), format((crc >>16) & 255, '3d'), format((crc >>8) & 255, '3d'), format(crc & 255, '3d'), "  cmpbuf=", ' '.join(format(x,'3d') for x in cmpbuf) )
+
+          buf = struct.pack(fstr, *fields)
+          #print("buf=",' '.join(format(x, '02x') for x in buf))
+          self._txt._socket_lock.acquire()
+          res = self._txt._sock.send(buf)
+          
+          retbuf = self._txt._sock.recv(512)
+          self._txt._update_timer = time.time()
+          self._txt._socket_lock.release()
+
+          if len(retbuf) == 0:
+            print('ERROR: no data received in ftTXTexchange thread during exchange data compressed, possibly due to network error or CRC failure')
+            print('Connection to TXT aborted')
+            self._txt_stop_event.set()
+            return
+          #print("retbuf=",','.join(format(ord(x),'4d') for x in retbuf))
+          # head of response is uncompressed
+          self._prev_recv_crc = self._recv_crc # save previous checksum 
+          resphead       = struct.unpack('<IIIHH', retbuf[:16])
+          response_id    = resphead[0]
+          extra_size     = resphead[1] # size of compressed data
+          self._recv_crc = resphead[2] # CRC32 checksum of compressed data
+          nr_ext         = resphead[3] # number of active extensions
+          #dmy_align      = resphead[4] # dummy align
+          if response_id != m_resp_id:
+            print('ResponseID ', hex(response_id),' of exchangeData command in exchange thread does not match')
+            print('Connection to TXT aborted')
+            self._txt_stop_event.set()
+            return
+          #response=[response_id]
+          if self._prev_recv_crc != self._recv_crc:
+            # uncompress body of response
+            self.compBuffer.Reset()
+            self.compBuffer.m_compressed=retbuf[16:]
+            response = list(map(lambda x: self.compBuffer.GetWord(), range(77)))
+            #print(self._recv_crc, response)
+            self._txt._exchange_data_lock.acquire()
+
+            def conv_null(a,b):
+              return [a[i] if b[i]==0 else 0 if (b[i]==1 and a[i]==1) else 1 if (b[i]==1 and a[i]==0) else b[i] for i in range(len(b))]
+
+
+            # MASTER
+            self._txt._current_input[:8]          = conv_null(self._txt._current_input[:8], response[:8])
+            self._txt._current_counter[:4]        = conv_null(self._txt._current_counter[:4], response[8:12])
+            self._txt._current_counter_value[:4]  = conv_null(self._txt._current_counter_value[:4], response[12:16])
+            self._txt._current_counter_cmd_id[:4] = conv_null(self._txt._current_counter_cmd_id[:4], response[16:20])
+            self._txt._current_motor_cmd_id[:4]   = conv_null(self._txt._current_motor_cmd_id[:4], response[20:24])
+            self._txt._current_sound_cmd_id[0]    = conv_null([self._txt._current_sound_cmd_id[0]], [response[24]])[0]
+            #self._txt._current_ir[:26]            = conv_null(self._txt._current_ir[:26], response[25:52])
+            # EXTENSION
+            self._txt._current_input[8:]          = conv_null(self._txt._current_input[8:], response[52:60])
+            self._txt._current_counter[4:]        = conv_null(self._txt._current_counter[4:], response[60:64])
+            self._txt._current_counter_value[4:]  = conv_null(self._txt._current_counter_value[4:], response[64:68])
+            self._txt._current_counter_cmd_id[4:] = conv_null(self._txt._current_counter_cmd_id[4:], response[68:72])
+            self._txt._current_motor_cmd_id[4:]   = conv_null(self._txt._current_motor_cmd_id[4:], response[72:76])
+            #self._txt._current_sound_cmd_id[1]    = conv_null([self._txt._current_sound_cmd_id[1]], [response[76]])
+            # last 3 are not used
+            #dummy                             = response[77:80]
+
+            self._txt.handle_data(self._txt)
+            self._txt._exchange_data_lock.release()
+            #end_time=time.time()
+            #print("time=",end_time-start_time)
+          
         else:
-          print('Received data size (', len(data),') does not match length of format string (',struct.calcsize(fstr),')')
-          print('Connection to TXT aborted')
-          self._txt_stop_event.set()
-          return
-        response_id = response[0]
-        if response_id != m_resp_id:
-          print('ResponseID ', hex(response_id),' of exchangeData command in exchange thread does not match')
-          print('Connection to TXT aborted')
-          self._txt_stop_event.set()
-          return
-        self._txt._exchange_data_lock.acquire()
-        self._txt._current_input          = response[1:9]
-        self._txt._current_counter        = response[9:13]
-        self._txt._current_counter_value  = response[13:17]
-        self._txt._current_counter_cmd_id = response[17:21]
-        self._txt._current_motor_cmd_id   = response[21:25]
-        self._txt._current_sound_cmd_id   = response[25]
-        self._txt._current_ir             = response[26:52]
-        self._txt.handle_data(self._txt)
-        self._txt._exchange_data_lock.release()
+          m_id          = 0xCC3597BA
+          m_resp_id     = 0x4EEFAC41
+          self._txt._exchange_data_lock.acquire()
+          fields  = [m_id]
+          fields += self._txt._pwm[:8]
+          fields += self._txt._motor_sync[:4]
+          fields += self._txt._motor_dist[:4]
+          fields += self._txt._motor_cmd_id[:4]
+          fields += self._txt._counter[:4]
+          fields += [self._txt._sound[0], self._txt._sound_index[0], self._txt._sound_repeat[0],0,0]
+          self._txt._exchange_data_lock.release()
+          buf = struct.pack('<I8h4h4h4h4hHHHbb', *fields)
+          self._txt._socket_lock.acquire()
+          res = self._txt._sock.send(buf)
+          data = self._txt._sock.recv(512)
+          self._txt._update_timer = time.time()
+          self._txt._socket_lock.release()
+          fstr    = '<I8h4h4h4h4hH4bB4bB4bB4bB4bBb'
+          response_id = 0
+          if len(data) == struct.calcsize(fstr):
+            response = struct.unpack(fstr, data)
+          else:
+            print('Received data size (', len(data),') does not match length of format string (',struct.calcsize(fstr),')')
+            print('Connection to TXT aborted')
+            self._txt_stop_event.set()
+            return
+          response_id = response[0]
+          if response_id != m_resp_id:
+            print('ResponseID ', hex(response_id),' of exchangeData command in exchange thread does not match')
+            print('Connection to TXT aborted')
+            self._txt_stop_event.set()
+            return
+          self._txt._exchange_data_lock.acquire()
+          self._txt._current_input[:8]          = response[1:9]
+          self._txt._current_counter[:4]        = response[9:13]
+          self._txt._current_counter_value[:4]  = response[13:17]
+          self._txt._current_counter_cmd_id[:4] = response[17:21]
+          self._txt._current_motor_cmd_id[:4]   = response[21:25]
+          self._txt._current_sound_cmd_id[0]    = response[25]
+          self._txt._current_ir                 = response[26:52]
+          self._txt.handle_data(self._txt)
+          self._txt._exchange_data_lock.release()
+      
        except Exception as err:
         self._txt_stop_event.set()
         print('Network error ',err)
         self._txt.handle_error('Network error', err)
         return
        self._txt._exchange_data_lock.acquire()
        self._txt._update_status = 1
@@ -1971,40 +2632,76 @@
     """
     self._camera_data_lock.acquire()
     data = self._m_framedata
     self._m_framedata = []
     self._camera_data_lock.release()
     return data
 
+class BTJoystickEval(threading.Thread):
+  """
+  Thread zur kontinuierlichen Abfrage einer fischertech Bluetooth Fernbedienung
+  sleep_between_updates ist die Zeit, die zwischen zwei Abfragen gewartet wird.
+  Typischerweise wird diese Thread-Klasse vom Endanwender nicht direkt verwendet.
+  """
+  def __init__(self, txt, sleep_between_updates, stop_event, jsdev):
+    threading.Thread.__init__(self)
+    self._txt                               = txt
+    self._bt_joystick_sleep_between_updates = sleep_between_updates
+    self._bt_joystick_stop_event            = stop_event
+    self._bt_joystick_interval_timer        = time.time()
+    self._jsdev                             = jsdev
+    return
+  
+  def run(self):
+    while not self._bt_joystick_stop_event.is_set():
+      if (self._bt_joystick_sleep_between_updates > 0):
+        time.sleep(self._bt_joystick_sleep_between_updates)
+      self._txt._bt_joystick_lock.acquire()
+      if self._jsdev:
+        buf = self._jsdev.read(8)
+        if buf:
+          t, v, evt, n = struct.unpack('IhBB', buf)
+          if evt & 0x02:
+            #print("axe ", n, " value=", v)
+            if n == 0:
+              self._txt._bt_ljoy_left_right = v
+            elif n == 1:
+              self._txt._bt_ljoy_up_down = v
+            elif n == 2:
+              self._txt._bt_rjoy_left_right = v
+            elif n == 3:
+              self._txt._bt_rjoy_up_down = v
+      self._txt._bt_joystick_lock.release()
+
 class ftrobopy(ftTXT):
   """
     Erweiterung der Klasse ftrobopy.ftTXT. In dieser Klasse werden verschiedene fischertechnik Elemente
     auf einer hoeheren Abstraktionsstufe (aehnlich den Programmelementen aus der ROBOPro Software) fuer den End-User zur Verfuegung gestellt.
     Derzeit sind die folgenden Programmelemente implementiert:
     
     * **motor**, zur Ansteuerung der Motorausgaenge M1-M4
     * **output**, zur Ansteuerung der universellen Ausgaenge O1-O8
     * **input**, zum Einlesen von Werten der Eingaenge I1-I8
     * **resistor**, zum Messen eines Ohm'schen Widerstaenden
     * **ultrasonic**, zur Bestimmung von Distanzen mit Hilfe des Ultraschall Moduls
     * **voltage**, zum Messen einer Spannung
     * **colorsensor**, zur Abfrage des fischertechnik Farbsensors
     * **trailfollower**, zur Abfrage des fischertechnik Spursensors
-    * **joystick**, zur Abfrage eines Joysticks einer fischertechnik IR-Fernbedienung
+    * **joystick**, zur Abfrage eines Joysticks einer fischertechnik IR-Fernbedienung (BT-Fernbedienung nur mit cfw > 0.9.4 moeglich)
     * **joybutton**, zur Abfrage eines Buttons einer fischertechnik IR-Fernbedienung
     * **joydipswitch**, zur Abfrage der DIP-Schalter-Einstellung einer IR-Fernbedienung
 
     Ausserdem werden die folgenden Sound-Routinen zur Verfuegung gestellt:
     
     * **play_sound**
     * **stop_sound**
     * **sound_finished**
     
   """
-  def __init__(self, host='127.0.0.1', port=65000, update_interval=0.01, special_connection='127.0.0.1'):
+  def __init__(self, host='127.0.0.1', port=65000, update_interval=0.01, special_connection='127.0.0.1', use_extension=False, use_TransferAreaMode=False):
 
     """
       Initialisierung der ftrobopy Klasse:
       
       * Aufbau der Socket-Verbindung zum TXT Controller mit Hilfe der Basisklasse ftTXT und Abfrage des Geraetenamens und der Firmwareversionsnummer
       * Initialisierung aller Datenfelder der ftTXT Klasse mit Defaultwerten und Setzen aller Ausgaenge des TXT auf 0
       * Starten eines Python-Hintergrundthreads der die Kommunikation mit dem TXT aufrechterhaelt
@@ -2024,14 +2721,22 @@
 
       :param update_interval: Zeit (in Sekunden) zwischen zwei Aufrufen des Datenaustausch-Prozesses mit dem TXT
       :type update_intervall: float
 
       :param special_connection: IP-Adresse des TXT, falls dieser ueber einen Router im WLAN-Netz angesprochen wird (z.B. '10.0.2.7')
       :type special_connection: string
 
+      :param use_extension: Default: False. Erlaubt einen zweiten TXT-Kontroller am Extension Port.
+      :type boolean:
+
+      :param use_TransferAreaMode: Default False. Verwendet eine shared-Memory Methode (TransferAreaMode) zum Datenaustausch mit der Motorplatine (nur sinnvoll im Offline Modus)
+      :type boolean:
+
+
+
       :return: Leer
       
       Anwedungsbeispiel:
       
       >>> import ftrobopy
       >>> ftrob = ftrobopy.ftrobopy('auto')
     """
@@ -2080,15 +2785,14 @@
           elif probe_socket('192.168.9.2'): # Blutooth
             host = '192.168.9.2'
           elif probe_socket(special_connection):  # non standard port, e.g. home network
             host = special_connection
           else:
             print("Error: could not auto detect TXT connection. Please specify host and port manually !")
             return
-          
     if host[:6] == 'direct':
       # check if running on FT-txt
       if str.find(socket.gethostname(), 'FT-txt') < 0 and str.find(socket.gethostname(), 'ft-txt') < 0:
         print("ftrobopy konnte nicht initialisiert werden.")
         print("Der 'direct'-Modus kann nur im Download/Offline-Betrieb auf dem TXT verwendet werden !")
         return None
       # check if TxtMainControl is running, if yes quit
@@ -2103,36 +2807,42 @@
         except IOError:
           continue
         except:
           print("ftrobopy konnte nicht im 'direct'-Modus initialisiert werden.")
           return
       ftTXT.__init__(self, directmode=True)
     else:
-      ftTXT.__init__(self, host, port)
+      ftTXT.__init__(self, host, port, use_extension=use_extension, use_TransferAreaMode=use_TransferAreaMode)
     self._txt_is_initialzed = True
     self.queryStatus()
     if self.getVersionNumber() < 0x4010500:
       print('ftrobopy needs at least firmwareversion ',hex(0x4010500), '.')
       sys.exit()
     print('Connected to ', self.getDevicename(), self.getFirmwareVersion())
-    for i in range(8):
+    if use_extension:
+      n = 16
+    else:
+      n = 8
+    for i in range(n):
       self.setPwm(i,0)
     self.startOnline(update_interval)
-    self.updateConfig()
+    #self.updateConfig(ftTXT.C_EXT_MASTER)
+    #if (use_extension):
+    #  self.updateConfig(ftTXT.C_EXT_SLAVE)
 
   def __del__(self):
     if self._txt_is_initialized:
       self.stopCameraOnline()
       self.stopOnline()
       if self._sock:
         self._sock.close()
       if self._ser_ms:
         self._ser_ms.close()
 
-  def motor(self, output):
+  def motor(self, output, ext=ftTXT.C_EXT_MASTER, wait=True):
     """
       Diese Funktion erzeugt ein Motor-Objekt, das zur Ansteuerung eines Motors verwendet wird,
       der an einem der Motorausgaenge M1-M4 des TXT angeschlossen ist. Falls auch die schnellen
       Zaehler C1-C4 angeschlossen sind (z.b. durch die Verwendung von Encodermotoren oder Zaehlraedern)
       koennen auch Achsumdrehungen genau gemessen werden und damit zurueckgelegte Distanzen bestimmt werden.
       Ausserdem koennen jeweils zwei Motorausgaenge miteinander synchronisiert werden, um z.b. perfekten
       Geradeauslauf bei Robotermodellen zu erreichen.
@@ -2172,26 +2882,34 @@
       
       Anwendungsbeispiel:
 
       >>> Motor1.setSpeed(512)
 
       Laesst den Motor mit maximaler Umdrehungsgeschwindigkeit laufen.
 
-      **setDistance** (distance, syncto=None)
+      **setDistance** (distance, syncto=None, sn=None)
       
       Einstellung der Motordistanz, die ueber die schnellen Counter gemessen wird, die dafuer natuerlich angeschlossen
       sein muessen.
       
-      :param distance: Gibt an, um wieviele Counter-Zaehlungen sich der Motor drehen soll (der Encodermotor gibt 72 Impulse pro Achsumdrehung)
+      :param distance: Gibt an, um wieviele Counter-Zaehlungen sich der Motor drehen soll.
+                       (Der Encodermotor des TXTs gibt 190 Impulse pro 3 Achsumdrehungen, also 63 1/3 pro Umlauf)
+                       (Der Encodermotor des TX gibt 72 Impulse pro Umlauf)
       :type distance: integer
       
       :param syncto: Hiermit koennen zwei Motoren synchronisiert werden um z.B. perfekten Geradeauslauf
                      zu ermoeglichen. Als Parameter wird hier das zu synchronisierende Motorobjekt uebergeben.
       :type syncto: ftrobopy.motor Objekt
       
+      :param sn: Um mit synchronisierten Motoren Kurven fahren zu koennen, ist es mit diesem Parameter moeglich,
+                 einen Counter (waehrend der Synchronfahrt) gezielt zu manipulieren.
+                 Als Parameter wird hier die Nummer des synchronisierten Motoreingangs uebergeben.
+                 Der Wert des Distanz-Parameters wird in diesem Fall auf den Counter aufaddiert (oder subtrahiert, je nach Vorzeichen)
+      :type sn: integer
+      
       :return: Leer
       
       Anwendungsbeispiel:
       
       Der Motor am Anschluss M1 wird mit dem Motor am Anschluss M2 synchronisiert. Die Motoren M1 und M2 laufen
       so lange, bis beide Motoren die eingestellte Distanz (Achsumdrehungen / 72) erreicht haben. Ist einer oder beide Motoren
       nicht mit den schnellen Zaehlereingaengen verbunden, laufen die Motoren bis zur Beendigung des Python-Programmes !
@@ -2227,73 +2945,82 @@
       :return: Leer
       
       Anwendungsbeispiel:
       
       >>> Motor1.stop()
     """
     class mot(object):
-      def __init__(self, outer, output):
+      def __init__(self, outer, output, ext):
         self._outer=outer
         self._output=output
+        self._ext=ext
         self._speed=0
         self._distance=0
         self._outer._exchange_data_lock.acquire()
         self.setSpeed(0)
         self.setDistance(0)
         self._outer._exchange_data_lock.release()
       def setSpeed(self, speed):
         self._outer._exchange_data_lock.acquire()
         self._speed=speed
         if speed > 0:
-         self._outer.setPwm((self._output-1)*2, self._speed)
-         self._outer.setPwm((self._output-1)*2+1, 0)
+         self._outer.setPwm((self._output-1)*2, self._speed, self._ext)
+         self._outer.setPwm((self._output-1)*2+1, 0, self._ext)
         else:
-          self._outer.setPwm((self._output-1)*2, 0)
-          self._outer.setPwm((self._output-1)*2+1, -self._speed)
+          self._outer.setPwm((self._output-1)*2, 0, self._ext)
+          self._outer.setPwm((self._output-1)*2+1, -self._speed, self._ext)
         self._outer._exchange_data_lock.release()
-      def setDistance(self, distance, syncto=None):
+      def setDistance(self, distance, syncto=None, sn=None):
         self._outer._exchange_data_lock.acquire()
         if syncto:
           self._distance     = distance
           syncto._distance   = distance
-          self._command_id   = self._outer.getCurrentMotorCmdId(self._output-1)
-          syncto._command_id = syncto._outer.getCurrentMotorCmdId(self._output-1)
-          self._outer.setMotorDistance(self._output-1, distance)
-          self._outer.setMotorDistance(syncto._output-1, distance)
-          self._outer.setMotorSyncMaster(self._output-1, syncto._output)
-          self._outer.setMotorSyncMaster(syncto._output-1, self._output)
-          self._outer.incrMotorCmdId(self._output-1)
-          self._outer.incrMotorCmdId(syncto._output-1)
+          self._command_id   = self._outer.getCurrentMotorCmdId(self._output-1, self._ext)
+          syncto._command_id = syncto._outer.getCurrentMotorCmdId(self._output-1, self._ext)
+          self._outer.setMotorDistance(self._output-1, distance, self._ext)
+          self._outer.setMotorDistance(syncto._output-1, distance, self._ext)
+          self._outer.setMotorSyncMaster(self._output-1, 4*self._ext + syncto._output, self._ext)
+          self._outer.setMotorSyncMaster(syncto._output-1, 4*self._ext + self._output, self._ext)
+          self._outer.incrMotorCmdId(self._output-1, self._ext)
+          self._outer.incrMotorCmdId(syncto._output-1, self._ext)
+        elif sn:
+          self._distance     = distance
+          self._command_id   = self._outer.getCurrentMotorCmdId(self._output-1, self._ext)
+          self._outer.setMotorDistance(self._output-1, distance, self._ext)
+          self._outer.setMotorSyncMaster(self._output-1, sn, self._ext)
+          self._outer.incrMotorCmdId(self._output-1, self._ext)
         else:
           self._distance     = distance
-          self._command_id   = self._outer.getCurrentMotorCmdId(self._output-1)
-          self._outer.setMotorDistance(self._output-1, distance)
-          self._outer.setMotorSyncMaster(self._output-1, 0)
-          self._outer.incrMotorCmdId(self._output-1)
+          self._command_id   = self._outer.getCurrentMotorCmdId(self._output-1, self._ext)
+          self._outer.setMotorDistance(self._output-1, distance, self._ext)
+          self._outer.setMotorSyncMaster(self._output-1, 0, self._ext)
+          self._outer.incrMotorCmdId(self._output-1, self._ext)
         self._outer._exchange_data_lock.release()
       def finished(self):
-        if self._outer.getMotorCmdId(self._output-1) == self._outer.getCurrentMotorCmdId(self._output-1):
+        if self._outer.getMotorCmdId(self._output-1, self._ext) == self._outer.getCurrentMotorCmdId(self._output-1, self._ext):
           return True
         else:
           return False
       def getCurrentDistance(self):
-        return self._outer.getCurrentCounterValue(idx=self._output-1)
+        return self._outer.getCurrentCounterValue(idx=self._output-1, ext=self._ext)
       def stop(self):
         self._outer._exchange_data_lock.acquire()
         self.setSpeed(0)
         self.setDistance(0)
         self._outer._exchange_data_lock.release()
     
-    M, I = self.getConfig()
+    M, I = self.getConfig(ext)
     M[output-1] = ftTXT.C_MOTOR
-    self.setConfig(M, I)
-    self.updateConfig()
-    return mot(self, output)
+    self.setConfig(M, I, ext)
+    self.updateConfig(ext)
+    if wait:
+      self.updateWait()
+    return mot(self, output, ext)
 
-  def output(self, num, level=0):
+  def output(self, num, level=0, ext=ftTXT.C_EXT_MASTER, wait=True):
     """
       Diese Funktion erzeugt ein allgemeines Output-Objekt, das zur Ansteuerung von Elementen verwendet
       wird, die an den Ausgaengen O1-O8 angeschlossen sind.
       
       Anwendungsbeispiel:
       
       Am Ausgang O7 ist eine Lampe oder eine LED angeschlossen:
@@ -2311,31 +3038,35 @@
       einer Lampe zu regeln.
       
       Anwendungsbeispiel:
 
       >>> Lampe.setLevel(512)
     """
     class out(object):
-      def __init__(self, outer, num, level):
+      def __init__(self, outer, num, level, ext):
         self._outer=outer
         self._num=num
         self._level=level
+        self._ext=ext
+        self.setLevel(level)
       def setLevel(self, level):
         self._level=level
         self._outer._exchange_data_lock.acquire()
-        self._outer.setPwm(num-1, self._level)
+        self._outer.setPwm(num-1, self._level, self._ext)
         self._outer._exchange_data_lock.release()
     
-    M, I = self.getConfig()
+    M, I = self.getConfig(ext)
     M[int((num-1)/2)] = ftTXT.C_OUTPUT
-    self.setConfig(M, I)
-    self.updateConfig()
-    return out(self, num, level)    
+    self.setConfig(M, I, ext)
+    self.updateConfig(ext)
+    if wait:
+      self.updateWait()
+    return out(self, num, level, ext)
 
-  def input(self, num):
+  def input(self, num, ext=ftTXT.C_EXT_MASTER, wait=True):
     """
       Diese Funktion erzeugt ein digitales (Ein/Aus) Input-Objekt, an einem der Eingaenge I1-I8.  Dies kann z.B. ein Taster, ein Photo-Transistor oder auch ein Reed-Kontakt sein.
       
       Anwendungsbeispiel:
       
       >>> Taster = ftrob.input(5)
       
@@ -2353,64 +3084,95 @@
       
       Anwendungsbeispiel:
 
       >>> if Taster.state() == 1:
             print("Der Taster an Eingang I5 wurde gedrueckt.")
     """
     class inp(object):
-      def __init__(self, outer, num):
+      def __init__(self, outer, num, ext):
         self._outer=outer
         self._num=num
+        self._ext=ext
       def state(self):
-        return self._outer.getCurrentInput(num-1)
-    
-    M, I = self.getConfig()
+        return self._outer.getCurrentInput(num-1, self._ext)
+
+    M, I = self.getConfig(ext)
     I[num-1]= (ftTXT.C_SWITCH, ftTXT.C_DIGITAL)
-    self.setConfig(M, I)
-    self.updateConfig()
-    return inp(self, num)
-  
-  def resistor(self, num):
+    self.setConfig(M, I, ext)
+    if self._use_TransferAreaMode:
+      ftTA2py.fX1config_uni(ext, num-1, I[num-1][0], I[num-1][1] )
+    self.updateConfig(ext)
+    if wait:
+      self.updateWait()
+    return inp(self, num, ext)
+
+  def resistor(self, num, ext=ftTXT.C_EXT_MASTER, wait=True):
     """
       Diese Funktion erzeugt ein analoges Input-Objekt zur Abfrage eines Widerstandes, der an einem der Eingaenge I1-I8 angeschlossenen ist. Dies kann z.B. ein temperaturabhaengiger Widerstand (NTC-Widerstand) oder auch ein Photowiderstand sein.
-    
+
       Anwendungsbeispiel:
-    
+
       >>> R = ftrob.resistor(7)
-    
+
       Das so erzeugte Widerstands-Objekt hat folgende Methoden:
-    
+
       **value** ()
-    
+
       Mit dieser Methode wird der Widerstand abgefragt.
-    
+
       :param num: Nummer des Eingangs, an dem der Widerstand angeschlossen ist (1 bis 8)
       :type num: integer
-    
+
       :return: Der am Eingang anliegende Widerstandswert in Ohm fuer Widerstaende bis 15kOhm, fuer hoehere Widerstandswerte wird immer 15000 zurueckgegeben
       :rtype: integer
-    
+
       Anwendungsbeispiel:
-    
+
       >>> print("Der Widerstand betraegt ", R.value())
+
+      **ntcTemperature** ()
+
+      Mit dieser Methode wird die Temperatur des fischertechnik NTC-Widerstands abgefragt.
+
+      :return: Die Temperatur des am Eingang angeschlossenen Widerstandes in Grad Celsius.
+      :rtype: float
+
+      Anwendungsbeispiel:
+
+      >>> print("Die Temperatur des fischertechnik NTC-Widerstands betraegt ", R.ntcTemperature())
     """
     class inp(object):
-      def __init__(self, outer, num):
+      def __init__(self, outer, num, ext):
         self._outer=outer
         self._num=num
+        self._ext=ext
       def value(self):
-        return self._outer.getCurrentInput(num-1)
-  
-    M, I = self.getConfig()
+        return self._outer.getCurrentInput(num-1, self._ext)
+      def ntcTemperature(self):
+        r = self.value()
+        if r != 0:
+          x = log(self.value())
+          y = x * x * 1.39323522
+          z = x * -43.9417405
+          T = y + z + 271.870481
+        else:
+          T = 10000
+        return T
+
+    M, I = self.getConfig(ext)
     I[num-1]= (ftTXT.C_RESISTOR, ftTXT.C_ANALOG)
-    self.setConfig(M, I)
-    self.updateConfig()
-    return inp(self, num)
+    self.setConfig(M, I, ext)
+    if self._use_TransferAreaMode:
+      ftTA2py.fX1config_uni(ext, num-1, I[num-1][0], I[num-1][1] )
+    self.updateConfig(ext)
+    if wait:
+      self.updateWait()
+    return inp(self, num, ext)
 
-  def ultrasonic(self, num):
+  def ultrasonic(self, num, ext=ftTXT.C_EXT_MASTER, wait=True):
     """
       Diese Funktion erzeugt ein Objekt zur Abfrage eines an einem der Eingaenge I1-I8 angeschlossenen
       TX/TXT-Ultraschall-Distanzmessers.
       
       Anwendungsbeispiel:
 
       >>> ultraschall = ftrob.ultrasonic(6)
@@ -2428,27 +3190,32 @@
       :rtype: integer
 
       Anwendungsbeispiel:
       
       >>> print("Der Abstand zur Wand betraegt ", ultraschall.distance(), " cm.")
     """
     class inp(object):
-      def __init__(self, outer, num):
+      def __init__(self, outer, num, ext):
         self._outer=outer
         self._num=num
+        self._ext=ext
       def distance(self):
-        return self._outer.getCurrentInput(num-1)
+        return self._outer.getCurrentInput(num-1, self._ext)
     
-    M, I = self.getConfig()
+    M, I = self.getConfig(ext)
     I[num-1]= (ftTXT.C_ULTRASONIC, ftTXT.C_ANALOG)
-    self.setConfig(M, I)
-    self.updateConfig()
-    return inp(self, num)
+    self.setConfig(M, I, ext)
+    if self._use_TransferAreaMode:
+      ftTA2py.fX1config_uni(ext, num-1, I[num-1][0], I[num-1][1] )
+    self.updateConfig(ext)
+    if wait:
+      self.updateWait()
+    return inp(self, num, ext)
   
-  def voltage(self, num):
+  def voltage(self, num, ext=ftTXT.C_EXT_MASTER, wait=True):
     """
       Diese Funktion erzeugt ein analoges Input-Objekt zur Abfrage des Spannungspegels, der an einem der Eingaenge I1-I8 angeschlossenen ist. Damit kann z.B. auch der Ladezustand des Akkus ueberwacht werden. Der fischertechnik Farbsensor kann auch mit diesem Objekt abgefragt werden.
       
       Anwendungsbeispiel:
       
       >>> batterie = ftrob.voltage(7)
       
@@ -2465,27 +3232,32 @@
       :rtype: integer
       
       Anwendungsbeispiel:
       
       >>> print("Die Spannung betraegt ", batterie.voltage(), " mV")
       """
     class inp(object):
-      def __init__(self, outer, num):
+      def __init__(self, outer, num, ext):
         self._outer=outer
         self._num=num
+        self._ext=ext
       def voltage(self):
-        return self._outer.getCurrentInput(num-1)
+        return self._outer.getCurrentInput(num-1, self._ext)
     
-    M, I = self.getConfig()
+    M, I = self.getConfig(ext)
     I[num-1]= (ftTXT.C_VOLTAGE, ftTXT.C_ANALOG)
-    self.setConfig(M, I)
-    self.updateConfig()
-    return inp(self, num)
+    self.setConfig(M, I, ext)
+    if self._use_TransferAreaMode:
+      ftTA2py.fX1config_uni(ext, num-1, I[num-1][0], I[num-1][1] )
+    self.updateConfig(ext)
+    if wait:
+      self.updateWait()
+    return inp(self, num, ext)
 
-  def colorsensor(self, num):
+  def colorsensor(self, num, ext=ftTXT.C_EXT_MASTER, wait=True):
     """
       Diese Funktion erzeugt ein analoges Input-Objekt zur Abfrage des fischertechnik Farbsensors.
       Beim Farbsensor handelt es sich um einen Fototransistor, der das von einer Oberflaeche
       reflektierte Licht einer roten Lichtquelle misst. Der Abstand zwischen Farbsensor und zu
       bestimmender Oberflaeche sollte zwischen 5mm und 10mm liegen.
       Die Farben 'weiss', 'rot' und 'blau' koennen mit dieser Methode zuverlaessig unterschieden werden.
       
@@ -2514,35 +3286,40 @@
       Anwendungsbeispiel:
       
       >>> farbsensor = txt.colorsensor(5)
       >>> print("Der Farbwert ist      : ", farbsensor.value())
       >>> print("Die erkannte Farbe ist: ", farbsensor.color())
       """
     class inp(object):
-      def __init__(self, outer, num):
+      def __init__(self, outer, num, ext):
         self._outer=outer
         self._num=num
+        self._ext=ext
       def value(self):
-        return self._outer.getCurrentInput(num-1)
+        return self._outer.getCurrentInput(num-1, self._ext)
       def color(self):
-        c = self._outer.getCurrentInput(num-1)
+        c = self._outer.getCurrentInput(num-1, self._ext)
         if c < 200:
           return 'weiss'
         elif c < 1000:
           return 'rot'
         else:
           return 'blau'
     
-    M, I = self.getConfig()
+    M, I = self.getConfig(ext)
     I[num-1]= (ftTXT.C_VOLTAGE, ftTXT.C_ANALOG)
-    self.setConfig(M, I)
-    self.updateConfig()
-    return inp(self, num)
+    self.setConfig(M, I, ext)
+    if self._use_TransferAreaMode:
+      ftTA2py.fX1config_uni(ext, num-1, I[num-1][0], I[num-1][1] )
+    self.updateConfig(ext)
+    if wait:
+      self.updateWait()
+    return inp(self, num, ext)
 
-  def trailfollower(self, num):
+  def trailfollower(self, num, ext=ftTXT.C_EXT_MASTER, wait=True):
     """
       Diese Funktion erzeugt ein digitales Input-Objekt zur Abfrage eines Spursensors, der an einem der Eingaenge I1-I8 angeschlossenen ist.
       (Intern ist diese Funktion identisch zur voltage()-Funktion und misst die anliegende Spannung in mV).
       Ab einer Spannung von 600mV wird eine digitale 1 (Spur ist weiss) zurueckgeliefert, ansonsten ist der Wert eine digitale 0 (Spur ist schwarz).
       Falls fuer den Spursensor ein analoger Eingangswert benoetigt wird, kann auch die voltage()-Funktion verwendet werden.
     
       Anwendungsbeispiel:
@@ -2562,31 +3339,36 @@
       :rtype: integer
     
       Anwendungsbeispiel:
     
       >>> print("Der Wert des Spursensors ist ", L.state())
     """
     class inp(object):
-      def __init__(self, outer, num):
+      def __init__(self, outer, num, ext):
         self._outer=outer
         self._num=num
+        self._ext=ext
       def state(self):
-        if self._outer.getCurrentInput(num-1) == 1: # in direct-mode digital 1 is set by motor-shield if voltage is > 600mV
+        if self._outer.getCurrentInput(num-1, self._ext) == 1: # in direct-mode digital 1 is set by motor-shield if voltage is > 600mV
          return 1
         else:
-          if self._outer.getCurrentInput(num-1) > 600: # threshold in mV between digital 0 and 1. Use voltage()-Function instead, if analog value of trailfollower is needed.
+          if self._outer.getCurrentInput(num-1, self._ext) > 600: # threshold in mV between digital 0 and 1. Use voltage()-Function instead, if analog value of trailfollower is needed.
             return 1
           else:
             return 0
     
-    M, I = self.getConfig()
+    M, I = self.getConfig(ext)
     I[num-1]= (ftTXT.C_VOLTAGE, ftTXT.C_DIGITAL)
-    self.setConfig(M, I)
-    self.updateConfig()
-    return inp(self, num)
+    self.setConfig(M, I, ext)
+    if self._use_TransferAreaMode:
+      ftTA2py.fX1config_uni(ext, num-1, I[num-1][0], I[num-1][1] )
+    self.updateConfig(ext)
+    if wait:
+      self.updateWait()
+    return inp(self, num, ext)
   
   def joystick(self, joynum, remote_number=0, remote_type=0):
     """
       Diese Funktion erzeugt ein Input-Objekt zur Abfrage eines Joysticks einer fischertechnik IR-Fernbedienung.
 
       :param joynum: Nummer des Joysticks, der abgefragt werden soll.
        
@@ -2599,69 +3381,148 @@
       
       + OFF OFF : Nummer 1
       + ON  OFF : Nummer 2
       + OFF ON  : Nummer 3
       + ON  ON  : Nummer 4
       
       Wird der parameter remote_number=0 gesetzt, kann damit jede der 4 moeglichen Fernbedienungen abgefragt werden, unabhaengig von ihren DIP-Schalter Einstellungen. Dies ist die Standardeinstellung, falls der Parameter nicht angegeben wird.
+
+      :param remote_type: 0: (rote) IR Infrarot-Fernbedienung, 1: (blaue) BT Bluetooth-Fernbedienung
+
+      Anmerkungen zur BT-Fernbedienung:
+
+      * Die BT-Fernbedienung kann derzeit nur mit der Community-Firmware (cfw Version > 0.9.4) im Offline-Modus (direct) verwendet werden.
+      * Bevor die BT-Fernbedienung verwendet werden kann, muss zuerst der ft_bt_server-Prozess gestartet werden. Dies kann auf der TXT-Kommandozeile mit dem Befehl: **sudo ft_bt_server** erreicht werden. Alternativ kann der ft_bt_server-Prozess auch ueber die cfw-App **LNT BT-Server** ueber den Touchscreen des TXT gestartet werden.
+      * Es kann nur eine BT Fernbedienung abgefragt werden. Der Parameter :param remote_number: wird dann automatisch auf 0 gesetzt.
+      * Die Buttons/Knoepfe der blauen BT-Fernbedienung werden von dieser nicht uebertragen und koennen deshalb nicht abgefragt werden.
+      * Die BT-Fernbedienung hat intern die doppelte (integer) Aufloesung [-30 ... +30] der IR-Fernbedienung [-15 ... +15]. Beide Wertebereiche werden auf den (float) Bereich [-1.0 ... +1.0] gemappt.
+
+      **Achtung Neu :** das Mapping auf den Wertebereich [-1.0 ... +1.0] besteht erst seit der ftrobopy-Version 1.86. In den vorherigen Versionen wurde der (integer) Bereich [-15 ... +15] zurueckgelifert.
+
+      Insgesamt koennen an einem TXT gleichzeitig 4 verschiedene IR- und eine BT-Fernsteuerung abgefragt werden.
       
       Anwendungsbeispiel:
     
-      >>> joystickLinks   = ftrob.joystick(0)
-      >>> joystickRechts  = ftrob.joystick(1)
-      >>> joystickNummer3 = ftrob.joystick(0, 2) # linker Joystick, der Fernbedienung Nummer 2 (Dip-Switch: ON OFF)
+      >>> joystickLinks      = ftrob.joystick(0)       # linker Joystick aller 4 moeglichen IR-Fernbedienungen
+      >>> joystickRechts     = ftrob.joystick(1)       # rechter Joystick aller 4 moeglichen IR-Fernbedienungen
+      >>> joystickNummer3    = ftrob.joystick(0, 2)    # linker Joystick der IR-Fernbedienung Nummer 2 (Dip-Switch: ON OFF)
+      >>> joystickBlauLinks  = ftrob.joystick(0, 0, 1) # linker Joystick der BT-Fernbedienung
+      >>> joystickBlauRechts = ftrob.joystick(0, 0, 1) # linker Joystick der BT-Fernbedienung
     
       Das so erzeugte Joystick-Objekt hat folgende Methoden:
+
+      **isConnected** ()
+
+      Mit dieser Methode kann getested werden, ob ein Joystick per Bluetooth mit dem TXT verbunden ist und ob der Abfrage-Thread laeuft. Fuer IR-Joysticks ist dies immer True, da IR-Joysticks nicht extra verbunden werden muessen (der TXT lauscht grundsaetzlich immer an der IR-LED, ob ein Signal empfangen wird).
+
+      :return: True oder False
+
+      Anwendungsbeispiel:
+
+      >>> joy1 = txt.joystick(0,0,1) # 1=BT Joystick
+      >>> joy2 = txt.joystick(0,0,0) # 0=IR Joystick
+      >>> if joy1.isConnected():
+      >>>   print("Ein Bluetooth Joystick ist verbunden.")
+      >>> if joy2.isConnected(): # fuer IR Joysticks ist dieser Wert immer True
+      >>>   print("Ein IR Joystick ist verbunden")
+
     
       **leftright** ()
     
       Mit dieser Methode wird die horizontale (links-rechts) Achse abgefragt.
 
-      :return: -15 (Joystick ganz nach links) bis +15 (Joystick ganz nach recht), 0: Mittelstellung
+      :return: -1.0 (Joystick ganz nach links) bis +1.0 (Joystick ganz nach recht), 0: Mittelstellung
 
       **updown** ()
       
       Mit dieser Methode wird die vertikale (hoch-runter) Achse abgefragt.
       
-      :return: -15 (Joystick ganz nach unten) bis +15 (Joystick ganz nach oben), 0: Mittelstellung
+      :return: -1.0 (Joystick ganz nach unten) bis +1.0 (Joystick ganz nach oben), 0: Mittelstellung
       
       Anwendungsbeispiel:
       
       >>> joystick1 = ftrob.joystick(0) # linker Joystick einer bel. IR-Fernsteuerung
       >>> print("Links-Rechts-Stellung=", joystick1.leftright(), " Hoch-Runter-Stellung=", joystick1.updown())
     """
     class remote(object):
-      def __init__(self, outer, joynum, remote_number, remote_type):
+      def __init__(self, outer, joynum, remote_number, remote_type, update_interval=0.01):
         # remote_number: 0=any, 1-4=remote1-4
         # remote_type: IR=0, BT=1
         self._outer=outer
         self._joynum=joynum
         self._remote_number=remote_number
         self._remote_type=remote_type
+        self._jsdev = None
+        if self._remote_type==1: # BT remote
+          self._remote_number = 0 # only 1 BT remote is supported
+          try:
+            self._jsdev = open('/dev/input/js0', 'rb') # open joystick device
+          except:
+            self._jsdev = None
+            print("Failed to open BT Joystick")
+          if self._jsdev:
+            if self._outer._bt_joystick_stop_event.is_set():
+               self._outer._bt_joystick_stop_event.clear()
+            if self._outer._bt_joystick_thread is None:
+              self._outer._bt_joystick_thread = BTJoystickEval(txt=self._outer, sleep_between_updates=update_interval, stop_event=self._outer._bt_joystick_stop_event, jsdev=self._jsdev)
+              self._outer._bt_joystick_thread.setDaemon(True)
+              self._outer._bt_joystick_thread.start()
+        return None
+
+      def isConnected(self):
+        return (not self._outer._bt_joystick_stop_event.is_set()) and (self._outer._bt_joystick_thread is not None)
+          
       def leftright(self):
         if remote_type==0: # IR remote
           if joynum==0: # left joystick on remote
-            return self._outer._ir_current_ljoy_left_right[remote_number]
+            return 1.0 * self._outer._ir_current_ljoy_left_right[remote_number] / 15.0
           else: # right joystick on remote
-            return self._outer._ir_current_rjoy_left_right[remote_number]
-        else: # BT remote (not yet supported)
-          return 0
+            return 1.0 * self._outer._ir_current_rjoy_left_right[remote_number] / 15.0
+        else: # BT remote
+          if joynum==0: # left joystick on remote
+            v = 1.0 * self._outer._bt_ljoy_left_right
+            if v < 0:
+              v /= 32767.0
+            else:
+              v /= 32512.0
+            return v
+          else: # right joystick on remote 
+            v = 1.0 * self._outer._bt_rjoy_left_right
+            if v < 0:
+              v /= 32767.0
+            else:
+              v /= 32512.0
+            return v
       def updown(self):
         if remote_type==0: # IR remote
           if joynum==0: # left joystick on remote
-            return self._outer._ir_current_ljoy_up_down[remote_number]
+            return 1.0 * self._outer._ir_current_ljoy_up_down[remote_number] / 15.0
           else: # right joystick on remote
-            return self._outer._ir_current_rjoy_up_down[remote_number]
-        else: # BT remote (not yet supported)
-          return 0
+            return 1.0 * self._outer._ir_current_rjoy_up_down[remote_number] / 15.0
+        else: # BT remote 
+          if joynum==0: # left joystick on remote
+            v = 1.0 * self._outer._bt_ljoy_up_down
+            if v <= 0:
+              v /= -32767.0
+            else:
+              v /= -32512.0
+            return v
+          else: # right joystick on remote
+            v = 1.0 * self._outer._bt_rjoy_up_down
+            if v <= 0:
+              v /= -32767.0
+            else:
+              v /= -32512.0
+            return v
     return remote(self, joynum, remote_number, remote_type)
 
   def joybutton(self, buttonnum, remote_number=0, remote_type=0):
     """
       Diese Funktion erzeugt ein Input-Objekt zur Abfrage eines Buttons einer fischertechnik IR-Fernbedienung.
+      Die Funktion kann nur mit den IR-Fernbedienungen sinnvoll verwendet werden. Die blaue BT-Fernbedienung uebertraegt die Button-Signale nicht.
 
       :param buttonnum: Nummer des Buttons, der abgefragt werden soll.
        
       + 0: linker Button (ON)
       + 1: rechter Button (OFF)
       
       :param remote_number: (optionaler Parameter) Nummer der IR-Fernbedienung.
@@ -2671,25 +3532,30 @@
       + OFF OFF  : Nummer 1
       + ON  OFF  : Nummer 2
       + OFF ON   : Nummer 3
       + ON  ON   : Nummer 4
       
       Wird der parameter remote_number=0 gesetzt, kann damit jede der 4 moeglichen Fernbedienungen abgefragt werden, unabhaengig von ihren DIP-Schalter Einstellungen. Dies ist die Standardeinstellung, falls der Parameter nicht angegeben wird.
       
+      :param remote_type: 0: (rote) IR Infrarot-Fernbedienung, 1: (blaue) BT Bluetooth-Fernbedienung
+
+      Dieser Parameter ist nur aus Gruenden der Kompatibilitaet vorhanden. Die BT-Fernbedienung uebertraegt keine Button-Signale.
+      
       Anwendungsbeispiel:
     
       >>> buttonON    = ftrob.joybutton(0)
       >>> buttonOFF   = ftrob.joybutton(1)
       >>> buttonOFF_2 = ftrob.joybutton(0, 4) # linker (ON)-Button, der Fernbedienung Nummer 4 (Dip-Switch: ON ON)
     
       Das so erzeugte Button-Objekt hat die folgende Methode:
     
       **pressed** ()
     
       Mit dieser Methode wird abgefragt, ob der Button gedrueckt ist.
+      Anmerkung: Im Falle der BT-Fernbedienung wird hier immer der Wert False zurueckgeliefert.
 
       :return: False (=Button ist nicht gedrueckt) oder True (=Button ist gedrueckt)
       :rtype: boolean
 
       Anwendungsbeispiel:
       
       >>> button1 = ftrob.joybutton(0) # linker (ON) Button einer bel. IR-Fernsteuerung
@@ -2713,22 +3579,27 @@
             else:
               return False
           else: # right button (OFF) on remote
             if (self._outer._ir_current_buttons[remote_number]) >> 1 == 1:
               return True
             else:
               return False
-        else: # BT remote (not yet supported)
-          return 0
+        else: # BT remote has no buttons
+          return False
     return remote(self, buttonnum, remote_number, remote_type)
 
   def joydipswitch(self, remote_type=0):
     """
       Diese Funktion erzeugt ein Input-Objekt zur Abfrage des DIP-Schalters einer fischertechnik IR-Fernbedienung.
+      Die Funktion kann nur mit den IR-Fernbedienungen sinnvoll verwendet werden. Die blaue BT-Fernbedienung hat keine DIP-Schalter.
+
+      :param remote_type: 0: (rote) IR Infrarot-Fernbedienung, 1: (blaue) BT Bluetooth-Fernbedienung
 
+      Dieser Parameter ist nur aus Gruenden der Kompatibilitaet vorhanden. Die BT-Fernbedienung hat keine DIP-Schalter.
+      
       Anwendungsbeispiel:
     
       >>> IR_DipSchalter = ftrob.joydipswitch()
     
       Das so erzeugte Button-Objekt hat die folgende Methode:
     
       **setting** ()
@@ -2736,15 +3607,15 @@
       Mit dieser Methode wird die DIP-Schalter-Einstellung abgefragt:
       
       + OFF OFF  = 0
       + ON  OFF  = 1
       + OFF ON   = 2
       + ON  ON   = 3
 
-      :return: Wert des DIP-Schalters (0-3)
+      :return: Wert des DIP-Schalters (0-3). Der Rueckgabewert bei Verwendung der BT-Fernbedienung ist hier immer 0.
       :rtype: integer
       
       Anwendungsbeispiel:
  
       >>> IR_DipSchalter = ftrob.joydipswitch()
       >>> print("Die aktuelle Einstellung des DIP-Schalters ist: ", IR_DipSchalter.setting())
     """
@@ -2752,36 +3623,36 @@
       def __init__(self, outer, remote_type):
         # remote_type: IR=0, BT=1
         self._outer=outer
         self._remote_type=remote_type
       def setting(self):
         if remote_type==0: # IR remote
           return self._outer._ir_current_dip_switch[0]
-        else: # BT remote (not yet supported)
+        else: # BT remote has no dip switches
           return 0
     return remote(self, remote_type)
 
-  def sound_finished(self):
+  def sound_finished(self, ext=ftTXT.C_EXT_MASTER):
     """
       Ueberpruefen, ob der zuletzt gespielte Sounds bereits abgelaufen ist
       
       :return: True (Sound ist fertig) oder False (Sound wird noch abgespielt)
       :rtype: boolean
 
       Anwendungsbeispiel:
       
       >>> while not ftrob.sound_finished():
             pass
     """
-    if self._current_sound_cmd_id == self.getSoundCmdId():
+    if self._current_sound_cmd_id[ext] == self.getSoundCmdId(ext):
       return True
     else:
       return False
 
-  def play_sound(self, idx, repeat=1, volume=100):
+  def play_sound(self, idx, repeat=1, volume=100, ext=ftTXT.C_EXT_MASTER):
     """
       Einen Sound ein- oder mehrmals abspielen.
       
       *  0 : Kein Sound (=Soundausgabe stoppen)
       *  1 : Flugzeug
       *  2 : Alarm
       *  3 : Glocke
@@ -2825,29 +3696,29 @@
       
       Anwendungsbeispiel:
       
       >>> ftrob.play_sound(27, 5) # 5 mal hintereinander das Fahrgeraeusch abspielen
       >>> ftrob.play_sound(5, repeat=2, volume=10) # 2 mal hintereinander leise hupen
     """
     
-    if idx != self.getSoundIndex():
-      self.setSoundIndex(idx)
+    if idx != self.getSoundIndex(ext):
+      self.setSoundIndex(idx, ext)
     if volume != self.getSoundVolume and self._directmode:
       self.setSoundVolume(volume)
-    self.setSoundRepeat(repeat)
-    self.incrSoundCmdId()
+    self.setSoundRepeat(repeat, ext)
+    self.incrSoundCmdId(ext)
 
-  def stop_sound(self):
+  def stop_sound(self, ext=ftTXT.C_EXT_MASTER):
     """
       Die Aktuelle Soundausgabe stoppen. Dabei wird der abzuspielende Sound-Index auf 0 (=Kein Sound)
       und der Wert fuer die Anzahl der Wiederholungen auf 1 gesetzt.
 
       :return: Leer
       
       Anwendungsbeispiel:
       
       >>> ftrob.stop_sound()
     """
-    self.setSoundIndex(0)
-    self.setSoundRepeat(1)
-    self.incrSoundCmdId()
+    self.setSoundIndex(0, ext)
+    self.setSoundRepeat(1, ext)
+    self.incrSoundCmdId(ext)
```


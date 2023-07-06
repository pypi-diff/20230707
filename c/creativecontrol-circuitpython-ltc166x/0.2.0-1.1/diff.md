# Comparing `tmp/creativecontrol-circuitpython-ltc166x-0.2.0.tar.gz` & `tmp/creativecontrol-circuitpython-ltc166x-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creativecontrol-circuitpython-ltc166x-0.2.0.tar", last modified: Thu Jul  6 23:47:06 2023, max compression
+gzip compressed data, was "creativecontrol-circuitpython-ltc166x-1.1.tar", last modified: Mon May 29 17:40:35 2023, max compression
```

## Comparing `creativecontrol-circuitpython-ltc166x-0.2.0.tar` & `creativecontrol-circuitpython-ltc166x-1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:47:06.960801 creativecontrol-circuitpython-ltc166x-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:47:06.952801 creativecontrol-circuitpython-ltc166x-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:47:06.956801 creativecontrol-circuitpython-ltc166x-0.2.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:47:06.956801 creativecontrol-circuitpython-ltc166x-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:47:06.956801 creativecontrol-circuitpython-ltc166x-0.2.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-06 23:47:06.960801 creativecontrol-circuitpython-ltc166x-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:47:06.960801 creativecontrol-circuitpython-ltc166x-0.2.0/creativecontrol_circuitpython_ltc166x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-06 23:47:06.000000 creativecontrol-circuitpython-ltc166x-0.2.0/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-06 23:47:06.000000 creativecontrol-circuitpython-ltc166x-0.2.0/creativecontrol_circuitpython_ltc166x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:47:06.000000 creativecontrol-circuitpython-ltc166x-0.2.0/creativecontrol_circuitpython_ltc166x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 23:47:06.000000 creativecontrol-circuitpython-ltc166x-0.2.0/creativecontrol_circuitpython_ltc166x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 23:47:06.000000 creativecontrol-circuitpython-ltc166x-0.2.0/creativecontrol_circuitpython_ltc166x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-07-06 23:46:57.000000 creativecontrol-circuitpython-ltc166x-0.2.0/creativecontrol_circuitpython_ltc166x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:47:06.960801 creativecontrol-circuitpython-ltc166x-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-06 23:46:57.000000 creativecontrol-circuitpython-ltc166x-0.2.0/examples/creativecontrol_circuitpython_ltc166x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-06 23:46:57.000000 creativecontrol-circuitpython-ltc166x-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-06 23:46:48.000000 creativecontrol-circuitpython-ltc166x-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 23:47:06.960801 creativecontrol-circuitpython-ltc166x-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.591308 creativecontrol-circuitpython-ltc166x-1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.587309 creativecontrol-circuitpython-ltc166x-1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.587309 creativecontrol-circuitpython-ltc166x-1.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.587309 creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.587309 creativecontrol-circuitpython-ltc166x-1.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-29 17:40:35.591308 creativecontrol-circuitpython-ltc166x-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.591308 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-29 17:40:35.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-29 17:40:35.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:40:35.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-29 17:40:35.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:40:35.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-29 17:40:27.000000 creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:40:35.591308 creativecontrol-circuitpython-ltc166x-1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-29 17:40:27.000000 creativecontrol-circuitpython-ltc166x-1.1/examples/creativecontrol_circuitpython_ltc166x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-29 17:40:27.000000 creativecontrol-circuitpython-ltc166x-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-29 17:40:16.000000 creativecontrol-circuitpython-ltc166x-1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:40:35.591308 creativecontrol-circuitpython-ltc166x-1.1/setup.cfg
```

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `creativecontrol-circuitpython-ltc166x-1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/.github/workflows/release_gh.yml` & `creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/.github/workflows/release_pypi.yml` & `creativecontrol-circuitpython-ltc166x-1.1/.github/workflows/release_pypi.yml`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/.gitignore` & `creativecontrol-circuitpython-ltc166x-1.1/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -45,10 +45,7 @@
 # IDE-specific files
 .idea
 .vscode
 *~
 
 # PYPI Dist
 dist
-
-# VS Code Workspace
-*.code-workspace
```

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/.pre-commit-config.yaml` & `creativecontrol-circuitpython-ltc166x-1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/.pylintrc` & `creativecontrol-circuitpython-ltc166x-1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/CODE_OF_CONDUCT.md` & `creativecontrol-circuitpython-ltc166x-1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/LICENSE` & `creativecontrol-circuitpython-ltc166x-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/LICENSES/CC-BY-4.0.txt` & `creativecontrol-circuitpython-ltc166x-1.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/LICENSES/MIT.txt` & `creativecontrol-circuitpython-ltc166x-1.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/LICENSES/Unlicense.txt` & `creativecontrol-circuitpython-ltc166x-1.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/PKG-INFO` & `creativecontrol-circuitpython-ltc166x-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creativecontrol-circuitpython-ltc166x
-Version: 0.2.0
+Version: 1.1
 Summary: CircuitPython library for control of LTC166X 8-bit and 10-bit DACs.
 Author-email: creativecontrol <t@creativecontrol.cc>
 License: MIT
 Project-URL: Homepage, https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X
 Keywords: adafruit,blinka,circuitpython,micropython,creativecontrol_circuitpython_ltc166x,LTC1660,LTC1665,DAC
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/README.rst` & `creativecontrol-circuitpython-ltc166x-1.1/README.rst`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO` & `creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: creativecontrol-circuitpython-ltc166x
-Version: 0.2.0
+Version: 1.1
 Summary: CircuitPython library for control of LTC166X 8-bit and 10-bit DACs.
 Author-email: creativecontrol <t@creativecontrol.cc>
 License: MIT
 Project-URL: Homepage, https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X
 Keywords: adafruit,blinka,circuitpython,micropython,creativecontrol_circuitpython_ltc166x,LTC1660,LTC1665,DAC
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/creativecontrol_circuitpython_ltc166x.egg-info/SOURCES.txt` & `creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/creativecontrol_circuitpython_ltc166x.py` & `creativecontrol-circuitpython-ltc166x-1.1/creativecontrol_circuitpython_ltc166x.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,22 +10,16 @@
 
 
 * Author(s): Thadeus Frazier-Reed
 
 Implementation Notes
 --------------------
 
-**TODO:**
-
-* Add Sleep and Wake control
-* Add example for multiple chained DACs
-
-
-* Influenced by
-  http://www.kerrywong.com/2010/05/02/a-library-for-ltc1665ltc1660/
+*
+http://www.kerrywong.com/2010/05/02/a-library-for-ltc1665ltc1660/
 
 **Hardware:**
 
 * Linear Technologies LTC166X datasheet:
   https://www.analog.com/media/en/technical-documentation/data-sheets/166560fa.pdf
 
 Multiple LTC1665/LTC1660’s can be controlled from a
@@ -47,137 +41,72 @@
 """
 
 import microcontroller
 from busio import SPI
 import digitalio
 from adafruit_bus_device.spi_device import SPIDevice
 
-__version__ = "0.2.0"
+__version__ = "01.1"
 __repo__ = (
     "https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X.git"
 )
 
 
-DAC_WAKE = 0x00
-DAC_A = 0x01
-DAC_B = 0x02
-DAC_C = 0x03
-DAC_D = 0x04
-DAC_E = 0x05
-DAC_F = 0x06
-DAC_G = 0x07
-DAC_H = 0x08
-DAC_SLEEP = 0x0E
-DAC_ALL = 0x0F
-
-
 class LTC166X:
     """
-    LTC166X 8 or 10-bit digital to analog converter.
-
-    :param microcontroller.Pin sck: SPI clock pin.
-    :param microcontroller.Pin mosi: SPI output pin.
-    :param microcontroller.Pin csel: SPI chip select pin.
-    :param int bits: DAC bit depth.
-    :param bool debug: Debug the SPI output values.
+    LTC166X 8 or 10-bit digital to analog converter.  This class has a similar
+    interface as the CircuitPython AnalogOut class and can be used in place
+    of that module.
+    :param ~busio.SPI spi: The SPI bus.
+    :param int address: The address of the device if set differently from the default.
     """
 
     def __init__(
         self,
         sck: microcontroller.Pin,
         mosi: microcontroller.Pin,
-        csel: microcontroller.Pin,
+        csld: microcontroller.Pin,
         debug: bool = False,
     ) -> None:
         """ """
         self._num_channels = 8
         self._data_bits = 12
-        self._cs = digitalio.DigitalInOut(csel)
+        self._cs = digitalio.DigitalInOut(csld)
         self._spi = SPI(clock=sck, MOSI=mosi)
         self._bit_depth = None
         self._range = pow(2, self._bit_depth)
         self._device = SPIDevice(
             self._spi, self._cs, baudrate=5000000, polarity=0, phase=0
         )
         self._debug = debug
 
-    def get_bit_depth(self):
-        """
-        Return bit_depth based on device used.
-        """
-        return self._bit_depth
-
     def get_device_range(self):
         """
         Return device range based on device used.
         """
         return self._range
 
-    def sleep(self, dac):
-        """
-        Put DAC in sleep mode.
-        """
-
-    def wake_no_change(self, dac):
-        """
-        Wake DAC with no value updates.
-        """
-
-    def write_chained_dac_values(self, dacs: list):
+    def write_dac_values(self, values):
         """
-        Write list of values to a chain of DACs. All lists should be the same length.
-
-        :param dacs: list of lists of values from 0 to device range. Each list represents a DAC.
-
-        [[DAC 1], [DAC 2], [DAC 3], etc.]
-        """
-        for index, _ in enumerate(dacs[0]):
-            dac_chain_list = [dac[index] for dac in dacs]
-            with self._device as spi:
-                for chain_index, chain_value in enumerate(dac_chain_list):
-                    self.write_value_to_spi(spi, chain_value, chain_index + 1)
-
-    def write_dac_value(self, value: int, address: int):
-        """
-        Write a single DAC value.
-
-        :param value: DAC value from 0 to device range.
-        :param address: DAC address DAC A = 1 ... DAC H = 8 ... ALL DACs = 15
-        """
-        with self._device as spi:
-            self.write_value_to_spi(spi, value, address)
-
-    def write_dac_values(self, values: list):
-        """
-        Write to list of values to DAC.
+        Write to DAC using adafruit_bus_device.
 
         :param values: list of values from 0 to device range.
         """
-        for index, value in enumerate(values):
-            with self._device as spi:
-                self.write_value_to_spi(spi, value, index + 1)
-
-    def write_value_to_spi(self, spi: SPIDevice, value: int, address: int):
-        """
-        Write a single value to SPI.
-
-        :param spi: SPIDevice.
-        :param value: DAC value from 0 to device range.
-        :param address: DAC address DAC A = 1 ... DAC H = 8 ... ALL DACs = 15
-        """
-        assert 0 <= value <= self._range
-        out = 0x0000
-        # Set the top 4 bits to the address based on array position.
-        out |= address << self._data_bits
-        # Set the next n bits based on bit depth.
-        out |= value << (self._data_bits - self._bit_depth)
-        out_bytes = out.to_bytes(2, "big")
-        if self._debug:
-            print(f"{address} {hex(out)} {out_bytes} {len(out_bytes)}")
-        spi.write(out_bytes)
+        with self._device as spi:
+            for idx, value in enumerate(values):
+                assert 0 <= value <= self._range
+                out = 0x0000
+                # Set the top 4 bits to the address based on array position.
+                out |= (idx % self._num_channels) + 1 << self._data_bits
+                # Set the next n bits based on bit depth.
+                out |= value << (self._data_bits - self._bit_depth)
+                out_bytes = out.to_bytes(2, "big")
+                if self._debug:
+                    print(f"{idx} {hex(out)} {out_bytes} {len(out_bytes)}")
+                spi.write(out_bytes)
 
 
 class LTC1660(LTC166X):
     """
     Extended class for 10bit Octal DAC
     """
```

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/examples/creativecontrol_circuitpython_ltc166x_simpletest.py` & `creativecontrol-circuitpython-ltc166x-1.1/examples/creativecontrol_circuitpython_ltc166x_simpletest.py`

 * *Files identical despite different names*

### Comparing `creativecontrol-circuitpython-ltc166x-0.2.0/pyproject.toml` & `creativecontrol-circuitpython-ltc166x-1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "creativecontrol-circuitpython-ltc166x"
 description = "CircuitPython library for control of LTC166X 8-bit and 10-bit DACs."
-version = "0.2.0"
+version = "01.1"
 readme = "README.rst"
 authors = [
     {name = "creativecontrol", email = "t@creativecontrol.cc"}
 ]
 urls = {Homepage = "https://github.com/creativecontrol/creativecontrol_CircuitPython_LTC166X"}
 keywords = [
     "adafruit",
```


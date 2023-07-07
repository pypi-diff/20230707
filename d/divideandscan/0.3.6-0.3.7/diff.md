# Comparing `tmp/divideandscan-0.3.6.tar.gz` & `tmp/divideandscan-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "divideandscan-0.3.6.tar", max compression
+gzip compressed data, was "divideandscan-0.3.7.tar", max compression
```

## Comparing `divideandscan-0.3.6.tar` & `divideandscan-0.3.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1320 2023-03-15 21:18:45.283874 divideandscan-0.3.6/LICENSE
--rw-r--r--   0        0        0    14973 2023-03-15 21:18:45.283874 divideandscan-0.3.6/README.md
--rw-r--r--   0        0        0       29 2023-03-15 21:18:45.283874 divideandscan-0.3.6/das/__init__.py
--rw-r--r--   0        0        0     3895 2023-03-15 21:18:45.283874 divideandscan-0.3.6/das/common.py
--rwxr-xr-x   0        0        0    12421 2023-03-15 21:18:45.283874 divideandscan-0.3.6/das/divideandscan.py
--rw-r--r--   0        0        0     1406 2023-03-15 21:18:45.283874 divideandscan-0.3.6/das/dns.py
--rw-r--r--   0        0        0     7856 2023-03-15 21:18:45.283874 divideandscan-0.3.6/das/drawnmap.py
--rw-r--r--   0        0        0     2247 2023-03-15 21:18:45.283874 divideandscan-0.3.6/das/parsenmap.py
--rw-r--r--   0        0        0     1737 2023-03-15 21:18:45.283874 divideandscan-0.3.6/das/parsers/__init__.py
--rw-r--r--   0        0        0      669 2023-03-15 21:18:45.283874 divideandscan-0.3.6/das/parsers/masscan.py
--rw-r--r--   0        0        0      599 2023-03-15 21:18:45.283874 divideandscan-0.3.6/das/parsers/naabu.py
--rw-r--r--   0        0        0      868 2023-03-15 21:18:45.283874 divideandscan-0.3.6/das/parsers/nimscan.py
--rw-r--r--   0        0        0      648 2023-03-15 21:18:45.283874 divideandscan-0.3.6/das/parsers/nmap.py
--rw-r--r--   0        0        0      660 2023-03-15 21:18:45.283874 divideandscan-0.3.6/das/parsers/rustscan.py
--rw-r--r--   0        0        0      590 2023-03-15 21:18:45.283874 divideandscan-0.3.6/das/parsers/sx.py
--rw-r--r--   0        0        0     9206 2023-03-15 21:18:45.283874 divideandscan-0.3.6/das/report.py
--rw-r--r--   0        0        0     6965 2023-03-15 21:18:45.283874 divideandscan-0.3.6/das/scan.py
--rw-r--r--   0        0        0     1139 2023-03-15 21:18:45.283874 divideandscan-0.3.6/pyproject.toml
--rw-r--r--   0        0        0    16140 1970-01-01 00:00:00.000000 divideandscan-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1320 2023-07-07 21:28:52.598816 divideandscan-0.3.7/LICENSE
+-rw-r--r--   0        0        0    14973 2023-07-07 21:28:52.598816 divideandscan-0.3.7/README.md
+-rw-r--r--   0        0        0       29 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/__init__.py
+-rw-r--r--   0        0        0     3895 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/common.py
+-rwxr-xr-x   0        0        0    12593 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/divideandscan.py
+-rw-r--r--   0        0        0     1406 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/dns.py
+-rw-r--r--   0        0        0     7856 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/drawnmap.py
+-rw-r--r--   0        0        0     2247 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/parsenmap.py
+-rw-r--r--   0        0        0     1737 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/parsers/__init__.py
+-rw-r--r--   0        0        0      669 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/parsers/masscan.py
+-rw-r--r--   0        0        0      599 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/parsers/naabu.py
+-rw-r--r--   0        0        0      868 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/parsers/nimscan.py
+-rw-r--r--   0        0        0      648 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/parsers/nmap.py
+-rw-r--r--   0        0        0      660 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/parsers/rustscan.py
+-rw-r--r--   0        0        0      590 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/parsers/sx.py
+-rw-r--r--   0        0        0     9261 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/report.py
+-rw-r--r--   0        0        0     7144 2023-07-07 21:28:52.602816 divideandscan-0.3.7/das/scan.py
+-rw-r--r--   0        0        0     1139 2023-07-07 21:28:52.602816 divideandscan-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0    16143 1970-01-01 00:00:00.000000 divideandscan-0.3.7/PKG-INFO
```

### Comparing `divideandscan-0.3.6/LICENSE` & `divideandscan-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.6/README.md` & `divideandscan-0.3.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 </p>
 
 <p align="center">
   <strong>Divide <strike>Et Impera</strike> And Scan (and also merge the scan results)</strong>
 </p>
 
 <p align="center">
-  <a href="https://github.com/snovvcrash/DivideAndScan/blob/main/pyproject.toml#L3"><img src="https://img.shields.io/badge/version-0.3.6-success" alt="version" /></a>
+  <a href="https://github.com/snovvcrash/DivideAndScan/blob/main/pyproject.toml#L3"><img src="https://img.shields.io/badge/version-0.3.7-success" alt="version" /></a>
   <a href="https://github.com/snovvcrash/DivideAndScan/search?l=python"><img src="https://img.shields.io/badge/python-3.9-blue?logo=python&logoColor=white" alt="python" /></a>
   <a href="https://www.codacy.com/gh/snovvcrash/DivideAndScan/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=snovvcrash/DivideAndScan&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/35f0bdfece9846d7aab3888b01642813" alt="codacy" /></a>
   <a href="https://github.com/snovvcrash/DivideAndScan/actions/workflows/publish-to-pypi.yml"><img src="https://github.com/snovvcrash/DivideAndScan/actions/workflows/publish-to-pypi.yml/badge.svg" alt="pypi" /></a>
   <a href="https://github.com/snovvcrash/DivideAndScan/actions/workflows/publish-to-docker-hub.yml"><img src="https://github.com/snovvcrash/DivideAndScan/actions/workflows/publish-to-docker-hub.yml/badge.svg" alt="docker" /></a>
 </p>
 
 ---
```

### Comparing `divideandscan-0.3.6/das/common.py` & `divideandscan-0.3.7/das/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 __author__ = '@snovvcrash'
 __site__ = 'https://github.com/snovvcrash/DivideAndScan'
-__version__ = '0.3.6'
+__version__ = '0.3.7'
 
 import time
 from datetime import datetime, timedelta
 
 BANNER = """\
 \033[0;37m -----------------------------------------------------------------------------------------------
 \033[0;37m|\033[1;31m  ________  \033[0;37m.__      .__    .___        \033[1;31m_____\033[0;37m              .__\033[1;31m__________\033[0;37m   \033[1;31m                    |
```

### Comparing `divideandscan-0.3.6/das/divideandscan.py` & `divideandscan-0.3.7/das/divideandscan.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 	  das scan -ports 22 -show -raw
 	  das scan -hosts 192.168.1.0/24,10.10.13.37 -oA report1 -nmap '-Pn -sVC -O'
 	  das -db testdb scan -ports 22,80,443,445 -oA report2 -parallel
 	  das -db testdb scan -ports ports.txt -oA report2 -parallel -proc 4
 	""".replace('\t', '')
 	scan_parser = subparser.add_parser('scan', formatter_class=RawDescriptionHelpFormatter, epilog=scan_epilog, help='run targeted Nmap scans against hosts and ports from DB')
 	scan_parser.add_argument('-nmap', action='store', type=str, default=None, help='custom Nmap options, so the final command will be "sudo nmap <OPTIONS> -oA scan/$output $ip -p$ports" (default is "sudo nmap -Pn -sV --version-intensity 6 -O -oA scan/$output $ip -p$ports")')
+	scan_parser.add_argument('-limit', action='store', type=int, default=None, help='do NOT include hosts whose port list length is less than <LIMIT>')
 	scan_parser.add_argument('-raw', action='store_true', default=False, help='when -show is used, print the results in a raw list (no decorations or colors)')
 	scan_parser.add_argument('-dns', action='store_true', default=False, help='when -hosts and -show are used, include domain names associated with corresponding IP addresses')
 	group_parallel = scan_parser.add_argument_group('parallelism')
 	group_parallel.add_argument('-parallel', action='store_true', default=False, help='run Nmap in multiple processes, number of processes is set with -p (-processes) argument')
 	group_parallel.add_argument('-proc', action='store', type=int, default=None, help='number of parallel Nmap processes (if no value is provided, it will default to the number of processors on the machine)')
 	group_action = scan_parser.add_mutually_exclusive_group(required=True)
 	group_action.add_argument('-show', action='store_true', default=False, help='only show DB data, do not launch Nmap')
@@ -169,31 +170,31 @@
 		output = {'oA': args.oA, 'oX': args.oX, 'oN': args.oN, 'oG': args.oG}
 
 		P = Path.home() / '.das' / 'db' / f'{args.db}.json'
 		if P.exists() and not args.raw:
 			logger.print_info(f'Using DB -> {P.resolve()}')
 
 		if args.show:
-			ss = ScanShow(str(P), args.hosts, args.ports, args.raw)
+			ss = ScanShow(str(P), args.hosts, args.ports, args.limit, args.raw)
 			if args.hosts:
 				ss.nmap_by_hosts(args.dns)
 			elif args.ports:
 				ss.nmap_by_ports()
 
 		elif any(o for o in output.values()):
 			Parallelism = namedtuple('Parallelism', 'enabled processes')
 			parallel = Parallelism(args.parallel, args.proc)
 
-			sr = ScanRun(str(P), args.hosts, args.ports)
+			sr = ScanRun(str(P), args.hosts, args.ports, args.limit)
 			if args.hosts:
 				sr.nmap_by_hosts(args.nmap, parallel)
 			elif args.ports:
 				sr.nmap_by_ports(args.nmap, parallel)
 
-			nm = NmapMerger(args.db, args.hosts, args.ports, output)
+			nm = NmapMerger(str(P), args.hosts, args.ports, output)
 			nm.generate()
 
 	elif args.subparser == 'dns':
 		P = Path.home() / '.das' / 'db' / f'{args.db}.json'
 		if P.exists():
 			logger.print_info(f'Using DB -> {P.resolve()}')
```

### Comparing `divideandscan-0.3.6/das/dns.py` & `divideandscan-0.3.7/das/dns.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.6/das/drawnmap.py` & `divideandscan-0.3.7/das/drawnmap.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.6/das/parsenmap.py` & `divideandscan-0.3.7/das/parsenmap.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.6/das/parsers/__init__.py` & `divideandscan-0.3.7/das/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.6/das/parsers/masscan.py` & `divideandscan-0.3.7/das/parsers/masscan.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.6/das/parsers/naabu.py` & `divideandscan-0.3.7/das/parsers/naabu.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.6/das/parsers/nimscan.py` & `divideandscan-0.3.7/das/parsers/nimscan.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.6/das/parsers/nmap.py` & `divideandscan-0.3.7/das/parsers/nmap.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.6/das/parsers/rustscan.py` & `divideandscan-0.3.7/das/parsers/rustscan.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.6/das/parsers/sx.py` & `divideandscan-0.3.7/das/parsers/sx.py`

 * *Files identical despite different names*

### Comparing `divideandscan-0.3.6/das/report.py` & `divideandscan-0.3.7/das/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,20 +253,24 @@
 		with open(merged_xml, mode='a', encoding='utf-8') as mfd:
 			with open(xml_file) as fd:
 				nmap_xml, n = ET.parse(fd), 0
 				for host in nmap_xml.findall('host'):
 					hostnames = host.find('hostnames')
 					if hostnames is not None:
 						ip = host.find('address').attrib['addr']
-						domains = self.db.search(self.Host.ip == ip)[0]['domains']
-						if domains:
-							for domain in domains:
-								hostname = SubElement(hostnames, 'hostname')
-								hostname.set('name', domain)
-								hostname.set('type', 'A')
+						try:
+							domains = self.db.search(self.Host.ip == ip)[0]['domains']
+						except:
+							pass
+						else:
+							if domains:
+								for domain in domains:
+									hostname = SubElement(hostnames, 'hostname')
+									hostname.set('name', domain)
+									hostname.set('type', 'A')
 
 					chost = ET.tostring(host, encoding='unicode', method='xml')
 					mfd.write(chost)
 					mfd.flush()
 					n += 1
 
 		return n
```

### Comparing `divideandscan-0.3.6/das/scan.py` & `divideandscan-0.3.7/das/scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from das.common import Logger
 
 
 class ScanBase:
 	"""Base class for searching DB and/or initiating Nmap scans."""
 
-	def __init__(self, db_path, hosts, ports, raw_output=False):
+	def __init__(self, db_path, hosts, ports, limit=None, raw_output=False):
 		"""
 		Constructor.
 
 		:param db_path: a TinyDB database file path
 		:type db_path: str
 		:param hosts: a string with comma-separated ip values to interact with ("all" for all the hosts in DB)
 		:type hosts: str
@@ -76,14 +76,15 @@
 
 			self.port_dict = defaultdict(set)
 			for item in result:
 				self.port_dict[item['port']].add(item['ip'])
 
 			self.total_scans += len(self.port_dict)
 
+		self.limit = limit
 		self.raw_output = raw_output
 		if not self.raw_output:
 			Logger.print_info(f'Total scans -> {self.total_scans}')
 
 	@abstractmethod
 	def nmap_by_hosts(self):
 		"""Interface for a DB host searching method."""
@@ -102,14 +103,17 @@
 		"""
 		Search DB by hosts and print mapping "live_host -> [open_ports]". No Nmap scan is launched.
 		
 		:param dns: a boolean flag which, when presented, indicates that domain names associated with corresponding IPs must be printed
 		:type dns: bool
 		"""
 		for ip, ports in sorted(self.ip_dict.items(), key=lambda x: socket.inet_aton(x[0])):
+			if self.limit is not None and len(ports) >= self.limit:
+				continue
+
 			sorted_ports = sorted(ports)
 			if self.raw_output:
 				for port in sorted_ports:
 					print(f'{ip}:{port}')
 			elif dns:
 				domains = self.db.search(self.Host.ip == ip)[0]['domains']
 				domains = f'[{",".join(domains)}]'
@@ -137,14 +141,17 @@
 		:param nmap_opts: custom Nmap options that will replace the default ones
 		:type nmap_opts: str
 		:param parallel: namedtuple('Parallelism', 'enabled processes')
 		:type parallel: collections.namedtuple
 		"""
 		nmap_commands, i = [], 1
 		for ip, ports in sorted(self.ip_dict.items(), key=lambda x: socket.inet_aton(x[0])):
+			if self.limit is not None and len(ports) >= self.limit:
+				continue
+
 			if not parallel.enabled:
 				Logger.print_separator(f'IP: {ip}', prefix=f'{i}/{self.total_scans}')
 
 			nmap_out = ip.replace('.', '-')
 			sorted_ports = ','.join([str(p) for p in sorted(ports)])
 
 			if nmap_opts is None:
```

### Comparing `divideandscan-0.3.6/pyproject.toml` & `divideandscan-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "divideandscan"
-version = "0.3.6"
+version = "0.3.7"
 description = "Divide full port scan results and use it for targeted Nmap runs"
 authors = ["Sam Freeside <snovvcrash@protonmail.ch>"]
 license = "BSD-2-Clause"
 readme = "README.md"
 homepage = "https://github.com/snovvcrash/DivideAndScan"
 repository = "https://github.com/snovvcrash/DivideAndScan"
 keywords = ["pentest", "scan", "nmap", "masscan", "rustscan"]
@@ -20,15 +20,15 @@
 exclude = [".gitignore"]
 
 [tool.poetry.scripts]
 das = 'das.divideandscan:main'
 divideandscan = 'das.divideandscan:main'
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
+python = ">=3.9,<3.12"
 tinydb = "^4.6.1"
 netaddr = "^0.8.0"
 defusedxml = "^0.7.1"
 plotly = "^5.8.2"
 dash = "^2.5.1"
 networkx = "^2.8.4"
 pandas = "^1.4.2"
```

### Comparing `divideandscan-0.3.6/PKG-INFO` & `divideandscan-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: divideandscan
-Version: 0.3.6
+Version: 0.3.7
 Summary: Divide full port scan results and use it for targeted Nmap runs
 Home-page: https://github.com/snovvcrash/DivideAndScan
 License: BSD-2-Clause
 Keywords: pentest,scan,nmap,masscan,rustscan
 Author: Sam Freeside
 Author-email: snovvcrash@protonmail.ch
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Requires-Dist: dash (>=2.5.1,<3.0.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: dnspython (>=2.3.0,<3.0.0)
 Requires-Dist: netaddr (>=0.8.0,<0.9.0)
 Requires-Dist: networkx (>=2.8.4,<3.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
@@ -33,15 +33,15 @@
 </p>
 
 <p align="center">
   <strong>Divide <strike>Et Impera</strike> And Scan (and also merge the scan results)</strong>
 </p>
 
 <p align="center">
-  <a href="https://github.com/snovvcrash/DivideAndScan/blob/main/pyproject.toml#L3"><img src="https://img.shields.io/badge/version-0.3.6-success" alt="version" /></a>
+  <a href="https://github.com/snovvcrash/DivideAndScan/blob/main/pyproject.toml#L3"><img src="https://img.shields.io/badge/version-0.3.7-success" alt="version" /></a>
   <a href="https://github.com/snovvcrash/DivideAndScan/search?l=python"><img src="https://img.shields.io/badge/python-3.9-blue?logo=python&logoColor=white" alt="python" /></a>
   <a href="https://www.codacy.com/gh/snovvcrash/DivideAndScan/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=snovvcrash/DivideAndScan&amp;utm_campaign=Badge_Grade"><img src="https://app.codacy.com/project/badge/Grade/35f0bdfece9846d7aab3888b01642813" alt="codacy" /></a>
   <a href="https://github.com/snovvcrash/DivideAndScan/actions/workflows/publish-to-pypi.yml"><img src="https://github.com/snovvcrash/DivideAndScan/actions/workflows/publish-to-pypi.yml/badge.svg" alt="pypi" /></a>
   <a href="https://github.com/snovvcrash/DivideAndScan/actions/workflows/publish-to-docker-hub.yml"><img src="https://github.com/snovvcrash/DivideAndScan/actions/workflows/publish-to-docker-hub.yml/badge.svg" alt="docker" /></a>
 </p>
 
 ---
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: divideandscan Version: 0.3.6 Summary: Divide full
+Metadata-Version: 2.1 Name: divideandscan Version: 0.3.7 Summary: Divide full
 port scan results and use it for targeted Nmap runs Home-page: https://
 github.com/snovvcrash/DivideAndScan License: BSD-2-Clause Keywords:
 pentest,scan,nmap,masscan,rustscan Author: Sam Freeside Author-email:
-snovvcrash@protonmail.ch Requires-Python: >=3.9,<3.11 Classifier: Environment
+snovvcrash@protonmail.ch Requires-Python: >=3.9,<3.12 Classifier: Environment
 :: Console Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3 Classifier: Topic :: Security Requires-
+Programming Language :: Python :: 3.11 Classifier: Topic :: Security Requires-
 Dist: dash (>=2.5.1,<3.0.0) Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: dnspython (>=2.3.0,<3.0.0) Requires-Dist: netaddr
 (>=0.8.0,<0.9.0) Requires-Dist: networkx (>=2.8.4,<3.0.0) Requires-Dist: pandas
 (>=1.4.2,<2.0.0) Requires-Dist: plotly (>=5.8.2,<6.0.0) Requires-Dist: python-
 nmap (>=0.7.1,<0.8.0) Requires-Dist: scipy (>=1.8.1,<2.0.0) Requires-Dist:
 tinydb (>=4.6.1,<5.0.0) Project-URL: Repository, https://github.com/snovvcrash/
 DivideAndScan Description-Content-Type: text/markdown
```


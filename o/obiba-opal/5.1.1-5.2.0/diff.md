# Comparing `tmp/obiba_opal-5.1.1.tar.gz` & `tmp/obiba_opal-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obiba_opal-5.1.1.tar", max compression
+gzip compressed data, was "obiba_opal-5.2.0.tar", max compression
```

## Comparing `obiba_opal-5.1.1.tar` & `obiba_opal-5.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35147 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/LICENSE.txt
--rw-r--r--   0        0        0     3571 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/README.md
--rw-r--r--   0        0        0     1536 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/obiba_opal/__init__.py
--rw-r--r--   0        0        0     6537 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/obiba_opal/analysis.py
--rwxr-xr-x   0        0        0    13633 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/obiba_opal/console.py
--rwxr-xr-x   0        0        0    19710 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/obiba_opal/core.py
--rwxr-xr-x   0        0        0     7183 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/obiba_opal/data.py
--rwxr-xr-x   0        0        0    14684 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/obiba_opal/dictionary.py
--rw-r--r--   0        0        0    24652 2023-04-28 13:13:51.895934 obiba_opal-5.1.1/obiba_opal/exports.py
--rwxr-xr-x   0        0        0     4776 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/file.py
--rw-r--r--   0        0        0    47546 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/imports.py
--rw-r--r--   0        0        0    12875 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/io.py
--rw-r--r--   0        0        0    34898 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/perm.py
--rwxr-xr-x   0        0        0    11397 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/project.py
--rw-r--r--   0        0        0     1325 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/security.py
--rw-r--r--   0        0        0     4871 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/sql.py
--rwxr-xr-x   0        0        0    10891 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/subjects.py
--rw-r--r--   0        0        0    15854 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/system.py
--rw-r--r--   0        0        0    14338 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/obiba_opal/table.py
--rw-r--r--   0        0        0      804 2023-04-28 13:13:51.899936 obiba_opal-5.1.1/pyproject.toml
--rw-r--r--   0        0        0     4529 1970-01-01 00:00:00.000000 obiba_opal-5.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     3573 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/README.md
+-rw-r--r--   0        0        0     1536 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/__init__.py
+-rw-r--r--   0        0        0     6537 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/analysis.py
+-rwxr-xr-x   0        0        0    14113 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/console.py
+-rwxr-xr-x   0        0        0    19035 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/core.py
+-rwxr-xr-x   0        0        0     7155 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/data.py
+-rwxr-xr-x   0        0        0    14671 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/dictionary.py
+-rw-r--r--   0        0        0    23109 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/exports.py
+-rwxr-xr-x   0        0        0     4730 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/file.py
+-rw-r--r--   0        0        0    47546 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/imports.py
+-rw-r--r--   0        0        0    12920 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/io.py
+-rw-r--r--   0        0        0    34898 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/perm.py
+-rwxr-xr-x   0        0        0    11397 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/project.py
+-rw-r--r--   0        0        0     1325 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/security.py
+-rw-r--r--   0        0        0     4862 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/sql.py
+-rwxr-xr-x   0        0        0    10891 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/subjects.py
+-rw-r--r--   0        0        0    17656 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/system.py
+-rw-r--r--   0        0        0    14315 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/obiba_opal/table.py
+-rw-r--r--   0        0        0      826 2023-07-07 11:42:01.876052 obiba_opal-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4568 1970-01-01 00:00:00.000000 obiba_opal-5.2.0/PKG-INFO
```

### Comparing `obiba_opal-5.1.1/LICENSE.txt` & `obiba_opal-5.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.1/README.md` & `obiba_opal-5.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 # on Debian systems
 sudo apt-get install python3-pycurl
 
 # on RPM systems
 sudo yum install python3-pycurl
 ```
 
+### CLI
+
 To get the options of the command line:
 
 ```shell
 opal --help
 ```
 
 This command will display which sub-commands are available. For each sub-command you can get the help message as well:
@@ -39,15 +41,15 @@
 ```shell
 opal <subcommand> --help
 ```
 
 The objective of having sub-command is to hide the complexity of applying some use cases to the Opal REST API. More
 sub-commands will be developed in the future.
 
-## Development
+### API
 
 Opal Python client can be easily extended by using the [exposed classes](https://github.com/obiba/opal-python-client/blob/master/obiba_opal/__init__.py). The classes `*Command` return an Opal task object, to be followed with the `TaskService`. The classes `*Service` perform immediate operations. 
 
 ```python
 from obiba_opal import OpalClient, HTTPError, Formatter, ImportCSVCommand, TaskService, FileService, DictionaryService
 
 # if 2-factor auth is enabled, user will be asked for the secret code
```

### Comparing `obiba_opal-5.1.1/obiba_opal/__init__.py` & `obiba_opal-5.2.0/obiba_opal/__init__.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.1/obiba_opal/analysis.py` & `obiba_opal-5.2.0/obiba_opal/analysis.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.1/obiba_opal/console.py` & `obiba_opal-5.2.0/obiba_opal/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #
 # Opal commands main entry point
 #
 import argparse
 import sys
+import getpass
 
 from obiba_opal.core import Formatter, HTTPError
 from obiba_opal.project import ProjectService, BackupProjectCommand, RestoreProjectCommand
 from obiba_opal.table import CopyTableCommand, DeleteTableService, BackupViewService, RestoreViewService
 from obiba_opal.dictionary import DictionaryService, ExportAnnotationsService, ImportAnnotationsService
 from obiba_opal.data import DataService, EntityService
 from obiba_opal.analysis import AnalysisCommand, ExportAnalysisService
@@ -15,31 +16,33 @@
 from obiba_opal.subjects import UserService, GroupService
 from obiba_opal.perm import ProjectPermService, DatasourcePermService, TablePermService, VariablePermService, ResourcePermService, ResourcesPermService, RPermService, DataSHIELDPermService, SystemPermService
 from obiba_opal.imports import ImportPluginCommand, ImportCSVCommand, ImportIDMapService, ImportIDService, ImportLimeSurveyCommand, ImportOpalCommand, ImportRDSCommand, ImportRSASCommand, ImportRSPSSCommand, ImportRSTATACommand, ImportSQLCommand, ImportVCFCommand, ImportXMLCommand
 from obiba_opal.system import PluginService, SystemService, TaxonomyService, TaskService, RESTService
 from obiba_opal.sql import SQLService, SQLHistoryService
 from obiba_opal.security import EncryptService, DecryptService
 
+def prompt_password():
+    return getpass.getpass(prompt='Enter password: ')
 
 def add_opal_arguments(parser):
     """
     Add Opal access arguments
     """
     parser.add_argument('--opal', '-o', required=False, default='http://localhost:8080',
                         help='Opal server base url (default: http://localhost:8080)')
     parser.add_argument('--user', '-u', required=False, help='Credentials auth: user name (requires a password)')
-    parser.add_argument('--password', '-p', required=False,
+    parser.add_argument('--password', '-p', required=False, nargs="?",
                         help='Credentials auth: user password (requires a user name)')
     parser.add_argument('--token', '-tk', required=False, help='Token auth: User access token')
     parser.add_argument('--ssl-cert', '-sc', required=False,
                         help='Two-way SSL auth: certificate/public key file (requires a private key)')
     parser.add_argument('--ssl-key', '-sk', required=False,
                         help='Two-way SSL auth: private key file (requires a certificate)')
     parser.add_argument('--verbose', '-v', action='store_true', help='Verbose output')
-
+    parser.add_argument('--no-ssl-verify', '-nv', action='store_true', help='Do not verify SSL certificates for HTTPS.')
 
 def add_subcommand(subparsers, name, help, add_args_func, default_func):
     """
     Make a sub-parser, add default arguments to it, add sub-command arguments and set the sub-command callback function.
     """
     subparser = subparsers.add_parser(name, help=help)
     add_opal_arguments(subparser)
@@ -167,16 +170,21 @@
                   SQLService.do_command)
     add_subcommand(subparsers, 'sql-history', 'SQL execution history of current user or of other users (administrator only).',
                   SQLHistoryService.add_arguments,
                   SQLHistoryService.do_command)
 
     # Execute selected command
     args = parser.parse_args()
+
     if hasattr(args, 'func'):
         try:
+          # Prompt for a missing password only when user/password is required
+          if not (args.ssl_cert or args.ssl_key) and not args.token:
+            if not args.password or len(args.password) == 0:
+              args.password = prompt_password()
           args.func(args)
         except HTTPError as e:
             Formatter.print_json(e.error, args.json if hasattr(args, 'json') else False)
             sys.exit(2)
         except Exception as e:
             if hasattr(e, 'message'):
                 print(e.message)
```

### Comparing `obiba_opal-5.1.1/obiba_opal/core.py` & `obiba_opal-5.2.0/obiba_opal/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,198 +1,209 @@
 """
-Based on PyCurl http://pycurl.sourceforge.net/
-See also http://www.angryobjects.com/2011/10/15/http-with-python-pycurl-by-example/
-Curl options http://curl.haxx.se/libcurl/c/curl_easy_setopt.html
+Based on Python Request library https://docs.python-requests.org/en/latest/index.html
 """
 
-import random
 import base64
 import getpass
 import json
 import os
-import pycurl
+from requests import Session, Request, Response
 import urllib.error
 import urllib.parse
 import urllib.request
 from functools import reduce
 from http import HTTPStatus
-
+from http.client import HTTPConnection
 
 class OpalClient:
     """
     OpalClient holds the configuration for connecting to Opal.
     """
 
     def __init__(self, server=None):
-        self.curl_options = {}
+        self.session = Session()
         self.headers = {}
         self.base_url = self.__ensure_entry('Opal address', server)
         self.id = None
         self.rid = None
 
+    def __del__(self):
+        self.close()
+
     @classmethod
     def build(cls, loginInfo):
+        """
+        Creates a client instance
+
+        :param loginInfo - login related information
+        """
         if loginInfo.isSsl():
             return OpalClient.buildWithCertificate(loginInfo.data['server'], loginInfo.data['cert'],
-                                                   loginInfo.data['key'])
+                                                   loginInfo.data['key'], loginInfo.data['no_ssl_verify'])
         elif loginInfo.isToken():
-            return OpalClient.buildWithToken(loginInfo.data['server'], loginInfo.data['token'])
+            return OpalClient.buildWithToken(loginInfo.data['server'], loginInfo.data['token'], loginInfo.data['no_ssl_verify'])
         else:
             return OpalClient.buildWithAuthentication(loginInfo.data['server'], loginInfo.data['user'],
-                                                      loginInfo.data['password'])
+                                                      loginInfo.data['password'], loginInfo.data['no_ssl_verify'])
 
     @classmethod
-    def buildWithCertificate(cls, server, cert, key):
+    def buildWithCertificate(cls, server, cert, key, no_ssl_verify: bool = False):
+        """
+        Creates a client instance authenticated by a certificate/key combination
+
+        :param server - Opal server address
+        :param cert - public certificate/key (must be named as 'publickey.pem')
+        :param key - private key (must be named as 'privatekey.pem')
+        :param no_ssl_verify - if True, the SSL certificate is not verified (not recommended)
+        """
+
         client = cls(server)
         if client.base_url.startswith('https:'):
-            client.verify_peer(0)
-            client.verify_host(0)
-        client.keys(cert, key)
+            client.session.verify = False if no_ssl_verify else True
+        client.session.cert = (cert, key)
+
         return client
 
     @classmethod
-    def buildWithAuthentication(cls, server, user, password):
+    def buildWithAuthentication(cls, server, user, password, no_ssl_verify: bool = False):
+        """
+        Creates a client instance authenticated by a user/password
+
+        :param server - Opal server address
+        :param user - username
+        :param password - user password
+        :param no_ssl_verify - if True, the SSL certificate is not verified (not recommended)
+        """
         client = cls(server)
         if client.base_url.startswith('https:'):
-            client.verify_peer(0)
-            client.verify_host(0)
+            client.session.verify = False if no_ssl_verify else True
         client.credentials(user, password)
-    
+
         # need to know whether a OTP is needed
         try:
             client.init_otp()
         except Exception as e:
             # do the close as the exception is raised in the builder
             client.close()
             raise e
-        
+
         return client
 
     @classmethod
-    def buildWithToken(cls, server, token):
+    def buildWithToken(cls, server, token, no_ssl_verify: bool = False):
+        """
+        Creates a client instance authenticated by a token configured by an Opal user
+
+        :param server - Opal server address
+        :param token - token key
+        :param no_ssl_verify - if True, the SSL certificate is not verified (not recommended)
+        """
         client = cls(server)
         if client.base_url.startswith('https:'):
-            client.verify_peer(0)
-            client.verify_host(0)
+            client.session.verify = False if no_ssl_verify else True
         client.token(token)
         return client
 
     def __ensure_entry(self, text, entry, pwd=False):
         e = entry
         if not entry:
             if pwd:
                 e = getpass.getpass(prompt=text + ': ')
             else:
                 e = input(text + ': ')
         return e
 
     def credentials(self, user, password):
+        """
+        Creates the authorization header and attempts to input the required user/password
+
+        :param user - username
+        :param password - user password
+        """
         u = self.__ensure_entry('User name', user)
         p = self.__ensure_entry('Password', password, True)
-        return self.header('Authorization', 'Basic ' + base64.b64encode((u + ':' + p).encode('utf-8')).decode('utf-8'))
+        return self.header('Authorization', 'Basic ' + base64.b64encode('{}:{}'.format(u, p).encode('utf-8')).decode('utf-8'))
 
     def token(self, token):
+        """
+        Creates the authorization header and attempts to input the required token
+
+        :param token - token key
+        """
         tk = self.__ensure_entry('Token', token, True)
         return self.header('X-Opal-Auth', tk)
 
     def init_otp(self):
-        # check if an OTP is needed
+        """
+        Checks if an OTP is needed and if yes, prompts the user for the security code
+        """
         request = self.new_request()
         profile_url = '/system/subject-profile/_current'
         response = request.accept_json().get().resource(profile_url).send()
         if response.code == 401:
             otp_header = response.get_header('WWW-Authenticate').split(' ')[0]
             if otp_header == 'X-Opal-TOTP' or otp_header == 'X-Obiba-TOTP':
                 val = input('Enter 6-digits code: ')
                 # validate code and get the opalsid cookie for further requests
                 request = self.new_request()
                 request.header(otp_header, val).accept_json().get().resource(profile_url).send()
 
-    def keys(self, cert_file, key_file, key_pwd=None, ca_certs=None):
-        self.curl_option(pycurl.SSLCERT, cert_file)
-        self.curl_option(pycurl.SSLKEY, key_file)
-        if key_pwd:
-            self.curl_option(pycurl.KEYPASSWD, key_pwd)
-        if ca_certs:
-            self.curl_option(pycurl.CAINFO, ca_certs)
-        self.headers.pop('Authorization', None)
-        return self
-
-    def verify_peer(self, verify):
-        return self.curl_option(pycurl.SSL_VERIFYPEER, verify)
-
-    def verify_host(self, verify):
-        return self.curl_option(pycurl.SSL_VERIFYHOST, verify)
-
-    def ssl_version(self, version):
-        return self.curl_option(pycurl.SSLVERSION, version)
-
-    def curl_option(self, opt, value):
-        self.curl_options[opt] = value
+    def verify(self, value):
+        """
+        Ignore or validate certificate
+
+        :param value = True/False to validation or not. Value can also be a CA_BUNDLE file or directory (e.g. 'verify=/etc/ssl/certs/ca-certificates.crt')
+        """
+        self.session.verify = value
         return self
 
     def header(self, key, value):
-        self.headers[key] = value
+        """
+        Adds a header to session headers used by the request
+
+        :param key - header key
+        :param value - header value
+        """
+        header = {}
+        header[key] = value
+
+        self.session.headers.update(header)
         return self
 
     def new_request(self):
-        if self.id is None:
-            # iterate until file does not exists
-            self.id = random.choice(list(range(1, 999999, 1)))
-            self.cookie_file = "%s/opal-cookie-%s.dat" % (self.get_app_workdir(), self.id)
-            while os.path.exists(self.cookie_file):
-                self.id = random.choice(list(range(1, 999999, 1)))
-                self.cookie_file = "/tmp/opal-cookie-%s.dat" % self.id
         return OpalRequest(self)
 
-    def get_app_home(self):
-        app_home = os.environ['OBIBA_HOME'] if 'OBIBA_HOME' in os.environ else None
-        if not app_home:
-            app_home = '/tmp/.obiba'
-            try:
-                app_home = os.path.expanduser('~/.obiba')
-            except Exception as e:
-                pass
-        
-        os.makedirs(app_home, exist_ok=True)
-        return app_home
-
-    def get_app_workdir(self):
-        app_home = self.get_app_home()
-        workdir = '%s/work' % app_home
-        os.makedirs(workdir, exist_ok=True)
-        return workdir
-
     def close(self):
         if self.id is not None:
             # request to close session
             try:
                 self.new_request().resource('/auth/session/_current').delete().send()
+                self.session.close()
             except Exception as e:
                 pass
             self.id = None
-        if self.cookie_file:
-            try:
-                os.remove(self.cookie_file)
-            except OSError:
-                pass
-        
+
     class LoginInfo:
+        """
+        Class used to parse and hold the login info
+        """
         data = None
 
         @classmethod
         def parse(cls, args):
             data = {}
             argv = vars(args)
 
             if argv.get('opal'):
                 data['server'] = argv['opal']
             else:
                 raise ValueError('Opal server information is missing.')
 
+            data['no_ssl_verify'] = argv.get('no_ssl_verify')
+
             if argv.get('user') and argv.get('password'):
                 data['user'] = argv['user']
                 data['password'] = argv['password']
             elif argv.get('token'):
                 data['token'] = argv['token']
             elif argv.get('ssl_cert') and argv.get('ssl_key'):
                 data['cert'] = argv['ssl_cert']
@@ -218,57 +229,73 @@
 class OpalRequest:
     """
     Opal request.
     """
 
     def __init__(self, opal_client):
         self.client = opal_client
-        self.curl_options = {}
+        self.options = {}
         self.headers = {'Accept': 'application/json'}
         self._verbose = False
+        self.params = {}
         self._fail_on_error = False
-
-    def curl_option(self, opt, value):
-        self.curl_options[opt] = value
-        return self
+        self.files = None
+        self.data = None
 
     def timeout(self, value):
-        return self.curl_option(pycurl.TIMEOUT, value)
-
-    def connection_timeout(self, value):
-        return self.curl_option(pycurl.CONNECTTIMEOUT, value)
+        """
+        Sets the connection and read timeout
+        Note: value can be a tupple to have different timeouts for connection and reading (connTimout, readTimeout)
+
+        :param value - connection/read timout
+        """
+        self.options['timeout'] = value
+        return self
 
     def verbose(self):
+        """
+        Enables the verbose mode
+        """
+        HTTPConnection.debuglevel = 1
         self._verbose = True
-        return self.curl_option(pycurl.VERBOSE, True)
+        return self
 
     def fail_on_error(self):
-        #return self.curl_option(pycurl.FAILONERROR, True)
         self._fail_on_error = True
         return self
 
     def header(self, key, value):
+        """
+        Adds a header to session headers used by the request
+
+        :param key - header key
+        :param value - header value
+        """
         if value:
-            self.headers[key] = value
+            header = {}
+            header[key] = value
+            self.headers.update(header)
         return self
 
     def accept(self, value):
-        return self.header('Accept', value)
+        self.headers.update({'Accept': value})
+        return self
 
     def accept_json(self):
         return self.accept('application/json')
 
     def accept_xml(self):
         return self.accept('application/xml')
 
     def accept_text_csv(self):
         return self.accept('text/csv')
 
     def content_type(self, value):
-        return self.header('Content-Type', value)
+        self.headers.update({'Content-Type': value})
+        return self
 
     def content_type_json(self):
         return self.content_type('application/json')
 
     def content_type_text_plain(self):
         return self.content_type('text/plain')
 
@@ -298,188 +325,155 @@
 
     def delete(self):
         return self.method('DELETE')
 
     def options(self):
         return self.method('OPTIONS')
 
-    def __build_request(self):
-        curl = pycurl.Curl()
-        # curl options
-        for o in self.client.curl_options:
-            curl.setopt(o, self.client.curl_options[o])
-        for o in self.curl_options:
-            curl.setopt(o, self.curl_options[o])
-            # headers
-        hlist = []
-        for h in self.client.headers:
-            hlist.append(h + ": " + self.client.headers[h])
-        for h in self.headers:
-            hlist.append(h + ": " + self.headers[h])
-        curl.setopt(pycurl.HTTPHEADER, hlist)
-        if self.method:
-            curl.setopt(pycurl.CUSTOMREQUEST, self.method)
-        if self.resource:
-            curl.setopt(pycurl.URL, self.client.base_url + '/ws' + self.resource)
-        else:
-            raise ValueError('Resource is missing')
-        return curl
-
     def resource(self, ws):
         self.resource = ws
         return self
 
     def content(self, content):
+        """
+        Stores the request body
+
+        :param content - request body
+        """
         if self._verbose:
             print('* Content:')
             print(content)
-        encodedContent = content.encode('utf-8')
-        self.curl_option(pycurl.POST, 1)
-        self.curl_option(pycurl.POSTFIELDSIZE, len(encodedContent))
-        self.curl_option(pycurl.POSTFIELDS, encodedContent)
-        return self
 
-    def content_file(self, filename):
-        if self._verbose:
-            print('* File Content:')
-            print('[file=' + filename + ', size=' + str(os.path.getsize(filename)) + ']')
-        self.curl_option(pycurl.POST, 1)
-        self.curl_option(pycurl.POSTFIELDSIZE, os.path.getsize(filename))
-        reader = open(filename, 'rb')
-        self.curl_option(pycurl.READFUNCTION, reader.read)
+        self.data = content.encode('utf-8')
         return self
 
     def content_upload(self, filename):
-        path = os.path.expanduser(filename)
+        """
+        Sets the file associate with the upload
+
+        Note: Requests library takes care of mutlti-part setting in the header
+        """
         if self._verbose:
             print('* File Content:')
-            print('[file=' + filename + ', size=' + str(os.path.getsize(path)) + ']')
-            # self.curl_option(pycurl.POST,1)
-        self.curl_option(pycurl.HTTPPOST, [('file1', (pycurl.FORM_FILE, path))])
+            print('[file=' + filename + ', size=' + str(os.path.getsize(filename)) + ']')
+        self.files = {'file': (os.path.basename(filename), open(filename, 'rb'))}
         return self
 
-    def send(self, buffer=None):
-        curl = self.__build_request()
-        hbuf = HeaderStorage()
-        cbuf = Storage()
-        if buffer:
-            curl.setopt(curl.WRITEFUNCTION, buffer.write)
-        else:
-            curl.setopt(curl.WRITEFUNCTION, cbuf.store)
-        curl.setopt(curl.HEADERFUNCTION, hbuf.store)
-        curl.setopt(curl.COOKIEJAR, self.client.cookie_file)
-        curl.setopt(curl.COOKIEFILE, self.client.cookie_file)
-        curl.perform()
-        response = OpalResponse(curl.getinfo(pycurl.HTTP_CODE), hbuf.headers, cbuf.content.decode('utf-8'))
-        curl.close()
+    def __build_request(self):
+        request = Request()
+        request.method = self.method if self.method else 'GET'
 
-        if self._fail_on_error and response.code >= 400:
-            raise HTTPError(response)
+        for option in self.options:
+            setattr(request, option, self.options[option])
 
-        return response
+        # Combine the client and the request headers
+        request.headers = {}
+        request.headers.update(self.client.session.headers)
+        request.headers.update(self.headers)
 
-class Storage:
-    """
-    Content storage.
-    """
+        if self.resource:
+            path = self.resource
+            request.url = self.client.base_url + '/ws' + path
 
-    def __init__(self):
-        self.content = bytearray()
-        self.line = 0
-
-    def store(self, buf):
-        self.line = self.line + 1
-        self.content = self.content + buf
+            if self.params:
+                request.params = self.params
+        else:
+            raise ValueError('Resource is missing')
 
-    def __str__(self):
-        return self.contents.decode('utf-8')
+        if self.files is not None:
+            request.files = self.files
 
+        if self.data is not None:
+            request.data = self.data
 
-class HeaderStorage(Storage):
-    """
-    Store response headers in a dictionary: key is the header name,
-    value is header value or the list of header values.
-    """
+        return request
 
-    def __init__(self):
-        Storage.__init__(self)
-        self.headers = {}
+    def send(self, fp = None):
+        """
+        Sends the request via client session object
+        """
+        request = self.__build_request()
+        response = OpalResponse(self.client.session.send(request.prepare()))
 
-    def store(self, buf):
-        Storage.store(self, buf)
-        header = buf.decode('utf-8').partition(':')
-        if header[1]:
-            value = header[2].rstrip().strip()
-            if header[0] in self.headers:
-                current_value = self.headers[header[0]]
-                if isinstance(current_value, str):
-                    self.headers[header[0]] = list(current_value)
-                self.headers[header[0]].append(value)
-            else:
-                self.headers[header[0]] = value
+        if self._fail_on_error and response.code >= 400:
+            raise HTTPError(response)
 
+        if fp is not None:
+            fp.write(response.content)
+
+        return response
 
 class OpalResponse:
     """
     Response from Opal: code, headers and content
     """
 
-    def __init__(self, code, headers, content):
-        self.code = code
-        self.headers = headers
-        self.content = content
+    def __init__(self, response: Response = Response()):
+        self.response = response
+
+    @property
+    def code(self):
+        return self.response.status_code
+
+    @property
+    def headers(self):
+        return self.response.headers
+
+    @property
+    def content(self):
+        return self.response.content
 
     def from_json(self):
-        if self.content is None:
+        if self.response is None or self.response.content is None:
             return None
         else:
             try:
-                return json.loads(self.content)
+                return self.response.json()
             except Exception as e:
                 if type(self.content) == str:
-                    return self.content
+                    return self.response.content
                 else:
                     # FIXME silently fail
                     return None
 
     def pretty_json(self):
         return json.dumps(self.from_json(), sort_keys=True, indent=2)
 
     def get_header(self, header: str) -> str:
         value = None
-        if header in self.headers:
-            value = self.headers[header]
-        elif header.lower() in self.headers:
-            value = self.headers[header.lower()]
+        if header in self.response.headers:
+            value = self.response.headers[header]
+        elif header.lower() in self.response.headers:
+            value = self.response.headers[header.lower()]
         return value
 
     def get_location(self):
         return self.get_header('Location')
 
     def extract_cookie_value(self, name: str):
-        if 'set-cookie' in self.headers:
-            if type(self.headers['set-cookie']) == str:
-                return self._extract_cookie_single_value(name, self.headers['set-cookie'])
+        if 'set-cookie' in self.response.headers:
+            if type(self.response.headers['set-cookie']) == str:
+                return self._extract_cookie_single_value(name, self.response.headers['set-cookie'])
             else:
-                for header in self.headers['set-cookie']:
+                for header in self.response.headers['set-cookie']:
                     rval = self._extract_cookie_single_value(name, header)
                     if rval is not None:
                         return rval
         return None
 
     def _extract_cookie_single_value(self, name: str, header: str):
         cookie_parts = header.split(';')
         if len(cookie_parts) > 0:
             cookie_parts = cookie_parts[0].split('=')
             if len(cookie_parts) == 2 and cookie_parts[0] == name:
                 return cookie_parts[1]
         return None
 
     def __str__(self):
-        return self.content
+        return self.response.content.decode('utf-8')
 
 class Formatter:
 
     @classmethod
     def to_json(self, data: any, pretty: bool = False):
         if pretty:
             return json.dumps(data, sort_keys=True, indent=2)
@@ -601,23 +595,23 @@
         else:
             return p
 
     def build(self):
         return self.__str__()
 
 class HTTPError(Exception):
-    def __init__(self, response: OpalResponse, message: str = None):            
+    def __init__(self, response: OpalResponse, message: str = None):
         # Call the base class constructor with the parameters it needs
         super().__init__(message if message else 'HTTP Error: %s' % response.code)
         self.code = response.code
         http_status = [x for x in list(HTTPStatus) if x.value == response.code][0]
         self.message = message if message else '%s: %s' % (http_status.phrase, http_status.description)
-        self.error = response.from_json() if response.content else { 'code': response.code, 'status': self.message }
+        self.error = response.from_json() if response.content else {'code': response.code, 'status': self.message}
         # case the reported error is not a dict
         if type(self.error) != dict:
-            self.error = { 'code': response.code, 'status': self.error }
+            self.error = {'code': response.code, 'status': self.error}
 
     def is_client_error(self) -> bool:
         return self.code >= 400 and self.code < 500
-    
+
     def is_server_error(self) -> bool:
-        return self.code >= 500
+        return self.code >= 500
```

### Comparing `obiba_opal-5.1.1/obiba_opal/data.py` & `obiba_opal-5.2.0/obiba_opal/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,28 +72,28 @@
         :param project: The project name
         :param table: The table name
         :param id: The entity identifier
         :param pos: Position of the value to query in case of a repeatable variable (starting at 0)
         :param fd: Get raw value into the provided file descriptor (see os.fdopen()), useful for downloading a binary value
         """
         return self._get_data('%s.%s:%s' % (project, table, variable), id, pos, fd)
-    
+
     def _get_data(self, name: str, id: str = None, pos: str = None, fd = None) -> any:
         """
         Execute data command
 
         :param name: Fully qualified name of a table or a variable, for instance: opal-data.questionnaire or opal-data.questionnaire:Q1
         :param id: Entity identifier. If missing the list of entities is returned
         :param pos: Position of the value to query in case of a repeatable variable (starting at 0)
         :param fd: Get raw value into the provided file descriptor (see os.fdopen()), useful for downloading a binary value
         """
         request = self.client.new_request()
         if self.verbose:
             request.verbose()
-        
+
         resolver = core.MagmaNameResolver(name)
         raw = resolver.is_variable() and id and fd is not None
         ws = self._make_ws(resolver, id, pos, raw)
         request.fail_on_error().get().resource(ws)
         if raw:
             fp = os.fdopen(fd, 'wb')
             response = request.accept('*/*').send(fp)
@@ -102,15 +102,15 @@
         else:
             response = request.send()
             return response.from_json()
 
     def _make_ws(self, resolver: core.MagmaNameResolver, id: str = None, pos: str = None, raw: bool = False):
         """
         Build the web service resource path
-        """        
+        """
         ws = resolver.get_table_ws()
         if id:
             ws = '%s/valueSet/%s' % (ws, id)
             if resolver.is_variable():
                 ws = '%s/variable/%s' % (ws, resolver.variable)
                 if raw:
                     ws = '%s/value' % ws
@@ -149,15 +149,15 @@
         client = core.OpalClient.build(core.OpalClient.LoginInfo.parse(args))
         try:
             res = None
             if args.tables:
                 res = EntityService(client, args.verbose).get_entity_tables(args.id, args.type)
             else:
                 res = EntityService(client, args.verbose).get_entity(args.id, args.type)
-        
+
             # format response
             core.Formatter.print_json(res, args.json)
         finally:
             client.close()
 
     def get_entity(self, id: str, type: str = None) -> dict:
         request = self.client.new_request()
```

### Comparing `obiba_opal-5.1.1/obiba_opal/dictionary.py` & `obiba_opal-5.2.0/obiba_opal/dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         """
         Execute variable command
         """
         # Build and send request
         client = core.OpalClient.build(core.OpalClient.LoginInfo.parse(args))
         try:
             res = DictionaryService(client, args.verbose)._get_dictionary(args.name)
-        
+
             # format response
             core.Formatter.print_json(res, args.json)
         finally:
             client.close()
 
     def get_datasources(self) -> list:
         """
@@ -54,19 +54,19 @@
     def get_datasource(self, project: str) -> dict:
         """
         Get a datasource.
 
         :param project: The project name associated to the datasource
         """
         return self._get_dictionary(project)
-    
+
     def get_tables(self, project: str) -> list:
         """
         Get the tables of a datasource.
-        
+
         :param project: The project name associated to the datasource
         """
         return self._get_dictionary('%s.*' % project)
 
     def get_table(self, project: str, table: str) -> dict:
         """
         Get a table of a datasource.
@@ -90,29 +90,29 @@
         Get a variable of a table in a datasource.
 
         :param project: The project name associated to the datasource
         :param table: The table name
         :param variable: The variable name
         """
         return self._get_dictionary('%s.%s:%s' % (project, table, variable))
-    
+
     def delete_tables(self, project: str, tables: list = None):
         """
         Delete provided or all tables.
 
         :param client: Opal connection object
         :param project: The project name
         :param tables: List of table names to be deleted (default is all)
         :param verbose: Verbose requests
         """
         tables_ = tables
         if not tables:
             tables_ = self.get_tables(project)
             tables_ = [x['name'] for x in tables_]
-        
+
         for table in tables_:
             request = self.client.new_request()
             if self.verbose:
                 request.verbose()
             request.fail_on_error().delete().resource(core.UriBuilder(['datasource', project, 'table', table]).build()).send()
 
     def _get_dictionary(self, name: str) -> any:
@@ -233,15 +233,15 @@
     """
     Import dictionary annotations from previous export.
     """
 
     def __init__(self, client: core.OpalClient, verbose: bool = False):
         self.client = client
         self.verbose = verbose
-    
+
     @classmethod
     def add_arguments(cls, parser):
         """
         Add command specific options
         """
         parser.add_argument('--input', '-in',
                             help='CSV/TSV input file, typically the output of the "export-annot" command (default is stdin)',
@@ -295,16 +295,16 @@
         if locale:
             params['locale'] = locale
 
         builder = core.UriBuilder(['datasource', datasource, 'table', table, 'variables', '_attribute'], params=params)
         form = '&'.join([urllib.parse.urlencode({'variable': x}) for x in variables])
         if self.verbose:
             request.verbose()
-        
-        request.put().resource(builder.build()).content(form).send()
+
+        request.put().resource(builder.build()).content_type_form_urlencoded().content(form).send()
 
     def _append_row(self, dictionary, row, tables=None, taxonomies=None):
         if row[0] not in dictionary:
             dictionary[row[0]] = {}
         self._append_table(dictionary, row, tables, taxonomies)
 
     def _append_table(self, dictionary, row, tables=None, taxonomies=None):
```

### Comparing `obiba_opal-5.1.1/obiba_opal/exports.py` & `obiba_opal-5.2.0/obiba_opal/exports.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,71 +17,67 @@
         """
         Add data command specific options
         """
         parser.add_argument('--datasource', '-d', required=True, help='Project name')
         parser.add_argument('--tables', '-t', nargs='+', required=True, help='The list of tables to be exported')
         parser.add_argument('--name', '-n', required=True, help='Opal datasource plugin name')
         parser.add_argument('--config', '-c', required=True, help='A JSON file containing the export configuration')
-        parser.add_argument('--incremental', '-i', action='store_true', help='Incremental export')
         parser.add_argument('--identifiers', '-id', required=False, help='Name of the ID mapping')
         parser.add_argument('--json', '-j', action='store_true', help='Pretty JSON formatting of the response')
 
     @classmethod
     def do_command(cls, args):
         """
         Execute export data command
         """
         # Build and send request
         client = core.OpalClient.build(core.OpalClient.LoginInfo.parse(args))
         config = json.loads(open(args.config).read())
         try:
             res = cls(client, args.verbose) \
-                .export(args.name, args.datasource, args.tables, config, args.identifiers, args.incremental)
+                .export_data(args.name, args.datasource, args.tables, config, args.identifiers)
             # format response
             core.Formatter.print_json(res, args.json)
         finally:
             client.close()
 
-    def export_data(self, name: str, project: str, tables: list, config: str, identifiers: str = None, incremental: bool = False) -> dict:
+    def export_data(self, name: str, project: str, tables: list, config: str, identifiers: str = None) -> dict:
         """
         Export tables using a plugin.
 
         :param name: The name of the plugin.
         :param project: The project name
         :param tables: The table names to export
         :param config: The plugin configuration dictionary
         :param identifiers: The name of the ID mapping
-        :param incremental: Incremental export
         """
         configStr = json.dumps(config)
-        exporter = io.OpalExporter.build(client=self.client, datasource=project , tables=tables, 
+        exporter = io.OpalExporter.build(client=self.client, datasource=project , tables=tables,
                                          identifiers=identifiers, output=configStr,
-                                         incremental=incremental,
                                          verbose=self.verbose)
         response = exporter.submit(name)
         return response.from_json()
 
 class ExportCSVCommand:
     """
     Export some tables in CSV format.
     """
 
     def __init__(self, client: core.OpalClient, verbose: bool = False):
         self.client = client
         self.verbose = verbose
-    
+
     @classmethod
     def add_arguments(cls, parser):
         """
         Add data command specific options
         """
         parser.add_argument('--datasource', '-d', required=True, help='Project name')
         parser.add_argument('--tables', '-t', nargs='+', required=True, help='The list of tables to be exported')
         parser.add_argument('--output', '-out', required=True, help='Output directory name')
-        parser.add_argument('--incremental', '-i', action='store_true', help='Incremental export')
         parser.add_argument('--id-name', '-in', required=False, help='Name of the ID column name')
         parser.add_argument('--identifiers', '-id', required=False, help='Name of the ID mapping')
         parser.add_argument('--no-multilines', '-nl', action='store_true',
                             help='Do not write value sequences as multiple lines')
         parser.add_argument('--json', '-j', action='store_true', help='Pretty JSON formatting of the response')
 
     @classmethod
@@ -89,35 +85,33 @@
         """
         Execute export data command
         """
         # Build and send request
         client = core.OpalClient.build(core.OpalClient.LoginInfo.parse(args))
         try:
             res = cls(client, args.verbose) \
-                .export(args.datasource, args.tables, args.output, args.id_name, args.identifiers, args.incremental, not args.no_multilines)
+                .export_data(args.datasource, args.tables, args.output, args.id_name, args.identifiers, not args.no_multilines)
             # format response
             core.Formatter.print_json(res, args.json)
         finally:
             client.close()
 
-    def export_data(self, project: str, tables: list, output: str, id_name: str = None, identifiers: str = None, incremental: bool = False, multilines: bool = True) -> dict:
+    def export_data(self, project: str, tables: list, output: str, id_name: str = None, identifiers: str = None, multilines: bool = True) -> dict:
         """
         Export tables in CSV files.
 
         :param project: The project name
         :param tables: The table names to export
         :param output: The output directory path
         :param id_name: The name of the ID column name
         :param identifiers: The name of the ID mapping
-        :param incremental: Incremental export
         :param multilines: Write value sequences as multiple lines
         """
         exporter = io.OpalExporter.build(client=self.client, datasource=project , tables=tables, entityIdNames = id_name,
                                          identifiers=identifiers, output=output,
-                                         incremental=incremental,
                                          multilines=multilines, verbose=self.verbose)
         response = exporter.submit('csv')
         return response.from_json()
 
 class ExportRDSCommand:
     """
     Data export in RDS (using R).
@@ -146,38 +140,36 @@
         """
         Execute export data command
         """
         # Build and send request
         client = core.OpalClient.build(core.OpalClient.LoginInfo.parse(args))
         try:
             res = cls(client, args.verbose) \
-                .export(args.datasource, args.tables, args.output, args.id_name, args.identifiers, args.incremental, not args.no_multilines)
+                .export_data(args.datasource, args.tables, args.output, args.id_name, args.identifiers, not args.no_multilines)
             # format response
             core.Formatter.print_json(res, args.json)
         finally:
             client.close()
 
-    def export_data(self, project: str, tables: list, output: str, id_name: str = None, identifiers: str = None, incremental: bool = False, multilines: bool = True) -> dict:
+    def export_data(self, project: str, tables: list, output: str, id_name: str = None, identifiers: str = None, multilines: bool = True) -> dict:
         """
         Export tables in a RDS file.
 
         :param project: The project name
         :param tables: The table names to export
         :param output: The output file path (.rds)
         :param id_name: The name of the ID column name
         :param identifiers: The name of the ID mapping
-        :param incremental: Incremental export
         :param multilines: Write value sequences as multiple lines
         """
         if not (output.endswith('.rds')):
             raise Exception('Output must be a RDS file (.rds).')
-        
+
         exporter = io.OpalExporter.build(client=self.client, datasource=project , tables=tables, entityIdNames = id_name,
                                          identifiers=identifiers, output=output,
-                                         incremental=incremental,
                                          multilines=multilines, verbose=self.verbose)
         response = exporter.submit('RDS')
         return response.from_json()
 
 class ExportRSASCommand:
     """
     Data export in SAS (using R).
@@ -207,38 +199,36 @@
         """
         Execute export data command
         """
         # Build and send request
         client = core.OpalClient.build(core.OpalClient.LoginInfo.parse(args))
         try:
             res = cls(client, args.verbose) \
-                .export(args.datasource, args.tables, args.output, args.id_name, args.identifiers, args.incremental, not args.no_multilines)
+                .export_data(args.datasource, args.tables, args.output, args.id_name, args.identifiers, not args.no_multilines)
             # format response
             core.Formatter.print_json(res, args.json)
         finally:
             client.close()
 
-    def export_data(self, project: str, tables: list, output: str, id_name: str = None, identifiers: str = None, incremental: bool = False, multilines: bool = True) -> dict:
+    def export_data(self, project: str, tables: list, output: str, id_name: str = None, identifiers: str = None, multilines: bool = True) -> dict:
         """
         Export tables in a SAS file.
 
         :param project: The project name
         :param tables: The table names to export
         :param output: The output file path (.sas7bdat or .xpt)
         :param id_name: The name of the ID column name
         :param identifiers: The name of the ID mapping
-        :param incremental: Incremental export
         :param multilines: Write value sequences as multiple lines
         """
         if not (output.endswith('.sas7bdat')) and not (output.endswith('.xpt')):
             raise Exception('Output must be a SAS file (.sas7bdat or .xpt).')
-    
+
         exporter = io.OpalExporter.build(client=self.client, datasource=project , tables=tables, entityIdNames = id_name,
                                          identifiers=identifiers, output=output,
-                                         incremental=incremental,
                                          multilines=multilines, verbose=self.verbose)
         response = None
         if output.endswith('.sas7bdat'):
             response = exporter.submit('RSAS')
         else:
             response = exporter.submit('RXPT')
         return response.from_json()
@@ -272,38 +262,36 @@
         """
         Execute export data command
         """
         # Build and send request
         client = core.OpalClient.build(core.OpalClient.LoginInfo.parse(args))
         try:
             res = cls(client, args.verbose) \
-                .export(args.datasource, args.tables, args.output, args.id_name, args.identifiers, args.incremental, not args.no_multilines)
+                .export_data(args.datasource, args.tables, args.output, args.id_name, args.identifiers, not args.no_multilines)
             # format response
             core.Formatter.print_json(res, args.json)
         finally:
             client.close()
 
-    def export_data(self, project: str, tables: list, output: str, id_name: str = None, identifiers: str = None, incremental: bool = False, multilines: bool = True) -> dict:
+    def export_data(self, project: str, tables: list, output: str, id_name: str = None, identifiers: str = None, multilines: bool = True) -> dict:
         """
         Export tables in a SPSS file.
 
         :param project: The project name
         :param tables: The table names to export
         :param output: The output file path (.sav or .zsav)
         :param id_name: The name of the ID column name
         :param identifiers: The name of the ID mapping
-        :param incremental: Incremental export
         :param multilines: Write value sequences as multiple lines
         """
         if not (output.endswith('.sav')) and not (output.endswith('.zsav')):
             raise Exception('Output must be a SPSS file (.sav or .zsav).')
 
         exporter = io.OpalExporter.build(client=self.client, datasource=project , tables=tables, entityIdNames = id_name,
                                          identifiers=identifiers, output=output,
-                                         incremental=incremental,
                                          multilines=multilines, verbose=self.verbose)
         response = None
         if output.endswith('.sav'):
             response = exporter.submit('RSPSS')
         else:
             response = exporter.submit('RZSPSS')
         return response.from_json()
@@ -337,38 +325,36 @@
         """
         Execute export data command
         """
         # Build and send request
         client = core.OpalClient.build(core.OpalClient.LoginInfo.parse(args))
         try:
             res = cls(client, args.verbose) \
-                .export(args.datasource, args.tables, args.output, args.id_name, args.identifiers, args.incremental, not args.no_multilines)
+                .export_data(args.datasource, args.tables, args.output, args.id_name, args.identifiers, not args.no_multilines)
             # format response
             core.Formatter.print_json(res, args.json)
         finally:
             client.close()
 
-    def export_data(self, project: str, tables: list, output: str, id_name: str = None, identifiers: str = None, incremental: bool = False, multilines: bool = True) -> dict:
+    def export_data(self, project: str, tables: list, output: str, id_name: str = None, identifiers: str = None, multilines: bool = True) -> dict:
         """
         Export tables in a STATA file.
 
         :param project: The project name
         :param tables: The table names to export
         :param output: The output file path (.dta)
         :param id_name: The name of the ID column name
         :param identifiers: The name of the ID mapping
-        :param incremental: Incremental export
         :param multilines: Write value sequences as multiple lines
         """
         if not (output.endswith('.dta')):
             raise Exception('Output must be a Stata file (.dta).')
 
         exporter = io.OpalExporter.build(client=self.client, datasource=project , tables=tables, entityIdNames = id_name,
                                          identifiers=identifiers, output=output,
-                                         incremental=incremental,
                                          multilines=multilines, verbose=self.verbose)
         response = exporter.submit('RSTATA')
         return response.from_json()
 
 
 class ExportSQLCommand:
     """
@@ -383,46 +369,44 @@
     def add_arguments(cls, parser):
         """
         Add data command specific options
         """
         parser.add_argument('--datasource', '-d', required=True, help='Project name')
         parser.add_argument('--tables', '-t', nargs='+', required=True, help='The list of tables to be exported')
         parser.add_argument('--database', '-db', required=True, help='Name of the SQL database')
-        parser.add_argument('--incremental', '-i', action='store_true', help='Incremental export')
         parser.add_argument('--identifiers', '-id', required=False, help='Name of the ID mapping')
         parser.add_argument('--json', '-j', action='store_true', help='Pretty JSON formatting of the response')
 
     @classmethod
     def do_command(cls, args):
         """
         Execute export data command
         """
         # Build and send request
         client = core.OpalClient.build(core.OpalClient.LoginInfo.parse(args))
         try:
             res = cls(client, args.verbose) \
-                .export(args.datasource, args.tables, args.database, args.identifiers, args.incremental)
+                .export_data(args.datasource, args.tables, args.database, args.identifiers)
             # format response
             core.Formatter.print_json(res, args.json)
         finally:
             client.close()
-    
-    def export_data(self, project: str, tables: list, database: str, identifiers: str = None, incremental: bool = False):
+
+    def export_data(self, project: str, tables: list, database: str, identifiers: str = None):
         """
         Export tables in a SQL database.
 
         :param project: The project name
         :param tables: The table names to export
         :param database: The SQL database name. See ProjectService.get_databases() for a list of databases with 'export' usage.
         :param identifiers: The name of the ID mapping
-        :param incremental: Incremental export
         """
         exporter = io.OpalExporter.build(client=self.client, datasource=project , tables=tables,
                                                     identifiers=identifiers, output=database,
-                                                    incremental=incremental, verbose=self.verbose)
+                                                    verbose=self.verbose)
         response = exporter.submit('jdbc')
         return response.from_json()
 
 class ExportXMLCommand:
     """
     Data export in XML.
     """
@@ -435,55 +419,53 @@
     def add_arguments(cls, parser):
         """
         Add data command specific options
         """
         parser.add_argument('--datasource', '-d', required=True, help='Project name')
         parser.add_argument('--tables', '-t', nargs='+', required=True, help='The list of tables to be exported')
         parser.add_argument('--output', '-out', required=True, help='Output zip file name that will be exported')
-        parser.add_argument('--incremental', '-i', action='store_true', help='Incremental export')
         parser.add_argument('--identifiers', '-id', required=False, help='Name of the ID mapping')
         parser.add_argument('--json', '-j', action='store_true', help='Pretty JSON formatting of the response')
 
     @classmethod
     def do_command(cls, args):
         """
         Execute export data command
         """
         # Check output filename extension
         client = core.OpalClient.build(core.OpalClient.LoginInfo.parse(args))
         try:
             res = cls(client, args.verbose) \
-                .export(args.datasource, args.tables, args.output, args.identifiers, args.incremental)
+                .export_data(args.datasource, args.tables, args.output, args.identifiers)
             # format response
             core.Formatter.print_json(res, args.json)
         finally:
             client.close()
 
-    def export_data(self, project: str, tables: list, output: str, identifiers: str = None, incremental: bool = False) -> dict:
+    def export_data(self, project: str, tables: list, output: str, identifiers: str = None) -> dict:
         """
         Export tables in an Opal archive file.
 
         :param project: The project name
         :param tables: The table names to export
         :param output: The output file path (.zip)
         :param id_name: The name of the ID column name
         :param identifiers: The name of the ID mapping
-        :param incremental: Incremental export
         :param multilines: Write value sequences as multiple lines
         """
         if not (output.endswith('.zip')):
             raise Exception('Output must be a zip file.')
 
         exporter = io.OpalExporter.build(client=self.client, datasource=project , tables=tables,
                                          identifiers=identifiers, output=output,
-                                         incremental=incremental,
+                                         incremental=False,
                                          verbose=self.verbose)
         response = exporter.submit('xml')
         return response.from_json()
-        
+
 
 class ExportVCFCommand:
     """
     Export some VCF/BCF files.
     """
 
     def __init__(self, client: core.OpalClient, verbose: bool = False):
@@ -509,15 +491,15 @@
         """
         Execute delete command
         """
         # Build and send requests
         client = core.OpalClient.build(core.OpalClient.LoginInfo.parse(args))
         try:
             res = ExportVCFCommand(client, args.verbose) \
-                .export(args.project, args.vcf, args.destination, not args.no_case_controls, args.filter_table)
+                .export_data(args.project, args.vcf, args.destination, not args.no_case_controls, args.filter_table)
         finally:
             client.close()
 
     def export_data(self, project: str, vcf: list, destination: str, case_controls: bool = True, filter_table: str = None) -> dict:
         """
         Export VCF/BCF files.
```

### Comparing `obiba_opal-5.1.1/obiba_opal/file.py` & `obiba_opal-5.2.0/obiba_opal/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,18 +74,20 @@
         request.fail_on_error()
 
         if self.verbose:
             request.verbose()
 
         file = FileService.OpalFile(path)
 
+
         fp = os.fdopen(fd, 'wb')
         request.get().resource(file.get_ws()).accept('*/*').header('X-File-Key', download_password).send(fp)
         fp.flush()
 
+
     def upload_file(self, upload: str, path: str):
         """
         Upload a file to Opal.
 
         :param path: The destination folder path in Opal
         :param upload: The source file path to upload
         """
@@ -93,17 +95,17 @@
         request.fail_on_error().accept_json()
 
         if self.verbose:
             request.verbose()
 
         file = FileService.OpalFile(path)
 
-        request.content_upload(upload).accept('text/html').content_type('multipart/form-data')
+        request.content_upload(upload).accept('text/html')
         request.post().resource(file.get_ws()).send()
-    
+
     def delete_file(self, path: str):
         """
         Delete a file in Opal.
 
         :param path: The destination file path in Opal
         """
         request = self.client.new_request()
@@ -111,15 +113,15 @@
 
         if self.verbose:
             request.verbose()
 
         file = FileService.OpalFile(path)
 
         request.delete().resource(file.get_ws()).send()
-    
+
     def file_info(self, path) -> dict:
         """
         Get information about a file in Opal.
 
         :param path: The destination file path in Opal
         """
         request = self.client.new_request()
@@ -128,15 +130,15 @@
         if self.verbose:
             request.verbose()
 
         file = FileService.OpalFile(path)
 
         response = request.get().resource(file.get_meta_ws()).send()
         return response.from_json()
-    
+
     class OpalFile:
         """
         File on Opal file system
         """
 
         def __init__(self, path):
             self.path = path
```

### Comparing `obiba_opal-5.1.1/obiba_opal/imports.py` & `obiba_opal-5.2.0/obiba_opal/imports.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.1/obiba_opal/io.py` & `obiba_opal-5.2.0/obiba_opal/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,26 +285,27 @@
     def submit(self):
         # copy options
         options = {
             'destination': self.destination,
             'nonIncremental': not self.incremental,
             'noVariables': False,
             'noValues': False,
+            'destinationTableName': None,
             'copyNullValues': self.nulls,
             'tables': []
         }
         if self.tables:
             tables2copy = self.tables
 
             def table_fullname(t): return self.datasource + '.' + t
 
             options['tables'] = list(map(table_fullname, tables2copy))
         # name option will be ignored if more than one table
         if self.name:
-            options.destinationTableName = self.name
+            options['destinationTableName'] = self.name
 
         if self.verbose:
             print("** Copy options:")
             print(options)
             print("**")
 
         # submit data copy job
```

### Comparing `obiba_opal-5.1.1/obiba_opal/perm.py` & `obiba_opal-5.2.0/obiba_opal/perm.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.1/obiba_opal/project.py` & `obiba_opal-5.2.0/obiba_opal/project.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.1/obiba_opal/security.py` & `obiba_opal-5.2.0/obiba_opal/security.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.1/obiba_opal/sql.py` & `obiba_opal-5.2.0/obiba_opal/sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,23 +45,23 @@
             if args.format == 'json':
                 request.accept_json().content_type_text_plain()
                 response = request.post().resource(uri).content(args.query).send()
                 # output to stdout
                 if args.json:
                     print(response.pretty_json())
                 else:
-                    print(response.content)
+                    print(str(response))
             else:
                 request.accept_text_csv().content_type_form_urlencoded()
                 body = 'query=' + urllib.parse.quote(args.query)
                 if args.id_name:
                     body = body + '&id=' + urllib.parse.quote(args.id_name)
                 response = request.post().resource(uri).content(body).send()
                 # output to stdout
-                print(response.content)
+                print(str(response))
         finally:
             client.close()
 
 
 class SQLHistoryService:
     """
     Get and filter SQL service history.
@@ -103,10 +103,10 @@
                 request.verbose()
             request.fail_on_error()
             response = request.accept_json().get().resource(uri).send()
             # output to stdout
             if args.json:
                 print(response.pretty_json())
             else:
-                print(response.content)
+                print(str(response))
         finally:
             client.close()
```

### Comparing `obiba_opal-5.1.1/obiba_opal/subjects.py` & `obiba_opal-5.2.0/obiba_opal/subjects.py`

 * *Files identical despite different names*

### Comparing `obiba_opal-5.1.1/obiba_opal/system.py` & `obiba_opal-5.2.0/obiba_opal/table.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,403 +1,361 @@
 """
-Opal system data
+Table/view copy and management.
 """
 
 import obiba_opal.core as core
-from typing import Union
-import ast
-import json
-import sys
-import time
+import obiba_opal.io as io
+from obiba_opal.dictionary import DictionaryService
+import os
+import zipfile
 
-class SystemService:
+
+class CopyTableCommand:
     """
-    Get some system information.
+    Execute a copy table command.
     """
 
+    def __init__(self, client: core.OpalClient, verbose: bool = False):
+        self.client = client
+        self.verbose = verbose
+
     @classmethod
     def add_arguments(cls, parser):
         """
-        Add system command specific options
+        Add data command specific options
         """
+        parser.add_argument('--project', '-pr', required=True, help='Source project name')
+        parser.add_argument('--tables', '-t', nargs='+', required=False,
+                            help='List of table names to be copied (default is all)')
+        parser.add_argument('--destination', '-d', required=True, help='Destination project name')
+        parser.add_argument('--name', '-na', required=False,
+                            help='New table name (required if source and destination are the same, ignored if more than one table is to be copied)')
+        parser.add_argument('--incremental', '-i', action='store_true', help='Incremental copy')
+        parser.add_argument('--nulls', '-nu', action='store_true', help='Copy the null values')
         parser.add_argument('--json', '-j', action='store_true', help='Pretty JSON formatting of the response')
 
-        parser.add_argument('--version', action='store_true', required=False,
-                            help='Opal version number')
-        parser.add_argument('--env', action='store_true', required=False,
-                            help='Opal java execution environment (JVM related statistic properties')
-        parser.add_argument('--status', action='store_true', required=False,
-                            help='Opal application status (JVM related dynamic properties)')
-        parser.add_argument('--conf', action='store_true', required=False,
-                            help='Opal application configuration')
-
     @classmethod
     def do_command(cls, args):
         """
-        Execute SYSTEM command
+        Execute copy data command
         """
         # Build and send request
         client = core.OpalClient.build(core.OpalClient.LoginInfo.parse(args))
         try:
-            request = client.new_request()
-            request.fail_on_error()
-
-            request.accept_json()
-
-            if args.verbose:
-                request.verbose()
-
-            # send request
-            request.get().resource(cls.do_ws(args))
-            response = request.send()
-
+            res = CopyTableCommand(client, args.verbose).copy_tables(args.project, args.tables, args.destination, args.name, args.incremental, args.nulls)
             # format response
-            res = response.content
-
-            if args.json:
-                res = response.pretty_json()
-
-            # output to stdout
-            print(res)
+            core.Formatter.print_json(res, args.json)
         finally:
             client.close()
 
-    @classmethod
-    def do_ws(cls, args):
-        """
-        Build the web service resource path
-        """
-        if args.version:
-            args.json = False
-            return "/system/version"
-        if args.env:
-            return "/system/env"
-        if args.status:
-            return "/system/status"
-        if args.conf:
-            return "/system/conf"
-        return "/system/conf/general"
-
-
-class PluginService:
-    """
-    Plugins management.
-    """
-
-    @classmethod
-    def add_arguments(cls, parser):
-        """
-        Add plugin command specific options
+    def copy_tables(self, project: str, tables: list, destination: str, name: str, incremental: bool, nulls: bool) -> dict:
         """
+        Execute copy data command
 
-        parser.add_argument('--list', '-ls', action='store_true', help='List the installed plugins.')
-        parser.add_argument('--updates', '-lu', action='store_true', help='List the installed plugins that can be updated.')
-        parser.add_argument('--available', '-la', action='store_true', help='List the new plugins that could be installed.')
-        parser.add_argument('--install', '-i', required=False,
-                            help='Install a plugin by providing its name or name:version or a path to a plugin archive file (in Opal file system). If no version is specified, the latest version is installed. Requires system restart to be effective.')
-        parser.add_argument('--remove', '-rm', required=False,
-                            help='Remove a plugin by providing its name. Requires system restart to be effective.')
-        parser.add_argument('--reinstate', '-ri', required=False,
-                            help='Reinstate a plugin that was previously removed by providing its name.')
-        parser.add_argument('--fetch', '-f', required=False, help='Get the named plugin description.')
-        parser.add_argument('--configure', '-c', required=False,
-                            help='Configure the plugin site properties. Usually requires to restart the associated service to be effective.')
-        parser.add_argument('--status', '-su', required=False,
-                            help='Get the status of the service associated to the named plugin.')
-        parser.add_argument('--start', '-sa', required=False, help='Start the service associated to the named plugin.')
-        parser.add_argument('--stop', '-so', required=False, help='Stop the service associated to the named plugin.')
-        parser.add_argument('--json', '-j', action='store_true', help='Pretty JSON formatting of the response')
-
-    @classmethod
-    def do_command(cls, args):
-        """
-        Execute plugin command
-        """
-        # Build and send request
-        client = core.OpalClient.build(core.OpalClient.LoginInfo.parse(args))
-        try:
-            request = client.new_request()
-            request.fail_on_error().accept_json()
-
-            if args.verbose:
-                request.verbose()
-
-            if args.list:
-                response = request.get().resource('/plugins').send()
-            elif args.updates:
-                response = request.get().resource('/plugins/_updates').send()
-            elif args.available:
-                response = request.get().resource('/plugins/_available').send()
-            elif args.install:
-                if args.install.startswith('/'):
-                    response = request.post().resource('/plugins?file=' + args.install).send()
-                else:
-                    nameVersion = args.install.split(':')
-                    if len(nameVersion) == 1:
-                        response = request.post().resource('/plugins?name=' + nameVersion[0]).send()
-                    else:
-                        response = request.post().resource(
-                            '/plugins?name=' + nameVersion[0] + '&version=' + nameVersion[1]).send()
-            elif args.fetch:
-                response = request.get().resource('/plugin/' + args.fetch).send()
-            elif args.configure:
-                request.content_type_text_plain()
-                print('Enter plugin site properties (one property per line, Ctrl-D to end input):')
-                request.content(sys.stdin.read())
-                response = request.put().resource('/plugin/' + args.configure + '/cfg').send()
-            elif args.remove:
-                response = request.delete().resource('/plugin/' + args.remove).send()
-            elif args.reinstate:
-                response = request.put().resource('/plugin/' + args.reinstate).send()
-            elif args.status:
-                response = request.get().resource('/plugin/' + args.status + '/service').send()
-            elif args.start:
-                response = request.put().resource('/plugin/' + args.start + '/service').send()
-            elif args.stop:
-                response = request.delete().resource('/plugin/' + args.stop + '/service').send()
+        :param project: The project name
+        :param tables: List of table names to be copied (default is all)
+        :param destination: Destination project name
+        :param name: New table name (required if source and destination are the same, ignored if more than one table is to be copied)
+        :param incremental: Incremental copy
+        :param nulls: Copy the null values
+        """
+        tables_ = tables
+        if not tables:
+            tables_ = self._retrieve_datasource_tables(project)
+        copier = io.OpalCopier.build(client=self.client, datasource=project, tables=tables_,
+                                    destination=destination, name=name,
+                                    incremental=incremental, nulls=nulls,
+                                    verbose=self.verbose)
+        response = copier.submit()
+        return response.from_json()
 
-            # format response
-            res = response.content
-            if args.json:
-                res = response.pretty_json()
+    def _retrieve_datasource_tables(self, project: str) -> list:
+        request = self.client.new_request()
+        if self.verbose:
+            request.verbose()
+        response = request.fail_on_error().get().resource(
+            core.UriBuilder(['datasource', project, 'tables']).build()).send().from_json()
 
-            # output to stdout
-            print(res)
-        finally:
-            client.close()
+        tables = []
+        for table in response:
+            tables.append(str(table['name']))
 
+        return tables
 
-class TaxonomyService:
+class DeleteTableService:
     """
-    Taxonomies management.
+    Delete some tables in a project.
     """
 
+    def __init__(self, client: core.OpalClient, verbose: bool = False):
+        self.client = client
+        self.verbose = verbose
+
     @classmethod
     def add_arguments(cls, parser):
         """
-        Add file command specific options
+        Add command specific options
         """
-        parser.add_argument('--download', '-dl', required=False, help='Download a taxonomy by name (YAML format).')
-        parser.add_argument('--import-file', '-if', required=False, help='Import a taxonomy from the provided Opal file path (YAML format).')
-        parser.add_argument('--delete', '-dt', required=False, help='Delete a taxonomy by name.')
-        parser.add_argument('--force', '-f', action='store_true', help='Skip confirmation.')
-        parser.add_argument('--json', '-j', action='store_true', help='Pretty JSON formatting of the response')
+        parser.add_argument('--project', '-pr', required=True, help='Project name to which the tables belong')
+        parser.add_argument('--tables', '-t', nargs='+', required=False,
+                            help='List of table names which will be deleted (default is all)')
 
     @classmethod
     def do_command(cls, args):
         """
-        Execute taxonomy command
+        Execute delete command
         """
-        # Build and send request
+        # Build and send requests
         client = core.OpalClient.build(core.OpalClient.LoginInfo.parse(args))
         try:
-            request = client.new_request()
-            request.fail_on_error().accept_json()
-
-            if args.verbose:
-                request.verbose()
-
-
-            # send request
-            if args.download:
-                taxo = cls.OpalTaxonomyResource(args.download)
-                response = request.get().resource(taxo.get_download_ws()).accept('text/plain').send()
-            elif args.import_file:
-                response = request.post().resource(core.UriBuilder(['system', 'conf', 'taxonomies', 'import', '_file']).query('file',args.import_file).build()).send()
-            elif args.delete:
-                taxo = cls.OpalTaxonomyResource(args.delete)
-                # confirm
-                if args.force:
-                    response = request.delete().resource(taxo.get_ws()).send()
-                else:
-                    confirmed = input('Delete the taxonomy "' + args.delete + '"? [y/N]: ')
-                    if confirmed == 'y':
-                        response = request.delete().resource(taxo.get_ws()).send()
-                    else:
-                        print('Aborted.')
-                        sys.exit(0)
-            else:
-                response = request.get().resource('/system/conf/taxonomies/summaries').send()
-
-            # format response
-            res = response.content
-            if args.json and not args.download and not args.delete and not args.import_file:
-                res = response.pretty_json()
-
-            # output to stdout
-            print(res)
+            DictionaryService(client, args.verbose).delete_tables(args.project, args.tables)
         finally:
             client.close()
 
-    class OpalTaxonomyResource:
-        """
-        Taxonomy reference
-        """
-
-        def __init__(self, name):
-            self.name = name
-
-        def get_ws(self):
-            return '/system/conf/taxonomy/' + self.name
 
-        def get_download_ws(self):
-            return '/system/conf/taxonomy/' + self.name + '/_download'
-
-
-class TaskService:
+class BackupViewService:
     """
-    Tasks management.
+    Backup views of a project: download view's JSON representation and save it in a file, one for each view, for later restore.
     """
 
     def __init__(self, client: core.OpalClient, verbose: bool = False):
         self.client = client
         self.verbose = verbose
 
     @classmethod
     def add_arguments(cls, parser):
         """
-        Add task command specific options
+        Add command specific options
         """
-        parser.add_argument('--id', required=False,
-                            help='The task ID. If not provided, it will be read from the standard input (from the JSON representation of the task or a plain value).')
-        parser.add_argument('--show', '-sh', action='store_true', help='Show JSON representation of the task')
-        parser.add_argument('--status', '-st', action='store_true', help='Get the status of the task')
-        parser.add_argument('--wait', '-w', action='store_true', help='Wait for the task to complete (successfully or not)')
-        parser.add_argument('--cancel', '-c', action='store_true', help='Cancel the task')
-        parser.add_argument('--delete', '-d', action='store_true', help='Delete the task')
-        parser.add_argument('--json', '-j', action='store_true', help='Pretty JSON formatting of the response')
+        parser.add_argument('--project', '-pr', required=True, help='Source project name')
+        parser.add_argument('--views', '-vw', nargs='+', required=False,
+                            help='List of view names to be backed up (default is all)')
+        parser.add_argument('--output', '-out', required=False, help='Output directory name (default is current directory)')
+        parser.add_argument('--force', '-f', action='store_true',
+                            help='Skip confirmation when overwriting the backup file.')
 
     @classmethod
     def do_command(cls, args):
         """
-        Execute task command
+        Retrieve table DTOs of the project, look for the views, download the views in JSON into a file in provided or current directory
         """
+
         # Build and send request
-        # Extract task identifier from stdin: can be the ID or the task in JSON
         client = core.OpalClient.build(core.OpalClient.LoginInfo.parse(args))
-        service = TaskService(client, args.verbose)
         try:
-            if not args.id:
-                id = sys.stdin.read().strip('\n')
-                if id.startswith('{'):
-                    id = str(json.loads(id)['id'])
-                args.id = id
-
-            if args.show or not (args.show or args.wait or args.status or args.cancel or args.delete):
-                res = service.get_task(args.id)
-                core.Formatter.print_json(res, args.json)
-            if args.wait:
-                status = service.wait_task(args.id)
-                print('\r\033[K' + status)
-            if args.status:
-                print(service.get_task(args.id)['status'])
-            if args.cancel:
-                service.cancel_task(args.id)
-            if args.delete:
-                service.delete_task(args.id)
+            BackupViewService(client, args.verbose).backup_views(args.project, args.views, args.output, args.force)
         finally:
             client.close()
 
-    def get_task(self, id: Union[str, int]):
-        request = self._make_request()
-        request.get().resource('/shell/command/%s' % id)
-        response = request.send()
-        return response.from_json()
+    def backup_view(self, project: str, view, outdir, force: bool):
+        outfile = view + '.json'
+        print('Backup of', view, 'in', outfile, '...')
 
-    def delete_task(self, id: Union[str, int]):
-        request = self._make_request()
-        request.delete().resource('/shell/command/%s' % id).send()
+        outpath = os.path.join(outdir, outfile)
+
+        request = self.client.new_request()
+        request.fail_on_error()
+        if self.verbose:
+            request.verbose()
+        response = request.get().resource(core.UriBuilder(['datasource', project, 'view', view]).build()).send()
 
-    def cancel_task(self, id: Union[str, int]):
-        request = self._make_request().content_type_text_plain()
-        request.content('CANCELED')
-        request.put().resource('/shell/command/%s/status' % id).send()
-
-    def wait_task(self, id: Union[str, int]):
-        task = self.get_task(id)
-        while task['status'] not in ['SUCCEEDED', 'CANCELED', 'FAILED']:
-            if 'progress' in task:
-                progress = task['progress']
-                if 'message' in progress:
-                    sys.stdout.write('\r\033[K' + str(progress['percent']) + '% ' + progress['message'])
-                else:
-                    sys.stdout.write('\r\033[K' + str(progress['percent']) + '%')
+        dowrite = True
+        if os.path.exists(outpath) and not force:
+            dowrite = False
+            confirmed = input('Overwrite the file "' + outpath + '"? [y/N]: ')
+            if confirmed == 'y':
+                dowrite = True
+
+        if dowrite:
+            out = open(outpath, 'w+')
+            out.write(str(response))
+            out.close()
+
+    def backup_views(self, project: str, views: list, output: str, force: bool) -> list:
+        """
+        Retrieve table DTOs of the project, look for the views, download the views in JSON into a file in provided or current directory
+
+        :param client: Opal connection object
+        :param project: The project name
+        :param views: List of view names to be backed up (default is all)
+        :param output: Output directory name (default is current directory)
+        :param force: Skip confirmation when overwriting the backup file
+        :param verbose: Verbose requests
+        """
+
+        views_ = views
+        obsviews = self._retrieve_datasource_views(project)
+        if not views_:
+            views_ = obsviews
+        else:
+            safeviews = []
+            for view in views_:
+                if view in obsviews:
+                    safeviews.append(view)
+            views_ = safeviews
+        if not views_:
+            print('No views to backup in project', project)
+        else:
+            # prepare output directory
+            outdir = output
+            if not outdir:
+                outdir = os.getcwd()
             else:
-                sys.stdout.write('.')
-            sys.stdout.flush()
-            time.sleep(1)
-            task = self.get_task(id)
-        return task['status']
+                outdir = os.path.normpath(outdir)
+            if self.verbose:
+                print('Output directory is', outdir)
+            if not os.path.exists(outdir):
+                if self.verbose:
+                    print('Creating output directory ...')
+                os.makedirs(outdir)
+
+            # backup each view
+            for view in views_:
+                self.backup_view(project, view, outdir, force)
+        return views_
 
-    def _make_request(self):
+    def _retrieve_datasource_views(self, project: str) -> list:
         request = self.client.new_request()
         request.fail_on_error()
-        request.accept_json()
         if self.verbose:
             request.verbose()
-        return request
+        response = request.get().resource(core.UriBuilder(['datasource', project, 'tables']).build()).send().from_json()
+
+        views = []
+        for table in response:
+            if 'viewLink' in table:
+                views.append(str(table['name']))
+
+        return views
 
 
-class RESTService:
+class RestoreViewService:
     """
-    Perform raw web services requests.
+    Restore views of a project: upload view's JSON representation and make it a view.
     """
 
+    def __init__(self, client: core.OpalClient, verbose: bool = False):
+        self.client = client
+        self.verbose = verbose
+
     @classmethod
     def add_arguments(cls, parser):
         """
-        Add REST command specific options
+        Add data command specific options
         """
-        parser.add_argument('ws', help='Web service path, for instance: /datasource/xxx/table/yyy/variable/vvv')
-        parser.add_argument('--method', '-m', required=False,
-                            help='HTTP method (default is GET, others are POST, PUT, DELETE, OPTIONS)')
-        parser.add_argument('--accept', '-a', required=False, help='Accept header (default is application/json)')
-        parser.add_argument('--content-type', '-ct', required=False,
-                            help='Content-Type header (default is application/json)')
-        parser.add_argument('--headers', '-hs', required=False,
-                            help='Custom headers in the form of: { "Key2": "Value2", "Key2": "Value2" }')
-        parser.add_argument('--json', '-j', action='store_true', help='Pretty JSON formatting of the response')
+        parser.add_argument('--project', '-pr', required=True, help='Destination project name')
+        parser.add_argument('--views', '-vw', nargs='+', required=False,
+                            help='List of view names to be restored (default is all the JSON files that are found in the backup directory/zip archive)')
+        parser.add_argument('--input', '-in', required=False,
+                            help='Input directory name or input zip file containing JSON views (default is current directory)')
+        parser.add_argument('--force', '-f', action='store_true',
+                            help='Skip confirmation when overwriting an existing view.')
 
     @classmethod
     def do_command(cls, args):
         """
-        Execute REST command
+        Retrieve table DTOs of the project, look for the views, download the views in JSON into a file in provided or current directory
         """
+
         # Build and send request
         client = core.OpalClient.build(core.OpalClient.LoginInfo.parse(args))
-        try:
-            request = client.new_request()
-            request.fail_on_error()
+        service = RestoreViewService(client, args.verbose)
+        service.restore_views(args.project, args.views, args.input, args.force)
+
+    def restore_views(self, project: str, views: list, input: str = None, force: bool = False):
+        obsviews = self._retrieve_datasource_views(project)
 
-            if args.accept:
-                request.accept(args.accept)
+        # list input directory content
+        indir = input
+        if not indir:
+            indir = os.getcwd()
+        else:
+            indir = os.path.normpath(indir)
+        print('Input directory is', indir)
+
+        if indir.endswith('.zip'):
+            with zipfile.ZipFile(indir, 'r') as inzip:
+                for viewfile in [filename for filename in inzip.namelist() if
+                                    filename.endswith('.json') and (not views or filename[:-5] in views)]:
+                    self._restore_zipped_view(project, obsviews, viewfile, inzip, force)
+        else:
+            for viewfile in self._list_json_files(indir, views):
+                self._restore_view(project, obsviews, viewfile, force)
+
+    def _retrieve_datasource_views(self, project: str):
+        request = self._make_request()
+        response = request.get().resource(core.UriBuilder(['datasource', project, 'tables']).build()).send().from_json()
+
+        views = []
+        for table in response:
+            if 'viewLink' in table:
+                views.append(str(table['name']))
+
+        return views
+
+    def _restore_view(self, project: str, obsviews: list, infile: str, force: bool = False):
+        view = os.path.basename(infile[:-5])  # supposed to be a .json file path
+
+        dowrite = True
+        if view in obsviews and not force:
+            dowrite = False
+            confirmed = input('Overwrite the view "' + view + '"? [y/N]: ')
+            if confirmed == 'y':
+                dowrite = True
+
+        if dowrite:
+            print('Restore of', view, 'from', infile, '...')
+
+            request =  self._make_request()
+            with open(infile, 'r') as inf:
+                request.content(inf.read())
+            request.content_type_json()
+
+            if view in obsviews:
+                request.put().resource(
+                    core.UriBuilder(['datasource', project, 'view', view]).query('comment', 'restore-view').build()).send()
             else:
-                request.accept_json()
+                request.post().resource(
+                    core.UriBuilder(['datasource', project, 'views']).query('comment', 'restore-view').build()).send()
 
-            if args.content_type:
-                request.content_type(args.content_type)
-                print('Enter content:')
-                request.content(sys.stdin.read())
-
-            if args.headers:
-                headers = ast.literal_eval(args.headers)
-                for key in list(headers.keys()):
-                    request.header(key, headers[key])
-
-            if args.verbose:
-                request.verbose()
-
-            # send request
-            request.method(args.method).resource(args.ws)
-            response = request.send()
+    def _restore_zipped_view(self, project: str, obsviews: list, infile: str, zippedinput, force: bool = False):
+        view = infile[:-5]  # supposed to be a .json file name
 
-            # format response
-            res = response.content
-            if args.json:
-                res = response.pretty_json()
-            elif args.method in ['OPTIONS']:
-                res = response.headers['Allow']
+        dowrite = True
+        if view in obsviews and not force:
+            dowrite = False
+            confirmed = input('Overwrite the view "' + view + '"? [y/N]: ')
+            if confirmed == 'y':
+                dowrite = True
+
+        if dowrite:
+            print('Restore of', view, 'from', infile, '...')
+
+            request = self._make_request()
+            request.content(zippedinput.read(infile))
+            request.content_type_json()
+
+            if view in obsviews:
+                request.put().resource(
+                    core.UriBuilder(['datasource', project, 'view', view]).query('comment',
+                                                                                        'restore-view').build()).send()
+            else:
+                request.post().resource(
+                    core.UriBuilder(['datasource', project, 'views']).query('comment',
+                                                                                    'restore-view').build()).send()
+
+    def _list_json_files(self, dirref: str, basenames):
+        matches = []
+        for root, dirnames, filenames in os.walk(dirref):
+            for filename in filenames:
+                if filename.endswith('.json'):
+                    if not basenames or filename[:-5] in basenames:
+                        matches.append(os.path.join(root, filename))
+        return matches
 
-            # output to stdout
-            print(res)
-        finally:
-            client.close()
+    def _make_request(self, fail_safe: bool = False):
+        request = self.client.new_request()
+        if not fail_safe:
+            request.fail_on_error()
+        if self.verbose:
+            request.verbose()
+        return request
```

### Comparing `obiba_opal-5.1.1/pyproject.toml` & `obiba_opal-5.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "obiba-opal"
-version = "5.1.1"
+version = "5.2.0"
 description = "OBiBa/Opal python client."
 authors = ["Yannick Marcon <yannick.marcon@obiba.org>"]
 maintainers = ["Yannick Marcon <yannick.marcon@obiba.org>"]
 license = "GPL-v3"
 readme = "README.md"
 packages = [{include = "obiba_opal"}]
 homepage = "https://www.obiba.org"
@@ -12,15 +12,16 @@
 documentation = "https://opaldoc.obiba.org/en/latest/python-user-guide/"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/obiba/opal-python-client/issues"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pycurl = "^7.45.2"
+requests = "^2.31.0"
+urllib3 = "1.26.15"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 
 [tool.poetry.scripts]
 opal = 'obiba_opal.console:run'
```

### Comparing `obiba_opal-5.1.1/PKG-INFO` & `obiba_opal-5.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obiba-opal
-Version: 5.1.1
+Version: 5.2.0
 Summary: OBiBa/Opal python client.
 Home-page: https://www.obiba.org
 License: GPL-v3
 Author: Yannick Marcon
 Author-email: yannick.marcon@obiba.org
 Maintainer: Yannick Marcon
 Maintainer-email: yannick.marcon@obiba.org
@@ -12,15 +12,16 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pycurl (>=7.45.2,<8.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: urllib3 (==1.26.15)
 Project-URL: Bug Tracker, https://github.com/obiba/opal-python-client/issues
 Project-URL: Documentation, https://opaldoc.obiba.org/en/latest/python-user-guide/
 Project-URL: Repository, https://github.com/obiba/opal-python-client
 Description-Content-Type: text/markdown
 
 # Opal Python [![Build Status](https://app.travis-ci.com/obiba/opal-python-client.svg?branch=master)](https://app.travis-ci.com/github/obiba/opal-python-client)
 
@@ -48,14 +49,16 @@
 # on Debian systems
 sudo apt-get install python3-pycurl
 
 # on RPM systems
 sudo yum install python3-pycurl
 ```
 
+### CLI
+
 To get the options of the command line:
 
 ```shell
 opal --help
 ```
 
 This command will display which sub-commands are available. For each sub-command you can get the help message as well:
@@ -63,15 +66,15 @@
 ```shell
 opal <subcommand> --help
 ```
 
 The objective of having sub-command is to hide the complexity of applying some use cases to the Opal REST API. More
 sub-commands will be developed in the future.
 
-## Development
+### API
 
 Opal Python client can be easily extended by using the [exposed classes](https://github.com/obiba/opal-python-client/blob/master/obiba_opal/__init__.py). The classes `*Command` return an Opal task object, to be followed with the `TaskService`. The classes `*Service` perform immediate operations. 
 
 ```python
 from obiba_opal import OpalClient, HTTPError, Formatter, ImportCSVCommand, TaskService, FileService, DictionaryService
 
 # if 2-factor auth is enabled, user will be asked for the secret code
```


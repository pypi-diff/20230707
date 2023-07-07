# Comparing `tmp/emailalert-1.4.5.tar.gz` & `tmp/emailalert-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.4.5.tar", last modified: Fri Jul  7 02:39:38 2023, max compression
+gzip compressed data, was "emailalert-1.4.6.tar", last modified: Fri Jul  7 02:50:10 2023, max compression
```

## Comparing `emailalert-1.4.5.tar` & `emailalert-1.4.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 02:39:38.232474 emailalert-1.4.5/
--rw-rw-rw-   0        0        0      178 2023-07-07 02:39:38.230475 emailalert-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-07-07 02:16:16.000000 emailalert-1.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 02:39:38.158083 emailalert-1.4.5/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-07-07 02:39:37.000000 emailalert-1.4.5/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-07-07 02:39:37.000000 emailalert-1.4.5/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 02:39:37.000000 emailalert-1.4.5/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-07 02:39:37.000000 emailalert-1.4.5/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-07 02:39:38.219427 emailalert-1.4.5/sck/
--rw-rw-rw-   0        0        0        0 2023-07-07 01:24:44.000000 emailalert-1.4.5/sck/__init__.py
--rw-rw-rw-   0        0        0     4395 2023-07-07 02:38:58.000000 emailalert-1.4.5/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-07-07 02:39:38.234474 emailalert-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-07-07 02:39:09.000000 emailalert-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 02:50:10.407427 emailalert-1.4.6/
+-rw-rw-rw-   0        0        0      178 2023-07-07 02:50:10.402171 emailalert-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-07-07 02:16:16.000000 emailalert-1.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 02:50:10.338172 emailalert-1.4.6/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-07-07 02:50:10.000000 emailalert-1.4.6/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-07-07 02:50:10.000000 emailalert-1.4.6/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 02:50:10.000000 emailalert-1.4.6/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-07 02:50:10.000000 emailalert-1.4.6/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 02:50:10.379761 emailalert-1.4.6/sck/
+-rw-rw-rw-   0        0        0        0 2023-07-07 01:24:44.000000 emailalert-1.4.6/sck/__init__.py
+-rw-rw-rw-   0        0        0     4395 2023-07-07 02:49:25.000000 emailalert-1.4.6/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-07-07 02:50:10.415453 emailalert-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-07-07 02:49:58.000000 emailalert-1.4.6/setup.py
```

### Comparing `emailalert-1.4.5/README.md` & `emailalert-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.4.5/sck/emailalert.py` & `emailalert-1.4.6/sck/emailalert.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     # Create a MIME text object
     #msg = MIMEText(message)
     msg = MIMEMultipart()
     msg['Subject'] = subject
     msg['From'] = sender
     #msg['To'] = recipient
     msg['To'] = ';'.join(recipients)
-    msg['cc'] = ';'.join(recipients_cc)
+    msg['CC'] = ';'.join(recipients_cc)
 
     table_html = ''
     if folder_paths != 'null':
         # Get all file paths in the folders
         attachment_paths,attachment_filename = get_files_in_folders(folder_paths)
 
         # Create the HTML table with CSS styles
```


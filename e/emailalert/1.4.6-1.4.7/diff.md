# Comparing `tmp/emailalert-1.4.6.tar.gz` & `tmp/emailalert-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.4.6.tar", last modified: Fri Jul  7 02:50:10 2023, max compression
+gzip compressed data, was "emailalert-1.4.7.tar", last modified: Fri Jul  7 06:00:03 2023, max compression
```

## Comparing `emailalert-1.4.6.tar` & `emailalert-1.4.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 02:50:10.407427 emailalert-1.4.6/
--rw-rw-rw-   0        0        0      178 2023-07-07 02:50:10.402171 emailalert-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-07-07 02:16:16.000000 emailalert-1.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 02:50:10.338172 emailalert-1.4.6/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-07-07 02:50:10.000000 emailalert-1.4.6/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-07-07 02:50:10.000000 emailalert-1.4.6/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 02:50:10.000000 emailalert-1.4.6/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-07 02:50:10.000000 emailalert-1.4.6/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-07 02:50:10.379761 emailalert-1.4.6/sck/
--rw-rw-rw-   0        0        0        0 2023-07-07 01:24:44.000000 emailalert-1.4.6/sck/__init__.py
--rw-rw-rw-   0        0        0     4395 2023-07-07 02:49:25.000000 emailalert-1.4.6/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-07-07 02:50:10.415453 emailalert-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-07-07 02:49:58.000000 emailalert-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 06:00:03.572757 emailalert-1.4.7/
+-rw-rw-rw-   0        0        0      178 2023-07-07 06:00:03.569780 emailalert-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-07-07 02:16:16.000000 emailalert-1.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 06:00:03.534050 emailalert-1.4.7/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-07-07 06:00:03.000000 emailalert-1.4.7/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-07-07 06:00:03.000000 emailalert-1.4.7/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 06:00:03.000000 emailalert-1.4.7/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-07 06:00:03.000000 emailalert-1.4.7/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-07 06:00:03.564775 emailalert-1.4.7/sck/
+-rw-rw-rw-   0        0        0        0 2023-07-07 01:24:44.000000 emailalert-1.4.7/sck/__init__.py
+-rw-rw-rw-   0        0        0     2865 2023-07-07 05:59:43.000000 emailalert-1.4.7/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-07-07 06:00:03.573758 emailalert-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-07-07 05:59:50.000000 emailalert-1.4.7/setup.py
```

### Comparing `emailalert-1.4.6/README.md` & `emailalert-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.4.6/sck/emailalert.py` & `emailalert-1.4.7/sck/emailalert.py`

 * *Files 23% similar despite different names*

```diff
@@ -30,57 +30,16 @@
     msg['From'] = sender
     #msg['To'] = recipient
     msg['To'] = ';'.join(recipients)
     msg['CC'] = ';'.join(recipients_cc)
 
     table_html = ''
     if folder_paths != 'null':
-        # Get all file paths in the folders
-        attachment_paths,attachment_filename = get_files_in_folders(folder_paths)
-
-        # Create the HTML table with CSS styles
-        table_html = '''
-        <style>
-            table {
-                border-collapse: collapse;
-                width: 70%;
-            }
-            th {
-                background-color: #f2f2f2;
-            }
-            th, td {
-                border: 1px solid black;
-                padding: 8px;
-                width: 300px;
-                text-align: left;
-            }        
-            table tr:hover {
-                background-color: #e6e6e6 !important;
-            }
-        </style>
-
-        <table>
-            <tr>
-                <th>データ仕様</th>
-                <th>エラー発生ファイル</th>
-            </tr>
-        '''
-        for index, (file_name, file_path) in enumerate(zip(attachment_filename, attachment_paths)):
-            spec = 'MCO'
-            if 'VHS' in file_path:
-                spec = 'LDD'
-            elif 'TT' in file_path:
-                spec = 'Tokyo'
-            row_color = "#d1ffd4" if index % 2 != 0 else "#ffffff"
-            table_html += f'<tr style="background-color: {row_color};" onmouseover="this.style.backgroundColor=\'#e6e6e6\';" onmouseout="this.style.backgroundColor=\'{row_color}\';">'
-            table_html += f'<td style="width:30px;font-weight:bold">{spec}</td><td style="font-weight:bold">{file_name}</td></tr>'
-            
-
-        table_html += '</table>'
-
+        table_html = folder_paths
+       
     # Create the email body as HTML
     message = message_header
     message += f'<html><body>{table_html}</body></html>'
     message += message_footer
 
     # Attach the email body
     msg.attach(MIMEText(message, 'html'))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```


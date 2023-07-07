# Comparing `tmp/vastai-0.1.3.tar.gz` & `tmp/vastai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vastai-0.1.3.tar", last modified: Thu Jun 15 21:40:39 2023, max compression
+gzip compressed data, was "vastai-0.1.4.tar", last modified: Fri Jul  7 02:25:46 2023, max compression
```

## Comparing `vastai-0.1.3.tar` & `vastai-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:40:39.157441 vastai-0.1.3/
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)     1064 2023-06-15 20:54:21.000000 vastai-0.1.3/LICENSE.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       38 2023-06-15 20:55:37.000000 vastai-0.1.3/MANIFEST.in
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33954 2023-06-15 21:40:39.157441 vastai-0.1.3/PKG-INFO
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33343 2023-06-15 21:40:11.000000 vastai-0.1.3/README.md
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      641 2023-06-15 21:40:32.000000 vastai-0.1.3/pyproject.toml
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       38 2023-06-15 21:40:39.157441 vastai-0.1.3/setup.cfg
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)     1054 2023-06-15 21:20:12.000000 vastai-0.1.3/setup.py
-drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:40:39.157441 vastai-0.1.3/vastai/
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:02:15.000000 vastai-0.1.3/vastai/__init__.py
--rwxrwxr-x   0 jcannell  (1000) jcannell  (1000)    75501 2023-06-15 20:33:35.000000 vastai-0.1.3/vastai/vast.py
-drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:40:39.157441 vastai-0.1.3/vastai.egg-info/
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33954 2023-06-15 21:40:39.000000 vastai-0.1.3/vastai.egg-info/PKG-INFO
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      283 2023-06-15 21:40:39.000000 vastai-0.1.3/vastai.egg-info/SOURCES.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        1 2023-06-15 21:40:39.000000 vastai-0.1.3/vastai.egg-info/dependency_links.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       44 2023-06-15 21:40:39.000000 vastai-0.1.3/vastai.egg-info/entry_points.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        9 2023-06-15 21:40:39.000000 vastai-0.1.3/vastai.egg-info/requires.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        7 2023-06-15 21:40:39.000000 vastai-0.1.3/vastai.egg-info/top_level.txt
+drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-07-07 02:25:46.700773 vastai-0.1.4/
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)     1064 2023-06-15 20:54:21.000000 vastai-0.1.4/LICENSE.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       38 2023-06-15 20:55:37.000000 vastai-0.1.4/MANIFEST.in
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33954 2023-07-07 02:25:46.700773 vastai-0.1.4/PKG-INFO
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33343 2023-06-15 21:40:11.000000 vastai-0.1.4/README.md
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      641 2023-07-07 02:25:38.000000 vastai-0.1.4/pyproject.toml
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       38 2023-07-07 02:25:46.700773 vastai-0.1.4/setup.cfg
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)     1054 2023-07-07 02:25:30.000000 vastai-0.1.4/setup.py
+drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-07-07 02:25:46.700773 vastai-0.1.4/vastai/
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:02:15.000000 vastai-0.1.4/vastai/__init__.py
+-rwxrwxr-x   0 jcannell  (1000) jcannell  (1000)    76750 2023-07-06 22:53:54.000000 vastai-0.1.4/vastai/vast.py
+drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-07-07 02:25:46.700773 vastai-0.1.4/vastai.egg-info/
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33954 2023-07-07 02:25:46.000000 vastai-0.1.4/vastai.egg-info/PKG-INFO
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      283 2023-07-07 02:25:46.000000 vastai-0.1.4/vastai.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        1 2023-07-07 02:25:46.000000 vastai-0.1.4/vastai.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       44 2023-07-07 02:25:46.000000 vastai-0.1.4/vastai.egg-info/entry_points.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        9 2023-07-07 02:25:46.000000 vastai-0.1.4/vastai.egg-info/requires.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        7 2023-07-07 02:25:46.000000 vastai-0.1.4/vastai.egg-info/top_level.txt
```

### Comparing `vastai-0.1.3/LICENSE.txt` & `vastai-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vastai-0.1.3/PKG-INFO` & `vastai-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastai
-Version: 0.1.3
+Version: 0.1.4
 Summary: Vast.ai Python CLI
 Home-page: https://github.com/vast-ai/vast-python
 Author: Vast.ai
 Author-email: "vast.ai" <support@vast.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/vast-ai/vast-python
 Project-URL: Bug Tracker, https://github.com/vast-ai/vast-python/issues
```

### Comparing `vastai-0.1.3/README.md` & `vastai-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vastai-0.1.3/pyproject.toml` & `vastai-0.1.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vastai"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="vast.ai", email="support@vast.ai" },
 ]
 description = "Vast.ai Python CLI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `vastai-0.1.3/setup.py` & `vastai-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='vastai',
-    version='0.1.0',  # choose your own version
+    version='0.1.4',  # choose your own version
     packages=['vastai'],
     entry_points={
         'console_scripts': [
             'vastai = vastai.vast:main',  # you need a main function in your vast.py file
         ],
     },
     description='Vast.ai Python CLI',
```

### Comparing `vastai-0.1.3/vastai/vast.py` & `vastai-0.1.4/vastai/vast.py`

 * *Files 2% similar despite different names*

```diff
@@ -1006,14 +1006,43 @@
             print(rj["msg"]);
     else:
         print(r.text);
         print("failed with error {r.status_code}".format(**locals()));
 
 
 
+@parser.command(
+    argument("id", help="id of instance to prepay for", type=int),
+    argument("amount", help="amount of instance credit prepayment (default discount func of 0.2 for 1 month, 0.3 for 3 months)", type=float),
+    usage="./vast prepay instance <id> <amount>",
+    help="Deposit credits into reserved instance.",
+)
+def prepay__instance(args):
+    """
+    :param argparse.Namespace args: should supply all the command-line options
+    :rtype:
+    """
+    url       = apiurl(args, "/instances/prepay/{id}/".format(id=args.id))
+    json_blob = { "amount": args.amount }
+    if (args.explain):
+        print("request json: ")
+        print(json_blob)
+    r = requests.put(url, json=json_blob)
+    r.raise_for_status()
+
+    rj = r.json();
+    if rj["success"]:
+        timescale = round( rj["timescale"], 3)
+        discount_rate = 100.0*round( rj["discount_rate"], 3)
+        print("prepaid for {timescale} months of instance {args.id} applying ${args.amount} credits for a discount of {discount_rate}%.".format(**(locals())));
+    else:
+        print(rj["msg"]);
+
+'''
+'''
 
 
 @parser.command(
     argument("id", help="id of instance to reboot", type=int),
     usage="./vast reboot instance <id> [--raw]",
     help="Reboot (stop/start) an instance",
 )
@@ -1704,14 +1733,15 @@
 @parser.command(
     argument("id", help="id of machine to list", type=int),
     argument("-g", "--price_gpu", help="per gpu rental price in $/hour  (price for active instances)", type=float),
     argument("-s", "--price_disk",
              help="storage price in $/GB/month (price for inactive instances), default: $0.15/GB/month", type=float),
     argument("-u", "--price_inetu", help="price for internet upload bandwidth in $/GB", type=float),
     argument("-d", "--price_inetd", help="price for internet download bandwidth in $/GB", type=float),
+    argument("-r", "--discount_rate", help="Max long term prepay discount rate fraction, default: 0.4 ", type=float),
     argument("-m", "--min_chunk", help="minimum amount of gpus", type=int),
     argument("-e", "--end_date", help="unix timestamp of the available until date (optional)", type=int),
     usage="./vast list machine id [--price_gpu PRICE_GPU] [--price_inetu PRICE_INETU] [--price_inetd PRICE_INETD] [--api-key API_KEY]",
     help="[Host] list a machine for rent",
 )
 def list__machine(args):
     """
@@ -1719,31 +1749,32 @@
 
     :param argparse.Namespace args: should supply all the command-line options
     :rtype:
     """
     req_url = apiurl(args, "/machines/create_asks/")
 
     json_blob = {'machine': args.id, 'price_gpu': args.price_gpu,
-                                    'price_disk': args.price_disk, 'price_inetu': args.price_inetu,
-                                    'price_inetd': args.price_inetd, 'min_chunk': args.min_chunk,
-                                    'end_date': args.end_date}
+                        'price_disk': args.price_disk, 'price_inetu': args.price_inetu,
+                        'price_inetd': args.price_inetd, 'min_chunk': args.min_chunk,
+                        'end_date': args.end_date, 'credit_discount_max': args.discount_rate}
     if (args.explain):
         print("request json: ")
         print(json_blob)
     r = requests.put(req_url, json=json_blob)
     if (r.status_code == 200):
         rj = r.json();
         if (rj["success"]):
             price_gpu_ = str(args.price_gpu) if args.price_gpu is not None else "def";
             price_inetu_ = str(args.price_inetu);
             price_inetd_ = str(args.price_inetd);
             min_chunk_ = str(args.min_chunk);
             end_date_ = str(args.end_date);
+            discount_rate_ = str(args.discount_rate)
             print(
-                "offers created for machine {args.id},  @ ${price_gpu_}/gpu/day, ${price_inetu_}/GB up, ${price_inetd_}/GB down, {min_chunk_}/min gpus, till {end_date_}".format(
+                "offers created for machine {args.id},  @ ${price_gpu_}/gpu/day, ${price_inetu_}/GB up, ${price_inetd_}/GB down, {min_chunk_}/min gpus, max discount_rate {discount_rate_}, till {end_date_}".format(
                     **locals()));
         else:
             print(rj["msg"]);
     else:
         print(r.text);
         print("failed with error {r.status_code}".format(**locals()));
 
@@ -1921,15 +1952,15 @@
 
 
 @parser.command(
     argument("id", help="id of machine to schedule maintenance for", type=int),
     argument("--sdate",      help="maintenance start date in unix epoch time (UTC seconds)", type=float),
     argument("--duration",   help="maintenance duration in hours", type=float),
     usage="./vast schedule maintenance id [--sdate START_DATE --duration DURATION]",
-    help="[Host] Schedule an upcoming maintenance window for a machine, notifying active clients",
+    help="[Host] Schedule upcoming maint window",
     epilog=deindent("""
         Example: ./vast.py schedule maint 8207 --sdate 1677562671 --duration 0.5
     """),
     )
 def schedule__maint(args):
     """
     :param argparse.Namespace args: should supply all the command-line options
```

### Comparing `vastai-0.1.3/vastai.egg-info/PKG-INFO` & `vastai-0.1.4/vastai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastai
-Version: 0.1.3
+Version: 0.1.4
 Summary: Vast.ai Python CLI
 Home-page: https://github.com/vast-ai/vast-python
 Author: Vast.ai
 Author-email: "vast.ai" <support@vast.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/vast-ai/vast-python
 Project-URL: Bug Tracker, https://github.com/vast-ai/vast-python/issues
```


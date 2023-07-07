# Comparing `tmp/ztffp-2.0.0.tar.gz` & `tmp/ztffp-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztffp-2.0.0.tar", last modified: Sat May 20 19:20:38 2023, max compression
+gzip compressed data, was "ztffp-2.0.1.tar", last modified: Fri Jul  7 19:37:48 2023, max compression
```

## Comparing `ztffp-2.0.0.tar` & `ztffp-2.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 stroh     (1000) stroh     (1000)        0 2023-05-20 19:20:38.653017 ztffp-2.0.0/
--rw-r--r--   0 stroh     (1000) stroh     (1000)    35148 2023-05-19 18:21:17.000000 ztffp-2.0.0/LICENSE.txt
--rw-r--r--   0 stroh     (1000) stroh     (1000)    41186 2023-05-20 19:20:38.653017 ztffp-2.0.0/PKG-INFO
--rwxr-xr-x   0 stroh     (1000) stroh     (1000)     9839 2023-05-18 17:29:18.000000 ztffp-2.0.0/README.md
--rw-r--r--   0 stroh     (1000) stroh     (1000)      962 2023-05-20 00:49:35.000000 ztffp-2.0.0/pyproject.toml
--rw-r--r--   0 stroh     (1000) stroh     (1000)       38 2023-05-20 19:20:38.653017 ztffp-2.0.0/setup.cfg
-drwxr-xr-x   0 stroh     (1000) stroh     (1000)        0 2023-05-20 19:20:38.646350 ztffp-2.0.0/src/
-drwxr-xr-x   0 stroh     (1000) stroh     (1000)        0 2023-05-20 19:20:38.653017 ztffp-2.0.0/src/ztffp.egg-info/
--rw-r--r--   0 stroh     (1000) stroh     (1000)    41186 2023-05-20 19:20:38.000000 ztffp-2.0.0/src/ztffp.egg-info/PKG-INFO
--rw-r--r--   0 stroh     (1000) stroh     (1000)      213 2023-05-20 19:20:38.000000 ztffp-2.0.0/src/ztffp.egg-info/SOURCES.txt
--rw-r--r--   0 stroh     (1000) stroh     (1000)        1 2023-05-20 19:20:38.000000 ztffp-2.0.0/src/ztffp.egg-info/dependency_links.txt
--rw-r--r--   0 stroh     (1000) stroh     (1000)       73 2023-05-20 19:20:38.000000 ztffp-2.0.0/src/ztffp.egg-info/requires.txt
--rw-r--r--   0 stroh     (1000) stroh     (1000)        6 2023-05-20 19:20:38.000000 ztffp-2.0.0/src/ztffp.egg-info/top_level.txt
--rwxr-xr-x   0 stroh     (1000) stroh     (1000)    27974 2023-05-20 00:21:15.000000 ztffp-2.0.0/src/ztffp.py
+drwxr-xr-x   0 stroh     (1000) stroh     (1000)        0 2023-07-07 19:37:48.037967 ztffp-2.0.1/
+-rw-r--r--   0 stroh     (1000) stroh     (1000)    35148 2023-05-19 18:21:17.000000 ztffp-2.0.1/LICENSE.txt
+-rw-r--r--   0 stroh     (1000) stroh     (1000)    51066 2023-07-07 19:37:48.037967 ztffp-2.0.1/PKG-INFO
+-rwxr-xr-x   0 stroh     (1000) stroh     (1000)     9839 2023-05-18 17:29:18.000000 ztffp-2.0.1/README.md
+-rw-r--r--   0 stroh     (1000) stroh     (1000)      983 2023-07-07 19:35:29.000000 ztffp-2.0.1/pyproject.toml
+-rw-r--r--   0 stroh     (1000) stroh     (1000)       38 2023-07-07 19:37:48.037967 ztffp-2.0.1/setup.cfg
+drwxr-xr-x   0 stroh     (1000) stroh     (1000)        0 2023-07-07 19:37:48.037967 ztffp-2.0.1/src/
+-rw-r--r--   0 stroh     (1000) stroh     (1000)        0 2023-05-22 23:36:39.000000 ztffp-2.0.1/src/__init__.py
+drwxr-xr-x   0 stroh     (1000) stroh     (1000)        0 2023-07-07 19:37:48.037967 ztffp-2.0.1/src/ztffp.egg-info/
+-rw-r--r--   0 stroh     (1000) stroh     (1000)    51066 2023-07-07 19:37:48.000000 ztffp-2.0.1/src/ztffp.egg-info/PKG-INFO
+-rw-r--r--   0 stroh     (1000) stroh     (1000)      229 2023-07-07 19:37:48.000000 ztffp-2.0.1/src/ztffp.egg-info/SOURCES.txt
+-rw-r--r--   0 stroh     (1000) stroh     (1000)        1 2023-07-07 19:37:48.000000 ztffp-2.0.1/src/ztffp.egg-info/dependency_links.txt
+-rw-r--r--   0 stroh     (1000) stroh     (1000)       73 2023-07-07 19:37:48.000000 ztffp-2.0.1/src/ztffp.egg-info/requires.txt
+-rw-r--r--   0 stroh     (1000) stroh     (1000)       15 2023-07-07 19:37:48.000000 ztffp-2.0.1/src/ztffp.egg-info/top_level.txt
+-rwxr-xr-x   0 stroh     (1000) stroh     (1000)    27974 2023-05-20 00:21:15.000000 ztffp-2.0.1/src/ztffp.py
```

### Comparing `ztffp-2.0.0/LICENSE.txt` & `ztffp-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ztffp-2.0.0/PKG-INFO` & `ztffp-2.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ztffp
-Version: 2.0.0
+Version: 2.0.1
 Summary: ZTF Forced-Photometry library (Unaffiliated)
 Author-email: "Michael C. Stroh" <ztffp@michaelcstroh.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,8 +682,246 @@
 Project-URL: Source, https://github.com/mcstroh/ztffp/
 Keywords: astronomy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+
+# ztf_fp
+Author: Michael C. Stroh, Northwestern University
+
+Website: [www.michaelcstroh.com](https://www.michaelcstroh.com)
+
+A python library to streamline requesting Zwicky Transient Facility (ZTF) forced photometry.
+
+## A simple command line example
+
+```
+python ztf_fp.py 256.7975042 58.0974194 -source_name 2021kjb
+```
+### Output
+```
+Sending ZTF request for (R.A.,Decl)=(256.7975042,58.0974194)
+wget --http-user=ztffps --http-passwd=dontgocrazy! -O ztffp_493YUZW74Q.txt "https://ztfweb.ipac.caltech.edu/cgi-bin/requestForcedPhotometry.cgi?ra=256.797504&dec=58.097419&jdstart=2459269.628723&jdend=2459329.628723&email=<REDACTED>&userpass=<REDACTED>"
+
+Waiting for the email (rechecking every 20 seconds).
+Downloading file...
+	wget --http-user=ztffps --http-password=dontgocrazy! -O forcedphotometry_req00015274_lc.txt "https://ztfweb.ipac.caltech.edu/ztf/ops/forcedphot/lc/0/15/req15274/cksum16bf0dfcd7fc6781336f6d0792a8874d/forcedphotometry_req00015274_lc.txt"
+Downloading file...
+	wget --http-user=ztffps --http-password=dontgocrazy! -O forcedphotometry_req00015274_log.txt "https://ztfweb.ipac.caltech.edu/ztf/ops/forcedphot/lc/0/15/req15274/cksum16bf0dfcd7fc6781336f6d0792a8874d/forcedphotometry_req00015274_log.txt"
+Downloaded: 2021kjb_lc.txt
+Downloaded: 2021kjb_log.txt
+ZTF_r: 15 detections and 3 upper limits.
+ZTF_g: 13 detections and 4 upper limits.
+Creating ./2021kjb
+     ZTF wget log: ./2021kjb/ztffp_493YUZW74Q.txt
+     ZTF downloaded file: ./2021kjb/2021kjb_lc.txt
+     ZTF downloaded file: ./2021kjb/2021kjb_log.txt
+     ZTF figure: ./2021kjb/2021kjb_lc.png
+```
+
+## Requirements
+### Software installed on your system
+- python 3.6+
+- wget (MacOS often is missing this. If so, check out brew, macports or anaconda.)
+- Email address reachable with IMAP
+
+### Python libraries
+- astropy (for possible time and coordinate conversions)
+- matplotlib (for possible plotting, but easily removable)
+- numpy
+- pandas 
+- lxml
+
+## Installation
+```
+git clone https://github.com/mcstroh/ztf_fp.git
+```
+
+## Setup
+The library requires your ZTF forced photometry credentials (email and password), and your credentials to access your email address where the links to the ZTF light curve are sent.
+
+For bash/zsh equivalents (e.g., .bashrc, .bash_profile, .zshrc, etc)
+
+```
+### ZTF forced photometry service
+ztf_email_address="john_doe@mydomain.com"
+ztf_email_password="1234567890password"
+ztf_email_imapserver="imap.mydomain.com"
+ztf_user_password="01234ztf"
+export ztf_email_address
+export ztf_email_password
+export ztf_email_imapserver
+export ztf_user_password
+```
+
+or for csh/tcsh equivalents (e.g.,.cshrc, tcshrc, etc.)
+
+```
+setenv ztf_email_address john_doe@mydomain.com
+setenv ztf_email_password 1234567890password
+setenv ztf_email_imapserver imap.mydomain.com
+setenv ztf_user_password 01234ztf
+```
+
+Note that if the email you registered with the ZTF forced photometry is an alias for another address, you will need to also define
+
+```
+ztf_user_address="john_doe_1234@mydomain.com"
+export ztf_user_address
+```
+or the equivalent for csh and tcsh shells.
+
+### Check your email configuration - IMPORTANT TO DO THIS FIRST!
+It is important to verify that the script is able to use your email credentials so that you don't spam the ZTF forced photometry service with duplicate requests while you debug your email setup.
+
+Run the following to see if the script can access your email with the provided credentials.
+
+#### Input
+```
+python ztf_fp.py -emailtest
+```
+#### Successful output
+```
+Your email inbox was found and contains 600 messages.
+If this is not correct, please check your settings.
+```
+#### Output if it definitely is not working
+```
+Your inbox was not located. Please check your settings.
+```
+
+
+## More about running on the command line
+
+Sexagesimal coordinates are also supported:
+```
+python ztf_fp.py 17:07:11.40 +58:05:50.71 -source_name 2021kjb
+```
+
+By default, the script requests forced photometry from the 60 days prior to the moment you submit the job (equivalent to ```-days 60```), but this is easily changed. 
+
+You may also specify date ranges in JD (```-jdstart``` and ```-jdend``` arguments) or MJD (```-mjdstart``` and ```-mjdend``` arguments).
+
+
+### List of available options
+```
+usage: ztf_fp.py <ra> <decl> [-h] [-logfile [logfile]] [-plotfile [plotfile]] [-emailtest] [-source_name [source_name]] [-mjdstart [mjdstart]]
+                             [-mjdend [mjdend]] [-jdstart [jdstart]] [-jdend [jdend]] [-ztf_all_jd] [-days [days]] [-emailcheck [emailcheck]]
+                             [-skip_clean] [-directory_path [directory_path]] [-fivemindelay [fivemindelay]] [-skip_plot]
+                             [ra] [decl]
+
+Grab ZTF forced photometry on the given location.
+
+positional arguments:
+  ra                    Right ascension of the target. Can be provided in DDD.ddd or HH:MM:SS.ss formats.
+  decl                  Declination of the target. Can be provided in +/-DDD.ddd or DD:MM:SS.ss formats.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -logfile [logfile]    Log file to process instead of submitting a new job.
+  -plotfile [plotfile]  Light curve file to plot instead of submitting and downloading a new job.
+  -emailtest            Test your email settings. This is performed without sending a request to the ZTF server.
+  -source_name [source_name]
+                        Source name that will be used to name output files.
+  -mjdstart [mjdstart]  Start of date range for forced photometry query. Overrides -jdstart.
+  -mjdend [mjdend]      End of date range for forced photometry query. Overrides -jdstop
+  -jdstart [jdstart]    Start of date range for forced photometry query.
+  -jdend [jdend]        End of date range for forced photometry query.
+  -ztf_all_jd           Use the full range of ZTF public dates.
+  -days [days]          Number of days prior to jdend to query (or number of days prior to today if jdend is not given).
+  -emailcheck [emailcheck]
+                        How often to recheck your email for the ZTF results.
+  -skip_clean           After completion skip placing all output files in the same directory.
+  -directory_path [directory_path]
+                        Path to directory for clean-up. Requires -directory option.
+  -fivemindelay [fivemindelay]
+                        How often (in seconds) to query the email after 5 minutes have elapsed.
+  -skip_plot            Skip making the plot. Useful for automated and batch use cases, or if user wants to use their personal plotting code.
+```
+
+## Automated / batch job requests
+
+This file supports being imported as a library and called for batch processing. See ztf_bulk_example.py for a working example of calling ztf_fp.py using an external script.
+
+Below we show the body of ztf_bulk_example.py
+```
+#! python
+#
+# Run ztf_fp.py on a list of coordinates
+#
+# M.C. Stroh (Northwestern University)
+#
+#
+from multiprocessing import Pool, cpu_count
+import numpy as np
+import pandas as pd
+import ztf_fp
+
+
+
+def ztf_forced_photometry(row):
+
+    # Send ZTF forced photometry request
+    ztf_file_names = ztf_fp.run_ztf_fp(days=20, ra=row.ra, decl=row.decl, source_name=row.source_name, directory_path='/tmp', verbose=False, do_plot=False)
+    
+
+    #
+    # Do something intelligent with the output
+    #     For this example we'll simply list the files
+    for ztf_file_name in ztf_file_names:
+        print(ztf_file_name)
+
+    return
+
+
+
+def batch_ztf_forced_photometry():
+
+    #
+    # Populate a pandas dataframe with the positions you are interested in
+    # This is a simple example using a couple of SN Ia discovered by the Young Supernova Experiment
+    data = [['2021kcc',194.0331000,-4.9606139],['2021jze',154.9723750,-3.7354000]]
+    
+    # The column names are used in the ztf_forced_photometry function defined above
+    df = pd.DataFrame(data, columns = ['source_name','ra','decl'])
+
+
+    n_workers = int(np.floor(cpu_count()/2)) # Requires casting as an integer for pool argument / don't hit the ZTF server too hard
+    pool_vals = [x for _, x in df.iterrows()] # Turn to list for pool mapping function below
+
+    # Now send to the list to be completed
+    print(f"Processing {len(pool_vals)} ZTF forced photometry requests utilizing {n_workers} workers.")
+    ztf_pool = Pool(n_workers)
+    res = ztf_pool.map(ztf_forced_photometry, pool_vals)  
+    ztf_pool.close()
+    ztf_pool.join()
+
+
+
+if __name__ == "__main__":
+    batch_ztf_forced_photometry()
+```
+
+### Output
+```
+Processing 2 ZTF forced photometry requests utilizing 4 workers.
+Sending ZTF request for (R.A.,Decl)=(194.0331,-4.9606139)
+wget --http-user=ztffps --http-passwd=dontgocrazy! -O ztffp_TAFLM4V59R.txt "https://ztfweb.ipac.caltech.edu/cgi-bin/requestForcedPhotometry.cgi?ra=194.0331&dec=-4.960614&jdstart=2459311.592520&jdend=2459331.592520&email=<REDACTED>&userpass=<REDACTED>"
+Sending ZTF request for (R.A.,Decl)=(154.972375,-3.7354)
+wget --http-user=ztffps --http-passwd=dontgocrazy! -O ztffp_4B3X481ZRP.txt "https://ztfweb.ipac.caltech.edu/cgi-bin/requestForcedPhotometry.cgi?ra=154.972375&dec=-3.7354&jdstart=2459311.592520&jdend=2459331.592520&email=<REDACTED>&userpass=<REDACTED>"
+
+
+/tmp/2021kcc/ztffp_TAFLM4V59R.txt
+/tmp/2021kcc/2021kcc_lc.txt
+/tmp/2021kcc/2021kcc_log.txt
+/tmp/2021jze/ztffp_4B3X481ZRP.txt
+/tmp/2021jze/2021jze_lc.txt
+/tmp/2021jze/2021jze_log.txt
+```
+If you are not interested in the output files, you can direct the files to /tmp using the ```-directory_path``` option similar to the above example.
+
+## Acknowledgements
+This project is created at the [Center for Interdisciplinary Exploration and Research in Astrophysics](https://ciera.northwestern.edu) at [Northwestern University](https://www.northwestern.edu/). This work is supported by the Heising-Simons Foundation under grant #2018-0911 awarded to [Raffaella Margutti](https://sites.northwestern.edu/raffaellamargutti).
```

### Comparing `ztffp-2.0.0/README.md` & `ztffp-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ztffp-2.0.0/pyproject.toml` & `ztffp-2.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [project]
 name = "ztffp"
-version = "2.0.0"
+version = "2.0.1"
 description = "ZTF Forced-Photometry library (Unaffiliated)"
+readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
 keywords = ["astronomy"]
 authors = [
   {name = "Michael C. Stroh", email = "ztffp@michaelcstroh.com" }
 ]
 classifiers = [
```

### Comparing `ztffp-2.0.0/src/ztffp.egg-info/PKG-INFO` & `ztffp-2.0.1/src/ztffp.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ztffp
-Version: 2.0.0
+Version: 2.0.1
 Summary: ZTF Forced-Photometry library (Unaffiliated)
 Author-email: "Michael C. Stroh" <ztffp@michaelcstroh.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,8 +682,246 @@
 Project-URL: Source, https://github.com/mcstroh/ztffp/
 Keywords: astronomy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+
+# ztf_fp
+Author: Michael C. Stroh, Northwestern University
+
+Website: [www.michaelcstroh.com](https://www.michaelcstroh.com)
+
+A python library to streamline requesting Zwicky Transient Facility (ZTF) forced photometry.
+
+## A simple command line example
+
+```
+python ztf_fp.py 256.7975042 58.0974194 -source_name 2021kjb
+```
+### Output
+```
+Sending ZTF request for (R.A.,Decl)=(256.7975042,58.0974194)
+wget --http-user=ztffps --http-passwd=dontgocrazy! -O ztffp_493YUZW74Q.txt "https://ztfweb.ipac.caltech.edu/cgi-bin/requestForcedPhotometry.cgi?ra=256.797504&dec=58.097419&jdstart=2459269.628723&jdend=2459329.628723&email=<REDACTED>&userpass=<REDACTED>"
+
+Waiting for the email (rechecking every 20 seconds).
+Downloading file...
+	wget --http-user=ztffps --http-password=dontgocrazy! -O forcedphotometry_req00015274_lc.txt "https://ztfweb.ipac.caltech.edu/ztf/ops/forcedphot/lc/0/15/req15274/cksum16bf0dfcd7fc6781336f6d0792a8874d/forcedphotometry_req00015274_lc.txt"
+Downloading file...
+	wget --http-user=ztffps --http-password=dontgocrazy! -O forcedphotometry_req00015274_log.txt "https://ztfweb.ipac.caltech.edu/ztf/ops/forcedphot/lc/0/15/req15274/cksum16bf0dfcd7fc6781336f6d0792a8874d/forcedphotometry_req00015274_log.txt"
+Downloaded: 2021kjb_lc.txt
+Downloaded: 2021kjb_log.txt
+ZTF_r: 15 detections and 3 upper limits.
+ZTF_g: 13 detections and 4 upper limits.
+Creating ./2021kjb
+     ZTF wget log: ./2021kjb/ztffp_493YUZW74Q.txt
+     ZTF downloaded file: ./2021kjb/2021kjb_lc.txt
+     ZTF downloaded file: ./2021kjb/2021kjb_log.txt
+     ZTF figure: ./2021kjb/2021kjb_lc.png
+```
+
+## Requirements
+### Software installed on your system
+- python 3.6+
+- wget (MacOS often is missing this. If so, check out brew, macports or anaconda.)
+- Email address reachable with IMAP
+
+### Python libraries
+- astropy (for possible time and coordinate conversions)
+- matplotlib (for possible plotting, but easily removable)
+- numpy
+- pandas 
+- lxml
+
+## Installation
+```
+git clone https://github.com/mcstroh/ztf_fp.git
+```
+
+## Setup
+The library requires your ZTF forced photometry credentials (email and password), and your credentials to access your email address where the links to the ZTF light curve are sent.
+
+For bash/zsh equivalents (e.g., .bashrc, .bash_profile, .zshrc, etc)
+
+```
+### ZTF forced photometry service
+ztf_email_address="john_doe@mydomain.com"
+ztf_email_password="1234567890password"
+ztf_email_imapserver="imap.mydomain.com"
+ztf_user_password="01234ztf"
+export ztf_email_address
+export ztf_email_password
+export ztf_email_imapserver
+export ztf_user_password
+```
+
+or for csh/tcsh equivalents (e.g.,.cshrc, tcshrc, etc.)
+
+```
+setenv ztf_email_address john_doe@mydomain.com
+setenv ztf_email_password 1234567890password
+setenv ztf_email_imapserver imap.mydomain.com
+setenv ztf_user_password 01234ztf
+```
+
+Note that if the email you registered with the ZTF forced photometry is an alias for another address, you will need to also define
+
+```
+ztf_user_address="john_doe_1234@mydomain.com"
+export ztf_user_address
+```
+or the equivalent for csh and tcsh shells.
+
+### Check your email configuration - IMPORTANT TO DO THIS FIRST!
+It is important to verify that the script is able to use your email credentials so that you don't spam the ZTF forced photometry service with duplicate requests while you debug your email setup.
+
+Run the following to see if the script can access your email with the provided credentials.
+
+#### Input
+```
+python ztf_fp.py -emailtest
+```
+#### Successful output
+```
+Your email inbox was found and contains 600 messages.
+If this is not correct, please check your settings.
+```
+#### Output if it definitely is not working
+```
+Your inbox was not located. Please check your settings.
+```
+
+
+## More about running on the command line
+
+Sexagesimal coordinates are also supported:
+```
+python ztf_fp.py 17:07:11.40 +58:05:50.71 -source_name 2021kjb
+```
+
+By default, the script requests forced photometry from the 60 days prior to the moment you submit the job (equivalent to ```-days 60```), but this is easily changed. 
+
+You may also specify date ranges in JD (```-jdstart``` and ```-jdend``` arguments) or MJD (```-mjdstart``` and ```-mjdend``` arguments).
+
+
+### List of available options
+```
+usage: ztf_fp.py <ra> <decl> [-h] [-logfile [logfile]] [-plotfile [plotfile]] [-emailtest] [-source_name [source_name]] [-mjdstart [mjdstart]]
+                             [-mjdend [mjdend]] [-jdstart [jdstart]] [-jdend [jdend]] [-ztf_all_jd] [-days [days]] [-emailcheck [emailcheck]]
+                             [-skip_clean] [-directory_path [directory_path]] [-fivemindelay [fivemindelay]] [-skip_plot]
+                             [ra] [decl]
+
+Grab ZTF forced photometry on the given location.
+
+positional arguments:
+  ra                    Right ascension of the target. Can be provided in DDD.ddd or HH:MM:SS.ss formats.
+  decl                  Declination of the target. Can be provided in +/-DDD.ddd or DD:MM:SS.ss formats.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -logfile [logfile]    Log file to process instead of submitting a new job.
+  -plotfile [plotfile]  Light curve file to plot instead of submitting and downloading a new job.
+  -emailtest            Test your email settings. This is performed without sending a request to the ZTF server.
+  -source_name [source_name]
+                        Source name that will be used to name output files.
+  -mjdstart [mjdstart]  Start of date range for forced photometry query. Overrides -jdstart.
+  -mjdend [mjdend]      End of date range for forced photometry query. Overrides -jdstop
+  -jdstart [jdstart]    Start of date range for forced photometry query.
+  -jdend [jdend]        End of date range for forced photometry query.
+  -ztf_all_jd           Use the full range of ZTF public dates.
+  -days [days]          Number of days prior to jdend to query (or number of days prior to today if jdend is not given).
+  -emailcheck [emailcheck]
+                        How often to recheck your email for the ZTF results.
+  -skip_clean           After completion skip placing all output files in the same directory.
+  -directory_path [directory_path]
+                        Path to directory for clean-up. Requires -directory option.
+  -fivemindelay [fivemindelay]
+                        How often (in seconds) to query the email after 5 minutes have elapsed.
+  -skip_plot            Skip making the plot. Useful for automated and batch use cases, or if user wants to use their personal plotting code.
+```
+
+## Automated / batch job requests
+
+This file supports being imported as a library and called for batch processing. See ztf_bulk_example.py for a working example of calling ztf_fp.py using an external script.
+
+Below we show the body of ztf_bulk_example.py
+```
+#! python
+#
+# Run ztf_fp.py on a list of coordinates
+#
+# M.C. Stroh (Northwestern University)
+#
+#
+from multiprocessing import Pool, cpu_count
+import numpy as np
+import pandas as pd
+import ztf_fp
+
+
+
+def ztf_forced_photometry(row):
+
+    # Send ZTF forced photometry request
+    ztf_file_names = ztf_fp.run_ztf_fp(days=20, ra=row.ra, decl=row.decl, source_name=row.source_name, directory_path='/tmp', verbose=False, do_plot=False)
+    
+
+    #
+    # Do something intelligent with the output
+    #     For this example we'll simply list the files
+    for ztf_file_name in ztf_file_names:
+        print(ztf_file_name)
+
+    return
+
+
+
+def batch_ztf_forced_photometry():
+
+    #
+    # Populate a pandas dataframe with the positions you are interested in
+    # This is a simple example using a couple of SN Ia discovered by the Young Supernova Experiment
+    data = [['2021kcc',194.0331000,-4.9606139],['2021jze',154.9723750,-3.7354000]]
+    
+    # The column names are used in the ztf_forced_photometry function defined above
+    df = pd.DataFrame(data, columns = ['source_name','ra','decl'])
+
+
+    n_workers = int(np.floor(cpu_count()/2)) # Requires casting as an integer for pool argument / don't hit the ZTF server too hard
+    pool_vals = [x for _, x in df.iterrows()] # Turn to list for pool mapping function below
+
+    # Now send to the list to be completed
+    print(f"Processing {len(pool_vals)} ZTF forced photometry requests utilizing {n_workers} workers.")
+    ztf_pool = Pool(n_workers)
+    res = ztf_pool.map(ztf_forced_photometry, pool_vals)  
+    ztf_pool.close()
+    ztf_pool.join()
+
+
+
+if __name__ == "__main__":
+    batch_ztf_forced_photometry()
+```
+
+### Output
+```
+Processing 2 ZTF forced photometry requests utilizing 4 workers.
+Sending ZTF request for (R.A.,Decl)=(194.0331,-4.9606139)
+wget --http-user=ztffps --http-passwd=dontgocrazy! -O ztffp_TAFLM4V59R.txt "https://ztfweb.ipac.caltech.edu/cgi-bin/requestForcedPhotometry.cgi?ra=194.0331&dec=-4.960614&jdstart=2459311.592520&jdend=2459331.592520&email=<REDACTED>&userpass=<REDACTED>"
+Sending ZTF request for (R.A.,Decl)=(154.972375,-3.7354)
+wget --http-user=ztffps --http-passwd=dontgocrazy! -O ztffp_4B3X481ZRP.txt "https://ztfweb.ipac.caltech.edu/cgi-bin/requestForcedPhotometry.cgi?ra=154.972375&dec=-3.7354&jdstart=2459311.592520&jdend=2459331.592520&email=<REDACTED>&userpass=<REDACTED>"
+
+
+/tmp/2021kcc/ztffp_TAFLM4V59R.txt
+/tmp/2021kcc/2021kcc_lc.txt
+/tmp/2021kcc/2021kcc_log.txt
+/tmp/2021jze/ztffp_4B3X481ZRP.txt
+/tmp/2021jze/2021jze_lc.txt
+/tmp/2021jze/2021jze_log.txt
+```
+If you are not interested in the output files, you can direct the files to /tmp using the ```-directory_path``` option similar to the above example.
+
+## Acknowledgements
+This project is created at the [Center for Interdisciplinary Exploration and Research in Astrophysics](https://ciera.northwestern.edu) at [Northwestern University](https://www.northwestern.edu/). This work is supported by the Heising-Simons Foundation under grant #2018-0911 awarded to [Raffaella Margutti](https://sites.northwestern.edu/raffaellamargutti).
```

### Comparing `ztffp-2.0.0/src/ztffp.py` & `ztffp-2.0.1/src/ztffp.py`

 * *Files identical despite different names*


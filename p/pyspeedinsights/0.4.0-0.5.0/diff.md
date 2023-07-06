# Comparing `tmp/pyspeedinsights-0.4.0.tar.gz` & `tmp/pyspeedinsights-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspeedinsights-0.4.0.tar", last modified: Thu Jul  6 03:19:33 2023, max compression
+gzip compressed data, was "pyspeedinsights-0.5.0.tar", last modified: Thu Jul  6 22:24:26 2023, max compression
```

## Comparing `pyspeedinsights-0.4.0.tar` & `pyspeedinsights-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 03:19:33.918669 pyspeedinsights-0.4.0/
--rw-r--r--   0 will       (501) staff       (20)     1080 2022-05-27 03:33:19.000000 pyspeedinsights-0.4.0/LICENSE
--rw-r--r--   0 will       (501) staff       (20)    13978 2023-07-06 03:19:33.918898 pyspeedinsights-0.4.0/PKG-INFO
--rw-r--r--   0 will       (501) staff       (20)    12781 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/README.md
--rw-r--r--   0 will       (501) staff       (20)      699 2023-07-04 16:04:18.000000 pyspeedinsights-0.4.0/pyproject.toml
--rw-r--r--   0 will       (501) staff       (20)     1625 2023-07-06 03:19:33.919954 pyspeedinsights-0.4.0/setup.cfg
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 03:19:33.900952 pyspeedinsights-0.4.0/src/
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 03:19:33.904585 pyspeedinsights-0.4.0/src/pyspeedinsights/
--rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 03:33:19.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/__init__.py
--rw-r--r--   0 will       (501) staff       (20)      142 2022-06-07 16:31:02.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/__main__.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 03:19:33.911060 pyspeedinsights-0.4.0/src/pyspeedinsights/api/
--rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 04:37:52.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/api/__init__.py
--rw-r--r--   0 will       (501) staff       (20)     2478 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/api/keys.py
--rw-r--r--   0 will       (501) staff       (20)     5239 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/api/request.py
--rw-r--r--   0 will       (501) staff       (20)     5946 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/api/response.py
--rw-r--r--   0 will       (501) staff       (20)     6004 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/app.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 03:19:33.913115 pyspeedinsights-0.4.0/src/pyspeedinsights/cli/
--rw-r--r--   0 will       (501) staff       (20)        0 2022-06-06 20:47:32.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/cli/__init__.py
--rw-r--r--   0 will       (501) staff       (20)     2732 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/cli/choices.py
--rw-r--r--   0 will       (501) staff       (20)     4744 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/cli/commands.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 03:19:33.915038 pyspeedinsights-0.4.0/src/pyspeedinsights/core/
--rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 20:34:15.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/core/__init__.py
--rw-r--r--   0 will       (501) staff       (20)     9243 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/core/excel.py
--rw-r--r--   0 will       (501) staff       (20)     5471 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/core/sitemap.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 03:19:33.918090 pyspeedinsights-0.4.0/src/pyspeedinsights/utils/
--rw-r--r--   0 will       (501) staff       (20)        0 2022-06-06 20:47:32.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/utils/__init__.py
--rw-r--r--   0 will       (501) staff       (20)      174 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/utils/exceptions.py
--rw-r--r--   0 will       (501) staff       (20)      509 2022-11-04 03:53:30.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/utils/generic.py
--rw-r--r--   0 will       (501) staff       (20)     1685 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/utils/urls.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 03:19:33.907399 pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/
--rw-r--r--   0 will       (501) staff       (20)    13978 2023-07-06 03:19:33.000000 pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/PKG-INFO
--rw-r--r--   0 will       (501) staff       (20)      895 2023-07-06 03:19:33.000000 pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/SOURCES.txt
--rw-r--r--   0 will       (501) staff       (20)        1 2023-07-06 03:19:33.000000 pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/dependency_links.txt
--rw-r--r--   0 will       (501) staff       (20)       49 2023-07-06 03:19:33.000000 pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/entry_points.txt
--rw-r--r--   0 will       (501) staff       (20)      154 2023-07-06 03:19:33.000000 pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/requires.txt
--rw-r--r--   0 will       (501) staff       (20)       16 2023-07-06 03:19:33.000000 pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/top_level.txt
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 22:24:26.320972 pyspeedinsights-0.5.0/
+-rw-r--r--   0 will       (501) staff       (20)     1080 2022-05-27 03:33:19.000000 pyspeedinsights-0.5.0/LICENSE
+-rw-r--r--   0 will       (501) staff       (20)    13579 2023-07-06 22:24:26.321122 pyspeedinsights-0.5.0/PKG-INFO
+-rw-r--r--   0 will       (501) staff       (20)    12382 2023-07-06 22:20:00.000000 pyspeedinsights-0.5.0/README.md
+-rw-r--r--   0 will       (501) staff       (20)      699 2023-07-04 16:04:18.000000 pyspeedinsights-0.5.0/pyproject.toml
+-rw-r--r--   0 will       (501) staff       (20)     1625 2023-07-06 22:24:26.321920 pyspeedinsights-0.5.0/setup.cfg
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 22:24:26.310023 pyspeedinsights-0.5.0/src/
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 22:24:26.314734 pyspeedinsights-0.5.0/src/pyspeedinsights/
+-rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 03:33:19.000000 pyspeedinsights-0.5.0/src/pyspeedinsights/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)      142 2022-06-07 16:31:02.000000 pyspeedinsights-0.5.0/src/pyspeedinsights/__main__.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 22:24:26.318086 pyspeedinsights-0.5.0/src/pyspeedinsights/api/
+-rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 04:37:52.000000 pyspeedinsights-0.5.0/src/pyspeedinsights/api/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)     2478 2023-07-06 03:17:10.000000 pyspeedinsights-0.5.0/src/pyspeedinsights/api/keys.py
+-rw-r--r--   0 will       (501) staff       (20)     5239 2023-07-06 03:17:10.000000 pyspeedinsights-0.5.0/src/pyspeedinsights/api/request.py
+-rw-r--r--   0 will       (501) staff       (20)     6210 2023-07-06 22:20:00.000000 pyspeedinsights-0.5.0/src/pyspeedinsights/api/response.py
+-rw-r--r--   0 will       (501) staff       (20)     5644 2023-07-06 22:20:00.000000 pyspeedinsights-0.5.0/src/pyspeedinsights/app.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 22:24:26.318939 pyspeedinsights-0.5.0/src/pyspeedinsights/cli/
+-rw-r--r--   0 will       (501) staff       (20)        0 2022-06-06 20:47:32.000000 pyspeedinsights-0.5.0/src/pyspeedinsights/cli/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)     1010 2023-07-06 22:20:00.000000 pyspeedinsights-0.5.0/src/pyspeedinsights/cli/choices.py
+-rw-r--r--   0 will       (501) staff       (20)     4239 2023-07-06 22:20:00.000000 pyspeedinsights-0.5.0/src/pyspeedinsights/cli/commands.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 22:24:26.319800 pyspeedinsights-0.5.0/src/pyspeedinsights/core/
+-rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 20:34:15.000000 pyspeedinsights-0.5.0/src/pyspeedinsights/core/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)    10192 2023-07-06 22:20:00.000000 pyspeedinsights-0.5.0/src/pyspeedinsights/core/excel.py
+-rw-r--r--   0 will       (501) staff       (20)     5471 2023-07-06 03:17:10.000000 pyspeedinsights-0.5.0/src/pyspeedinsights/core/sitemap.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 22:24:26.320716 pyspeedinsights-0.5.0/src/pyspeedinsights/utils/
+-rw-r--r--   0 will       (501) staff       (20)        0 2022-06-06 20:47:32.000000 pyspeedinsights-0.5.0/src/pyspeedinsights/utils/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)      509 2022-11-04 03:53:30.000000 pyspeedinsights-0.5.0/src/pyspeedinsights/utils/generic.py
+-rw-r--r--   0 will       (501) staff       (20)     1685 2023-07-06 03:17:10.000000 pyspeedinsights-0.5.0/src/pyspeedinsights/utils/urls.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 22:24:26.316902 pyspeedinsights-0.5.0/src/pyspeedinsights.egg-info/
+-rw-r--r--   0 will       (501) staff       (20)    13579 2023-07-06 22:24:26.000000 pyspeedinsights-0.5.0/src/pyspeedinsights.egg-info/PKG-INFO
+-rw-r--r--   0 will       (501) staff       (20)      855 2023-07-06 22:24:26.000000 pyspeedinsights-0.5.0/src/pyspeedinsights.egg-info/SOURCES.txt
+-rw-r--r--   0 will       (501) staff       (20)        1 2023-07-06 22:24:26.000000 pyspeedinsights-0.5.0/src/pyspeedinsights.egg-info/dependency_links.txt
+-rw-r--r--   0 will       (501) staff       (20)       49 2023-07-06 22:24:26.000000 pyspeedinsights-0.5.0/src/pyspeedinsights.egg-info/entry_points.txt
+-rw-r--r--   0 will       (501) staff       (20)      154 2023-07-06 22:24:26.000000 pyspeedinsights-0.5.0/src/pyspeedinsights.egg-info/requires.txt
+-rw-r--r--   0 will       (501) staff       (20)       16 2023-07-06 22:24:26.000000 pyspeedinsights-0.5.0/src/pyspeedinsights.egg-info/top_level.txt
```

### Comparing `pyspeedinsights-0.4.0/LICENSE` & `pyspeedinsights-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.4.0/PKG-INFO` & `pyspeedinsights-0.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspeedinsights
-Version: 0.4.0
+Version: 0.5.0
 Summary: Measure your site speed, performance, accessibility and SEO in bulk from the command line with Python and the PageSpeed Insights API.
 Home-page: https://github.com/wjh18/pyspeedinsights
 Author: Will J. Holmes
 Author-email: will@wjholmes.com
 Project-URL: Documentation, https://github.com/wjh18/pyspeedinsights/blob/master/README.md
 Project-URL: Source, https://github.com/wjh18/pyspeedinsights
 Project-URL: Tracker, https://github.com/wjh18/pyspeedinsights/issues
@@ -37,25 +37,25 @@
 
 ## Why pyspeedinsights?
 
 Manually running each page of your website through Google's Lighthouse or PageSpeed Insights can be extremely time consuming, especially if it has a large number of pages.
 
 This makes it difficult to analyze its overall performance from a 10,000-foot view without manually testing many similar types of pages.
 
-That's what this package attempts to solve. While there are similar tools out there, pyspeedinsights is the only Python implementation built to support analysis in bulk via async requests.
+That's what this package attempts to solve. While there are similar tools out there, pyspeedinsights is the first Python implementation built to support analysis in bulk via async requests.
 
 Its user-friendly cli gives you the ability to analyze your entire site's speed, SEO, and accessibility results quickly and uncover bottlenecks by reviewing color-coded audit results and metrics for each page in Excel.
 
 ## Format Options
 
 The pyspeedinsights cli supports 3 overarching formats:
 
-1. **Single page JSON (`-f json`)**: Output the raw JSON response from the API to your working directory (single pages only).
-2. **Single page Excel (`-f excel`)**: Write color-coded Lighthouse audits and (optionally) metrics to an Excel sheet (single pages only).
-3. **Sitemap / Multi-page Excel (`-f sitemap`)**: Specify a sitemap file to parse and output your full site's color-coded Lighthouse audits and (optionally) metrics to an Excel sheet.
+1. **Single page JSON (`-f json`)**: Output the raw JSON response from the API to your working directory. If you want to analyze a single page in JSON, use this.
+2. **Single page Excel (`-f excel`)**: Write color-coded Lighthouse audits (any category) and/or PageSpeed CrUX metrics (performance category only) to an Excel sheet. If you want to analyze a single page in Excel, use this.
+3. **Sitemap / Multi-page Excel (`-f sitemap`)**: Specify a sitemap file to parse and output your full site's color-coded Lighthouse audits (any category) and/or PageSpeed CrUX metrics (performance category only) to an Excel sheet. If you want to analyze your entire site in Excel, use this.
 
 There are additional customizations available for request parameters and response processing via the cli as well.
 
 Please reference the [commands](#command-line-arguments) section for further instructions on how to specify formats and customize other options from the cli.
 
 ## Installation
 
@@ -73,35 +73,35 @@
 
 From a system Python3 install on Windows:
 
 ```shell
 py -m pip install pyspeedinsights
 ```
 
-To run the package as a module without installing it from PyPI, `cd` into the `src` directory and run:
+To run the package as a module without installing it from PyPI, clone or download it, `cd` into the `src` directory and run:
 
 ```shell
 python -m pyspeedinsights
 ```
 
 *Note that your PATH, OS or Python version may require that you modify these commands slightly. When in doubt, just install it like you would any other Python package.*
 
 ## Authorization
 
-The PageSpeed Insights API requires users to generate an API key for anything more than simple testing. Otherwise, you'll hit a rate limit rather quickly.
+The PageSpeed Insights API requires users to generate an API key for anything beyond running basic test requests. Otherwise, you'll hit a rate limit rather quickly.
 
 For this reason, a valid API key is currently required to use this package. Please see the [PageSpeed Insights API documentation](https://developers.google.com/speed/docs/insights/v5/get-started) for detailed instructions on how to generate a key.
 
 ### Keys & Quotas
 
 The key itself is added to the GET request URL as a query parameter.
 
 It's recommended to generate the key in *Google Cloud Console > Credentials* then restrict it to your host and the PageSpeed Insights API service. If you do go this route, make sure to enable the service in *Enabled APIs & Services*, as it may not be enabled by default.
 
-The API has a daily and per-minute request quota of 25,000 and 240, respectively. The package automatically sleeps requests for 1 second between each call to avoid hitting the per minute quota or overloading the API and getting hit with 500 errors.
+The API has a daily and per-minute request quota of 25,000 and 240, respectively. To comply with this, the package automatically sleeps requests for 1 second between each call to avoid hitting the per minute quota or overloading the API and getting hit with 500 errors.
 
 ### Keyring
 
 This package uses the `keyring` Python library to store API keys securely on your system's default keystore (e.g. MacOS Keychain for MacOS users).
 
 *Note: If you're unable to use keyring for whatever reason, a fallback input will prompt you for your API key from the command line at the start of each run.*
 
@@ -111,15 +111,15 @@
 
 ### Saving Your API Key
 
 To save your API key to your default keystore, run:
 
 ```shell
 keyring set system psikey
-````
+```
 
 The last argument has to be `psikey`. This is because `pyspeedinsights` looks for that username to read in your key during requests. `system` will instruct `keyring` to automatically detect your system's default keystore.
 
 You'll then receive a prompt where you can enter your key to save it.
 
 ### Verifying Your API Key
 
@@ -139,207 +139,172 @@
 keyring del system psikey
 ```
 
 Then verify that it's no longer accessible with `keyring get system psikey`.
 
 ## Sitemap Support
 
-Currently, only URLs to valid XML sitemaps are supported for reports that utilize sitemap format. Please see [sitemaps.org](https://sitemaps.org/protocol.html) for specification details.
+Currently, only URLs to valid XML sitemaps are supported for reports that utilize sitemap format. Please see [sitemaps.org](https://sitemaps.org/protocol.html) for specification details. Gzipped sitemap (e.g. `sitemap.xml.gz`) support is on the near-term roadmap.
 
 Your web server or sitemap plugin must also allow robots to crawl your sitemap. If you see any permission errors that would be the first thing to check. Certain security solutions like CloudFlare also block crawlers so whitelisting the server you're running the package from may also be preferrable.
 
 Your sitemap URL should be passed in as the positional argument for `url` when running `psi` from the command line.
 
 ### Sitemap Index
 
-Support for sitemap index detection was recently added. This requires no additional action on your part. Simply pass your sitemap index in as the `url` argument via the cli.
+Support for sitemap index detection is also supported. This requires no additional action on your part. Simply pass your sitemap index in as the `url` argument via the cli.
 
-If a sitemap index is detected, the package will recursively gather the URLs listed in each sitemap in your sitemap index and include them in requests. If a standard sitemap file is passed, only that sitemap will be processed.
+If a sitemap index is detected, the package will recursively gather the URLs listed in each sitemap in your sitemap index and include them in requests. If a standard sitemap file is passed, only the URLs in that sitemap will be processed.
 
 ## Command Line Arguments
 
 If you've installed `pyspeedinsights` with `pip`, the default command to run cli commands is `psi`.
 
 If you've simply cloned or downloaded the repo, you can run the cli as a module directly with `python -m pyspeedinsights`. Make sure to `cd` into the `src` directory first.
 
-For help with the following commands, run `psi --help`.
+For help with the following commands, run `psi --help` or `psi -h`.
+
+### Notable Defaults
+
+- `category` - `performance`
+- `strategy`- `desktop`
+- `locale` - `en` (US English)
 
 ### Quickstart
 
 To get you started quickly, here are a few example commands.
 
-Example of requesting a desktop performance report with all metrics for all the URLs in your sitemap:
+Example of requesting a desktop performance report for all the URLs in your sitemap:
 
-* `psi https://www.example.com/sitemap.xml -f sitemap -m all -c performance -s desktop -l en`
-  * Equivalent to: `psi https://www.example.com/sitemap.xml -f sitemap -m all` (`performance`, `desktop` and `en` are defaults)
+- `psi https://example.com/sitemap.xml -f sitemap -c performance -s desktop -l en`
+  - Equivalent to: `psi https://example.com/sitemap.xml -f sitemap`
 
-Example of the same report but also specifying a UTM campaign name/source and captcha token (experimental/untested):
+Example of the same report but also specifying a UTM campaign name/source and captcha token:
 
-* `psi https://www.example.com/sitemap.xml -f sitemap -m all -uc my-campaign-name -us my-campaign-source -t my-captcha-token`
+- `psi https://example.com/sitemap.xml -f sitemap -uc my-campaign-name -us my-campaign-source -t my-captcha-token`
 
 ### Request / Sitemap URL: `url` (required)
 
-The URL of the page you want to analyze *or* a path to a valid XML sitemap (index) if using sitemap format.
+The URL of the page you want to analyze *or* a path to a valid XML sitemap/index if sitemap format was selected.
 
 This must be a fully qualified url with an optional path. URLs without a scheme default to `https`. URL fragments (`#`) and query parameters (`?`) will be removed automatically.
 
-Valid commands:
+Some valid commands:
 
-* `psi https://example.com`
-* `psi https://www.example.com`
-* `psi https://example.com/test`
-* `psi example.com`
-  * Modified URL: `https://example.com`
-* `psi https://example.com#test`
-  * Modified URL: `https://example.com`
-
-Invalid commands:
-
-* `psi example`
-  * Throws an error
-* `psi example/path`
-  * Throws an error
+- `psi https://example.com`
+- `psi https://www.example.com`
+- `psi https://example.com/test`
+- `psi example.com`
+  - Modified URL: `https://example.com`
+- `psi https://example.com#test`
+  - Modified URL: `https://example.com`
+
+Some invalid commands:
+
+- `psi example`
+  - Throws an error
+- `psi example/path`
+  - Throws an error
 
 Sitemap example:
 
-* `psi https://www.example.com/sitemap.xml -f sitemap`
-  * Parses `sitemap.xml` and prepares requests for all `<loc>` elements.
+- `psi https://example.com/sitemap.xml -f sitemap`
+  - Parses `sitemap.xml` and prepares requests for all `<loc>` elements.
 
 Please see [sitemaps](#sitemap-support) for more info.
 
 ### Output Format: `-f` or `--format` (optional)
 
 The format of the Lighthouse results output.
 
-* `json` (default): Output the raw JSON response from the API to your working directory (single pages only). You can add a `-f json` argument explicitly or leave it out to simply default to JSON output.
+- `json` (default): Output the raw JSON response from the API to your working directory (single pages only). You can add a `-f json` argument explicitly or leave it out to simply default to JSON output.
 
-* `excel`: Write color-coded Lighthouse audits and (optionally) metrics to an Excel sheet (analyze the single `url` only).
+- `excel`: Write color-coded Lighthouse audits (any category) and/or PageSpeed CrUX metrics (performance category only) to an Excel sheet (analyze the single `url` only).
 
-* `sitemap`: Specify a sitemap (or index) file to parse and output your full site's color-coded Lighthouse audits and (optionally) metrics to an Excel sheet. When using this option, the `url` argument above needs to be a direct link to your XML sitemap. Please see [sitemaps](#sitemap-support) for more info.
+- `sitemap`: Specify a sitemap (or index) file to parse and output your full site's color-coded Lighthouse audits (any category) and/or PageSpeed CrUX metrics (performance category only) to an Excel sheet. When using this option, the `url` argument above needs to be a direct link to your XML sitemap/index. Please see [sitemaps](#sitemap-support) for more info.
 
 Example:
 
-* `psi https://example.com` - defaults to `json`
-* `psi https://example.com -f excel`
-* `psi https://example.com -f sitemap`
+- `psi https://example.com` - defaults to `json`
+- `psi https://example.com -f json`
+- `psi https://example.com -f excel`
+- `psi https://example.com -f sitemap`
 
 ### Metrics: `-m` or `--metrics` (optional)
 
-Specify which metric(s) you want to include in your report.
-
-This is only supported for the performance category (`-c performance`) with either `excel` or `sitemap` formats because the JSON output includes everything by default and categories other than performance don't include metrics in the response.
-
-If excluded, metrics will *not* be dumped to Excel. Add the `all` argument to retrieve all available metrics or specify individual metrics to include.
-
-Example:
+Deprecated in favor of automatically including CrUX metrics if they are available and `performance` category is selected. The previous metrics were debug metrics and subject to change by Google at any time, which made package maintenance difficult.
 
-* `psi https://example.com -f excel` - no metrics
-* `psi https://example.com -f excel -m all` - all available metrics
-* `psi https://example.com -f excel -m speedIndex` - just speedIndex
-* `psi https://example.com -f excel -m speedIndex totalBlockingTime` - just speedIndex and totalBlockingTime
-
-Full list of available metrics:
-
-* `observedCumulativeLayoutShift`
-* `observedLargestContentfulPaintAllFrames`
-* `maxPotentialFID`
-* `observedSpeedIndexTs`
-* `observedFirstContentfulPaintTs`
-* `observedTimeOrigin`
-* `observedFirstPaint`
-* `observedNavigationStartTs`
-* `observedLargestContentfulPaintAllFramesTs`
-* `speedIndex`
-* `observedFirstContentfulPaint`
-* `observedLastVisualChangeTs`
-* `cumulativeLayoutShiftMainFrame`
-* `observedLastVisualChange`
-* `cumulativeLayoutShift`
-* `largestContentfulPaint`
-* `observedDomContentLoaded`
-* `firstContentfulPaint`
-* `observedCumulativeLayoutShiftMainFrame`
-* `observedFirstVisualChange`
-* `observedFirstPaintTs`
-* `totalCumulativeLayoutShift`
-* `observedFirstMeaningfulPaint`
-* `interactive`
-* `observedTraceEnd`
-* `observedFirstMeaningfulPaintTs`
-* `totalBlockingTime`
-* `observedFirstContentfulPaintAllFramesTs`
-* `observedLargestContentfulPaint`
-* `observedNavigationStart`
-* `observedLoad`
-* `observedFirstVisualChangeTs`
-* `observedFirstContentfulPaintAllFrames`
-* `observedTimeOriginTs`
-* `observedTraceEndTs`
-* `observedLoadTs`
-* `observedDomContentLoadedTs`
-* `observedSpeedIndex`
-* `firstMeaningfulPaint`
-* `observedLargestContentfulPaintTs`
+The new metrics include user-friendly scores instead of raw performance metrics to help give you a quick overview of core metrics like CLS, LCP, etc.
 
 ### Category: `-c` or `--category` (optional)
 
 The Lighthouse category to run. Defaults to `performance`.
 
 Other options include `accessibility`, `best-practices`, `pwa` and `seo`.
 
+Metrics will only be included with the `performance` category.
+
 Example:
 
-* `psi https://www.example.com -c accessibility`
+- `psi https://example.com -c accessibility`
 
 ### Strategy: `-s` or `--strategy` (optional)
 
 The Lighthouse analysis strategy to use. Defaults to `desktop`.
 
 Other options include `mobile`.
 
 Example:
 
-* `psi https://www.example.com -s mobile`
+- `psi https://example.com -s mobile`
 
 ### Locale: `-l` or `--locale` (optional)
 
-The locale used to localize formatted results. Defaults to `en` (US).
+The locale used to localize formatted results (language). Defaults to `en` (US).
 
 Please see the PSI API docs for a [full list of locale options](https://developers.google.com/speed/docs/insights/languages).
 
 Example:
 
-* `psi https://www.example.com -l fr` - localize results to French
+- `psi https://example.com -l fr` - localize results to French
 
-### UTM Campaign: `-uc` or `--campaign` (optional) (experimental)
+### UTM Campaign: `-uc` or `--campaign` (optional)
 
 The UTM campaign name for analytics. Defaults to `None`.
 
-This option is currently experimental and hasn't been fully tested.
+This will add a query parameter to the request made by the PageSpeed Insights API (`?utm_campaign=audit`) so you can differentiate this traffic from real user traffic in Google Analytics.
+
+Pass in the name of your campaign, `audit` is just an example.
 
 Example:
 
-* `psi https://www.example.com -uc my-campaign-name`
+- `psi https://example.com -uc audit`
 
-### UTM Source: `-us` or `--source` (optional) (experimental)
+### UTM Source: `-us` or `--source` (optional)
 
 The UTM campaign source for analytics. Defaults to `None`.
 
-This option is currently experimental and hasn't been fully tested.
+This will add a query parameter to the request made by the PageSpeed Insights API (`?utm_source=psi`) so you can differentiate this traffic from real user traffic in Google Analytics.
+
+Feel free to customize the name of the source, `psi` is just an example.
 
 Example:
 
-* `psi https://www.example.com -us my-campaign-source`
+- `psi https://example.com -us psi`
 
-### Captcha Token: `-t` or `--token` (optional) (experimental)
+### Captcha Token: `-t` or `--token` (optional)
 
 The captcha token passed when filling out a captcha. Defaults to `None`.
 
-This option is currently experimental and hasn't been fully tested.
+This will add a query parameter to the request made by the PageSpeed Insights API (`?utm_source=psi`) containing your captcha token. If you have captcha protection enabled on your site, passing this token as an argument to bypass it will ensure that PSI can analyze your site.
 
 Example:
 
-* `psi https://www.example.com -t my-captcha-token`
+- `psi https://example.com -t my-captcha-token`
+
+## Help
+
+Please open an issue on GitHub if you run into any issues or need assistance.
 
 ## Contributing
 
 Contributors of all skill levels are welcome to help improve this package. Please see the [Contribution Guidelines](CONTRIBUTING.md) for details.
```

### Comparing `pyspeedinsights-0.4.0/README.md` & `pyspeedinsights-0.5.0/src/pyspeedinsights.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: pyspeedinsights
+Version: 0.5.0
+Summary: Measure your site speed, performance, accessibility and SEO in bulk from the command line with Python and the PageSpeed Insights API.
+Home-page: https://github.com/wjh18/pyspeedinsights
+Author: Will J. Holmes
+Author-email: will@wjholmes.com
+Project-URL: Documentation, https://github.com/wjh18/pyspeedinsights/blob/master/README.md
+Project-URL: Source, https://github.com/wjh18/pyspeedinsights
+Project-URL: Tracker, https://github.com/wjh18/pyspeedinsights/issues
+Keywords: google,google-apis,psi-api,page-speed-insights,page-speed-insights-api,pagespeedinsightsapi,python,cli
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
+Classifier: Topic :: Utilities
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # pyspeedinsights
 
 Measure your site speed, performance, accessibility and SEO in bulk from the command line with Python and the PageSpeed Insights API.
 
 Support for sitemap parsing and asynchronous requests with aiohttp. Outputs to JSON or a color-coded Excel sheet for further analysis.
 
 ![A screenshot of the tool's Excel output](https://raw.githubusercontent.com/wjh18/pyspeedinsights/master/images/screenshot.png)
@@ -12,25 +37,25 @@
 
 ## Why pyspeedinsights?
 
 Manually running each page of your website through Google's Lighthouse or PageSpeed Insights can be extremely time consuming, especially if it has a large number of pages.
 
 This makes it difficult to analyze its overall performance from a 10,000-foot view without manually testing many similar types of pages.
 
-That's what this package attempts to solve. While there are similar tools out there, pyspeedinsights is the only Python implementation built to support analysis in bulk via async requests.
+That's what this package attempts to solve. While there are similar tools out there, pyspeedinsights is the first Python implementation built to support analysis in bulk via async requests.
 
 Its user-friendly cli gives you the ability to analyze your entire site's speed, SEO, and accessibility results quickly and uncover bottlenecks by reviewing color-coded audit results and metrics for each page in Excel.
 
 ## Format Options
 
 The pyspeedinsights cli supports 3 overarching formats:
 
-1. **Single page JSON (`-f json`)**: Output the raw JSON response from the API to your working directory (single pages only).
-2. **Single page Excel (`-f excel`)**: Write color-coded Lighthouse audits and (optionally) metrics to an Excel sheet (single pages only).
-3. **Sitemap / Multi-page Excel (`-f sitemap`)**: Specify a sitemap file to parse and output your full site's color-coded Lighthouse audits and (optionally) metrics to an Excel sheet.
+1. **Single page JSON (`-f json`)**: Output the raw JSON response from the API to your working directory. If you want to analyze a single page in JSON, use this.
+2. **Single page Excel (`-f excel`)**: Write color-coded Lighthouse audits (any category) and/or PageSpeed CrUX metrics (performance category only) to an Excel sheet. If you want to analyze a single page in Excel, use this.
+3. **Sitemap / Multi-page Excel (`-f sitemap`)**: Specify a sitemap file to parse and output your full site's color-coded Lighthouse audits (any category) and/or PageSpeed CrUX metrics (performance category only) to an Excel sheet. If you want to analyze your entire site in Excel, use this.
 
 There are additional customizations available for request parameters and response processing via the cli as well.
 
 Please reference the [commands](#command-line-arguments) section for further instructions on how to specify formats and customize other options from the cli.
 
 ## Installation
 
@@ -48,35 +73,35 @@
 
 From a system Python3 install on Windows:
 
 ```shell
 py -m pip install pyspeedinsights
 ```
 
-To run the package as a module without installing it from PyPI, `cd` into the `src` directory and run:
+To run the package as a module without installing it from PyPI, clone or download it, `cd` into the `src` directory and run:
 
 ```shell
 python -m pyspeedinsights
 ```
 
 *Note that your PATH, OS or Python version may require that you modify these commands slightly. When in doubt, just install it like you would any other Python package.*
 
 ## Authorization
 
-The PageSpeed Insights API requires users to generate an API key for anything more than simple testing. Otherwise, you'll hit a rate limit rather quickly.
+The PageSpeed Insights API requires users to generate an API key for anything beyond running basic test requests. Otherwise, you'll hit a rate limit rather quickly.
 
 For this reason, a valid API key is currently required to use this package. Please see the [PageSpeed Insights API documentation](https://developers.google.com/speed/docs/insights/v5/get-started) for detailed instructions on how to generate a key.
 
 ### Keys & Quotas
 
 The key itself is added to the GET request URL as a query parameter.
 
 It's recommended to generate the key in *Google Cloud Console > Credentials* then restrict it to your host and the PageSpeed Insights API service. If you do go this route, make sure to enable the service in *Enabled APIs & Services*, as it may not be enabled by default.
 
-The API has a daily and per-minute request quota of 25,000 and 240, respectively. The package automatically sleeps requests for 1 second between each call to avoid hitting the per minute quota or overloading the API and getting hit with 500 errors.
+The API has a daily and per-minute request quota of 25,000 and 240, respectively. To comply with this, the package automatically sleeps requests for 1 second between each call to avoid hitting the per minute quota or overloading the API and getting hit with 500 errors.
 
 ### Keyring
 
 This package uses the `keyring` Python library to store API keys securely on your system's default keystore (e.g. MacOS Keychain for MacOS users).
 
 *Note: If you're unable to use keyring for whatever reason, a fallback input will prompt you for your API key from the command line at the start of each run.*
 
@@ -86,15 +111,15 @@
 
 ### Saving Your API Key
 
 To save your API key to your default keystore, run:
 
 ```shell
 keyring set system psikey
-````
+```
 
 The last argument has to be `psikey`. This is because `pyspeedinsights` looks for that username to read in your key during requests. `system` will instruct `keyring` to automatically detect your system's default keystore.
 
 You'll then receive a prompt where you can enter your key to save it.
 
 ### Verifying Your API Key
 
@@ -114,207 +139,172 @@
 keyring del system psikey
 ```
 
 Then verify that it's no longer accessible with `keyring get system psikey`.
 
 ## Sitemap Support
 
-Currently, only URLs to valid XML sitemaps are supported for reports that utilize sitemap format. Please see [sitemaps.org](https://sitemaps.org/protocol.html) for specification details.
+Currently, only URLs to valid XML sitemaps are supported for reports that utilize sitemap format. Please see [sitemaps.org](https://sitemaps.org/protocol.html) for specification details. Gzipped sitemap (e.g. `sitemap.xml.gz`) support is on the near-term roadmap.
 
 Your web server or sitemap plugin must also allow robots to crawl your sitemap. If you see any permission errors that would be the first thing to check. Certain security solutions like CloudFlare also block crawlers so whitelisting the server you're running the package from may also be preferrable.
 
 Your sitemap URL should be passed in as the positional argument for `url` when running `psi` from the command line.
 
 ### Sitemap Index
 
-Support for sitemap index detection was recently added. This requires no additional action on your part. Simply pass your sitemap index in as the `url` argument via the cli.
+Support for sitemap index detection is also supported. This requires no additional action on your part. Simply pass your sitemap index in as the `url` argument via the cli.
 
-If a sitemap index is detected, the package will recursively gather the URLs listed in each sitemap in your sitemap index and include them in requests. If a standard sitemap file is passed, only that sitemap will be processed.
+If a sitemap index is detected, the package will recursively gather the URLs listed in each sitemap in your sitemap index and include them in requests. If a standard sitemap file is passed, only the URLs in that sitemap will be processed.
 
 ## Command Line Arguments
 
 If you've installed `pyspeedinsights` with `pip`, the default command to run cli commands is `psi`.
 
 If you've simply cloned or downloaded the repo, you can run the cli as a module directly with `python -m pyspeedinsights`. Make sure to `cd` into the `src` directory first.
 
-For help with the following commands, run `psi --help`.
+For help with the following commands, run `psi --help` or `psi -h`.
+
+### Notable Defaults
+
+- `category` - `performance`
+- `strategy`- `desktop`
+- `locale` - `en` (US English)
 
 ### Quickstart
 
 To get you started quickly, here are a few example commands.
 
-Example of requesting a desktop performance report with all metrics for all the URLs in your sitemap:
+Example of requesting a desktop performance report for all the URLs in your sitemap:
 
-* `psi https://www.example.com/sitemap.xml -f sitemap -m all -c performance -s desktop -l en`
-  * Equivalent to: `psi https://www.example.com/sitemap.xml -f sitemap -m all` (`performance`, `desktop` and `en` are defaults)
+- `psi https://example.com/sitemap.xml -f sitemap -c performance -s desktop -l en`
+  - Equivalent to: `psi https://example.com/sitemap.xml -f sitemap`
 
-Example of the same report but also specifying a UTM campaign name/source and captcha token (experimental/untested):
+Example of the same report but also specifying a UTM campaign name/source and captcha token:
 
-* `psi https://www.example.com/sitemap.xml -f sitemap -m all -uc my-campaign-name -us my-campaign-source -t my-captcha-token`
+- `psi https://example.com/sitemap.xml -f sitemap -uc my-campaign-name -us my-campaign-source -t my-captcha-token`
 
 ### Request / Sitemap URL: `url` (required)
 
-The URL of the page you want to analyze *or* a path to a valid XML sitemap (index) if using sitemap format.
+The URL of the page you want to analyze *or* a path to a valid XML sitemap/index if sitemap format was selected.
 
 This must be a fully qualified url with an optional path. URLs without a scheme default to `https`. URL fragments (`#`) and query parameters (`?`) will be removed automatically.
 
-Valid commands:
+Some valid commands:
 
-* `psi https://example.com`
-* `psi https://www.example.com`
-* `psi https://example.com/test`
-* `psi example.com`
-  * Modified URL: `https://example.com`
-* `psi https://example.com#test`
-  * Modified URL: `https://example.com`
-
-Invalid commands:
-
-* `psi example`
-  * Throws an error
-* `psi example/path`
-  * Throws an error
+- `psi https://example.com`
+- `psi https://www.example.com`
+- `psi https://example.com/test`
+- `psi example.com`
+  - Modified URL: `https://example.com`
+- `psi https://example.com#test`
+  - Modified URL: `https://example.com`
+
+Some invalid commands:
+
+- `psi example`
+  - Throws an error
+- `psi example/path`
+  - Throws an error
 
 Sitemap example:
 
-* `psi https://www.example.com/sitemap.xml -f sitemap`
-  * Parses `sitemap.xml` and prepares requests for all `<loc>` elements.
+- `psi https://example.com/sitemap.xml -f sitemap`
+  - Parses `sitemap.xml` and prepares requests for all `<loc>` elements.
 
 Please see [sitemaps](#sitemap-support) for more info.
 
 ### Output Format: `-f` or `--format` (optional)
 
 The format of the Lighthouse results output.
 
-* `json` (default): Output the raw JSON response from the API to your working directory (single pages only). You can add a `-f json` argument explicitly or leave it out to simply default to JSON output.
+- `json` (default): Output the raw JSON response from the API to your working directory (single pages only). You can add a `-f json` argument explicitly or leave it out to simply default to JSON output.
 
-* `excel`: Write color-coded Lighthouse audits and (optionally) metrics to an Excel sheet (analyze the single `url` only).
+- `excel`: Write color-coded Lighthouse audits (any category) and/or PageSpeed CrUX metrics (performance category only) to an Excel sheet (analyze the single `url` only).
 
-* `sitemap`: Specify a sitemap (or index) file to parse and output your full site's color-coded Lighthouse audits and (optionally) metrics to an Excel sheet. When using this option, the `url` argument above needs to be a direct link to your XML sitemap. Please see [sitemaps](#sitemap-support) for more info.
+- `sitemap`: Specify a sitemap (or index) file to parse and output your full site's color-coded Lighthouse audits (any category) and/or PageSpeed CrUX metrics (performance category only) to an Excel sheet. When using this option, the `url` argument above needs to be a direct link to your XML sitemap/index. Please see [sitemaps](#sitemap-support) for more info.
 
 Example:
 
-* `psi https://example.com` - defaults to `json`
-* `psi https://example.com -f excel`
-* `psi https://example.com -f sitemap`
+- `psi https://example.com` - defaults to `json`
+- `psi https://example.com -f json`
+- `psi https://example.com -f excel`
+- `psi https://example.com -f sitemap`
 
 ### Metrics: `-m` or `--metrics` (optional)
 
-Specify which metric(s) you want to include in your report.
+Deprecated in favor of automatically including CrUX metrics if they are available and `performance` category is selected. The previous metrics were debug metrics and subject to change by Google at any time, which made package maintenance difficult.
 
-This is only supported for the performance category (`-c performance`) with either `excel` or `sitemap` formats because the JSON output includes everything by default and categories other than performance don't include metrics in the response.
-
-If excluded, metrics will *not* be dumped to Excel. Add the `all` argument to retrieve all available metrics or specify individual metrics to include.
-
-Example:
-
-* `psi https://example.com -f excel` - no metrics
-* `psi https://example.com -f excel -m all` - all available metrics
-* `psi https://example.com -f excel -m speedIndex` - just speedIndex
-* `psi https://example.com -f excel -m speedIndex totalBlockingTime` - just speedIndex and totalBlockingTime
-
-Full list of available metrics:
-
-* `observedCumulativeLayoutShift`
-* `observedLargestContentfulPaintAllFrames`
-* `maxPotentialFID`
-* `observedSpeedIndexTs`
-* `observedFirstContentfulPaintTs`
-* `observedTimeOrigin`
-* `observedFirstPaint`
-* `observedNavigationStartTs`
-* `observedLargestContentfulPaintAllFramesTs`
-* `speedIndex`
-* `observedFirstContentfulPaint`
-* `observedLastVisualChangeTs`
-* `cumulativeLayoutShiftMainFrame`
-* `observedLastVisualChange`
-* `cumulativeLayoutShift`
-* `largestContentfulPaint`
-* `observedDomContentLoaded`
-* `firstContentfulPaint`
-* `observedCumulativeLayoutShiftMainFrame`
-* `observedFirstVisualChange`
-* `observedFirstPaintTs`
-* `totalCumulativeLayoutShift`
-* `observedFirstMeaningfulPaint`
-* `interactive`
-* `observedTraceEnd`
-* `observedFirstMeaningfulPaintTs`
-* `totalBlockingTime`
-* `observedFirstContentfulPaintAllFramesTs`
-* `observedLargestContentfulPaint`
-* `observedNavigationStart`
-* `observedLoad`
-* `observedFirstVisualChangeTs`
-* `observedFirstContentfulPaintAllFrames`
-* `observedTimeOriginTs`
-* `observedTraceEndTs`
-* `observedLoadTs`
-* `observedDomContentLoadedTs`
-* `observedSpeedIndex`
-* `firstMeaningfulPaint`
-* `observedLargestContentfulPaintTs`
+The new metrics include user-friendly scores instead of raw performance metrics to help give you a quick overview of core metrics like CLS, LCP, etc.
 
 ### Category: `-c` or `--category` (optional)
 
 The Lighthouse category to run. Defaults to `performance`.
 
 Other options include `accessibility`, `best-practices`, `pwa` and `seo`.
 
+Metrics will only be included with the `performance` category.
+
 Example:
 
-* `psi https://www.example.com -c accessibility`
+- `psi https://example.com -c accessibility`
 
 ### Strategy: `-s` or `--strategy` (optional)
 
 The Lighthouse analysis strategy to use. Defaults to `desktop`.
 
 Other options include `mobile`.
 
 Example:
 
-* `psi https://www.example.com -s mobile`
+- `psi https://example.com -s mobile`
 
 ### Locale: `-l` or `--locale` (optional)
 
-The locale used to localize formatted results. Defaults to `en` (US).
+The locale used to localize formatted results (language). Defaults to `en` (US).
 
 Please see the PSI API docs for a [full list of locale options](https://developers.google.com/speed/docs/insights/languages).
 
 Example:
 
-* `psi https://www.example.com -l fr` - localize results to French
+- `psi https://example.com -l fr` - localize results to French
 
-### UTM Campaign: `-uc` or `--campaign` (optional) (experimental)
+### UTM Campaign: `-uc` or `--campaign` (optional)
 
 The UTM campaign name for analytics. Defaults to `None`.
 
-This option is currently experimental and hasn't been fully tested.
+This will add a query parameter to the request made by the PageSpeed Insights API (`?utm_campaign=audit`) so you can differentiate this traffic from real user traffic in Google Analytics.
+
+Pass in the name of your campaign, `audit` is just an example.
 
 Example:
 
-* `psi https://www.example.com -uc my-campaign-name`
+- `psi https://example.com -uc audit`
 
-### UTM Source: `-us` or `--source` (optional) (experimental)
+### UTM Source: `-us` or `--source` (optional)
 
 The UTM campaign source for analytics. Defaults to `None`.
 
-This option is currently experimental and hasn't been fully tested.
+This will add a query parameter to the request made by the PageSpeed Insights API (`?utm_source=psi`) so you can differentiate this traffic from real user traffic in Google Analytics.
+
+Feel free to customize the name of the source, `psi` is just an example.
 
 Example:
 
-* `psi https://www.example.com -us my-campaign-source`
+- `psi https://example.com -us psi`
 
-### Captcha Token: `-t` or `--token` (optional) (experimental)
+### Captcha Token: `-t` or `--token` (optional)
 
 The captcha token passed when filling out a captcha. Defaults to `None`.
 
-This option is currently experimental and hasn't been fully tested.
+This will add a query parameter to the request made by the PageSpeed Insights API (`?utm_source=psi`) containing your captcha token. If you have captcha protection enabled on your site, passing this token as an argument to bypass it will ensure that PSI can analyze your site.
 
 Example:
 
-* `psi https://www.example.com -t my-captcha-token`
+- `psi https://example.com -t my-captcha-token`
+
+## Help
+
+Please open an issue on GitHub if you run into any issues or need assistance.
 
 ## Contributing
 
 Contributors of all skill levels are welcome to help improve this package. Please see the [Contribution Guidelines](CONTRIBUTING.md) for details.
```

### Comparing `pyspeedinsights-0.4.0/pyproject.toml` & `pyspeedinsights-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.4.0/setup.cfg` & `pyspeedinsights-0.5.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyspeedinsights
-version = 0.4.0
+version = 0.5.0
 author = Will J. Holmes
 author_email = will@wjholmes.com
 description = Measure your site speed, performance, accessibility and SEO in bulk from the command line with Python and the PageSpeed Insights API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = google, google-apis, psi-api, page-speed-insights, page-speed-insights-api, pagespeedinsightsapi, python, cli
 url = https://github.com/wjh18/pyspeedinsights
```

### Comparing `pyspeedinsights-0.4.0/src/pyspeedinsights/api/keys.py` & `pyspeedinsights-0.5.0/src/pyspeedinsights/api/keys.py`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.4.0/src/pyspeedinsights/api/request.py` & `pyspeedinsights-0.5.0/src/pyspeedinsights/api/request.py`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.4.0/src/pyspeedinsights/api/response.py` & `pyspeedinsights-0.5.0/src/pyspeedinsights/api/response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 """Response processing and parsing for PSI API results."""
 
-import copy
 import json
 import logging
 from datetime import datetime
-from typing import Optional, Union
+from typing import Union
 
-from ..cli.choices import COMMAND_CHOICES
-from ..utils.exceptions import JSONKeyError
 from ..utils.generic import sort_dict_alpha
 
 logger = logging.getLogger(__name__)
 
+METRICS_ABBR = {
+    "CUMULATIVE_LAYOUT_SHIFT_SCORE": "CLS",
+    "EXPERIMENTAL_INTERACTION_TO_NEXT_PAINT": "INP(E)",
+    "EXPERIMENTAL_TIME_TO_FIRST_BYTE": "TTFB(E)",
+    "FIRST_CONTENTFUL_PAINT_MS": "FCP",
+    "FIRST_INPUT_DELAY_MS": "FID",
+    "INTERACTION_TO_NEXT_PAINT": "INP",
+    "LARGEST_CONTENTFUL_PAINT_MS": "LCP",
+}
+
 
 def process_json(json_resp: dict, category: str, strategy: str) -> None:
     """Dumps raw json response to a file in the working directory.
 
     Called within main() in pyspeedinsights.app.
     If json format is selected this is where program execution ends.
     """
@@ -23,39 +30,40 @@
     filename = f"psi-s-{strategy}-c-{category}-{date}.json"
 
     with open(filename, "w", encoding="utf-8") as f:
         json.dump(json_resp, f, ensure_ascii=False, indent=4)
         logger.info("JSON processed. Check your current working directory.")
 
 
-def process_excel(
-    json_resp: dict, category: str, metrics: Optional[list[str]]
-) -> dict[str, Union[dict, None]]:
+def process_excel(json_resp: dict, category: str) -> dict[str, Union[dict, None]]:
     """Calls various parsing operations for Excel / Sitemap formats.
 
     Called within main() in pyspeedinsights.app.
     Metrics results are only included if the category is performance.
     """
     json_err = "Malformed JSON response. Skipping Excel processing for URL: "
     try:
         audits_base = _get_audits_base(json_resp)  # Location of audits in json response
         metadata = _parse_metadata(json_resp, category)
         audit_results = _parse_audits(audits_base)
-    except JSONKeyError as err:
+    except KeyError as err:
         logger.error(f"{json_err}{err}", exc_info=True)
         return {}
 
-    if metrics is not None and category == "performance":
+    if category == "performance":
         try:
-            metrics_results = _parse_metrics(audits_base, metrics)
-        except JSONKeyError as err:
-            logger.error(f"{json_err}{err}", exc_info=True)
-            return {}
+            metrics_base = _get_metrics_base(
+                json_resp
+            )  # Loc of metrics in json response
+            metrics_results = _parse_metrics(metrics_base)
+        except KeyError as err:
+            logger.error(f"Metrics not available for this report: {err}", exc_info=True)
+            metrics_results = None
     else:
-        logger.warning("Skipping metrics (not chosen or non-performance category)")
+        logger.warning("Skipping metrics (non-performance category)")
         metrics_results = None
 
     results: dict[str, Union[dict, None]] = {
         "metadata": metadata,
         "audit_results": audit_results,
         "metrics_results": metrics_results,
     }
@@ -101,62 +109,62 @@
             audit_results[k] = (score * 100, num_value)
         else:
             audit_results[k] = ("n/a", "n/a")
     # Sort dict alphabetically so each audit is written to Excel in the same order.
     return sort_dict_alpha(audit_results)
 
 
-def _parse_metrics(
-    audits_base: dict, metrics: list[str]
-) -> dict[str, Union[int, float]]:
-    """Parses performance metrics from the JSON response to write to Excel.
+def _parse_metrics(metrics_base: dict) -> dict[str, Union[int, float]]:
+    """Parses performance metric scores from the JSON response to write to Excel.
 
-    Metrics have no scores associated with them.
+    Real-user experience data from CrUX dataset.
 
     Returns:
         A dict of metrics results with metric names as keys
-        and int or float metrics as values.
+        and their scores as values.
     """
-    if "all" in metrics:
-        logger.info("Parsing all metrics.")
-        metrics_to_use = copy.copy(COMMAND_CHOICES["metrics"])
-        # Remove 'all' to avoid key errors, as it doesn't exist in JSON resp.
-        if type(metrics_to_use) == list:
-            metrics_to_use.remove("all")
-    else:
-        logger.info("Parsing chosen metrics.")
-        metrics_to_use = metrics
-
-    # Create new dict of metrics based on user's chosen metrics.
+    logger.info("Parsing metrics data from JSON response.")
     metrics_results = {}
-    metrics_loc = audits_base["metrics"]["details"]["items"][0]
-    metrics_results = {field: metrics_loc[field] for field in metrics_to_use}
-    # Sort dict alphabetically so each metric is written to Excel in the same order.
-    return sort_dict_alpha(metrics_results)
+    for metric, result in metrics_base.items():
+        try:
+            abbr = METRICS_ABBR[metric]
+        except KeyError:
+            abbr = metric
+        score = result["distributions"][0]["proportion"]
+        score = round(score, 3) * 100
+        metrics_results[abbr] = score
+    # Ensure each metric is written to Excel under the same column.
+    desired_order_list = ("CLS", "FCP", "LCP", "FID", "INP", "INP(E)", "TTFB(E)")
+    return {k: metrics_results[k] for k in desired_order_list}
 
 
 def _get_audits_base(json_resp: dict) -> dict:
     """Gets the location of audits in the JSON response."""
     return json_resp["lighthouseResult"]["audits"]
 
 
+def _get_metrics_base(json_resp: dict) -> dict:
+    """Gets the location of metrics in the JSON response."""
+    return json_resp["loadingExperience"]["metrics"]
+
+
 def _get_timestamp(json_resp: dict) -> str:
     """Parses the timestamp of the analysis from the JSON response.
 
     Converts the timestamp to a Python datetime object.
 
     Returns:
         A str in format year-month-day_hour.minute.second.
     """
     logger.info("Parsing timestamp from JSON response.")
     time_format = "%Y-%m-%d_%H.%M.%S"
 
     try:
         timestamp = json_resp["analysisUTCTimestamp"]
-    except JSONKeyError:
+    except KeyError:
         logger.warning("Unable to parse timestamp. Falling back to local time.")
         date = datetime.now().strftime(time_format)
         return date
 
     ts_no_fractions = timestamp.split(".")[0]  # Remove fraction
     if ts_no_fractions[-1] != "Z":
         ts_no_fractions += "Z"  # Add Z back after fraction removal
```

### Comparing `pyspeedinsights-0.4.0/src/pyspeedinsights/app.py` & `pyspeedinsights-0.5.0/src/pyspeedinsights/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from .core.excel import ExcelWorkbook
 from .core.sitemap import (
     SitemapError,
     process_sitemap,
     request_sitemap,
     validate_sitemap_url,
 )
-from .utils.exceptions import JSONKeyError
 from .utils.generic import remove_dupes_from_list
 from .utils.urls import InvalidURLError
 
 
 def main() -> None:
     """Point of execution with `psi` from cli or via direct module invocation.
 
@@ -41,33 +40,26 @@
     arg_groups = create_arg_groups(parser, args)
     api_args_dict = arg_group_to_dict(arg_groups, "API Group")
     proc_args_dict = arg_group_to_dict(arg_groups, "Processing Group")
 
     logger.info("Parsing CLI arguments.")
 
     format = proc_args_dict.get("format")
-    metrics = proc_args_dict.get("metrics")
 
     url = api_args_dict.get("url")
     category = api_args_dict.get("category")
     strategy = api_args_dict.get("strategy")
 
     # API's default category and strategy with no query params.
     category = "performance" if category is None else category
     strategy = "desktop" if strategy is None else strategy
 
     json_output = format == "json" or format is None
     excel_output = format in ("excel", "sitemap")
 
-    if metrics is not None and json_output or category != "performance":
-        logger.warning(
-            "Metrics are only configurable for excel performance reports. "
-            "JSON performance reports will include all metrics by default."
-        )
-
     if format == "sitemap" and url is not None:
         try:
             sitemap = request_sitemap(url)
             request_urls = remove_dupes_from_list(process_sitemap(sitemap))
         # Let these exceptions bubble up from `core/sitemap.py`
         except (SitemapError, InvalidURLError) as err:
             logger.critical(err, exc_info=True)
@@ -98,19 +90,19 @@
 
     resp_num = 1  # use instead of enumerate for more control over skipping failures
     for response in responses:
         if json_output:
             logger.info("JSON format selected. Processing JSON.")
             process_json(response, category, strategy)
         elif excel_output:
-            excel_results = process_excel(response, category, metrics)
+            excel_results = process_excel(response, category)
 
             try:
                 final_url = response["lighthouseResult"]["finalUrl"]
-            except JSONKeyError as err:
+            except KeyError as err:
                 # For now, log this as critical and exit.
                 # A better solution would be to preserve the original request URL
                 # as a fallback. Temporarily, this is more helpful than just KeyError.
                 logger.critical(
                     f"The response data contains no URL: {err}", exc_info=True
                 )
                 sys.exit(1)
```

### Comparing `pyspeedinsights-0.4.0/src/pyspeedinsights/cli/commands.py` & `pyspeedinsights-0.5.0/src/pyspeedinsights/cli/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,32 +90,18 @@
         "--format",
         metavar="\b",
         dest="format",
         choices=COMMAND_CHOICES["format"],
         help=(
             "The format of the results: `json` (default), `excel` or `sitemap`. "
             "`json` outputs all response data to a json file (1 URL only). "
-            "`excel` writes Lighthouse audits and (optionally) metrics "
+            "`excel` writes Lighthouse audits and PageSpeed Insights metrics "
             "to an Excel file (1 URL only). "
             "`sitemap` parses the sitemap URL you provide and writes Lighthouse audits "
-            "and (optionally) metrics for all the pages in your sitemap to Excel."
-        ),
-    )
-    proc_group.add_argument(
-        "-m",
-        "--metrics",
-        metavar="\b",
-        dest="metrics",
-        choices=COMMAND_CHOICES["metrics"],
-        nargs="+",
-        help=(
-            "The additional metric(s) to include in your report. "
-            "For `excel` or `sitemap` formats only (`json` includes all metrics). "
-            "If excluded, only the default Lighthouse audits will be written to Excel. "
-            "Add the `all` argument to retrieve all available metrics."
+            "and PageSpeed Insights metrics for all the pages in your sitemap to Excel."
         ),
     )
     return parser
 
 
 def create_arg_groups(parser: ArgumentParser, args: Namespace) -> ArgGroups:
     """Creates separate namespaces for each arg group.
```

### Comparing `pyspeedinsights-0.4.0/src/pyspeedinsights/core/excel.py` & `pyspeedinsights-0.5.0/src/pyspeedinsights/core/excel.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     metadata: dict[str, Any]
     audit_results: AuditResults
     metrics_results: MetricsResults = None
     workbook: Workbook = None
     worksheet: Workbook.worksheet_class = None
     cur_cell: list[int] = field(default_factory=list)
     category_scores: list[int] = field(default_factory=list)
+    metrics_scores: list[int | float] = field(default_factory=list)
 
     def set_up_worksheet(self) -> None:
         """Creates the workbook, adds a worksheet, and sets up column headings."""
         self._create_workbook()
         self.worksheet = self.workbook.add_worksheet()
         logger.info("Excel worksheet created in workbook.")
 
@@ -37,21 +38,21 @@
         column_format = self._column_format()
         metadata_format = self._metadata_format()
 
         # Add metadata to the first cell of the Excel sheet.
         logger.info("Writing metadata to worksheet.")
         category = self.metadata["category"].upper()
         strategy = self.metadata["strategy"].upper()
-        metadata_value = f"{strategy} {category} REPORT"
+        metadata_value = f"{strategy} {category}"
         self.worksheet.write(row, col, metadata_value, metadata_format)
 
         # Add the URL heading with a wider column of merged cells.
         row += 2
-        col += 1
-        url_col_width = 3
+        # col += 1
+        url_col_width = 4
         self.worksheet.set_column(col, col, 15)
         self.worksheet.merge_range(
             row, col, row, col + url_col_width, "URL", column_format
         )
 
         # Add a column heading to record each page's overall category score.
         col += url_col_width + 1
@@ -63,23 +64,23 @@
         if self.worksheet is None:
             # Fallback if worksheet doesn't exist for some reason
             logger.warning("Worksheet not found. Creating.")
             self.set_up_worksheet()
 
         self._write_page_url()
         self._write_overall_category_score()
-        self._write_audit_results(self.audit_results, first_resp)
-        self._write_metrics_results(self.metrics_results, first_resp)
+        self._write_metrics_results(first_resp)
+        self._write_audit_results(first_resp)
 
         self.cur_cell[0] += 1  # Move down 1 row for next page's results
         self.cur_cell[1] = 5  # Reset to first results column
 
     def finalize_and_save(self) -> None:
         """Writes the average score to the worksheet and saves/closes it."""
-        self._write_average_score()
+        self._write_average_scores()
         self.workbook.close()
         logger.info("Workbook saved. Check your current directory!")
 
     def _create_workbook(self) -> None:
         """Creates an Excel workbook with a unique and descriptive name."""
         strategy = self.metadata["strategy"]
         category = self.metadata["category"]
@@ -105,78 +106,98 @@
         self.worksheet.write(
             self.cur_cell[0] + 2, self.cur_cell[1], category_score, cat_score_format
         )
         self.cur_cell[1] += 2
         # Add the score to a list so they can all be averaged at the end.
         self.category_scores.append(category_score)
 
-    def _write_average_score(self) -> None:
-        """Writes the average score next to the worksheet metadata."""
-        logger.info("Writing average score to worksheet.")
-        scores = self.category_scores
-        avg_score = sum(scores) / len(scores)
-        avg_score = round(avg_score, 2)
+    def _write_average_scores(self) -> None:
+        """Writes the average scores next to the worksheet metadata."""
+        logger.info("Writing average scores to worksheet.")
         format = self._metadata_format()
-        self.worksheet.write(0, 4, f"Avg Score: {avg_score}", format)
 
-    def _write_audit_results(
-        self, audit_results: AuditResults, first_resp: bool
-    ) -> None:
+        # Audits avg
+        cat_scores = self.category_scores
+        cat_score = self._avg_and_round_scores(cat_scores)
+        self.worksheet.write(0, 4, f"Cat. Score: {str(cat_score)}", format)
+
+        # Metrics avg
+        if self.metrics_scores:
+            m_scores = self.metrics_scores
+            avg_m_score = self._avg_and_round_scores(m_scores)
+            self.worksheet.write(0, 7, f"Metrics Avg: {str(avg_m_score)}", format)
+
+    def _write_audit_results(self, first_resp: bool) -> None:
         """Iterates through the audit results and writes them to the worksheet."""
         column_format = self._column_format()
         row, col = self.cur_cell
 
         logger.info("Writing audit results to worksheet.")
-        for title, scores in audit_results.items():
+        for title, scores in self.audit_results.items():
             self.worksheet.set_column(col, col + 1, 15)
             # cast() is a mypy workaround for issue #1178
             score, value = cast(tuple[Any, Any], scores)
             score_format = self._score_format(score)
             if first_resp:
                 logger.debug("Writing audit result headings to worksheet.")
                 self._write_results_headings(
                     row, col, title, column_format, result_type="audit"
                 )
             self.worksheet.write(row + 2, col, score, score_format)
             self.worksheet.write(row + 2, col + 1, value, score_format)
             col += 2
 
-        self.cur_cell[1] = col + 2
-
-    def _write_metrics_results(
-        self, metrics_results: MetricsResults, first_resp: bool
-    ) -> None:
+    def _write_metrics_results(self, first_resp: bool) -> None:
         """Iterates through the metrics results and writes them to the worksheet."""
         column_format = self._column_format()
-        data_format = self._data_format()
         row, col = self.cur_cell
 
-        if metrics_results is not None:
+        if self.metrics_results is not None:
             logger.info("Writing metrics results to worksheet.")
-            for title, score in metrics_results.items():
-                self.worksheet.set_column(col, col, 30)
+            ovr_score = 0
+            for title, score in self.metrics_results.items():
+                self.worksheet.set_column(col, col, 10)
                 if first_resp:
                     logger.debug("Writing metrics result headings to worksheet.")
                     self._write_results_headings(
                         row, col, title, column_format, result_type="metrics"
                     )
-                self.worksheet.write(row + 2, col, score, data_format)
+                score_format = self._score_format(score)
+                self.worksheet.write(row + 2, col, score, score_format)
+                ovr_score += score
                 col += 1
 
+            # For indiv. URL - will be averaged at the end
+            ovr_score = ovr_score / len(self.metrics_results)
+            ovr_score = round(ovr_score, 1)
+            self.metrics_scores.append(ovr_score)
+
+            self.cur_cell[1] = col + 2  # Don't overwrite metrics with audits
+
+        elif self.metrics_scores:
+            # No metrics results for this URL but previous URLs have written scores
+            # Needed for formatting reasons (set column to align with audit scores)
+            self.cur_cell[1] = 16
+
     def _write_results_headings(
         self, row: int, col: int, title: str, column_format: Format, result_type: str
     ) -> None:
         """Writes the headings for audit or metrics results to the worksheet."""
         if result_type == "audit":
             self.worksheet.merge_range(row, col, row, col + 1, title, column_format)
             self.worksheet.write(row + 1, col, "Score", column_format)
             self.worksheet.write(row + 1, col + 1, "Value", column_format)
         elif result_type == "metrics":
             self.worksheet.write(row, col, title, column_format)
-            self.worksheet.write(row + 1, col, "Value", column_format)
+            self.worksheet.write(row + 1, col, "Score", column_format)
+
+    def _avg_and_round_scores(self, scores):
+        """Helper for averaging and rounding scores."""
+        scores = sum(scores) / len(scores)
+        return round(scores, 1)
 
     def _column_format(self) -> Format:
         """Reusable formatting for column cells."""
         return self.workbook.add_format(
             {"font_size": 16, "bold": 1, "align": "center", "valign": "vcenter"}
         )
```

### Comparing `pyspeedinsights-0.4.0/src/pyspeedinsights/core/sitemap.py` & `pyspeedinsights-0.5.0/src/pyspeedinsights/core/sitemap.py`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.4.0/src/pyspeedinsights/utils/urls.py` & `pyspeedinsights-0.5.0/src/pyspeedinsights/utils/urls.py`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/PKG-INFO` & `pyspeedinsights-0.5.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: pyspeedinsights
-Version: 0.4.0
-Summary: Measure your site speed, performance, accessibility and SEO in bulk from the command line with Python and the PageSpeed Insights API.
-Home-page: https://github.com/wjh18/pyspeedinsights
-Author: Will J. Holmes
-Author-email: will@wjholmes.com
-Project-URL: Documentation, https://github.com/wjh18/pyspeedinsights/blob/master/README.md
-Project-URL: Source, https://github.com/wjh18/pyspeedinsights
-Project-URL: Tracker, https://github.com/wjh18/pyspeedinsights/issues
-Keywords: google,google-apis,psi-api,page-speed-insights,page-speed-insights-api,pagespeedinsightsapi,python,cli
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
-Classifier: Topic :: Utilities
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # pyspeedinsights
 
 Measure your site speed, performance, accessibility and SEO in bulk from the command line with Python and the PageSpeed Insights API.
 
 Support for sitemap parsing and asynchronous requests with aiohttp. Outputs to JSON or a color-coded Excel sheet for further analysis.
 
 ![A screenshot of the tool's Excel output](https://raw.githubusercontent.com/wjh18/pyspeedinsights/master/images/screenshot.png)
@@ -37,25 +12,25 @@
 
 ## Why pyspeedinsights?
 
 Manually running each page of your website through Google's Lighthouse or PageSpeed Insights can be extremely time consuming, especially if it has a large number of pages.
 
 This makes it difficult to analyze its overall performance from a 10,000-foot view without manually testing many similar types of pages.
 
-That's what this package attempts to solve. While there are similar tools out there, pyspeedinsights is the only Python implementation built to support analysis in bulk via async requests.
+That's what this package attempts to solve. While there are similar tools out there, pyspeedinsights is the first Python implementation built to support analysis in bulk via async requests.
 
 Its user-friendly cli gives you the ability to analyze your entire site's speed, SEO, and accessibility results quickly and uncover bottlenecks by reviewing color-coded audit results and metrics for each page in Excel.
 
 ## Format Options
 
 The pyspeedinsights cli supports 3 overarching formats:
 
-1. **Single page JSON (`-f json`)**: Output the raw JSON response from the API to your working directory (single pages only).
-2. **Single page Excel (`-f excel`)**: Write color-coded Lighthouse audits and (optionally) metrics to an Excel sheet (single pages only).
-3. **Sitemap / Multi-page Excel (`-f sitemap`)**: Specify a sitemap file to parse and output your full site's color-coded Lighthouse audits and (optionally) metrics to an Excel sheet.
+1. **Single page JSON (`-f json`)**: Output the raw JSON response from the API to your working directory. If you want to analyze a single page in JSON, use this.
+2. **Single page Excel (`-f excel`)**: Write color-coded Lighthouse audits (any category) and/or PageSpeed CrUX metrics (performance category only) to an Excel sheet. If you want to analyze a single page in Excel, use this.
+3. **Sitemap / Multi-page Excel (`-f sitemap`)**: Specify a sitemap file to parse and output your full site's color-coded Lighthouse audits (any category) and/or PageSpeed CrUX metrics (performance category only) to an Excel sheet. If you want to analyze your entire site in Excel, use this.
 
 There are additional customizations available for request parameters and response processing via the cli as well.
 
 Please reference the [commands](#command-line-arguments) section for further instructions on how to specify formats and customize other options from the cli.
 
 ## Installation
 
@@ -73,35 +48,35 @@
 
 From a system Python3 install on Windows:
 
 ```shell
 py -m pip install pyspeedinsights
 ```
 
-To run the package as a module without installing it from PyPI, `cd` into the `src` directory and run:
+To run the package as a module without installing it from PyPI, clone or download it, `cd` into the `src` directory and run:
 
 ```shell
 python -m pyspeedinsights
 ```
 
 *Note that your PATH, OS or Python version may require that you modify these commands slightly. When in doubt, just install it like you would any other Python package.*
 
 ## Authorization
 
-The PageSpeed Insights API requires users to generate an API key for anything more than simple testing. Otherwise, you'll hit a rate limit rather quickly.
+The PageSpeed Insights API requires users to generate an API key for anything beyond running basic test requests. Otherwise, you'll hit a rate limit rather quickly.
 
 For this reason, a valid API key is currently required to use this package. Please see the [PageSpeed Insights API documentation](https://developers.google.com/speed/docs/insights/v5/get-started) for detailed instructions on how to generate a key.
 
 ### Keys & Quotas
 
 The key itself is added to the GET request URL as a query parameter.
 
 It's recommended to generate the key in *Google Cloud Console > Credentials* then restrict it to your host and the PageSpeed Insights API service. If you do go this route, make sure to enable the service in *Enabled APIs & Services*, as it may not be enabled by default.
 
-The API has a daily and per-minute request quota of 25,000 and 240, respectively. The package automatically sleeps requests for 1 second between each call to avoid hitting the per minute quota or overloading the API and getting hit with 500 errors.
+The API has a daily and per-minute request quota of 25,000 and 240, respectively. To comply with this, the package automatically sleeps requests for 1 second between each call to avoid hitting the per minute quota or overloading the API and getting hit with 500 errors.
 
 ### Keyring
 
 This package uses the `keyring` Python library to store API keys securely on your system's default keystore (e.g. MacOS Keychain for MacOS users).
 
 *Note: If you're unable to use keyring for whatever reason, a fallback input will prompt you for your API key from the command line at the start of each run.*
 
@@ -111,15 +86,15 @@
 
 ### Saving Your API Key
 
 To save your API key to your default keystore, run:
 
 ```shell
 keyring set system psikey
-````
+```
 
 The last argument has to be `psikey`. This is because `pyspeedinsights` looks for that username to read in your key during requests. `system` will instruct `keyring` to automatically detect your system's default keystore.
 
 You'll then receive a prompt where you can enter your key to save it.
 
 ### Verifying Your API Key
 
@@ -139,207 +114,172 @@
 keyring del system psikey
 ```
 
 Then verify that it's no longer accessible with `keyring get system psikey`.
 
 ## Sitemap Support
 
-Currently, only URLs to valid XML sitemaps are supported for reports that utilize sitemap format. Please see [sitemaps.org](https://sitemaps.org/protocol.html) for specification details.
+Currently, only URLs to valid XML sitemaps are supported for reports that utilize sitemap format. Please see [sitemaps.org](https://sitemaps.org/protocol.html) for specification details. Gzipped sitemap (e.g. `sitemap.xml.gz`) support is on the near-term roadmap.
 
 Your web server or sitemap plugin must also allow robots to crawl your sitemap. If you see any permission errors that would be the first thing to check. Certain security solutions like CloudFlare also block crawlers so whitelisting the server you're running the package from may also be preferrable.
 
 Your sitemap URL should be passed in as the positional argument for `url` when running `psi` from the command line.
 
 ### Sitemap Index
 
-Support for sitemap index detection was recently added. This requires no additional action on your part. Simply pass your sitemap index in as the `url` argument via the cli.
+Support for sitemap index detection is also supported. This requires no additional action on your part. Simply pass your sitemap index in as the `url` argument via the cli.
 
-If a sitemap index is detected, the package will recursively gather the URLs listed in each sitemap in your sitemap index and include them in requests. If a standard sitemap file is passed, only that sitemap will be processed.
+If a sitemap index is detected, the package will recursively gather the URLs listed in each sitemap in your sitemap index and include them in requests. If a standard sitemap file is passed, only the URLs in that sitemap will be processed.
 
 ## Command Line Arguments
 
 If you've installed `pyspeedinsights` with `pip`, the default command to run cli commands is `psi`.
 
 If you've simply cloned or downloaded the repo, you can run the cli as a module directly with `python -m pyspeedinsights`. Make sure to `cd` into the `src` directory first.
 
-For help with the following commands, run `psi --help`.
+For help with the following commands, run `psi --help` or `psi -h`.
+
+### Notable Defaults
+
+- `category` - `performance`
+- `strategy`- `desktop`
+- `locale` - `en` (US English)
 
 ### Quickstart
 
 To get you started quickly, here are a few example commands.
 
-Example of requesting a desktop performance report with all metrics for all the URLs in your sitemap:
+Example of requesting a desktop performance report for all the URLs in your sitemap:
 
-* `psi https://www.example.com/sitemap.xml -f sitemap -m all -c performance -s desktop -l en`
-  * Equivalent to: `psi https://www.example.com/sitemap.xml -f sitemap -m all` (`performance`, `desktop` and `en` are defaults)
+- `psi https://example.com/sitemap.xml -f sitemap -c performance -s desktop -l en`
+  - Equivalent to: `psi https://example.com/sitemap.xml -f sitemap`
 
-Example of the same report but also specifying a UTM campaign name/source and captcha token (experimental/untested):
+Example of the same report but also specifying a UTM campaign name/source and captcha token:
 
-* `psi https://www.example.com/sitemap.xml -f sitemap -m all -uc my-campaign-name -us my-campaign-source -t my-captcha-token`
+- `psi https://example.com/sitemap.xml -f sitemap -uc my-campaign-name -us my-campaign-source -t my-captcha-token`
 
 ### Request / Sitemap URL: `url` (required)
 
-The URL of the page you want to analyze *or* a path to a valid XML sitemap (index) if using sitemap format.
+The URL of the page you want to analyze *or* a path to a valid XML sitemap/index if sitemap format was selected.
 
 This must be a fully qualified url with an optional path. URLs without a scheme default to `https`. URL fragments (`#`) and query parameters (`?`) will be removed automatically.
 
-Valid commands:
+Some valid commands:
 
-* `psi https://example.com`
-* `psi https://www.example.com`
-* `psi https://example.com/test`
-* `psi example.com`
-  * Modified URL: `https://example.com`
-* `psi https://example.com#test`
-  * Modified URL: `https://example.com`
-
-Invalid commands:
-
-* `psi example`
-  * Throws an error
-* `psi example/path`
-  * Throws an error
+- `psi https://example.com`
+- `psi https://www.example.com`
+- `psi https://example.com/test`
+- `psi example.com`
+  - Modified URL: `https://example.com`
+- `psi https://example.com#test`
+  - Modified URL: `https://example.com`
+
+Some invalid commands:
+
+- `psi example`
+  - Throws an error
+- `psi example/path`
+  - Throws an error
 
 Sitemap example:
 
-* `psi https://www.example.com/sitemap.xml -f sitemap`
-  * Parses `sitemap.xml` and prepares requests for all `<loc>` elements.
+- `psi https://example.com/sitemap.xml -f sitemap`
+  - Parses `sitemap.xml` and prepares requests for all `<loc>` elements.
 
 Please see [sitemaps](#sitemap-support) for more info.
 
 ### Output Format: `-f` or `--format` (optional)
 
 The format of the Lighthouse results output.
 
-* `json` (default): Output the raw JSON response from the API to your working directory (single pages only). You can add a `-f json` argument explicitly or leave it out to simply default to JSON output.
+- `json` (default): Output the raw JSON response from the API to your working directory (single pages only). You can add a `-f json` argument explicitly or leave it out to simply default to JSON output.
 
-* `excel`: Write color-coded Lighthouse audits and (optionally) metrics to an Excel sheet (analyze the single `url` only).
+- `excel`: Write color-coded Lighthouse audits (any category) and/or PageSpeed CrUX metrics (performance category only) to an Excel sheet (analyze the single `url` only).
 
-* `sitemap`: Specify a sitemap (or index) file to parse and output your full site's color-coded Lighthouse audits and (optionally) metrics to an Excel sheet. When using this option, the `url` argument above needs to be a direct link to your XML sitemap. Please see [sitemaps](#sitemap-support) for more info.
+- `sitemap`: Specify a sitemap (or index) file to parse and output your full site's color-coded Lighthouse audits (any category) and/or PageSpeed CrUX metrics (performance category only) to an Excel sheet. When using this option, the `url` argument above needs to be a direct link to your XML sitemap/index. Please see [sitemaps](#sitemap-support) for more info.
 
 Example:
 
-* `psi https://example.com` - defaults to `json`
-* `psi https://example.com -f excel`
-* `psi https://example.com -f sitemap`
+- `psi https://example.com` - defaults to `json`
+- `psi https://example.com -f json`
+- `psi https://example.com -f excel`
+- `psi https://example.com -f sitemap`
 
 ### Metrics: `-m` or `--metrics` (optional)
 
-Specify which metric(s) you want to include in your report.
+Deprecated in favor of automatically including CrUX metrics if they are available and `performance` category is selected. The previous metrics were debug metrics and subject to change by Google at any time, which made package maintenance difficult.
 
-This is only supported for the performance category (`-c performance`) with either `excel` or `sitemap` formats because the JSON output includes everything by default and categories other than performance don't include metrics in the response.
-
-If excluded, metrics will *not* be dumped to Excel. Add the `all` argument to retrieve all available metrics or specify individual metrics to include.
-
-Example:
-
-* `psi https://example.com -f excel` - no metrics
-* `psi https://example.com -f excel -m all` - all available metrics
-* `psi https://example.com -f excel -m speedIndex` - just speedIndex
-* `psi https://example.com -f excel -m speedIndex totalBlockingTime` - just speedIndex and totalBlockingTime
-
-Full list of available metrics:
-
-* `observedCumulativeLayoutShift`
-* `observedLargestContentfulPaintAllFrames`
-* `maxPotentialFID`
-* `observedSpeedIndexTs`
-* `observedFirstContentfulPaintTs`
-* `observedTimeOrigin`
-* `observedFirstPaint`
-* `observedNavigationStartTs`
-* `observedLargestContentfulPaintAllFramesTs`
-* `speedIndex`
-* `observedFirstContentfulPaint`
-* `observedLastVisualChangeTs`
-* `cumulativeLayoutShiftMainFrame`
-* `observedLastVisualChange`
-* `cumulativeLayoutShift`
-* `largestContentfulPaint`
-* `observedDomContentLoaded`
-* `firstContentfulPaint`
-* `observedCumulativeLayoutShiftMainFrame`
-* `observedFirstVisualChange`
-* `observedFirstPaintTs`
-* `totalCumulativeLayoutShift`
-* `observedFirstMeaningfulPaint`
-* `interactive`
-* `observedTraceEnd`
-* `observedFirstMeaningfulPaintTs`
-* `totalBlockingTime`
-* `observedFirstContentfulPaintAllFramesTs`
-* `observedLargestContentfulPaint`
-* `observedNavigationStart`
-* `observedLoad`
-* `observedFirstVisualChangeTs`
-* `observedFirstContentfulPaintAllFrames`
-* `observedTimeOriginTs`
-* `observedTraceEndTs`
-* `observedLoadTs`
-* `observedDomContentLoadedTs`
-* `observedSpeedIndex`
-* `firstMeaningfulPaint`
-* `observedLargestContentfulPaintTs`
+The new metrics include user-friendly scores instead of raw performance metrics to help give you a quick overview of core metrics like CLS, LCP, etc.
 
 ### Category: `-c` or `--category` (optional)
 
 The Lighthouse category to run. Defaults to `performance`.
 
 Other options include `accessibility`, `best-practices`, `pwa` and `seo`.
 
+Metrics will only be included with the `performance` category.
+
 Example:
 
-* `psi https://www.example.com -c accessibility`
+- `psi https://example.com -c accessibility`
 
 ### Strategy: `-s` or `--strategy` (optional)
 
 The Lighthouse analysis strategy to use. Defaults to `desktop`.
 
 Other options include `mobile`.
 
 Example:
 
-* `psi https://www.example.com -s mobile`
+- `psi https://example.com -s mobile`
 
 ### Locale: `-l` or `--locale` (optional)
 
-The locale used to localize formatted results. Defaults to `en` (US).
+The locale used to localize formatted results (language). Defaults to `en` (US).
 
 Please see the PSI API docs for a [full list of locale options](https://developers.google.com/speed/docs/insights/languages).
 
 Example:
 
-* `psi https://www.example.com -l fr` - localize results to French
+- `psi https://example.com -l fr` - localize results to French
 
-### UTM Campaign: `-uc` or `--campaign` (optional) (experimental)
+### UTM Campaign: `-uc` or `--campaign` (optional)
 
 The UTM campaign name for analytics. Defaults to `None`.
 
-This option is currently experimental and hasn't been fully tested.
+This will add a query parameter to the request made by the PageSpeed Insights API (`?utm_campaign=audit`) so you can differentiate this traffic from real user traffic in Google Analytics.
+
+Pass in the name of your campaign, `audit` is just an example.
 
 Example:
 
-* `psi https://www.example.com -uc my-campaign-name`
+- `psi https://example.com -uc audit`
 
-### UTM Source: `-us` or `--source` (optional) (experimental)
+### UTM Source: `-us` or `--source` (optional)
 
 The UTM campaign source for analytics. Defaults to `None`.
 
-This option is currently experimental and hasn't been fully tested.
+This will add a query parameter to the request made by the PageSpeed Insights API (`?utm_source=psi`) so you can differentiate this traffic from real user traffic in Google Analytics.
+
+Feel free to customize the name of the source, `psi` is just an example.
 
 Example:
 
-* `psi https://www.example.com -us my-campaign-source`
+- `psi https://example.com -us psi`
 
-### Captcha Token: `-t` or `--token` (optional) (experimental)
+### Captcha Token: `-t` or `--token` (optional)
 
 The captcha token passed when filling out a captcha. Defaults to `None`.
 
-This option is currently experimental and hasn't been fully tested.
+This will add a query parameter to the request made by the PageSpeed Insights API (`?utm_source=psi`) containing your captcha token. If you have captcha protection enabled on your site, passing this token as an argument to bypass it will ensure that PSI can analyze your site.
 
 Example:
 
-* `psi https://www.example.com -t my-captcha-token`
+- `psi https://example.com -t my-captcha-token`
+
+## Help
+
+Please open an issue on GitHub if you run into any issues or need assistance.
 
 ## Contributing
 
 Contributors of all skill levels are welcome to help improve this package. Please see the [Contribution Guidelines](CONTRIBUTING.md) for details.
```

### Comparing `pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/SOURCES.txt` & `pyspeedinsights-0.5.0/src/pyspeedinsights.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -18,10 +18,9 @@
 src/pyspeedinsights/cli/__init__.py
 src/pyspeedinsights/cli/choices.py
 src/pyspeedinsights/cli/commands.py
 src/pyspeedinsights/core/__init__.py
 src/pyspeedinsights/core/excel.py
 src/pyspeedinsights/core/sitemap.py
 src/pyspeedinsights/utils/__init__.py
-src/pyspeedinsights/utils/exceptions.py
 src/pyspeedinsights/utils/generic.py
 src/pyspeedinsights/utils/urls.py
```


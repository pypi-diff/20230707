# Comparing `tmp/idms-0.1.9.tar.gz` & `tmp/idms-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idms-0.1.9.tar", last modified: Thu Jul  1 09:29:19 2021, max compression
+gzip compressed data, was "idms-0.2.0.tar", last modified: Thu Jul  6 21:58:20 2023, max compression
```

## Comparing `idms-0.1.9.tar` & `idms-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:29:19.047413 idms-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2021-07-01 09:29:11.000000 idms-0.1.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      157 2021-07-01 09:29:11.000000 idms-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2925 2021-07-01 09:29:19.047413 idms-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2021-07-01 09:29:11.000000 idms-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:29:19.043413 idms-0.1.9/data/
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-07-01 09:29:11.000000 idms-0.1.9/data/data_file
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-07-01 09:29:11.000000 idms-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-07-01 09:29:19.047413 idms-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     8639 2021-07-01 09:29:11.000000 idms-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:29:19.043413 idms-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:29:19.043413 idms-0.1.9/src/idms/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-07-01 09:29:11.000000 idms-0.1.9/src/idms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:29:19.043413 idms-0.1.9/src/idms/api/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-07-01 09:29:11.000000 idms-0.1.9/src/idms/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10185 2021-07-01 09:29:11.000000 idms-0.1.9/src/idms/api/contentserver.py
--rw-r--r--   0 runner    (1001) docker     (121)      569 2021-07-01 09:29:11.000000 idms-0.1.9/src/idms/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:29:19.043413 idms-0.1.9/src/idms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2925 2021-07-01 09:29:18.000000 idms-0.1.9/src/idms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      446 2021-07-01 09:29:18.000000 idms-0.1.9/src/idms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-01 09:29:18.000000 idms-0.1.9/src/idms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-07-01 09:29:18.000000 idms-0.1.9/src/idms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      101 2021-07-01 09:29:18.000000 idms-0.1.9/src/idms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-07-01 09:29:18.000000 idms-0.1.9/src/idms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-01 09:29:19.047413 idms-0.1.9/src/sample/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-07-01 09:29:11.000000 idms-0.1.9/src/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-07-01 09:29:11.000000 idms-0.1.9/src/sample/package_data.dat
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-07-01 09:29:11.000000 idms-0.1.9/src/sample/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:58:20.329176 idms-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-06 21:58:09.000000 idms-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-06 21:58:09.000000 idms-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-06 21:58:20.329176 idms-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-07-06 21:58:09.000000 idms-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:58:20.325176 idms-0.2.0/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 21:58:09.000000 idms-0.2.0/data/data_file
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-06 21:58:09.000000 idms-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 21:58:20.329176 idms-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-06 21:58:09.000000 idms-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:58:20.325176 idms-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:58:20.325176 idms-0.2.0/src/idms/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 21:58:09.000000 idms-0.2.0/src/idms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:58:20.329176 idms-0.2.0/src/idms/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 21:58:09.000000 idms-0.2.0/src/idms/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-07-06 21:58:09.000000 idms-0.2.0/src/idms/api/contentserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-06 21:58:09.000000 idms-0.2.0/src/idms/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:58:20.329176 idms-0.2.0/src/idms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-06 21:58:20.000000 idms-0.2.0/src/idms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-06 21:58:20.000000 idms-0.2.0/src/idms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:58:20.000000 idms-0.2.0/src/idms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-06 21:58:20.000000 idms-0.2.0/src/idms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-06 21:58:20.000000 idms-0.2.0/src/idms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 21:58:20.000000 idms-0.2.0/src/idms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:58:20.329176 idms-0.2.0/src/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-06 21:58:09.000000 idms-0.2.0/src/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 21:58:09.000000 idms-0.2.0/src/sample/package_data.dat
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 21:58:09.000000 idms-0.2.0/src/sample/simple.py
```

### Comparing `idms-0.1.9/LICENSE.txt` & `idms-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `idms-0.1.9/PKG-INFO` & `idms-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 Metadata-Version: 2.1
 Name: idms
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python class to talk to idms REST and Search API, better known as iDMS.
-Home-page: https://github.com/pypa/idms
+Home-page: https://github.com/Provincie-Zuid-Holland/idms
 Author: Daniel Overdevest
 Author-email: d.overdevest@pzh.nl
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ProvZH/idms/issues
 Project-URL: Source, https://github.com/ProvZH/idms
-Description: # iDMS
-        
-        ![Upload Python Package](https://github.com/ProvZH/iDMS/workflows/Upload%20Python%20Package/badge.svg)
-        
-        
-        Python class to talk to iDMS REST and Search API within Provincie Zuid-Holland.
-        
-        # Goal
-        The goal of the package is to have an easy interface to use the API in Python.
-        
-        Mainly focussed to work with Content Server 20.2, see [API docs](
-        https://appworksdeveloper.opentext.com/webaccess/#url=%2Fawd%2Fresources%2Fapis%2Fcs-rest-api-for-cs-20-2&tab=501).
-        
-        # Quick start
-        ## Requirements
-        1. `pip install idms`
-        2. `pip install pandas` (optional - for easy data transformation)
-        3. `pip install openpyxl` (optional - to write to Excel file)
-        
-        ##  Sample code
-        ```python
-        import getpass
-        import idms.api.contentserver as cs
-        import pandas # optional
-        
-        baseUrl = "idms-url"
-        idms_username = getpass.getpass(prompt='IDMS username:')
-        idms_password = getpass.getpass(prompt='IDMS password:')
-        idms = cs.crawler(baseUrl, idms_username, idms_password)
-        
-        array = idms.search("overdevest prox[1,f] daniel)")
-        print(f"Found {len(array)} search results")
-        
-        # optional load results in a data frame to export results.
-        df = pd.DataFrame(arr)
-        print(df)
-        
-        # Export results to Excel
-        df.to_excel("searchresults.xlsx")
-        ```
-        
-        # Development
-        Package is hosted on GitHub. After each change increase version number and create a new Release on GitHub. The pipeline will trigger a release to PyPi (see status batch above).
-        
-        ## Collaborate?
-        Send a PR!
-        
-        # Disclaimer
-        The developers of this package are not affiliated with OpenText.
 Keywords: idms,contentserver,restapi,searchapi
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.5, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE.txt
+
+# iDMS
+
+![Upload Python Package](https://github.com/ProvZH/iDMS/workflows/Upload%20Python%20Package/badge.svg)
+
+
+Python class to talk to iDMS REST and Search API within Provincie Zuid-Holland.
+
+# Goal
+The goal of the package is to have an easy interface to use the API in Python.
+
+Mainly focussed to work with Content Server 21.4, see [API docs](
+https://developer.opentext.com/apis/14ba85a7-4693-48d3-8c93-9214c663edd2/d7540c64-7da2-4554-9966-069c56a9341d/09aaed57-c70b-4092-bace-762b42520293).
+
+# Quick start
+## Requirements
+1. `pip install idms`
+2. `pip install pandas` (optional - for easy data transformation)
+3. `pip install openpyxl` (optional - to write to Excel file)
+
+##  Sample code
+```python
+import getpass
+import idms.api.contentserver as cs
+import pandas # optional
+
+baseUrl = "idms-url"
+idms_username = getpass.getpass(prompt='IDMS username:')
+idms_password = getpass.getpass(prompt='IDMS password:')
+idms = cs.crawler(baseUrl, idms_username, idms_password)
+
+array = idms.search("overdevest prox[1,f] daniel)")
+print(f"Found {len(array)} search results")
+
+# optional load results in a data frame to export results.
+df = pd.DataFrame(arr)
+print(df)
+
+# Export results to Excel
+df.to_excel("searchresults.xlsx")
+```
+
+# Development
+Package is hosted on GitHub. After each change increase version number and create a new Release on GitHub. The pipeline will trigger a release to PyPi (see status batch above).
+
+## Collaborate?
+Send a PR!
+
+# Disclaimer
+The developers of this package are not affiliated with OpenText.
```

### Comparing `idms-0.1.9/README.md` & `idms-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 
 Python class to talk to iDMS REST and Search API within Provincie Zuid-Holland.
 
 # Goal
 The goal of the package is to have an easy interface to use the API in Python.
 
-Mainly focussed to work with Content Server 20.2, see [API docs](
-https://appworksdeveloper.opentext.com/webaccess/#url=%2Fawd%2Fresources%2Fapis%2Fcs-rest-api-for-cs-20-2&tab=501).
+Mainly focussed to work with Content Server 21.4, see [API docs](
+https://developer.opentext.com/apis/14ba85a7-4693-48d3-8c93-9214c663edd2/d7540c64-7da2-4554-9966-069c56a9341d/09aaed57-c70b-4092-bace-762b42520293).
 
 # Quick start
 ## Requirements
 1. `pip install idms`
 2. `pip install pandas` (optional - for easy data transformation)
 3. `pip install openpyxl` (optional - to write to Excel file)
```

### Comparing `idms-0.1.9/setup.py` & `idms-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
-long_description = (here / 'README.md').read_text(encoding='utf-8')
+long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
@@ -25,178 +25,157 @@
     # $ pip install sampleproject
     #
     # And where it will live on PyPI: https://pypi.org/project/sampleproject/
     #
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
-    name='idms',  # Required
-
+    name="idms",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.9',  # Required
-
+    version="0.2.0",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
-    description='Python class to talk to idms REST and Search API, better known as iDMS.',  # Optional
-
+    description="Python class to talk to idms REST and Search API, better known as iDMS.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
     # Often, this is the same as your README, so you can just read it in from
     # that file directly (as we have already done above)
     #
     # This field corresponds to the "Description" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#description-optional
     long_description=long_description,  # Optional
-
     # Denotes that our long_description is in Markdown; valid values are
     # text/plain, text/x-rst, and text/markdown
     #
     # Optional if long_description is written in reStructuredText (rst) but
     # required for plain-text or Markdown; if unspecified, "applications should
     # attempt to render [the long_description] as text/x-rst; charset=UTF-8 and
     # fall back to text/plain if it is not valid rst" (see link below)
     #
     # This field corresponds to the "Description-Content-Type" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#description-content-type-optional
-    long_description_content_type='text/markdown',  # Optional (see note above)
-
+    long_description_content_type="text/markdown",  # Optional (see note above)
     # This should be a valid link to your project's main homepage.
     #
     # This field corresponds to the "Home-Page" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#home-page-optional
-    url='https://github.com/pypa/idms',  # Optional
-
+    url="https://github.com/Provincie-Zuid-Holland/idms",  # Optional
     # This should be your name or the name of the organization which owns the
     # project.
-    author='Daniel Overdevest',  # Optional
-
+    author="Daniel Overdevest",  # Optional
     # This should be a valid email address corresponding to the author listed
     # above.
-    author_email='d.overdevest@pzh.nl',  # Optional
-
+    author_email="d.overdevest@pzh.nl",  # Optional
     # Classifiers help users find your project by categorizing it.
     #
     # For a list of valid classifiers, see https://pypi.org/classifiers/
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        'Development Status :: 4 - Beta',
-
+        "Development Status :: 4 - Beta",
         # Indicate who your project is intended for
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
-
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
         # Pick your license as you wish
-        'License :: OSI Approved :: MIT License',
-
+        "License :: OSI Approved :: MIT License",
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate you support Python 3. These classifiers are *not*
         # checked by 'pip install'. See instead 'python_requires' below.
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3 :: Only',
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3 :: Only",
     ],
-
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a list of additional keywords, separated
     # by commas, to be used to assist searching for the distribution in a
     # larger catalog.
-    keywords='idms, contentserver, restapi, searchapi',  # Optional
-
+    keywords="idms, contentserver, restapi, searchapi",  # Optional
     # When your source code is in a subdirectory under the project root, e.g.
     # `src/`, it is necessary to specify the `package_dir` argument.
-    package_dir={'': 'src'},  # Optional
-
+    package_dir={"": "src"},  # Optional
     # You can just specify package directories manually here if your project is
     # simple. Or you can use find_packages().
     #
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
     # called `my_module.py` to exist:
     #
     #   py_modules=["my_module"],
     #
-    packages=find_packages(where='src'),  # Required
-
+    packages=find_packages(where="src"),  # Required
     # Specify which Python versions you support. In contrast to the
     # 'Programming Language' classifiers above, 'pip install' will check this
     # and refuse to install the project if the version does not match. See
     # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
-    python_requires='>=3.5, <4',
-
+    python_requires=">=3.5, <4",
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['requests>=2.25.0'],  # Optional
-
+    install_requires=["requests>=2.25.0"],  # Optional
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
     # Similar to `install_requires` above, these must be valid existing
     # projects.
     extras_require={  # Optional
-        'dev': ['check-manifest', 'python-dotenv>=0.15.0', 'pandas>=1.1.4', 'openpyxl'],
-        'test': ['coverage'],
+        "dev": ["check-manifest", "python-dotenv>=0.15.0", "pandas>=1.1.4", "openpyxl"],
+        "test": ["coverage"],
     },
-
     # If there are data files included in your packages that need to be
     # installed, specify them here.
     package_data={  # Optional
-        'sample': ['package_data.dat'],
+        "sample": ["package_data.dat"],
     },
-
     # Although 'package_data' is the preferred approach, in some case you may
     # need to place data files outside of your packages. See:
     # http://docs.python.org/distutils/setupscript.html#installing-additional-files
     #
     # In this case, 'data_file' will be installed into '<sys.prefix>/my_data'
-    data_files=[('my_data', ['data/data_file'])],  # Optional
-
+    data_files=[("my_data", ["data/data_file"])],  # Optional
     # To provide executable scripts, use entry points in preference to the
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # `pip` to create the appropriate form of executable for the target
     # platform.
     #
     # For example, the following would provide a command called `sample` which
     # executes the function `main` from this package when invoked:
     entry_points={  # Optional
-        'console_scripts': [
-            'sample=sample:main',
+        "console_scripts": [
+            "sample=sample:main",
         ],
     },
-
     # List additional URLs that are relevant to your project as a dict.
     #
     # This field corresponds to the "Project-URL" metadata fields:
     # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
     #
     # Examples listed include a pattern for specifying where the package tracks
     # issues, where the source is hosted, where to say thanks to the package
     # maintainers, and where to support the project financially. The key is
     # what's used to render the link text on PyPI.
     project_urls={  # Optional
-        'Bug Reports': 'https://github.com/ProvZH/idms/issues',
+        "Bug Reports": "https://github.com/ProvZH/idms/issues",
         # 'Funding': 'https://donate.pypi.org',
         # 'Say Thanks!': 'http://saythanks.io/to/example',
-        'Source': 'https://github.com/ProvZH/idms',
+        "Source": "https://github.com/ProvZH/idms",
     },
 )
```

### Comparing `idms-0.1.9/src/idms/api/contentserver.py` & `idms-0.2.0/src/idms/api/contentserver.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,233 +3,302 @@
 import logging
 import json
 import datetime, time
 import copy
 import idms.functions as otfunc
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
+from urllib.parse import urlparse, urlunparse, parse_qs
 from functools import reduce
 
+
 def dotfield(input_dict: dict, input_key: str, notFound=None) -> str:
     """
     Magic function to get nested properties from dictionary writen as level1.level2.level3.
-    
-    Example: 
+
+    Example:
     dotfield({"a": {"b": {"c": "def"}}}, "a.b.c") -> "def"
     """
-    return reduce(lambda d, k: d.get(k) if d else notFound, input_key.split("."), input_dict)
+    return reduce(
+        lambda d, k: d.get(k) if d else notFound, input_key.split("."), input_dict
+    )
+
 
 class crawler:
-    def __init__(self, baseUrl: str, username: str = None, password: str = None, ticket: str = None):
-        
+    def __init__(
+        self,
+        baseUrl: str,
+        username: str = None,
+        password: str = None,
+        ticket: str = None,
+        verifySSL: bool = True,
+    ):
         # Settings for retry and auto retry if error code 500 is given
         retry = Retry(
             total=5,
             read=5,
             connect=5,
             backoff_factor=0.3,
             status_forcelist=(500, 502, 504),
         )
 
         # Mounts a session for re-use authorization
         self.baseUrl = baseUrl
         self.session = requests.Session()
+        self.session.verify = verifySSL
         self.session.mount(baseUrl, HTTPAdapter(max_retries=retry))
 
         # Safety measures to not to overload the server.
         self.maxCallsPerFolder = 10000
         self.gracefulSleepSeconds = 0.01
 
         # Type 0 is always a folder, 751 is for ProvZH an E-mailmap and 136 for Samengesteld document and 298 for a Collectie.
         self.folderTypes = [0, 751, 136, 298]
         self.folderTypesStopRecursive = [136, 298]
 
         self.includeParentsPath = True
-        self.outputColumns = ['properties.parent_id', 
-                              'properties.id', 
-                              'properties.size', 
-                              'properties.create_date', 
-                              'properties.modify_date', 
-                              'properties.owner', 
-                              'properties.create_user_id', 
-                              'properties.name', 
-                              'properties.description', 
-                              'properties.type', 
-                              'properties.type_name',
-                              'properties.summary',
-                              'properties.description_multilingual.nl',
-                              'regions.OTLocation',
-                              'systemattributes.Dossiernummer']
+        self.outputColumns = [
+            "properties.parent_id",
+            "properties.id",
+            "properties.size",
+            "properties.create_date",
+            "properties.modify_date",
+            "properties.owner",
+            "properties.create_user_id",
+            "properties.name",
+            "properties.description",
+            "properties.type",
+            "properties.type_name",
+            "properties.summary",
+            "properties.description_multilingual.nl",
+            "regions.OTLocation",
+            "systemattributes.Dossiernummer",
+        ]
 
         self.debugJson = False
 
         if ticket:
             self.ticket = ticket
         else:
             self.ticket = self.authorize(username, password)
 
-    def authorize(self, username: str, password: str) -> str: 
+    def authorize(self, username: str, password: str) -> str:
         """
         Function to authenticate yourself and get token for future requests.
         """
-        url = self.baseUrl + '/api/v1/auth'
-        body = {u'username': username, u'password': password}
+        url = self.baseUrl + "/api/v1/auth"
+        body = {"username": username, "password": password}
         response = self.session.post(url, data=body)
         try:
             r = response.json()
-            return r.get('ticket')
+            error = r.get("error")
+            if error:
+                raise Exception("Username or password not correct!")
+            else:
+                logging.info("Succesfull logged in to ContentServer.")
+            return r.get("ticket")
         except:
             print(response)
-            raise Exception('Username or password not correct!')
-     
+            raise Exception("Username or password not correct!")
+
     def flattenParents(self, listParents: list, lastNode: str = None) -> str:
         """
         Function to concat parents to string.
         listParents: [] (list)
         lastNode: DocumentName (str)
         Example: Central > Map 1 > Map 2 > DocumentName
         """
-        joinedString = " > ".join([a.get('name') for a in listParents])
+        joinedString = " > ".join([a.get("name") for a in listParents])
         if lastNode:
             return joinedString + " > " + str(lastNode)
         else:
             return joinedString
-    
+
     def parents(self, nodeId: str) -> list:
         """
         Recursive function to craw all parents of node.
         """
-        headers = {'otcsticket': self.ticket}
+        headers = {"otcsticket": self.ticket}
 
-        url = self.baseUrl + f"/api/v1/nodes/{nodeId}/ancestors"  
-        logging.debug(f'url: {url}')
+        url = self.baseUrl + f"/api/v1/nodes/{nodeId}/ancestors"
+        logging.debug(f"url: {url}")
         logging.debug(headers)
-        r = self.session.get(url, headers=headers, timeout=60*30)
+        r = self.session.get(url, headers=headers, timeout=60 * 30)
         r.raise_for_status()
         data = r.json()
-        return data.get('ancestors', [])
+        return data.get("ancestors", [])
 
     def parseNodeColumns(self, dataRow: dict, parents: list = []) -> dict:
         """
         Reduce dict to only usefull output columns based on: `self.outputColumns`
         """
         row = {}
 
         nodeId = dotfield(dataRow, "properties.id")
-        row['downloadUrl'] = f"/otcs/llisapi.dll?func=ll&objId={nodeId}&objAction=download"
-        row['viewUrl'] = f"/otcs/llisapi.dll?func=ll&objId={nodeId}&objAction=browse"
-        row['nodeType'] = otfunc.mimetype2FileType(dotfield(dataRow, "properties.mime_type"))
+        row[
+            "downloadUrl"
+        ] = f"/otcs/llisapi.dll?func=ll&objId={nodeId}&objAction=download"
+        row["viewUrl"] = f"/otcs/llisapi.dll?func=ll&objId={nodeId}&objAction=browse"
+        row["nodeType"] = otfunc.mimetype2FileType(
+            dotfield(dataRow, "properties.mime_type")
+        )
         for colName in self.outputColumns:
             row[colName] = dotfield(dataRow, colName)
-        
+
         if self.includeParentsPath:
-            row['locationPathString'] = self.flattenParents(parents)
+            row["locationPathString"] = self.flattenParents(parents)
 
         return row
-    
-    def children(self, nodeId: str, parents: list = None, stopRecursive: bool = False) -> list:
+
+    def children(
+        self, nodeId: str, parents: list = None, stopRecursive: bool = False
+    ) -> list:
         """
         Recursive function to craw children of node.
         """
-        headers = {'otcsticket': self.ticket}
+        headers = {"otcsticket": self.ticket}
 
         if not parents and self.includeParentsPath:
             parents = self.parents(nodeId)
         page = 1
         counter = 1
         limit = 100
         page_total = 9999999999999
         results = []
         while page <= page_total and counter < self.maxCallsPerFolder:
             counter = counter + 1
-            url = self.baseUrl + f"/api/v2/nodes/{nodeId}/nodes?limit={limit}&page={page}"  
-            logging.debug(f'url: {url}')
+            url = (
+                self.baseUrl + f"/api/v2/nodes/{nodeId}/nodes?limit={limit}&page={page}"
+            )
+            logging.debug(f"url: {url}")
             logging.debug(headers)
-            r = self.session.get(url, headers=headers, timeout=60*30)
+            r = self.session.get(url, headers=headers, timeout=60 * 30)
             r.raise_for_status()
-            page = page + 1 
+            page = page + 1
             data = r.json()
             if self.debugJson:
                 yyyymmddhhmmss = datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")
                 with open(f"debug_{yyyymmddhhmmss}.json", "w") as f:
                     json.dump(data, f)
 
             page_total = dotfield(data, "collection.paging.page_total", 0)
-            for result in data.get('results', []):
-                dataRow = result.get('data')
+            for result in data.get("results", []):
+                dataRow = result.get("data")
 
                 # Check if a node is a folder type. Some folder types are collections of other nodes
                 # the risk of recursive call a collection is that it can end in an infinity loop.
                 # folderTypesStopRecursive is a list of collectiontypes and children will be fetched.
                 # If there are also subfolders in that collection it won't fetch further.
-                if dotfield(dataRow, "properties.type") in self.folderTypes and stopRecursive == False:
+                if (
+                    dotfield(dataRow, "properties.type") in self.folderTypes
+                    and stopRecursive == False
+                ):
                     time.sleep(self.gracefulSleepSeconds)
                     # Recursive call
                     newParents = copy.deepcopy(parents)
-                    newParents.append({'id': dotfield(dataRow, "properties.id"), 'name': dotfield(dataRow, "properties.name"), 'parent_id': dotfield(dataRow, "properties.parent_id"), 'type': dotfield(dataRow, "properties.type"), 'volume_id': dotfield(dataRow, "properties.volume_id"), 'type_name': dotfield(dataRow, "properties.type_name")})
-                    if dotfield(dataRow, "properties.type") in self.folderTypesStopRecursive:
+                    newParents.append(
+                        {
+                            "id": dotfield(dataRow, "properties.id"),
+                            "name": dotfield(dataRow, "properties.name"),
+                            "parent_id": dotfield(dataRow, "properties.parent_id"),
+                            "type": dotfield(dataRow, "properties.type"),
+                            "volume_id": dotfield(dataRow, "properties.volume_id"),
+                            "type_name": dotfield(dataRow, "properties.type_name"),
+                        }
+                    )
+                    if (
+                        dotfield(dataRow, "properties.type")
+                        in self.folderTypesStopRecursive
+                    ):
                         stopRecursive = True
                     else:
                         stopRecursive = False
-                    childs = self.children(dotfield(dataRow, "properties.id"), newParents, stopRecursive)
+                    childs = self.children(
+                        dotfield(dataRow, "properties.id"), newParents, stopRecursive
+                    )
                     results = results + childs
-                
+
                 row = self.parseNodeColumns(dataRow, parents)
 
                 results.append(row)
-        
-        if counter >= self.maxCallsPerFolder:
-            raise Exception(f"Stopped due counter ({counter}) reached the maxCallsPerFolder ({self.maxCallsPerFolder}) limit!")
-
-        
-        return results 
 
-    def search(self, complexQuery: str, limit: int = 10, metadata: str = "true") -> list:
+        if counter >= self.maxCallsPerFolder:
+            raise Exception(
+                f"Stopped due counter ({counter}) reached the maxCallsPerFolder ({self.maxCallsPerFolder}) limit!"
+            )
+
+        return results
+
+    def search(
+        self,
+        complexQuery: str,
+        limit: int = 10,
+        metadata: str = "true",
+        slice: str = None,
+    ) -> list:
         """
-        Search API endpoint  
+        Search API endpoint
         Example: {self.baseUrl}/api/v2/search?where=`complexQuery`&limit=`limit`&metadata=`metadata`
-       
+
         :param str `complexQuery`:  See documentation for search options for a complexQuery: https://docs2.cer-rec.gc.ca/ll-eng/llisapi.dll?func=help.index&keyword=LL.Search%20Broker.Category
         """
         results = []
-        headers = {'otcsticket': self.ticket}
-        complexQueryUrlSafe = urllib.parse.quote(complexQuery, safe='')
+        headers = {"otcsticket": self.ticket}
         counter = 0
-        url = self.baseUrl + f"/api/v2/search?where={complexQueryUrlSafe}&limit={limit}&metadata={metadata}"
-        
+        url = self.baseUrl + "/api/v2/search"
+
+        base_data = {"where": complexQuery, "limit": limit, "metadata": metadata}
+        if slice:
+            base_data["slice"] = slice
+
         # Retrieve all pages of certain search query using a while loop with security of maxCallsPerFolder variable.
         while url != "" and counter < self.maxCallsPerFolder:
             counter = counter + 1
-
+            data = base_data.copy()
             # Query Content Server API to search for params
-            r = self.session.get(url, headers=headers, timeout=60*30)
+            if "?" in url:
+                url, params = url.split("?")
+
+                # Split the query string on the '&' character
+                query_params = params.split('&')
+
+                # Loop through each key-value pair and add it to the dictionary
+                for param in query_params:
+                    key, value = param.split('=')
+                    data[key] = value
+
+            logging.debug(data)
+            r = self.session.post(url, headers=headers, timeout=60 * 30, data=data)
             r.raise_for_status()
-            data = r.json()
+            search_results = r.json()
             if self.debugJson:
                 yyyymmddhhmmss = datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")
                 with open(f"debug_{yyyymmddhhmmss}.json", "w") as f:
-                    json.dump(data, f)
-            
+                    json.dump(search_results, f)
+
             # Extract only relevant columns from search results
-            for result in data.get('results', []):
-                dataRow = result.get('data')
+            for result in search_results.get("results", []):
+                dataRow = result.get("data")
                 row = self.parseNodeColumns(dataRow)
 
-                ancestorsList = dotfield(result, 'links.ancestors', [])
-                ancestorsStr = " > ".join([a.get('name') for a in ancestorsList])
-                row['locationPathString'] = ancestorsStr
-                row['complexQuery'] = complexQuery
+                ancestorsList = dotfield(result, "links.ancestors", [])
+                ancestorsStr = " > ".join([a.get("name") for a in ancestorsList])
+                row["locationPathString"] = ancestorsStr
+                row["complexQuery"] = complexQuery
                 results.append(row)
 
             # Determine if there is a next page and prepare for next while-loop.
-            nextUrl = dotfield(data, "collection.paging.links.next.href")
+            # nextUrl contains a GET url to retrieve the next page.
+            nextUrl = dotfield(search_results, "collection.paging.links.next.href")
             logging.debug(f" > nextUrl: {nextUrl}")
             if nextUrl:
                 url = self.baseUrl + nextUrl
             else:
                 url = ""
 
         # Inform user if stopped earlier due maxCallsPerFolder variable
         if counter >= self.maxCallsPerFolder:
-            raise Exception(f"Stopped due counter ({counter}) reached the maxCallsPerFolder ({self.maxCallsPerFolder}) limit!")
+            logging.warning(
+                f"Stopped due counter ({counter}) reached the maxCallsPerFolder ({self.maxCallsPerFolder}) limit!"
+            )
 
-        return results
+        return results
```

### Comparing `idms-0.1.9/src/idms/functions.py` & `idms-0.2.0/src/idms/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # from mimetype_description import get_mime_type_description
 
+
 def mimetype2FileType(mimetype: str) -> str:
     """
     Lookup table for mime type to file type.
     """
     convertDict = {
         "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet": "Excel",
         "application/x-zip-compressed": "Compressed folder",
         "application/x-outlook-msg": "Mail message",
-        "application/octet-stream": "Data file (csv?)"
+        "application/octet-stream": "Data file (csv?)",
     }
-    return convertDict.get(mimetype) or "Mimetype not Found: " + str(mimetype) # or get_mime_type_description(mimetype) 
+    return convertDict.get(mimetype) or "Mimetype not Found: " + str(
+        mimetype
+    )  # or get_mime_type_description(mimetype)
```

### Comparing `idms-0.1.9/src/idms.egg-info/PKG-INFO` & `idms-0.2.0/src/idms.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 Metadata-Version: 2.1
 Name: idms
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python class to talk to idms REST and Search API, better known as iDMS.
-Home-page: https://github.com/pypa/idms
+Home-page: https://github.com/Provincie-Zuid-Holland/idms
 Author: Daniel Overdevest
 Author-email: d.overdevest@pzh.nl
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ProvZH/idms/issues
 Project-URL: Source, https://github.com/ProvZH/idms
-Description: # iDMS
-        
-        ![Upload Python Package](https://github.com/ProvZH/iDMS/workflows/Upload%20Python%20Package/badge.svg)
-        
-        
-        Python class to talk to iDMS REST and Search API within Provincie Zuid-Holland.
-        
-        # Goal
-        The goal of the package is to have an easy interface to use the API in Python.
-        
-        Mainly focussed to work with Content Server 20.2, see [API docs](
-        https://appworksdeveloper.opentext.com/webaccess/#url=%2Fawd%2Fresources%2Fapis%2Fcs-rest-api-for-cs-20-2&tab=501).
-        
-        # Quick start
-        ## Requirements
-        1. `pip install idms`
-        2. `pip install pandas` (optional - for easy data transformation)
-        3. `pip install openpyxl` (optional - to write to Excel file)
-        
-        ##  Sample code
-        ```python
-        import getpass
-        import idms.api.contentserver as cs
-        import pandas # optional
-        
-        baseUrl = "idms-url"
-        idms_username = getpass.getpass(prompt='IDMS username:')
-        idms_password = getpass.getpass(prompt='IDMS password:')
-        idms = cs.crawler(baseUrl, idms_username, idms_password)
-        
-        array = idms.search("overdevest prox[1,f] daniel)")
-        print(f"Found {len(array)} search results")
-        
-        # optional load results in a data frame to export results.
-        df = pd.DataFrame(arr)
-        print(df)
-        
-        # Export results to Excel
-        df.to_excel("searchresults.xlsx")
-        ```
-        
-        # Development
-        Package is hosted on GitHub. After each change increase version number and create a new Release on GitHub. The pipeline will trigger a release to PyPi (see status batch above).
-        
-        ## Collaborate?
-        Send a PR!
-        
-        # Disclaimer
-        The developers of this package are not affiliated with OpenText.
 Keywords: idms,contentserver,restapi,searchapi
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.5, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE.txt
+
+# iDMS
+
+![Upload Python Package](https://github.com/ProvZH/iDMS/workflows/Upload%20Python%20Package/badge.svg)
+
+
+Python class to talk to iDMS REST and Search API within Provincie Zuid-Holland.
+
+# Goal
+The goal of the package is to have an easy interface to use the API in Python.
+
+Mainly focussed to work with Content Server 21.4, see [API docs](
+https://developer.opentext.com/apis/14ba85a7-4693-48d3-8c93-9214c663edd2/d7540c64-7da2-4554-9966-069c56a9341d/09aaed57-c70b-4092-bace-762b42520293).
+
+# Quick start
+## Requirements
+1. `pip install idms`
+2. `pip install pandas` (optional - for easy data transformation)
+3. `pip install openpyxl` (optional - to write to Excel file)
+
+##  Sample code
+```python
+import getpass
+import idms.api.contentserver as cs
+import pandas # optional
+
+baseUrl = "idms-url"
+idms_username = getpass.getpass(prompt='IDMS username:')
+idms_password = getpass.getpass(prompt='IDMS password:')
+idms = cs.crawler(baseUrl, idms_username, idms_password)
+
+array = idms.search("overdevest prox[1,f] daniel)")
+print(f"Found {len(array)} search results")
+
+# optional load results in a data frame to export results.
+df = pd.DataFrame(arr)
+print(df)
+
+# Export results to Excel
+df.to_excel("searchresults.xlsx")
+```
+
+# Development
+Package is hosted on GitHub. After each change increase version number and create a new Release on GitHub. The pipeline will trigger a release to PyPi (see status batch above).
+
+## Collaborate?
+Send a PR!
+
+# Disclaimer
+The developers of this package are not affiliated with OpenText.
```


# Comparing `tmp/biobb_pmx-3.8.1.tar.gz` & `tmp/biobb_pmx-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_pmx-3.8.1.tar", last modified: Thu Sep 15 13:49:55 2022, max compression
+gzip compressed data, was "dist/biobb_pmx-4.0.0.tar", last modified: Fri Jul  7 10:54:14 2023, max compression
```

## Comparing `biobb_pmx-3.8.1.tar` & `biobb_pmx-4.0.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2022-09-15 13:49:55.000000 biobb_pmx-3.8.1/
--rw-r--r--   0 pau        (501) staff       (20)     4517 2022-09-15 13:49:55.000000 biobb_pmx-3.8.1/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     3069 2022-09-15 13:48:24.000000 biobb_pmx-3.8.1/README.md
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2022-09-15 13:49:55.000000 biobb_pmx-3.8.1/biobb_pmx/
--rw-r--r--   0 pau        (501) staff       (20)       59 2022-09-15 13:47:51.000000 biobb_pmx-3.8.1/biobb_pmx/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2022-09-15 13:49:55.000000 biobb_pmx-3.8.1/biobb_pmx/pmx/
--rwxr-xr-x   0 pau        (501) staff       (20)      167 2022-09-15 08:59:19.000000 biobb_pmx-3.8.1/biobb_pmx/pmx/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)     2170 2021-10-26 11:38:29.000000 biobb_pmx-3.8.1/biobb_pmx/pmx/common.py
--rwxr-xr-x   0 pau        (501) staff       (20)    12984 2021-10-27 07:45:27.000000 biobb_pmx-3.8.1/biobb_pmx/pmx/pmxanalyse.py
--rwxr-xr-x   0 pau        (501) staff       (20)    17565 2022-09-15 09:08:26.000000 biobb_pmx-3.8.1/biobb_pmx/pmx/pmxatom_mapping.py
--rwxr-xr-x   0 pau        (501) staff       (20)     9667 2022-09-15 09:08:26.000000 biobb_pmx-3.8.1/biobb_pmx/pmx/pmxcreate_top.py
--rwxr-xr-x   0 pau        (501) staff       (20)    10431 2021-10-26 17:26:38.000000 biobb_pmx-3.8.1/biobb_pmx/pmx/pmxgentop.py
--rwxr-xr-x   0 pau        (501) staff       (20)    16114 2022-09-15 09:08:26.000000 biobb_pmx-3.8.1/biobb_pmx/pmx/pmxligand_hybrid.py
--rwxr-xr-x   0 pau        (501) staff       (20)     6627 2022-09-15 09:08:26.000000 biobb_pmx-3.8.1/biobb_pmx/pmx/pmxmerge_ff.py
--rwxr-xr-x   0 pau        (501) staff       (20)     9841 2021-10-26 17:26:38.000000 biobb_pmx-3.8.1/biobb_pmx/pmx/pmxmutate.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2022-09-15 13:49:55.000000 biobb_pmx-3.8.1/biobb_pmx/test/
--rwxr-xr-x   0 pau        (501) staff       (20)        0 2021-06-11 09:55:35.000000 biobb_pmx-3.8.1/biobb_pmx/test/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2022-09-15 13:49:55.000000 biobb_pmx-3.8.1/biobb_pmx.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     4517 2022-09-15 13:49:55.000000 biobb_pmx-3.8.1/biobb_pmx.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)      526 2022-09-15 13:49:55.000000 biobb_pmx-3.8.1/biobb_pmx.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2022-09-15 13:49:55.000000 biobb_pmx-3.8.1/biobb_pmx.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)      346 2022-09-15 13:49:55.000000 biobb_pmx-3.8.1/biobb_pmx.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)       20 2022-09-15 13:49:55.000000 biobb_pmx-3.8.1/biobb_pmx.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)       10 2022-09-15 13:49:55.000000 biobb_pmx-3.8.1/biobb_pmx.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)       38 2022-09-15 13:49:55.000000 biobb_pmx-3.8.1/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     1568 2022-09-15 13:47:24.000000 biobb_pmx-3.8.1/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-07 10:54:14.000000 biobb_pmx-4.0.0/
+-rwxr-xr-x   0 pau        (501) staff       (20)    11358 2021-06-11 09:55:35.000000 biobb_pmx-4.0.0/LICENSE
+-rw-r--r--   0 pau        (501) staff       (20)     4233 2023-07-07 10:54:14.000000 biobb_pmx-4.0.0/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     3224 2023-07-07 10:50:41.000000 biobb_pmx-4.0.0/README.md
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-07 10:54:14.000000 biobb_pmx-4.0.0/biobb_pmx/
+-rw-r--r--   0 pau        (501) staff       (20)       64 2023-07-07 10:50:03.000000 biobb_pmx-4.0.0/biobb_pmx/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-07 10:54:14.000000 biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/
+-rwxr-xr-x   0 pau        (501) staff       (20)      140 2023-06-30 14:28:12.000000 biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)     2170 2021-10-26 11:38:29.000000 biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/common.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    13168 2023-06-30 14:17:30.000000 biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/pmxanalyse.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    18149 2023-06-30 14:17:30.000000 biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/pmxatom_mapping.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     9994 2023-06-30 14:17:30.000000 biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/pmxcreate_top.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    10654 2023-07-07 08:35:58.000000 biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/pmxgentop.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    16722 2023-06-30 14:17:30.000000 biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/pmxligand_hybrid.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     6993 2023-06-30 14:30:03.000000 biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/pmxmerge_ff.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    10031 2023-06-30 14:17:30.000000 biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/pmxmutate.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-07 10:54:14.000000 biobb_pmx-4.0.0/biobb_pmx/test/
+-rwxr-xr-x   0 pau        (501) staff       (20)        0 2021-06-11 09:55:35.000000 biobb_pmx-4.0.0/biobb_pmx/test/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-07-07 10:54:14.000000 biobb_pmx-4.0.0/biobb_pmx.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     4233 2023-07-07 10:54:14.000000 biobb_pmx-4.0.0/biobb_pmx.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)      579 2023-07-07 10:54:14.000000 biobb_pmx-4.0.0/biobb_pmx.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-07-07 10:54:14.000000 biobb_pmx-4.0.0/biobb_pmx.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)      381 2023-07-07 10:54:14.000000 biobb_pmx-4.0.0/biobb_pmx.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)       37 2023-07-07 10:54:14.000000 biobb_pmx-4.0.0/biobb_pmx.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-07-07 10:54:14.000000 biobb_pmx-4.0.0/biobb_pmx.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)       38 2023-07-07 10:54:14.000000 biobb_pmx-4.0.0/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     1825 2023-07-07 10:44:47.000000 biobb_pmx-4.0.0/setup.py
```

### Comparing `biobb_pmx-3.8.1/PKG-INFO` & `biobb_pmx-4.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,111 @@
 Metadata-Version: 2.1
 Name: biobb_pmx
-Version: 3.8.1
+Version: 4.0.0
 Summary: Biobb_pmx is the Biobb module collection to perform PMX (http://pmx.mpibpc.mpg.de) executions.
 Home-page: https://github.com/bioexcel/biobb_pmx
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 License: UNKNOWN
 Project-URL: Documentation, http://biobb_pmx.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
-Description: [![](https://readthedocs.org/projects/biobb-pmx/badge/?version=latest)](https://biobb-pmx.readthedocs.io/en/latest/?badge=latest)
-        [![](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](https://anaconda.org/bioconda/biobb_pmx)
-        [![](https://img.shields.io/badge/docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pmx)
-        [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-        
-        # biobb_pmx
-        
-        ### Introduction
-        Biobb_pmx is the Biobb module collection to perform PMX (http://pmx.mpibpc.mpg.de) executions.
-        Biobb (BioExcel building blocks) packages are Python building blocks that
-        create new layer of compatibility and interoperability over popular
-        bioinformatics tools.
-        The latest documentation of this package can be found in our readthedocs site:
-        [latest API documentation](http://biobb_pmx.readthedocs.io/en/latest/).
-        
-        ### Version
-        v3.8.1 2022.3
-        
-        ### Installation
-        Using PIP:
-        
-        > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
-        
-        * Installation:
-        
-                pip install "biobb_pmx>=3.8.1"
-        
-        
-        * Usage: [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html)
-        
-        Using ANACONDA:
-        
-        * Installation:
-        
-        
-                conda install -c bioconda "biobb_pmx>=3.8.1"
-        
-        
-        * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pmx.readthedocs.io/en/latest/command_line.html)
-        
-        Using DOCKER:
-        
-        * Installation:
-        
-        
-                docker pull quay.io/biocontainers/biobb_pmx:3.8.1--pyhdfd78af_0
-        
-        
-        * Usage:
-        
-        
-                docker run quay.io/biocontainers/biobb_pmx:3.8.1--pyhdfd78af_0 <command>
-        
-        
-        [//]: # (Using SINGULARITY:)
-        
-        [//]: # (**MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.)
-        
-        [//]: # (* Installation:)
-        
-        
-        [//]: # (singularity pull --name biobb_pmx.sif shub://bioexcel/biobb_pmx)
-        
-        
-        [//]: # (* Usage:)
-        
-        [//]: # (singularity exec biobb_pmx.sif <command>)
-        
-        
-        The command list and specification can be found at the [Command Line documentation](https://biobb-pmx.readthedocs.io/en/latest/command_line.html).
-        
-        
-        ### Copyright & Licensing
-        This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
-        
-        * (c) 2015-2021 [Barcelona Supercomputing Center](https://www.bsc.es/)
-        * (c) 2015-2021 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
-        
-        Licensed under the
-        [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
-        
-        ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
-        
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
-Requires-Python: >=3.7
+Classifier: Operating System :: Unix
+Requires-Python: >=3.7,<3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![](https://readthedocs.org/projects/biobb-pmx/badge/?version=latest)](https://biobb-pmx.readthedocs.io/en/latest/?badge=latest)
+[![](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](https://anaconda.org/bioconda/biobb_pmx)
+[![](https://img.shields.io/badge/docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pmx?tab=tags)
+[![](https://img.shields.io/badge/singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pmx:4.0.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+# biobb_pmx
+
+### Introduction
+Biobb_pmx is the Biobb module collection to perform PMX (http://pmx.mpibpc.mpg.de) executions.
+Biobb (BioExcel building blocks) packages are Python building blocks that
+create new layer of compatibility and interoperability over popular
+bioinformatics tools.
+The latest documentation of this package can be found in our readthedocs site:
+[latest API documentation](http://biobb_pmx.readthedocs.io/en/latest/).
+
+### Version
+v4.0.0 2023.2
+
+### Installation
+Using PIP:
+
+> **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
+
+* Installation:
+
+        pip install "biobb_pmx>=4.0.0"
+
+
+* Usage: [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html)
+
+Using ANACONDA:
+
+* Installation:
+
+
+        conda install -c bioconda "biobb_pmx>=4.0.0"
+
+
+* Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pmx.readthedocs.io/en/latest/command_line.html)
+
+Using DOCKER:
+
+* Installation:
+
+
+        docker pull quay.io/biocontainers/biobb_pmx:4.0.0--pyhdfd78af_0
+
+
+* Usage:
+
+
+        docker run quay.io/biocontainers/biobb_pmx:4.0.0--pyhdfd78af_0 <command>
+
+
+Using SINGULARITY:
+
+**MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
+
+* Installation:
+
+
+        singularity pull --name biobb_pmx.sif https://depot.galaxyproject.org/singularity/biobb_pmx:4.0.0--pyhdfd78af_0
+
+
+* Usage:
+
+
+        singularity exec biobb_pmx.sif <command>
+
+
+The command list and specification can be found at the [Command Line documentation](https://biobb-pmx.readthedocs.io/en/latest/command_line.html).
+
+
+### Copyright & Licensing
+This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
+
+* (c) 2015-2022 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2022[Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+
+Licensed under the
+[Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
+
+![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
+
+
```

### Comparing `biobb_pmx-3.8.1/README.md` & `biobb_pmx-4.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,84 @@
 [![](https://readthedocs.org/projects/biobb-pmx/badge/?version=latest)](https://biobb-pmx.readthedocs.io/en/latest/?badge=latest)
 [![](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](https://anaconda.org/bioconda/biobb_pmx)
-[![](https://img.shields.io/badge/docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pmx)
+[![](https://img.shields.io/badge/docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pmx?tab=tags)
+[![](https://img.shields.io/badge/singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pmx:4.0.0--pyhdfd78af_0)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 # biobb_pmx
 
 ### Introduction
 Biobb_pmx is the Biobb module collection to perform PMX (http://pmx.mpibpc.mpg.de) executions.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_pmx.readthedocs.io/en/latest/).
 
 ### Version
-v3.8.1 2022.3
+v4.0.0 2023.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
-        pip install "biobb_pmx>=3.8.1"
+        pip install "biobb_pmx>=4.0.0"
 
 
 * Usage: [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pmx>=3.8.1"
+        conda install -c bioconda "biobb_pmx>=4.0.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pmx.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pmx.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pmx:3.8.1--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_pmx:4.0.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pmx:3.8.1--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_pmx:4.0.0--pyhdfd78af_0 <command>
 
 
-[//]: # (Using SINGULARITY:)
+Using SINGULARITY:
 
-[//]: # (**MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.)
+**MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
+
+* Installation:
 
-[//]: # (* Installation:)
 
+        singularity pull --name biobb_pmx.sif https://depot.galaxyproject.org/singularity/biobb_pmx:4.0.0--pyhdfd78af_0
 
-[//]: # (singularity pull --name biobb_pmx.sif shub://bioexcel/biobb_pmx)
 
+* Usage:
 
-[//]: # (* Usage:)
 
-[//]: # (singularity exec biobb_pmx.sif <command>)
+        singularity exec biobb_pmx.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-pmx.readthedocs.io/en/latest/command_line.html).
 
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2021 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2021 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2022 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2022[Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_pmx-3.8.1/biobb_pmx/pmx/common.py` & `biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/common.py`

 * *Files identical despite different names*

### Comparing `biobb_pmx-3.8.1/biobb_pmx/pmx/pmxanalyse.py` & `biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/pmxanalyse.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from biobb_common.tools.file_utils import launchlogger
 
 
 class Pmxanalyse(BiobbObject):
     """
     | biobb_pmx Pmxanalyse
     | Wrapper class for the `PMX analyse <https://github.com/deGrootLab/pmx>`_ module.
-   
+
     Args:
         input_a_xvg_zip_path (str): Path the zip file containing the dgdl.xvg files of the A state. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/xvg_A.zip>`_. Accepted formats: zip (edam:format_3987).
         input_b_xvg_zip_path (str): Path the zip file containing the dgdl.xvg files of the B state. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/xvg_B.zip>`_. Accepted formats: zip (edam:format_3987).
         output_result_path (str): Path to the TXT results file. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/ref_result.txt>`_. Accepted formats: txt (edam:format_2330).
         output_work_plot_path (str): Path to the PNG plot results file. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/ref_plot.png>`_. Accepted formats: png (edam:format_3603).
         properties (dic):
             * **method** (*str*) - ("CGI BAR JARZ") Choose one or more estimators to use. Values: CGI (Crooks Gaussian Intersection), BAR (Bennet Acceptance Ratio), JARZ (Jarzynski's estimator).
@@ -33,34 +33,34 @@
             * **rand** (*int*) - (None) [0~1000|1] Take a random subset of trajectories. Default is None (do not take random subset).
             * **index** (*str*) - (None) Zero-based index of files to analyze (e.g. "0 10 20 50 60"). It keeps the dhdl.xvg files according to their position in the list, sorted according to the filenames.
             * **prec** (*int*) - (2) [0~100|1] The decimal precision of the screen/file output.
             * **units** (*str*) - ("kJ") The units of the output. Values: kJ (Kilojoules), kcal (Kilocalories), kT (the product of the Boltzmann constant k and the temperature).
             * **no_ks** (*bool*) - (False) Whether to do a Kolmogorov-Smirnov test to check whether the Gaussian assumption for CGI holds.
             * **nbins** (*int*) - (20) [0~1000|1] Number of histograms bins for the plot.
             * **dpi** (*int*) - (300) [72~2048|1] Resolution of the plot.
-            * **pmx_path** (*str*) - ("pmx") Path to the PMX command line interface.
+            * **binary_path** (*str*) - ("pmx") Path to the PMX command line interface.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
             * **container_path** (*str*) - (None)  Path to the binary executable of your container.
             * **container_image** (*str*) - ("gromacs/gromacs:latest") Container Image identifier.
             * **container_volume_path** (*str*) - ("/data") Path to an internal directory in the container.
             * **container_working_dir** (*str*) - (None) Path to the internal CWD in the container.
             * **container_user_id** (*str*) - (None) User number id to be mapped inside the container.
             * **container_shell_path** (*str*) - ("/bin/bash") Path to the binary executable of the container shell.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_pmx.pmx.pmxanalyse import pmxanalyse
-            prop = { 
-                'method': 'CGI BAR JARZ', 
-                'temperature': 298.15, 
-                'dpi': 600 
+            from biobb_pmx.pmxbiobb.pmxanalyse import pmxanalyse
+            prop = {
+                'method': 'CGI BAR JARZ',
+                'temperature': 298.15,
+                'dpi': 600
             }
-            pmxanalyse(input_a_xvg_zip_path='/path/to/myAStateFiles.zip', 
+            pmxanalyse(input_a_xvg_zip_path='/path/to/myAStateFiles.zip',
                        input_b_xvg_zip_path='/path/to/myBStateFiles.zip',
                        output_result_path='/path/to/newResults.txt',
                        output_work_plot_path='/path/to/newResults.png',
                        properties=prop)
 
     Info:
         * wrapped_software:
@@ -69,20 +69,21 @@
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_a_xvg_zip_path: str, input_b_xvg_zip_path: str, output_result_path: str, output_work_plot_path: str, 
-                properties: Mapping = None, **kwargs) -> None:
+    def __init__(self, input_a_xvg_zip_path: str, input_b_xvg_zip_path: str, output_result_path: str, output_work_plot_path: str,
+                 properties: Mapping = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
+        self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
             "in": {},
             "out": {"output_result_path": output_result_path, "output_work_plot_path": output_work_plot_path}
         }
         # Should not be copied inside container
@@ -103,35 +104,35 @@
         self.prec = properties.get('prec', 2)
         self.units = properties.get('units', "kJ")
         self.no_ks = properties.get('no_ks', False)
         self.nbins = properties.get('nbins', 20)
         self.dpi = properties.get('dpi', 300)
 
         # Properties common in all PMX BB
-        self.pmx_path = properties.get('pmx_path', 'pmx')
+        self.binary_path = properties.get('binary_path', 'pmx')
 
         # Check the properties
         self.check_properties(properties)
+        self.check_arguments()
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`Pmxanalyse <pmx.pmxanalyse.Pmxanalyse>` pmx.pmxanalyse.Pmxanalyse object."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Check if executable is exists
         if not self.container_path:
-            if not Path(self.pmx_path).is_file():
-                if not shutil.which(self.pmx_path):
+            if not Path(self.binary_path).is_file():
+                if not shutil.which(self.binary_path):
                     raise FileNotFoundError(
-                        'Executable %s not found. Check if it is installed in your system and correctly defined in the properties' % self.pmx_path)
-
-
+                        'Executable %s not found. Check if it is installed in your system and correctly defined in the properties' % self.binary_path)
 
         list_a_dir = fu.create_unique_dir()
         list_b_dir = fu.create_unique_dir()
         list_a = list(filter(lambda f: Path(f).exists() and Path(f).stat().st_size > 10, fu.unzip_list(self.input_a_xvg_zip_path, list_a_dir, self.out_log)))
         list_b = list(filter(lambda f: Path(f).exists() and Path(f).stat().st_size > 10, fu.unzip_list(self.input_b_xvg_zip_path, list_b_dir, self.out_log)))
         string_a = " ".join(list_a)
         string_b = " ".join(list_b)
@@ -140,15 +141,15 @@
         if self.container_path:
             shutil.copytree(list_a_dir, Path(self.stage_io_dict.get("unique_dir")).joinpath(Path(list_a_dir).name))
             shutil.copytree(list_b_dir, Path(self.stage_io_dict.get("unique_dir")).joinpath(Path(list_b_dir).name))
             container_volume = " " + self.container_volume_path + "/"
             string_a = self.container_volume_path + "/" + container_volume.join(list_a)
             string_b = self.container_volume_path + "/" + container_volume.join(list_b)
 
-        self.cmd = [self.pmx_path, 'analyse',
+        self.cmd = [self.binary_path, 'analyse',
                     '-fA', string_a,
                     '-fB', string_b,
                     '-o', self.stage_io_dict["out"]["output_result_path"],
                     '-w', self.stage_io_dict["out"]["output_work_plot_path"]]
 
         if self.method:
             self.cmd.append('-m')
@@ -197,24 +198,25 @@
 
         # Copy files to host
         self.copy_to_host()
 
         self.tmp_files.extend([self.stage_io_dict.get("unique_dir"), list_a_dir, list_b_dir])
         self.remove_tmp_files()
 
+        self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
 def pmxanalyse(input_a_xvg_zip_path: str, input_b_xvg_zip_path: str,
                output_result_path: str, output_work_plot_path: str,
                properties: dict = None, **kwargs) -> int:
     """Execute the :class:`Pmxanalyse <pmx.pmxanalyse.Pmxanalyse>` class and
     execute the :meth:`launch() <pmx.pmxanalyse.Pmxanalyse.launch> method."""
 
-    return Pmxanalyse(input_a_xvg_zip_path=input_a_xvg_zip_path, 
+    return Pmxanalyse(input_a_xvg_zip_path=input_a_xvg_zip_path,
                       input_b_xvg_zip_path=input_b_xvg_zip_path,
                       output_result_path=output_result_path,
                       output_work_plot_path=output_work_plot_path,
                       properties=properties).launch()
 
 
 def main():
```

### Comparing `biobb_pmx-3.8.1/biobb_pmx/pmx/pmxatom_mapping.py` & `biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/pmxatom_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 """Module containing the PMX atom_mapping class and the command line interface."""
 import os
+import sys
 from pathlib import Path
 import shutil
 import argparse
 from typing import Mapping
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
@@ -50,15 +51,15 @@
             * **container_working_dir** (*str*) - (None) Path to the internal CWD in the container.
             * **container_user_id** (*str*) - (None) User number id to be mapped inside the container.
             * **container_shell_path** (*str*) - ("/bin/bash") Path to the binary executable of the container shell.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_pmx.pmx.pmxatom_mapping import pmxatom_mapping
+            from biobb_pmx.pmxbiobb.pmxatom_mapping import pmxatom_mapping
             prop = {
                 'no-alignment' : True,
                 'distance': 0.05
             }
             pmxatom_mapping(input_structure1_path='/path/to/myStructure1.pdb',
                     input_structure2_path='/path/to/myStructure2.pdb',
                     output_pairs1_path='/path/to/myPairs1.dat',
@@ -74,31 +75,32 @@
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
     def __init__(self, input_structure1_path: str, input_structure2_path: str, output_pairs1_path: str, output_pairs2_path: str,
-     output_log_path: str, output_structure1_path: str = None, output_structure2_path: str = None, output_morph1_path: str = None, 
-     output_morph2_path: str = None, output_scaffold1_path: str = None, output_scaffold2_path: str = None, output_score_path: str = None,
-     properties: Mapping = None, **kwargs) -> None:
+                 output_log_path: str, output_structure1_path: str = None, output_structure2_path: str = None, output_morph1_path: str = None,
+                 output_morph2_path: str = None, output_scaffold1_path: str = None, output_scaffold2_path: str = None, output_score_path: str = None,
+                 properties: Mapping = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
+        self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
             "in": {"input_structure1_path": input_structure1_path, "input_structure2_path": input_structure2_path},
             "out": {"output_pairs1_path": output_pairs1_path, "output_pairs2_path": output_pairs2_path,
-             "output_log_path": output_log_path, 
-             "output_structure1_path": output_structure1_path, "output_structure2_path": output_structure2_path,
-             "output_morph1_path": output_morph1_path, "output_morph2_path": output_morph2_path,
-             "output_scaffold1_path": output_scaffold1_path, "output_scaffold2_path": output_scaffold2_path,
-             "output_score_path": output_score_path}
+                    "output_log_path": output_log_path,
+                    "output_structure1_path": output_structure1_path, "output_structure2_path": output_structure2_path,
+                    "output_morph1_path": output_morph1_path, "output_morph2_path": output_morph2_path,
+                    "output_scaffold1_path": output_scaffold1_path, "output_scaffold2_path": output_scaffold2_path,
+                    "output_score_path": output_score_path}
         }
 
         # Properties specific for BB
         # self.noalignment = properties.get('noalignment', False)
         # self.nomcs = properties.get('nomcs', False)
         # self.noH2H = properties.get('noH2H', True)
         # self.H2Hpolar = properties.get('H2Hpolar', False)
@@ -121,74 +123,77 @@
         self.nochirality = properties.get('nochirality')
         self.distance = properties.get('distance')
         self.timeout = properties.get('timeout')
 
         # Properties common in all PMX BB
         self.gmx_lib = properties.get('gmx_lib', None)
         if not self.gmx_lib and os.environ.get('CONDA_PREFIX'):
+            python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
             self.gmx_lib = str(
-                Path(os.environ.get('CONDA_PREFIX')).joinpath("lib/python3.7/site-packages/pmx/data/mutff45/"))
+                Path(os.environ.get('CONDA_PREFIX')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
             if properties.get('container_path'):
-                self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.7/site-packages/pmx/data/mutff45/"))
-        self.pmx_path = properties.get('pmx_path', 'pmx')
+                self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.7/site-packages/pmx/data/mutff/"))
+        self.binary_path = properties.get('binary_path', 'pmx')
 
         # Check the properties
         self.check_properties(properties)
+        self.check_arguments()
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`Pmxmutate <pmx.pmxmutate.Pmxmutate>` pmx.pmxmutate.Pmxmutate object."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Check if executable exists
         if not self.container_path:
-            if not Path(self.pmx_path).is_file():
-                if not shutil.which(self.pmx_path):
+            if not Path(self.binary_path).is_file():
+                if not shutil.which(self.binary_path):
                     raise FileNotFoundError(
-                        'Executable %s not found. Check if it is installed in your system and correctly defined in the properties' % self.pmx_path)
+                        'Executable %s not found. Check if it is installed in your system and correctly defined in the properties' % self.binary_path)
 
-        self.cmd = [self.pmx_path, 'atomMapping',
+        self.cmd = [self.binary_path, 'atomMapping',
                     '-i1', self.stage_io_dict["in"]["input_structure1_path"],
                     '-i2', self.stage_io_dict["in"]["input_structure2_path"],
                     '-o1', self.stage_io_dict["out"]["output_pairs1_path"],
                     '-o2', self.stage_io_dict["out"]["output_pairs2_path"],
                     '-log', self.stage_io_dict["out"]["output_log_path"]
-                    ]                    
+                    ]
 
         if self.stage_io_dict["out"].get("output_structure1_path"):
             self.cmd.append('-opdb1')
             self.cmd.append(self.stage_io_dict["out"]["output_structure1_path"])
-  
+
         if self.stage_io_dict["out"].get("output_structure2_path"):
             self.cmd.append('-opdb2')
             self.cmd.append(self.stage_io_dict["out"]["output_structure2_path"])
-  
+
         if self.stage_io_dict["out"].get("output_morph1_path"):
             self.cmd.append('-opdbm1')
             self.cmd.append(self.stage_io_dict["out"]["output_morph1_path"])
-  
+
         if self.stage_io_dict["out"].get("output_morph2_path"):
             self.cmd.append('-opdbm2')
             self.cmd.append(self.stage_io_dict["out"]["output_morph2_path"])
- 
+
         if self.stage_io_dict["out"].get("output_scaffold1_path"):
             self.cmd.append('-n1')
             self.cmd.append(self.stage_io_dict["out"]["output_scaffold1_path"])
-  
+
         if self.stage_io_dict["out"].get("output_scaffold2_path"):
             self.cmd.append('-n2')
             self.cmd.append(self.stage_io_dict["out"]["output_scaffold2_path"])
- 
+
         if self.stage_io_dict["out"].get("output_score_path"):
             self.cmd.append('-score')
             self.cmd.append(self.stage_io_dict["out"]["output_score_path"])
- 
+
         if self.noalignment:
             self.cmd.append('--no-alignment')
         if self.nomcs:
             self.cmd.append('--no-mcs')
         if self.noH2H:
             self.cmd.append('--no-H2H')
         if self.H2Hpolar:
@@ -206,41 +211,45 @@
         if self.distance:
             self.cmd.append('--d')
             self.cmd.append(str(self.distance))
         if self.timeout:
             self.cmd.append('--timeout')
             self.cmd.append(str(self.timeout))
 
+        if self.gmx_lib:
+            self.env_vars_dict['GMXLIB'] = self.gmx_lib
+
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         self.tmp_files.append(self.stage_io_dict.get("unique_dir"))
         self.remove_tmp_files()
 
+        self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
 def pmxatom_mapping(input_structure1_path: str, input_structure2_path: str, output_pairs1_path: str, output_pairs2_path: str,
-     output_log_path: str, output_structure1_path: str = None, output_structure2_path: str = None, output_morph1_path: str = None, 
-     output_morph2_path: str = None, output_scaffold1_path: str = None, output_scaffold2_path: str = None, output_score_path: str = None,
-     properties: dict = None, **kwargs) -> int:
+                    output_log_path: str, output_structure1_path: str = None, output_structure2_path: str = None, output_morph1_path: str = None,
+                    output_morph2_path: str = None, output_scaffold1_path: str = None, output_scaffold2_path: str = None, output_score_path: str = None,
+                    properties: dict = None, **kwargs) -> int:
     """Execute the :class:`Pmxatom_mapping <pmx.pmxmutate.Pmxatom_mapping>` class and
     execute the :meth:`launch() <pmx.pmxatom_mapping.Pmxatom_mapping.launch> method."""
 
     return Pmxatom_mapping(input_structure1_path=input_structure1_path, input_structure2_path=input_structure2_path,
-                     output_pairs1_path=output_pairs1_path, output_pairs2_path=output_pairs2_path,
-                     output_log_path=output_log_path,
-                     output_structure1_path=output_structure1_path, output_structure2_path=output_structure2_path,
-                     output_morph1_path=output_morph1_path, output_morph2_path=output_morph2_path,
-                     output_scaffold1_path=output_scaffold1_path, output_scaffold2_path=output_scaffold2_path,
-                     output_score_path=output_score_path,
-                     properties=properties, **kwargs).launch()
+                           output_pairs1_path=output_pairs1_path, output_pairs2_path=output_pairs2_path,
+                           output_log_path=output_log_path,
+                           output_structure1_path=output_structure1_path, output_structure2_path=output_structure2_path,
+                           output_morph1_path=output_morph1_path, output_morph2_path=output_morph2_path,
+                           output_scaffold1_path=output_scaffold1_path, output_scaffold2_path=output_scaffold2_path,
+                           output_score_path=output_score_path,
+                           properties=properties, **kwargs).launch()
 
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Run PMX atom mapping module",
                                      formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('-c', '--config', required=False, help="This file can be a YAML file, JSON file or JSON string")
@@ -262,17 +271,18 @@
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call of each building block
     pmxatom_mapping(input_structure1_path=args.input_structure1_path, input_structure2_path=args.input_structure2_path,
-              output_pairs1_path=args.output_pairs1_path, output_pairs2_path=args.output_pairs2_path,
-              output_log_path=output_log_path,
-              output_structure1_path=output_structure1_path, output_structure2_path=output_structure2_path,
-              output_morph1_path=output_morph1_path, output_morph2_path=output_morph2_path,
-              output_scaffold1_path=output_scaffold1_path, output_scaffold2_path=output_scaffold2_path,
-              output_score_path=output_score_path,
-              properties=properties)
+                    output_pairs1_path=args.output_pairs1_path, output_pairs2_path=args.output_pairs2_path,
+                    output_log_path=args.output_log_path,
+                    output_structure1_path=args.output_structure1_path, output_structure2_path=args.output_structure2_path,
+                    output_morph1_path=args.output_morph1_path, output_morph2_path=args.output_morph2_path,
+                    output_scaffold1_path=args.output_scaffold1_path, output_scaffold2_path=args.output_scaffold2_path,
+                    output_score_path=args.output_score_path,
+                    properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_pmx-3.8.1/biobb_pmx/pmx/pmxcreate_top.py` & `biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/pmxcreate_top.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 """Module containing the PMX create_top class and the command line interface."""
 import os
+import sys
 from pathlib import Path, PurePath
 import shutil
 import argparse
 from typing import Mapping
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
@@ -22,28 +23,28 @@
         input_topology2_path (str): Path to the input topology file 2. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/ligand.itp>`_. Accepted formats: itp (edam:format_3883).
         output_topology_path (str): Path to the complete ligand topology file. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/ligand_top.zip>`_. Accepted formats: zip (edam:format_3987).
 
         properties (dic):
             * **force_field** (*str*) - ("amber99sb-star-ildn-mut.ff") Force-field to be included in the generated topology.
             * **water** (*str*) - ("tip3p") Water model to be included in the generated topology.
             * **system_name** (*str*) - ("Pmx topology") System name to be included in the generated topology.
-            * **mols** (*list*) - ([['Protein',1],['Ligand',1]]) Molecules to be included in the generated topology. 
+            * **mols** (*list*) - ([['Protein',1],['Ligand',1]]) Molecules to be included in the generated topology.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
             * **container_path** (*str*) - (None)  Path to the binary executable of your container.
             * **container_image** (*str*) - (None) Container Image identifier.
             * **container_volume_path** (*str*) - ("/inout") Path to an internal directory in the container.
             * **container_working_dir** (*str*) - (None) Path to the internal CWD in the container.
             * **container_user_id** (*str*) - (None) User number id to be mapped inside the container.
             * **container_shell_path** (*str*) - ("/bin/bash") Path to the binary executable of the container shell.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_pmx.pmx.pmxcreate_top import pmxcreate_top
+            from biobb_pmx.pmxbiobb.pmxcreate_top import pmxcreate_top
             prop = {
                 'remove_tmp' : True
             }
             pmxcreate_top(input_topology1_path='/path/to/myTopology1.itp',
                     input_topology2_path='/path/to/myTopology2.itp',
                     output_topology_path='/path/to/myMergedTopology.zip',
                     properties=prop)
@@ -55,51 +56,55 @@
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_topology1_path: str, input_topology2_path: str, output_topology_path: str, 
-     properties: Mapping = None, **kwargs) -> None:
+    def __init__(self, input_topology1_path: str, input_topology2_path: str, output_topology_path: str,
+                 properties: Mapping = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
+        self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
             "in": {"input_topology1_path": input_topology1_path, "input_topology2_path": input_topology2_path},
             "out": {"output_topology_path": output_topology_path}
         }
 
         # Properties specific for BB
         self.force_field = properties.get('force_field', "amber99sb-star-ildn-mut.ff")
         self.water = properties.get('water', "tip3p")
         self.system_name = properties.get('system_name', "Pmx topology")
-        self.mols = properties.get('mols', [['Protein',1],['Ligand',1]])
+        self.mols = properties.get('mols', [['Protein', 1], ['Ligand', 1]])
 
         # Properties common in all PMX BB
         self.gmx_lib = properties.get('gmx_lib', None)
         if not self.gmx_lib and os.environ.get('CONDA_PREFIX'):
+            python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
             self.gmx_lib = str(
-                Path(os.environ.get('CONDA_PREFIX')).joinpath("lib/python3.7/site-packages/pmx/data/mutff45/"))
+                Path(os.environ.get('CONDA_PREFIX')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
             if properties.get('container_path'):
-                self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.7/site-packages/pmx/data/mutff45/"))
-        self.pmx_path = properties.get('pmx_path', 'pmx')
+                self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.7/site-packages/pmx/data/mutff/"))
+        self.binary_path = properties.get('binary_path', 'pmx')
 
         # Check the properties
         self.check_properties(properties)
+        self.check_arguments()
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`Pmxcreate_top <pmx.pmxcreate_top.Pmxcreate_top>` pmx.pmxcreate_top.Pmxcreate_top object."""
 #        os.chdir("/Users/hospital/BioBB/Notebooks_dev/biobb_wf_pmx_tutorial_ligands/biobb_wf_pmx_tutorial/notebooks")
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         self.out_log.info('Running create_top from pmx package...\n')
 
         # Creating temporary folder
         self.tmp_folder = fu.create_unique_dir()
         self.out_log.info('Creating %s temporary folder' % self.tmp_folder)
@@ -114,68 +119,69 @@
         itp2_local = str(PurePath(self.tmp_folder).joinpath(itp2))
         shutil.copyfile(self.io_dict['in']['input_topology2_path'], itp2_local)
 
         top_local = str(PurePath(self.tmp_folder).joinpath("topology.top"))
 
         # _create_top function, taken from the pmx AZ tutorial:
         # https://github.com/deGrootLab/pmx/blob/develop/tutorials/AZtutorial.py
-        fp = open(top_local,'w')
+        fp = open(top_local, 'w')
         # BioBB signature
         fp.write("; Topology generated by the BioBB pmxcreate_top building block\n\n")
         # ff itp
         fp.write('#include "%s/forcefield.itp"\n\n' % self.force_field)
         # additional itp
-        #for i in self.itps:
-        #    fp.write('#include "%s"\n' % i) 
+        # for i in self.itps:
+        #    fp.write('#include "%s"\n' % i)
         fp.write('#include "%s"\n' % itp)
         fp.write('#include "%s"\n\n' % itp2)
         # water itp
-        fp.write('#include "%s/%s.itp"\n' % (self.force_field,self.water)) 
+        fp.write('#include "%s/%s.itp"\n' % (self.force_field, self.water))
         # ions
         fp.write('#include "%s/ions.itp"\n\n' % self.force_field)
         # system
         fp.write('[ system ]\n')
         fp.write('{0}\n\n'.format(self.system_name))
         # molecules
         fp.write('[ molecules ]\n')
         for mol in self.mols:
-            fp.write('%s %s\n' %(mol[0],mol[1]))
+            fp.write('%s %s\n' % (mol[0], mol[1]))
         fp.close()
 
         # zip topology
         current_cwd = os.getcwd()
         top_final = str(PurePath(current_cwd).joinpath(self.io_dict["out"]["output_topology_path"]))
 
         os.chdir(self.tmp_folder)
         fu.log('Compressing topology to: %s' % top_final, self.out_log, self.global_log)
         fu.zip_top(zip_file=top_final, top_file="topology.top", out_log=self.out_log)
         os.chdir(current_cwd)
 
         self.out_log.info('Exit code 0\n')
 
         # Run Biobb block
-        #self.run_biobb()
+        # self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         self.tmp_files.append(self.stage_io_dict.get("unique_dir"))
         self.remove_tmp_files()
 
+        self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
-def pmxcreate_top(input_topology1_path: str, input_topology2_path: str, output_topology_path: str, 
-     properties: dict = None, **kwargs) -> int:
+def pmxcreate_top(input_topology1_path: str, input_topology2_path: str, output_topology_path: str,
+                  properties: dict = None, **kwargs) -> int:
     """Execute the :class:`Pmxcreate_top <pmx.pmxcreate_top.Pmxcreate_top>` class and
     execute the :meth:`launch() <pmx.pmxmcreate_top.Pmxmcreate_top.launch> method."""
 
     return Pmxcreate_top(input_topology1_path=input_topology1_path, input_topology2_path=input_topology2_path,
-                     output_topology_path=output_topology_path, 
-                     properties=properties, **kwargs).launch()
+                         output_topology_path=output_topology_path,
+                         properties=properties, **kwargs).launch()
 
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Run PMX create_top module",
                                      formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('-c', '--config', required=False, help="This file can be a YAML file, JSON file or JSON string")
@@ -188,12 +194,13 @@
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call of each building block
     pmxcreate_top(input_topology1_path=args.input_topology1_path, input_topology2_path=args.input_topology2_path,
-              output_topology_path=args.output_topology_path, 
-              properties=properties)
+                  output_topology_path=args.output_topology_path,
+                  properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_pmx-3.8.1/biobb_pmx/pmx/pmxgentop.py` & `biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/pmxgentop.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,157 +1,161 @@
 #!/usr/bin/env python3
 
 """Module containing the PMX gentop class and the command line interface."""
 import os
+import sys
 import argparse
 import shutil
 from pathlib import Path
 from typing import Mapping
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_common.command_wrapper import cmd_wrapper
 
 
 class Pmxgentop(BiobbObject):
     """
     | biobb_pmx Pmxgentop
     | Wrapper class for the `PMX gentop <https://github.com/deGrootLab/pmx>`_ module.
 
     Args:
         input_top_zip_path (str): Path the input GROMACS topology TOP and ITP files in zip format. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/topology.zip>`_. Accepted formats: zip (edam:format_3987).
         output_top_zip_path (str): Path the output TOP topology in zip format. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/ref_output_topology.zip>`_. Accepted formats: zip (edam:format_3987).
         properties (dic):
             * **force_field** (*str*) - ("amber99sb-star-ildn-mut") Force field to use. If **input_top_zip_path** is a top file, it's not necessary to specify the forcefield, as it will be determined automatically. If **input_top_zip_path** is an itp file, then it's needed.
             * **split** (*bool*) - (False) Write separate topologies for the vdW and charge transformations.
             * **scale_mass** (*bool*) - (False) Scale the masses of morphing atoms so that dummies have a mass of 1.
-            * **gmx_lib** (*str*) - ("$CONDA_PREFIX/lib/python3.7/site-packages/pmx/data/mutff45/") Path to the GMXLIB folder in your computer.
-            * **pmx_path** (*str*) - ("pmx") Path to the PMX command line interface.
+            * **gmx_lib** (*str*) - ("$CONDA_PREFIX/lib/python3.7/site-packages/pmx/data/mutff/") Path to the GMXLIB folder in your computer.
+            * **binary_path** (*str*) - ("pmx") Path to the PMX command line interface.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
             * **container_path** (*str*) - (None)  Path to the binary executable of your container.
             * **container_image** (*str*) - ("gromacs/gromacs:latest") Container Image identifier.
             * **container_volume_path** (*str*) - ("/inout") Path to an internal directory in the container.
             * **container_working_dir** (*str*) - (None) Path to the internal CWD in the container.
             * **container_user_id** (*str*) - (None) User number id to be mapped inside the container.
             * **container_shell_path** (*str*) - ("/bin/bash") Path to the binary executable of the container shell.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_pmx.pmx.pmxgentop import pmxgentop
-            prop = { 
+            from biobb_pmx.pmxbiobb.pmxgentop import pmxgentop
+            prop = {
                 'gmx_lib': '/path/to/myGMXLIB/',
-                'force_field': 'amber99sb-star-ildn-mut' 
+                'force_field': 'amber99sb-star-ildn-mut'
             }
-            pmxgentop(input_top_zip_path='/path/to/myTopology.zip', 
-                    output_top_zip_path='/path/to/newTopology.zip', 
+            pmxgentop(input_top_zip_path='/path/to/myTopology.zip',
+                    output_top_zip_path='/path/to/newTopology.zip',
                     properties=prop)
 
     Info:
         * wrapped_software:
             * name: PMX gentop
             * version: >=1.0.1
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_top_zip_path: str, output_top_zip_path: str, 
+    def __init__(self, input_top_zip_path: str, output_top_zip_path: str,
                  properties: Mapping = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
+        self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
             "in": {},
             "out": {"output_top_zip_path": output_top_zip_path}
         }
         # Should not be copied inside container
         self.input_top_zip_path = input_top_zip_path
 
         # Properties specific for BB
         self.force_field = properties.get('force_field', "amber99sb-star-ildn-mut")
         self.split = properties.get('split', False)
         self.scale_mass = properties.get('scale_mass', False)
 
-        # Properties common.py in all PMX BB
+        # Properties common in all PMX BB
         self.gmx_lib = properties.get('gmx_lib', None)
         if not self.gmx_lib and os.environ.get('CONDA_PREFIX'):
-            self.gmx_lib = str(Path(os.environ.get('CONDA_PREFIX')).joinpath("lib/python3.7/site-packages/pmx/data/mutff45/"))
+            python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
+            self.gmx_lib = str(
+                Path(os.environ.get('CONDA_PREFIX')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
             if properties.get('container_path'):
-                self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.7/site-packages/pmx/data/mutff45/"))
-        self.pmx_path = properties.get('pmx_path', 'pmx')
+                self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.8/site-packages/pmx/data/mutff/"))
+        self.binary_path = properties.get('binary_path', 'pmx')
 
         # Check the properties
         self.check_properties(properties)
+        self.check_arguments()
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`Pmxgentop <pmx.pmxgentop.Pmxgentop>` pmx.pmxgentop.Pmxgentop object."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Check if executable exists
         if not self.container_path:
-            if not Path(self.pmx_path).is_file():
-                if not shutil.which(self.pmx_path):
-                    raise FileNotFoundError('Executable %s not found. Check if it is installed in your system and correctly defined in the properties' % self.pmx_path)
+            if not Path(self.binary_path).is_file():
+                if not shutil.which(self.binary_path):
+                    raise FileNotFoundError('Executable %s not found. Check if it is installed in your system and correctly defined in the properties' % self.binary_path)
 
         # Unzip topology to topology_out
         top_file = fu.unzip_top(zip_file=self.input_top_zip_path, out_log=self.out_log)
         top_dir = str(Path(top_file).parent)
 
         # Copy extra files to container: topology folder
         if self.container_path:
             fu.log('Container execution enabled', self.out_log)
             fu.log(f"Unique dir: {self.stage_io_dict['unique_dir']}", self.out_log)
             fu.log(f"{self.stage_io_dict['unique_dir']} files: {os.listdir(self.stage_io_dict['unique_dir'])}", self.out_log)
-            fu.log(f"Copy all files of the unzipped original topology to unique dir:", self.out_log)
+            fu.log(f"Copy all files of the unzipped original topology to unique dir: {self.out_log}")
             shutil.copytree(top_dir, str(Path(self.stage_io_dict.get("unique_dir")).joinpath(Path(top_dir).name)))
             top_file = str(Path(self.container_volume_path).joinpath(Path(top_dir).name, Path(top_file).name))
 
         output_file_name = fu.create_name(prefix=self.prefix, step=self.step, name=str(Path(top_file).name))
         unique_dir_output_file = str(Path(fu.create_unique_dir()).joinpath(output_file_name))
         fu.log(f"unique_dir_output_file: {unique_dir_output_file}", self.out_log)
 
         if self.container_path:
             fu.log("Change references for container:", self.out_log)
             unique_dir_output_file = str(Path(self.container_volume_path).joinpath(Path(output_file_name)))
             fu.log(f"    unique_dir_output_file: {unique_dir_output_file}", self.out_log)
 
-        self.cmd = [self.pmx_path, 'gentop',
-               '-o', str(Path(unique_dir_output_file)),
-               '-ff', self.force_field,
-               '-p', top_file]
+        self.cmd = [self.binary_path, 'gentop',
+                    '-o', str(Path(unique_dir_output_file)),
+                    '-ff', self.force_field,
+                    '-p', top_file]
 
         if self.split:
             self.cmd.append('--split')
         if self.scale_mass:
             self.cmd.append('--scale_mass')
 
         if self.gmx_lib:
-            self.environment = os.environ.copy()
-            self.environment['GMXLIB'] = self.gmx_lib
+            self.env_vars_dict['GMXLIB'] = self.gmx_lib
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         if self.container_path:
-            unique_dir_output_file = str(Path(container_io_dict.get("unique_dir")).joinpath(Path(unique_dir_output_file).name))
+            unique_dir_output_file = str(Path(self.stage_io_dict.get("unique_dir")).joinpath(Path(unique_dir_output_file).name))
 
         # Remove paths from top file
         with open(Path(unique_dir_output_file)) as top_fh:
             top_lines = top_fh.readlines()
         with open(Path(unique_dir_output_file), 'w') as top_fh:
             for line in top_lines:
                 top_fh.write(line.replace(str(Path(unique_dir_output_file).parent)+'/', ''))
@@ -163,24 +167,25 @@
                 fu.log(f'Copying {str(orig_itp_file)} to: {str(Path(unique_dir_output_file).parent)}', self.out_log, self.global_log)
 
         # zip topology
         fu.log('Compressing topology to: %s' % self.io_dict["out"]["output_top_zip_path"], self.out_log, self.global_log)
         fu.zip_top(zip_file=self.io_dict["out"]["output_top_zip_path"], top_file=str(Path(unique_dir_output_file)), out_log=self.out_log)
 
         self.tmp_files.extend([self.stage_io_dict.get("unique_dir"), top_dir])
-        self.remove_tmp_files()
+        # self.remove_tmp_files()
 
+        self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
 def pmxgentop(input_top_zip_path: str, output_top_zip_path: str, properties: dict = None, **kwargs) -> int:
     """Execute the :class:`Pmxgentop <pmx.pmxgentop.Pmxgentop>` class and
     execute the :meth:`launch() <pmx.pmxgentop.Pmxgentop.launch> method."""
 
-    return Pmxgentop(input_top_zip_path=input_top_zip_path, 
+    return Pmxgentop(input_top_zip_path=input_top_zip_path,
                      output_top_zip_path=output_top_zip_path,
                      properties=properties, **kwargs).launch()
 
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Wrapper class for the PMX gentop module",
```

### Comparing `biobb_pmx-3.8.1/biobb_pmx/pmx/pmxligand_hybrid.py` & `biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/pmxligand_hybrid.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-#!/usr/bin/env python3
+# !/usr/bin/env python3
 
 """Module containing the PMX ligand_hybrid class and the command line interface."""
 import os
+import sys
 from pathlib import Path
 import shutil
 import argparse
 from typing import Mapping
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
@@ -25,15 +26,15 @@
         input_scaffold1_path (str) (Optional): Path to the index of atoms to consider for the ligand structure 1. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/atoms_to_consider.ndx>`_. Accepted formats: ndx (edam:format_2033).
         input_scaffold2_path (str) (Optional): Path to the index of atoms to consider for the ligand structure 2. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/atoms_to_consider.ndx>`_. Accepted formats: ndx (edam:format_2033).
         output_log_path (str): Path to the log file. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/atom_mapping.log>`_. Accepted formats: log (edam:format_2330), txt (edam:format_2330), out (edam:format_2330).
         output_structure1_path (str): Path to the output hybrid structure based on the ligand 1. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/superimposed_ligand.pdb>`_. Accepted formats: pdb (edam:format_1476).
         output_structure2_path (str): Path to the output hybrid structure based on the ligand 2. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/superimposed_ligand.pdb>`_. Accepted formats: pdb (edam:format_1476).
         output_topology_path (str): Path to the output hybrid topology. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/ligand_hybrid.itp>`_. Accepted formats: itp (edam:format_3883).
         output_atomtypes_path (str): Path to the atom types for the output hybrid topology. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/ligand_hybrid_atomtypes.itp>`_. Accepted formats: itp (edam:format_3883).
- 
+
         properties (dic):
             * **fit** (*bool*) - (False) Fit ligand structure 1 onto ligand structure 2 (Only used if input_pairs_path is provided).
             * **split** (*bool*) - (False) Split the topology into separate transitions.
             * **scDUMm** (*float*) - (1.0) Scale dummy masses using the counterpart atoms.
             * **scDUMa** (*float*) - (1.0) Scale bonded dummy angle parameters.
             * **scDUMd** (*float*) - (1.0) Scale bonded dummy dihedral parameters.
             * **deAng** (*bool*) - (False) Decouple angles composed of 1 dummy and 2 non-dummies.
@@ -46,15 +47,15 @@
             * **container_working_dir** (*str*) - (None) Path to the internal CWD in the container.
             * **container_user_id** (*str*) - (None) User number id to be mapped inside the container.
             * **container_shell_path** (*str*) - ("/bin/bash") Path to the binary executable of the container shell.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_pmx.pmx.pmxligand_hybrid import pmxligand_hybrid
+            from biobb_pmx.pmxbiobb.pmxligand_hybrid import pmxligand_hybrid
             prop = {
                 'fit' : True,
                 'distance': 0.05
             }
             pmxligand_hybrid(input_structure1_path='/path/to/myStructure1.pdb',
                     input_structure2_path='/path/to/myStructure2.pdb',
                     input_topology1_path='/path/to/myTopology1.pdb',
@@ -75,99 +76,103 @@
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
     def __init__(self, input_structure1_path: str, input_structure2_path: str, input_topology1_path: str, input_topology2_path: str,
-     output_log_path: str, output_structure1_path: str, output_structure2_path: str, output_topology_path: str, output_atomtypes_path: str,
-     input_scaffold1_path: str = None, input_scaffold2_path: str = None, input_pairs_path: str = None,
-     properties: Mapping = None, **kwargs) -> None:
+                 output_log_path: str, output_structure1_path: str, output_structure2_path: str, output_topology_path: str, output_atomtypes_path: str,
+                 input_scaffold1_path: str = None, input_scaffold2_path: str = None, input_pairs_path: str = None,
+                 properties: Mapping = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
+        self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
             "in": {"input_structure1_path": input_structure1_path, "input_structure2_path": input_structure2_path,
-             "input_topology1_path": input_topology1_path, "input_topology2_path": input_topology2_path,
-             "input_scaffold1_path": input_scaffold1_path, "input_scaffold2_path": input_scaffold2_path,
-             "input_pairs_path": input_pairs_path},
+                   "input_topology1_path": input_topology1_path, "input_topology2_path": input_topology2_path,
+                   "input_scaffold1_path": input_scaffold1_path, "input_scaffold2_path": input_scaffold2_path,
+                   "input_pairs_path": input_pairs_path},
             "out": {"output_structure1_path": output_structure1_path, "output_structure2_path": output_structure2_path,
-             "output_topology_path": output_topology_path, "output_atomtypes_path": output_atomtypes_path,
-             "output_log_path": output_log_path}
+                    "output_topology_path": output_topology_path, "output_atomtypes_path": output_atomtypes_path,
+                    "output_log_path": output_log_path}
         }
 
         # Properties specific for BB
-        #self.fit = properties.get('fit', False)
-        #self.split = properties.get('split', False)
-        #self.scDUMm = properties.get('scDUMm', 1.0)
-        #self.scDUMa = properties.get('scDUMa', 1.0)
-        #self.scDUMd = properties.get('scDUMd', 1.0)
-        #self.deAng = properties.get('deAng', False)
-        #self.distance = properties.get('distance', 0.05)
+        # self.fit = properties.get('fit', False)
+        # self.split = properties.get('split', False)
+        # self.scDUMm = properties.get('scDUMm', 1.0)
+        # self.scDUMa = properties.get('scDUMa', 1.0)
+        # self.scDUMd = properties.get('scDUMd', 1.0)
+        # self.deAng = properties.get('deAng', False)
+        # self.distance = properties.get('distance', 0.05)
 
         self.fit = properties.get('fit')
         self.split = properties.get('split')
         self.scDUMm = properties.get('scDUMm')
         self.scDUMa = properties.get('scDUMa')
         self.scDUMd = properties.get('scDUMd')
         self.deAng = properties.get('deAng')
         self.distance = properties.get('distance')
 
         # Properties common in all PMX BB
         self.gmx_lib = properties.get('gmx_lib', None)
         if not self.gmx_lib and os.environ.get('CONDA_PREFIX'):
+            python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
             self.gmx_lib = str(
-                Path(os.environ.get('CONDA_PREFIX')).joinpath("lib/python3.7/site-packages/pmx/data/mutff45/"))
+                Path(os.environ.get('CONDA_PREFIX')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
             if properties.get('container_path'):
-                self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.7/site-packages/pmx/data/mutff45/"))
-        self.pmx_path = properties.get('pmx_path', 'pmx')
+                self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.7/site-packages/pmx/data/mutff/"))
+        self.binary_path = properties.get('binary_path', 'pmx')
 
         # Check the properties
         self.check_properties(properties)
+        self.check_arguments()
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`Pmxmutate <pmx.pmxmutate.Pmxmutate>` pmx.pmxmutate.Pmxmutate object."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Check if executable exists
         if not self.container_path:
-            if not Path(self.pmx_path).is_file():
-                if not shutil.which(self.pmx_path):
+            if not Path(self.binary_path).is_file():
+                if not shutil.which(self.binary_path):
                     raise FileNotFoundError(
-                        'Executable %s not found. Check if it is installed in your system and correctly defined in the properties' % self.pmx_path)
+                        'Executable %s not found. Check if it is installed in your system and correctly defined in the properties' % self.binary_path)
 
-        self.cmd = [self.pmx_path, 'ligandHybrid',
+        self.cmd = [self.binary_path, 'ligandHybrid',
                     '-i1', self.stage_io_dict["in"]["input_structure1_path"],
                     '-i2', self.stage_io_dict["in"]["input_structure2_path"],
                     '-itp1', self.stage_io_dict["in"]["input_topology1_path"],
                     '-itp2', self.stage_io_dict["in"]["input_topology2_path"],
                     '-pairs', self.stage_io_dict["in"]["input_pairs_path"],
                     '-oA', self.stage_io_dict["out"]["output_structure1_path"],
                     '-oB', self.stage_io_dict["out"]["output_structure2_path"],
                     '-oitp', self.stage_io_dict["out"]["output_topology_path"],
                     '-offitp', self.stage_io_dict["out"]["output_atomtypes_path"],
                     '-log', self.stage_io_dict["out"]["output_log_path"]
-                    ]                    
+                    ]
 
         if self.stage_io_dict["in"].get("output_scaffold1_path"):
             self.cmd.append('-n1')
             self.cmd.append(self.stage_io_dict["in"]["output_scaffold1_path"])
-  
+
         if self.stage_io_dict["in"].get("output_scaffold2_path"):
             self.cmd.append('-n2')
             self.cmd.append(self.stage_io_dict["in"]["output_scaffold2_path"])
-  
+
         if self.fit:
             self.cmd.append('--fit')
         if self.split:
             self.cmd.append('--split')
         if self.deAng:
             self.cmd.append('--deAng')
         if self.distance:
@@ -179,41 +184,45 @@
         if self.scDUMa:
             self.cmd.append('--scDUMa')
             self.cmd.append(str(self.scDUMa))
         if self.scDUMd:
             self.cmd.append('--scDUMd')
             self.cmd.append(str(self.scDUMd))
 
+        if self.gmx_lib:
+            self.env_vars_dict['GMXLIB'] = self.gmx_lib
+
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         self.tmp_files.append(self.stage_io_dict.get("unique_dir"))
         self.remove_tmp_files()
 
+        self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
 def pmxligand_hybrid(input_structure1_path: str, input_structure2_path: str, input_topology1_path: str, input_topology2_path: str,
-     output_log_path: str, output_structure1_path: str, output_structure2_path: str, output_topology_path: str, output_atomtypes_path: str,
-     input_scaffold1_path: str = None, input_scaffold2_path: str = None, input_pairs_path: str = None,
-     properties: dict = None, **kwargs) -> int:
+                     output_log_path: str, output_structure1_path: str, output_structure2_path: str, output_topology_path: str, output_atomtypes_path: str,
+                     input_scaffold1_path: str = None, input_scaffold2_path: str = None, input_pairs_path: str = None,
+                     properties: dict = None, **kwargs) -> int:
     """Execute the :class:`Pmxligand_hybrid <pmx.pmxmutate.Pmxligand_hybrid>` class and
     execute the :meth:`launch() <pmx.pmxligand_hybrid.Pmxligand_hybrid.launch> method."""
 
     return Pmxligand_hybrid(input_structure1_path=input_structure1_path, input_structure2_path=input_structure2_path,
-                     input_topology1_path=input_topology1_path, input_topology2_path=input_topology2_path,
-                     output_log_path=output_log_path,
-                     output_structure1_path=output_structure1_path, output_structure2_path=output_structure2_path,
-                     output_topology_path=output_topology_path, output_atomtypes_path=output_atomtypes_path,
-                     input_scaffold1_path=input_scaffold1_path, input_scaffold2_path=input_scaffold2_path,
-                     input_pairs_path=input_pairs_path,
-                     properties=properties, **kwargs).launch()
+                            input_topology1_path=input_topology1_path, input_topology2_path=input_topology2_path,
+                            output_log_path=output_log_path,
+                            output_structure1_path=output_structure1_path, output_structure2_path=output_structure2_path,
+                            output_topology_path=output_topology_path, output_atomtypes_path=output_atomtypes_path,
+                            input_scaffold1_path=input_scaffold1_path, input_scaffold2_path=input_scaffold2_path,
+                            input_pairs_path=input_pairs_path,
+                            properties=properties, **kwargs).launch()
 
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Run PMX ligand hybrid module",
                                      formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('-c', '--config', required=False, help="This file can be a YAML file, JSON file or JSON string")
@@ -235,16 +244,17 @@
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call of each building block
     pmxligand_hybrid(input_structure1_path=args.input_structure1_path, input_structure2_path=args.input_structure2_path,
-              input_topology1_path=args.input_topology1_path, input_topology2_path=args.input_topology2_path,
-              input_scaffold1_path=input_scaffold1_path, input_scaffold2_path=input_scaffold2_path,
-              input_pairs_path=input_pairs_path, output_log_path=output_log_path,
-              output_structure1_path=output_structure1_path, output_structure2_path=output_structure2_path,
-              output_topology1_path=output_topology1_path, output_topology2_path=output_topology2_path,
-              properties=properties)
+                     input_topology1_path=args.input_topology1_path, input_topology2_path=args.input_topology2_path,
+                     input_scaffold1_path=args.input_scaffold1_path, input_scaffold2_path=args.input_scaffold2_path,
+                     input_pairs_path=args.input_pairs_path, output_log_path=args.output_log_path,
+                     output_structure1_path=args.output_structure1_path, output_structure2_path=args.output_structure2_path,
+                     output_topology1_path=args.output_topology1_path, output_topology2_path=args.output_topology2_path,
+                     properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_pmx-3.8.1/biobb_pmx/pmx/pmxmerge_ff.py` & `biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/pmxmerge_ff.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 
 """Module containing the PMX merge_ff class and the command line interface."""
 import os
+import sys
 from pathlib import Path
 import glob
 import argparse
-import pmx
+from pmx import ligand_alchemy
 from typing import Mapping
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 
 
@@ -31,15 +32,15 @@
             * **container_working_dir** (*str*) - (None) Path to the internal CWD in the container.
             * **container_user_id** (*str*) - (None) User number id to be mapped inside the container.
             * **container_shell_path** (*str*) - ("/bin/bash") Path to the binary executable of the container shell.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_pmx.pmx.pmxmerge_ff import pmxmerge_ff
+            from biobb_pmx.pmxbiobb.pmxmerge_ff import pmxmerge_ff
             prop = {
                 'remove_tmp' : True
             }
             pmxmerge_ff(input_topology_path='/path/to/myTopologies.zip',
                     output_topology_path='/path/to/myMergedTopology.itp',
                     properties=prop)
 
@@ -50,87 +51,92 @@
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_topology_path: str, output_topology_path: str, 
-     properties: Mapping = None, **kwargs) -> None:
+    def __init__(self, input_topology_path: str, output_topology_path: str, properties: Mapping = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
+        self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
             "in": {"input_topology_path": input_topology_path},
             "out": {"output_topology_path": output_topology_path}
         }
 
         # Properties specific for BB
         # None yet
 
         # Properties common in all PMX BB
         self.gmx_lib = properties.get('gmx_lib', None)
         if not self.gmx_lib and os.environ.get('CONDA_PREFIX'):
+            python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
             self.gmx_lib = str(
-                Path(os.environ.get('CONDA_PREFIX')).joinpath("lib/python3.7/site-packages/pmx/data/mutff45/"))
+                Path(os.environ.get('CONDA_PREFIX')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
             if properties.get('container_path'):
-                self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.7/site-packages/pmx/data/mutff45/"))
-        self.pmx_path = properties.get('pmx_path', 'pmx')
+                self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.7/site-packages/pmx/data/mutff/"))
+        self.binary_path = properties.get('binary_path', 'pmx')
 
         # Check the properties
         self.check_properties(properties)
+        self.check_arguments()
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`Pmxmerge_ff <pmx.pmxmerge_ff.Pmxmerge_ff>` pmx.pmxmerge_ff.Pmxmerge_ff object."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Creating temporary folder
         self.tmp_folder = fu.create_unique_dir()
         self.out_log.info('Creating %s temporary folder' % self.tmp_folder)
 
         fu.unzip_list(self.stage_io_dict["in"]["input_topology_path"], self.tmp_folder, out_log=self.out_log)
         files = glob.glob(self.tmp_folder+"/*.itp")
         ffsIn_list = []
         for itp in files:
             ffsIn_list.append(itp)
 
         self.out_log.info('Running merge_FF_files from pmx package...\n')
-        pmx.ligand_alchemy._merge_FF_files( self.stage_io_dict["out"]["output_topology_path"], 
-        ffsIn=ffsIn_list)
-        #ffsIn=[self.stage_io_dict["in"]["input_topology1_path"],self.stage_io_dict["in"]["input_topology2_path"]] )
+        ligand_alchemy._merge_FF_files(self.stage_io_dict["out"]["output_topology_path"], ffsIn=ffsIn_list)
+        # ffsIn=[self.stage_io_dict["in"]["input_topology1_path"],self.stage_io_dict["in"]["input_topology2_path"]] )
 
         self.out_log.info('Exit code 0\n')
 
+        if self.gmx_lib:
+            self.env_vars_dict['GMXLIB'] = self.gmx_lib
+
         # Run Biobb block
-        #self.run_biobb()
+        # self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         self.tmp_files.append(self.stage_io_dict.get("unique_dir"))
         self.remove_tmp_files()
 
+        self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
-def pmxmerge_ff(input_topology_path: str, output_topology_path: str, 
-     properties: dict = None, **kwargs) -> int:
+def pmxmerge_ff(input_topology_path: str, output_topology_path: str, properties: dict = None, **kwargs) -> int:
     """Execute the :class:`Pmxmerge_ff <pmx.pmxmerge_ff.Pmxmerge_ff>` class and
     execute the :meth:`launch() <pmx.pmxmerge_ff.Pmxmerge_ff.launch> method."""
 
-    return Pmxmerge_ff(input_topology_path=input_topology_path, 
-                     output_topology_path=output_topology_path, 
-                     properties=properties, **kwargs).launch()
+    return Pmxmerge_ff(input_topology_path=input_topology_path,
+                       output_topology_path=output_topology_path,
+                       properties=properties, **kwargs).launch()
 
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Run PMX merge_ff module",
                                      formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('-c', '--config', required=False, help="This file can be a YAML file, JSON file or JSON string")
@@ -141,13 +147,14 @@
     required_args.add_argument('--output_topology_path', required=True, help="Path to the merged ligand topology file")
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call of each building block
-    pmxmerge_ff(input_topology_path=args.input_topology_path, 
-              output_topology_path=args.output_topology_path, 
-              properties=properties)
+    pmxmerge_ff(input_topology_path=args.input_topology_path,
+                output_topology_path=args.output_topology_path,
+                properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_pmx-3.8.1/biobb_pmx/pmx/pmxmutate.py` & `biobb_pmx-4.0.0/biobb_pmx/pmxbiobb/pmxmutate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #!/usr/bin/env python3
 
 """Module containing the PMX mutate class and the command line interface."""
 import os
 from pathlib import Path
-import re
+import sys
 import shutil
 import argparse
 from typing import Mapping
-from biobb_pmx.pmx.common import create_mutations_file, MUTATION_DICT
+from biobb_pmx.pmxbiobb.common import create_mutations_file, MUTATION_DICT
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_common.command_wrapper import cmd_wrapper
 
 
 class Pmxmutate(BiobbObject):
     """
     | biobb_pmx Pmxmutate
     | Wrapper class for the `PMX mutate <https://github.com/deGrootLab/pmx>`_ module.
 
@@ -24,29 +23,29 @@
         input_structure_path (str): Path to the input structure file. File type: input. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/data/pmx/frame99.pdb>`_. Accepted formats: pdb (edam:format_1476), gro (edam:format_2033).
         output_structure_path (str): Path to the output structure file. File type: output. `Sample file <https://github.com/bioexcel/biobb_pmx/raw/master/biobb_pmx/test/reference/pmx/ref_output_structure.pdb>`_. Accepted formats: pdb (edam:format_1476), gro (edam:format_2033).
         input_b_structure_path (str) (Optional): Path to the mutated input structure file. File type: input. Accepted formats: pdb (edam:format_1476), gro (edam:format_2033).
         properties (dic):
             * **mutation_list** (*str*) - ("2Ala") Mutation list in the format "Chain:Resnum MUT_AA_Code" or "Chain:Resnum MUT_NA_Code"  (no spaces between the elements) separated by commas. If no chain is provided as chain code all the chains in the pdb file will be mutated. ie: "A:15CYS". Possible MUT_AA_Code: 'ALA', 'ARG', 'ASN', 'ASP', 'ASPH', 'ASPP', 'ASH', 'CYS', 'CYS2', 'CYN', 'CYX', 'CYM', 'CYSH', 'GLU', 'GLUH', 'GLUP', 'GLH', 'GLN', 'GLY', 'HIS', 'HIE', 'HISE', 'HSE', 'HIP', 'HSP', 'HISH', 'HID', 'HSD', 'ILE', 'LEU', 'LYS', 'LYSH', 'LYP', 'LYN', 'LSN', 'MET', 'PHE', 'PRO', 'SER', 'SP1', 'SP2', 'THR', 'TRP', 'TYR', 'VAL'. Possible MUT_NA_Codes: 'A', 'T', 'C', 'G', 'U'.
             * **force_field** (*str*) - ("amber99sb-star-ildn-mut") Forcefield to use.
             * **resinfo** (*bool*) - (False) Show the list of 3-letter -> 1-letter residues.
-            * **gmx_lib** (*str*) - ("$CONDA_PREFIX/lib/python3.7/site-packages/pmx/data/mutff45/") Path to the GMXLIB folder in your computer.
-            * **pmx_path** (*str*) - ("pmx") Path to the PMX command line interface.
+            * **gmx_lib** (*str*) - ("$CONDA_PREFIX/lib/python3.7/site-packages/pmx/data/mutff/") Path to the GMXLIB folder in your computer.
+            * **binary_path** (*str*) - ("pmx") Path to the PMX command line interface.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
             * **container_path** (*str*) - (None)  Path to the binary executable of your container.
             * **container_image** (*str*) - (None) Container Image identifier.
             * **container_volume_path** (*str*) - ("/inout") Path to an internal directory in the container.
             * **container_working_dir** (*str*) - (None) Path to the internal CWD in the container.
             * **container_user_id** (*str*) - (None) User number id to be mapped inside the container.
             * **container_shell_path** (*str*) - ("/bin/bash") Path to the binary executable of the container shell.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_pmx.pmx.pmxmutate import pmxmutate
+            from biobb_pmx.pmxbiobb.pmxmutate import pmxmutate
             prop = {
                 'mutation_list': '2Ala, 3Val',
                 'gmx_lib': '/path/to/myGMXLIB/',
                 'force_field': 'amber99sb-star-ildn-mut'
             }
             pmxmutate(input_structure_path='/path/to/myStructure.pdb',
                     output_structure_path='/path/to/newStructure.pdb',
@@ -66,54 +65,57 @@
 
     def __init__(self, input_structure_path: str, output_structure_path: str, input_b_structure_path: str = None,
                  properties: Mapping = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
+        self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
             "in": {"input_structure_path": input_structure_path, "input_b_structure_path": input_b_structure_path},
             "out": {"output_structure_path": output_structure_path}
         }
 
         # Properties specific for BB
         self.force_field = properties.get('force_field', "amber99sb-star-ildn-mut")
         self.resinfo = properties.get('resinfo', False)
         self.mutation_list = properties.get('mutation_list', '2Ala')
         self.input_mutations_file = properties.get('mutations_file')
 
-
         # Properties common in all PMX BB
         self.gmx_lib = properties.get('gmx_lib', None)
         if not self.gmx_lib and os.environ.get('CONDA_PREFIX'):
+            python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
             self.gmx_lib = str(
-                Path(os.environ.get('CONDA_PREFIX')).joinpath("lib/python3.7/site-packages/pmx/data/mutff45/"))
+                Path(os.environ.get('CONDA_PREFIX')).joinpath(f"lib/python{python_version}/site-packages/pmx/data/mutff/"))
             if properties.get('container_path'):
-                self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.7/site-packages/pmx/data/mutff45/"))
-        self.pmx_path = properties.get('pmx_path', 'pmx')
+                self.gmx_lib = str(Path('/usr/local/').joinpath("lib/python3.7/site-packages/pmx/data/mutff/"))
+        self.binary_path = properties.get('binary_path', 'pmx')
 
         # Check the properties
         self.check_properties(properties)
+        self.check_arguments()
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`Pmxmutate <pmx.pmxmutate.Pmxmutate>` pmx.pmxmutate.Pmxmutate object."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Check if executable exists
         if not self.container_path:
-            if not Path(self.pmx_path).is_file():
-                if not shutil.which(self.pmx_path):
+            if not Path(self.binary_path).is_file():
+                if not shutil.which(self.binary_path):
                     raise FileNotFoundError(
-                        'Executable %s not found. Check if it is installed in your system and correctly defined in the properties' % self.pmx_path)
+                        'Executable %s not found. Check if it is installed in your system and correctly defined in the properties' % self.binary_path)
 
         # Generate mutations file
 
         mutations_dir = fu.create_unique_dir()
         self.input_mutations_file = create_mutations_file(input_mutations_path=str(Path(mutations_dir).joinpath('mutations.txt')),
                                                           mutation_list=self.mutation_list,
                                                           mutation_dict=MUTATION_DICT)
@@ -121,39 +123,39 @@
         # Copy extra files to container: mutations file
         if self.container_path:
             fu.log('Container execution enabled', self.out_log)
 
             shutil.copy2(self.input_mutations_file, self.stage_io_dict.get("unique_dir"))
             self.input_mutations_file = str(Path(self.container_volume_path).joinpath(Path(self.input_mutations_file).name))
 
-        self.cmd = [self.pmx_path, 'mutate',
+        self.cmd = [self.binary_path, 'mutate',
                     '-f', self.stage_io_dict["in"]["input_structure_path"],
                     '-o', self.stage_io_dict["out"]["output_structure_path"],
                     '-ff', self.force_field,
                     '--script', self.input_mutations_file]
 
         if self.stage_io_dict["in"].get("input_b_structure_path"):
             self.cmd.append('-fB')
             self.cmd.append(self.stage_io_dict["in"]["input_b_structure_path"])
         if self.resinfo:
             self.cmd.append('-resinfo')
 
         if self.gmx_lib:
-            self.environment = os.environ.copy()
-            self.environment['GMXLIB'] = self.gmx_lib
+            self.env_vars_dict['GMXLIB'] = self.gmx_lib
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         self.tmp_files.append(self.stage_io_dict.get("unique_dir"))
         self.remove_tmp_files()
 
+        self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
 def pmxmutate(input_structure_path: str, output_structure_path: str,
               input_b_structure_path: str = None, properties: dict = None,
               **kwargs) -> int:
     """Execute the :class:`Pmxmutate <pmx.pmxmutate.Pmxmutate>` class and
```

### Comparing `biobb_pmx-3.8.1/setup.py` & `biobb_pmx-4.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_pmx",
-    version="3.8.1",
+    version="4.0.0",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="Biobb_pmx is the Biobb module collection to perform PMX (http://pmx.mpibpc.mpg.de) executions.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_pmx",
     project_urls={
         "Documentation": "http://biobb_pmx.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs']),
-    install_requires=['biobb_common==3.8.1'],
-    python_requires='>=3.7',
+    install_requires=['biobb_common==4.0.0', 'pmx-biobb==4.1.3'],
+    python_requires='>=3.7,<3.11',
     entry_points={
         "console_scripts": [
-            "pmxanalyse = biobb_pmx.pmx.pmxanalyse:main",
-            "pmxgentop = biobb_pmx.pmx.pmxgentop:main",
-            "pmxmutate = biobb_pmx.pmx.pmxmutate:main",
-            "pmxatom_mapping = biobb_pmx.pmx.pmxatom_mapping:main",
-            "pmxcreate_top = biobb_pmx.pmx.pmxcreate_top:main",
-            "pmxligand_hybrid = biobb_pmx.pmx.pmxligand_hybrid:main",
-            "pmxmerge_ff = biobb_pmx.pmx.pmxmerge_ff:main"
+            "pmxanalyse = biobb_pmx.pmxbiobb.pmxanalyse:main",
+            "pmxgentop = biobb_pmx.pmxbiobb.pmxgentop:main",
+            "pmxmutate = biobb_pmx.pmxbiobb.pmxmutate:main",
+            "pmxatom_mapping = biobb_pmx.pmxbiobb.pmxatom_mapping:main",
+            "pmxcreate_top = biobb_pmx.pmxbiobb.pmxcreate_top:main",
+            "pmxligand_hybrid = biobb_pmx.pmxbiobb.pmxligand_hybrid:main",
+            "pmxmerge_ff = biobb_pmx.pmxbiobb.pmxmerge_ff:main"
         ]
     },
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: MacOS :: MacOS X",
-        "Operating System :: POSIX"
+        "Operating System :: POSIX",
+        "Operating System :: Unix"
     ],
 )
```


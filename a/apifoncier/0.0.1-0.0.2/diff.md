# Comparing `tmp/apifoncier-0.0.1.tar.gz` & `tmp/apifoncier-0.0.2.tar.gz`

## Comparing `apifoncier-0.0.1.tar` & `apifoncier-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apifoncier-0.0.1/src/__init__.py
--rw-r--r--   0        0        0    11958 2020-02-02 00:00:00.000000 apifoncier-0.0.1/src/apifoncier.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 apifoncier-0.0.1/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 apifoncier-0.0.1/LICENSE
--rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 apifoncier-0.0.1/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 apifoncier-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    10362 2020-02-02 00:00:00.000000 apifoncier-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 apifoncier-0.0.2/.pypirc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apifoncier-0.0.2/src/__init__.py
+-rw-r--r--   0        0        0    11958 2020-02-02 00:00:00.000000 apifoncier-0.0.2/src/apifoncier.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 apifoncier-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 apifoncier-0.0.2/LICENSE
+-rw-r--r--   0        0        0    10042 2020-02-02 00:00:00.000000 apifoncier-0.0.2/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 apifoncier-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10367 2020-02-02 00:00:00.000000 apifoncier-0.0.2/PKG-INFO
```

### Comparing `apifoncier-0.0.1/src/apifoncier.py` & `apifoncier-0.0.2/src/apifoncier.py`

 * *Files identical despite different names*

### Comparing `apifoncier-0.0.1/LICENSE` & `apifoncier-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apifoncier-0.0.1/README.md` & `apifoncier-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 > [Changements](https://rcadot.github.io/r.apifoncier/news/index.html)
 > pour plus d’informations.
 
 # Présentation du package
 
 Grâce au package `{r.apifoncier}`, vous pouvez interroger les
 différentes bases de données foncières produites par le Cerema et la
-DGALN directement depuis `R` ! *Une partie des données est interrogeable
+DGALN directement depuis `python` ! *Une partie des données est interrogeable
 uniquement avec un accès restreint lié à vos droits. Pensez à vous
 rendre sur
 [ConsultDF](https://consultdf.cerema.fr/consultdf/services/apidf) pour
 obtenir un accès.*
 
 # Installation
```

### Comparing `apifoncier-0.0.1/pyproject.toml` & `apifoncier-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling","pandas","requests","plotly.express"]
 build-backend = "hatchling.build"
 
 [project]
 name = "apifoncier"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Romain Cadot", email="romain.cadot@cerema.fr" },
 ]
 description = "Mobiliser les données foncières de l'api du Cerema directement avec python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `apifoncier-0.0.1/PKG-INFO` & `apifoncier-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apifoncier
-Version: 0.0.1
+Version: 0.0.2
 Summary: Mobiliser les données foncières de l'api du Cerema directement avec python
 Project-URL: Homepage, https://github.com/rcadot/py.apifoncier
 Project-URL: Bug Tracker, https://github.com/rcadot/py.apifoncier/issues
 Author-email: Romain Cadot <romain.cadot@cerema.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,15 +26,15 @@
 > [Changements](https://rcadot.github.io/r.apifoncier/news/index.html)
 > pour plus d’informations.
 
 # Présentation du package
 
 Grâce au package `{r.apifoncier}`, vous pouvez interroger les
 différentes bases de données foncières produites par le Cerema et la
-DGALN directement depuis `R` ! *Une partie des données est interrogeable
+DGALN directement depuis `python` ! *Une partie des données est interrogeable
 uniquement avec un accès restreint lié à vos droits. Pensez à vous
 rendre sur
 [ConsultDF](https://consultdf.cerema.fr/consultdf/services/apidf) pour
 obtenir un accès.*
 
 # Installation
```


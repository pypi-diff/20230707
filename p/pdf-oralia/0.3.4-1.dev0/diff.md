# Comparing `tmp/pdf_oralia-0.3.4.tar.gz` & `tmp/pdf_oralia-1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdf_oralia-0.3.4.tar", max compression
+gzip compressed data, was "pdf_oralia-1.dev0.tar", max compression
```

## Comparing `pdf_oralia-0.3.4.tar` & `pdf_oralia-1.dev0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       73 2023-07-07 19:25:36.792329 pdf_oralia-0.3.4/README.md
--rw-r--r--   0        0        0        0 2023-07-07 19:25:36.792329 pdf_oralia-0.3.4/pdf_oralia/__init__.py
--rw-r--r--   0        0        0     3056 2023-07-07 19:25:36.792329 pdf_oralia-0.3.4/pdf_oralia/extract.py
--rw-r--r--   0        0        0       59 2023-07-07 19:25:36.792329 pdf_oralia-0.3.4/pdf_oralia/pages/__init__.py
--rw-r--r--   0        0        0     2231 2023-07-07 19:25:36.792329 pdf_oralia-0.3.4/pdf_oralia/pages/charge.py
--rw-r--r--   0        0        0     4374 2023-07-07 19:25:36.792329 pdf_oralia-0.3.4/pdf_oralia/pages/locataire.py
--rw-r--r--   0        0        0       99 2023-07-07 19:25:36.792329 pdf_oralia-0.3.4/pdf_oralia/pages/patrimoine.py
--rw-r--r--   0        0        0      904 2023-07-07 19:25:36.792329 pdf_oralia-0.3.4/pdf_oralia/pages/recapitulatif.py
--rw-r--r--   0        0        0     1542 2023-07-07 19:25:36.792329 pdf_oralia-0.3.4/pdf_oralia/scripts.py
--rw-r--r--   0        0        0      563 2023-07-07 19:25:40.772110 pdf_oralia-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      589 1970-01-01 00:00:00.000000 pdf_oralia-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       73 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/pdf_oralia/__init__.py
+-rw-r--r--   0        0        0     3056 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/pdf_oralia/extract.py
+-rw-r--r--   0        0        0       59 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/pdf_oralia/pages/__init__.py
+-rw-r--r--   0        0        0     2206 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/pdf_oralia/pages/charge.py
+-rw-r--r--   0        0        0     4206 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/pdf_oralia/pages/locataire.py
+-rw-r--r--   0        0        0       99 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/pdf_oralia/pages/patrimoine.py
+-rw-r--r--   0        0        0      904 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/pdf_oralia/pages/recapitulatif.py
+-rw-r--r--   0        0        0     1542 2023-06-30 11:31:15.919082 pdf_oralia-1.dev0/pdf_oralia/scripts.py
+-rw-r--r--   0        0        0      562 2023-06-30 11:31:19.790868 pdf_oralia-1.dev0/pyproject.toml
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 pdf_oralia-1.dev0/PKG-INFO
```

### Comparing `pdf_oralia-0.3.4/pdf_oralia/extract.py` & `pdf_oralia-1.dev0/pdf_oralia/extract.py`

 * *Files identical despite different names*

### Comparing `pdf_oralia-0.3.4/pdf_oralia/pages/charge.py` & `pdf_oralia-1.dev0/pdf_oralia/pages/charge.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     "Locatif": float,
     "Déductible": float,
     "immeuble": str,
     "mois": str,
     "annee": str,
     "lot": str,
 }
-DEFAULT_FOURNISSEUR = "ROSIER MODICA MOTTEROZ SA"
 
 
 def is_it(page_text):
     if (
         "RECAPITULATIF DES OPERATIONS" in page_text
         and "COMPTE RENDU DE GESTION" not in page_text
     ):
@@ -59,16 +58,16 @@
                     r["Fournisseur"] = value
                 else:
                     r[header[i]] = value
 
             for k, v in additionnal_fields.items():
                 r[k] = v
 
-            if "honoraire" in row[RECAPITULATIF_DES_OPERATIONS].lower():
-                r["Fournisseur"] = DEFAULT_FOURNISSEUR
+            if "honoraire" in row[RECAPITULATIF_DES_OPERATIONS]:
+                r["Fournisseur"] = "IMI GERANCE"
 
             extracted.append(r)
 
     return extracted
 
 
 def table2df(tables):
@@ -80,9 +79,10 @@
             .dropna(subset=["Débits", "Crédits"], how="all")
         )
         df["Fournisseur"] = df["Fournisseur"].fillna(method="ffill")
         dfs.append(df)
     df = pd.concat(dfs)
 
     df["immeuble"] = df["immeuble"].apply(lambda x: x[0].capitalize())
+    print(df.columns)
     df["lot"] = df["RECAPITULATIF DES OPERATIONS"].apply(get_lot)
-    return df.astype(DF_TYPES)
+    return df.astype(DF_TYPES, errors="ignore")
```

### Comparing `pdf_oralia-0.3.4/pdf_oralia/pages/locataire.py` & `pdf_oralia-1.dev0/pdf_oralia/pages/locataire.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import numpy as np
 import pandas as pd
 
 DF_TYPES = {
     "Locataires": str,
     "Période": str,
     "Loyers": float,
     "Taxes": float,
@@ -30,15 +29,15 @@
         return True
     if not any(row):
         return True
     return False
 
 
 def extract(table, additionnal_fields: dict = {}):
-    """Turn table to dictionary with additional fields"""
+    """Turn table to dictionary with additionnal fields"""
     extracted = []
     header = table[0]
     for row in table[1:]:
         if not is_drop(row):
             r = dict()
             for i, value in enumerate(row):
                 if header[i] != "":
@@ -135,14 +134,16 @@
                     {
                         "Lot": last_row["Lot"],
                         "Type": last_row["Type"],
                         "Locataires": last_row["Locataires"],
                     }
                 )
                 joined.append(row)
+            else:
+                pass
 
     return joined
 
 
 def flat_tables(tables):
     tables_flat = []
     for table in tables:
@@ -154,13 +155,8 @@
     tables = flat_tables(tables)
     joined = join_row(tables)
     df = pd.DataFrame.from_records(joined)
 
     df["immeuble"] = df["immeuble"].apply(lambda x: x[0].capitalize())
     df["Type"] = df["Type"].apply(clean_type)
 
-    numeric_cols = [k for k, v in DF_TYPES.items() if v == float]
-    df[numeric_cols] = df[numeric_cols].replace("", np.nan)
-
-    df = df.drop(df[(df["Locataires"] == "") & (df["Période"] == "")].index)
-
-    return df.astype(DF_TYPES)
+    return df.astype(DF_TYPES, errors="ignore")
```

### Comparing `pdf_oralia-0.3.4/pdf_oralia/pages/recapitulatif.py` & `pdf_oralia-1.dev0/pdf_oralia/pages/recapitulatif.py`

 * *Files identical despite different names*

### Comparing `pdf_oralia-0.3.4/pdf_oralia/scripts.py` & `pdf_oralia-1.dev0/pdf_oralia/scripts.py`

 * *Files identical despite different names*

### Comparing `pdf_oralia-0.3.4/pyproject.toml` & `pdf_oralia-1.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdf-oralia"
-version = "v0.3.4"
+version = "1.dev"
 description = ""
 authors = ["Bertrand Benjamin <benjamin.bertrand@opytex.org>"]
 readme = "README.md"
 packages = [{include = "pdf_oralia"}]
 
 [tool.poetry.scripts]
 pdf-oralia = "pdf_oralia.scripts:main"
```

### Comparing `pdf_oralia-0.3.4/PKG-INFO` & `pdf_oralia-1.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdf-oralia
-Version: 0.3.4
+Version: 1.dev0
 Summary: 
 Author: Bertrand Benjamin
 Author-email: benjamin.bertrand@opytex.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


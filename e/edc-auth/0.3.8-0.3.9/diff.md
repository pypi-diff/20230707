# Comparing `tmp/edc_auth-0.3.8-py2.py3-none-any.whl.zip` & `tmp/edc_auth-0.3.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 83206 bytes, number of entries: 115
+Zip file size: 83183 bytes, number of entries: 115
 -rw-r--r--  2.0 unx      537 b- defN 21-Mar-29 22:12 edc_auth/__init__.py
--rw-r--r--  2.0 unx      253 b- defN 21-Jan-26 23:19 edc_auth/admin_site.py
+-rw-r--r--  2.0 unx      161 b- defN 21-May-12 12:29 edc_auth/admin_site.py
 -rw-r--r--  2.0 unx     1166 b- defN 21-Jan-29 00:54 edc_auth/apps.py
 -rw-r--r--  2.0 unx      798 b- defN 21-Jan-26 23:19 edc_auth/backends.py
 -rw-r--r--  2.0 unx      536 b- defN 21-Mar-29 22:12 edc_auth/constants.py
 -rw-r--r--  2.0 unx     1595 b- defN 21-Mar-08 01:25 edc_auth/export_users.py
 -rw-r--r--  2.0 unx     3106 b- defN 21-Jan-29 00:54 edc_auth/fix_export_permissions.py
 -rw-r--r--  2.0 unx     2936 b- defN 21-Jan-29 00:54 edc_auth/forms.py
 -rw-r--r--  2.0 unx     1687 b- defN 21-Mar-29 22:12 edc_auth/get_default_codenames_by_group.py
@@ -105,13 +105,13 @@
 -rw-r--r--  2.0 unx     4358 b- defN 21-Mar-08 01:25 edc_auth/tests/tests/test_group_permissions_updater.py
 -rw-r--r--  2.0 unx     2363 b- defN 21-Mar-08 01:25 edc_auth/tests/tests/test_roles.py
 -rw-r--r--  2.0 unx     5515 b- defN 21-Mar-08 01:25 edc_auth/tests/tests/test_user.py
 -rw-r--r--  2.0 unx     2919 b- defN 21-Mar-08 01:25 edc_auth/tests/tests/test_user_profile.py
 -rw-r--r--  2.0 unx       70 b- defN 21-Jan-26 23:19 edc_auth/views/__init__.py
 -rw-r--r--  2.0 unx     1881 b- defN 21-Feb-01 03:05 edc_auth/views/login_view.py
 -rw-r--r--  2.0 unx      963 b- defN 21-Jan-26 23:19 edc_auth/views/logout_view.py
--rw-r--r--  2.0 unx    35147 b- defN 21-Apr-23 11:54 edc_auth-0.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     4284 b- defN 21-Apr-23 11:54 edc_auth-0.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 21-Apr-23 11:54 edc_auth-0.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 21-Apr-23 11:54 edc_auth-0.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    10588 b- defN 21-Apr-23 11:54 edc_auth-0.3.8.dist-info/RECORD
-115 files, 207902 bytes uncompressed, 66118 bytes compressed:  68.2%
+-rw-r--r--  2.0 unx    35147 b- defN 21-May-12 12:29 edc_auth-0.3.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4284 b- defN 21-May-12 12:29 edc_auth-0.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 21-May-12 12:29 edc_auth-0.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 21-May-12 12:29 edc_auth-0.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    10588 b- defN 21-May-12 12:29 edc_auth-0.3.9.dist-info/RECORD
+115 files, 207810 bytes uncompressed, 66095 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -324,23 +324,23 @@
 
 Filename: edc_auth/views/login_view.py
 Comment: 
 
 Filename: edc_auth/views/logout_view.py
 Comment: 
 
-Filename: edc_auth-0.3.8.dist-info/LICENSE
+Filename: edc_auth-0.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: edc_auth-0.3.8.dist-info/METADATA
+Filename: edc_auth-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: edc_auth-0.3.8.dist-info/WHEEL
+Filename: edc_auth-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: edc_auth-0.3.8.dist-info/top_level.txt
+Filename: edc_auth-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: edc_auth-0.3.8.dist-info/RECORD
+Filename: edc_auth-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## edc_auth/admin_site.py

```diff
@@ -1,10 +1,5 @@
 from edc_model_admin.admin_site import EdcAdminSite
 
+from .apps import AppConfig
 
-class AdminSite(EdcAdminSite):
-    site_header = "Edc Authentication"
-    site_title = "Edc Authentication"
-    index_title = "Edc Authentication"
-
-
-edc_auth_admin = AdminSite(name="edc_auth_admin")
+edc_auth_admin = EdcAdminSite(name="edc_auth_admin", app_label=AppConfig.name)
```

## Comparing `edc_auth-0.3.8.dist-info/LICENSE` & `edc_auth-0.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edc_auth-0.3.8.dist-info/METADATA` & `edc_auth-0.3.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-auth
-Version: 0.3.8
+Version: 0.3.9
 Summary: Authentication for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc-auth
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django auth edc
 Platform: UNKNOWN
```

## Comparing `edc_auth-0.3.8.dist-info/RECORD` & `edc_auth-0.3.9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 edc_auth/__init__.py,sha256=83ejp_7tPBCresHPfrUp5yvTiCKsMAq-JfxsVESpD08,537
-edc_auth/admin_site.py,sha256=Wib6_JGVTPIYNcNl_W8LNPkIDMJRege8WHFUAalkWWY,253
+edc_auth/admin_site.py,sha256=Mlc14SZk7KxyjquCmegGWN2Q2Mz2XTNNv8T2CUSPQUo,161
 edc_auth/apps.py,sha256=8A3jZcMIKnpvQbo3wy5cn8mt25tzp4QRe2-DU3Lq-gI,1166
 edc_auth/backends.py,sha256=Jh_gywMyqDTc8A4N0ZUXT6E3WAAkH5HX-GGuBrklxxw,798
 edc_auth/constants.py,sha256=VD63avsEnCtKmBqLICeoYdpvB8C8Ovfr-lcXlXBqlyE,536
 edc_auth/export_users.py,sha256=UnTXh6J3ANu496TtlZkkVFP0PML6DPAj0ZEuXSXMyEk,1595
 edc_auth/fix_export_permissions.py,sha256=vvMVsROnj3jbhcqhtIxpinqADOfJjYYYVo4TdpZLl2k,3106
 edc_auth/forms.py,sha256=-6HGkfmL2a1FuRbJn22idEPC4s5dcqGcj46TjbKDxSQ,2936
 edc_auth/get_default_codenames_by_group.py,sha256=eIvwOdOkvXxmVyd9430BdeWXg6OkV--i9paPcpNBjnE,1687
@@ -104,12 +104,12 @@
 edc_auth/tests/tests/test_group_permissions_updater.py,sha256=3TrZMBZS2hpH-Mdqz6GQ9XJRFJBmY06GkmXbg39Sq7I,4358
 edc_auth/tests/tests/test_roles.py,sha256=SFWD3CQ98V3KU_TmMzqUVEIjG6UuZgUzYHoHs8U3Ags,2363
 edc_auth/tests/tests/test_user.py,sha256=csmGgd-oGbXoDFLf6-dhd3NZ3jOgukbzbAx7-2bfFk0,5515
 edc_auth/tests/tests/test_user_profile.py,sha256=4qIVbUYza3E0I_3QVEHfaq3DfKkfh7Ff1JREZgt56TY,2919
 edc_auth/views/__init__.py,sha256=6nIb80qhHbB7VaeOCFsBBpgiwgp5-PTlLBmbH0l-PSM,70
 edc_auth/views/login_view.py,sha256=FWcgGKRAZio1xyJ7ceEBKMIz08nqOSbi1IdBynpksE4,1881
 edc_auth/views/logout_view.py,sha256=i84LTzZJcRNcRTaBEEF2IaF4w3iQ-lyv_2dJ1qdnp3I,963
-edc_auth-0.3.8.dist-info/LICENSE,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
-edc_auth-0.3.8.dist-info/METADATA,sha256=VX9FVGewxd5ITVmjZNYJ6loTvHQsVbtQaelONDKYaME,4284
-edc_auth-0.3.8.dist-info/WHEEL,sha256=ADKeyaGyKF5DwBNE0sRE5pvW-bSkFMJfBuhzZ3rceP4,110
-edc_auth-0.3.8.dist-info/top_level.txt,sha256=fCOoqt2hJKn6Hapmfp_r1-JUXuA0CgyNLNitmT9tu-Q,9
-edc_auth-0.3.8.dist-info/RECORD,,
+edc_auth-0.3.9.dist-info/LICENSE,sha256=jOtLnuWt7d5Hsx6XXB2QxzrSe2sWWh3NgMfFRetluQM,35147
+edc_auth-0.3.9.dist-info/METADATA,sha256=5HXMWVDz4trsSw6wCoOgvKRWS6VlWrfu18RAdipHdTE,4284
+edc_auth-0.3.9.dist-info/WHEEL,sha256=ADKeyaGyKF5DwBNE0sRE5pvW-bSkFMJfBuhzZ3rceP4,110
+edc_auth-0.3.9.dist-info/top_level.txt,sha256=fCOoqt2hJKn6Hapmfp_r1-JUXuA0CgyNLNitmT9tu-Q,9
+edc_auth-0.3.9.dist-info/RECORD,,
```


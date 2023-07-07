# Comparing `tmp/ez0th-0.1.1.tar.gz` & `tmp/ez0th-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez0th-0.1.1.tar", last modified: Wed Jul  5 05:27:01 2023, max compression
+gzip compressed data, was "ez0th-0.1.2.tar", last modified: Fri Jul  7 05:35:14 2023, max compression
```

## Comparing `ez0th-0.1.1.tar` & `ez0th-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 05:27:01.750945 ez0th-0.1.1/
--rw-rw-rw-   0        0        0    13581 2023-07-05 05:27:01.750945 ez0th-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    11167 2023-07-05 05:24:33.000000 ez0th-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 05:27:01.738316 ez0th-0.1.1/ez0th/
--rw-rw-rw-   0        0        0    10115 2023-07-05 05:20:50.000000 ez0th-0.1.1/ez0th/__init__.py
--rw-rw-rw-   0        0        0     3199 2023-07-05 05:22:11.000000 ez0th-0.1.1/ez0th/test.py
-drwxrwxrwx   0        0        0        0 2023-07-05 05:27:01.749830 ez0th-0.1.1/ez0th.egg-info/
--rw-rw-rw-   0        0        0    13581 2023-07-05 05:27:01.000000 ez0th-0.1.1/ez0th.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-07-05 05:27:01.000000 ez0th-0.1.1/ez0th.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 05:27:01.000000 ez0th-0.1.1/ez0th.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-05 05:27:01.000000 ez0th-0.1.1/ez0th.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-05 05:27:01.000000 ez0th-0.1.1/ez0th.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 05:27:01.750945 ez0th-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      801 2023-07-05 05:26:53.000000 ez0th-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 05:35:14.128344 ez0th-0.1.2/
+-rw-rw-rw-   0        0        0    14268 2023-07-07 05:35:14.128344 ez0th-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11726 2023-07-07 05:34:26.000000 ez0th-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 05:35:14.103368 ez0th-0.1.2/ez0th/
+-rw-rw-rw-   0        0        0    10840 2023-07-07 05:31:04.000000 ez0th-0.1.2/ez0th/__init__.py
+-rw-rw-rw-   0        0        0     3467 2023-07-07 05:29:33.000000 ez0th-0.1.2/ez0th/test.py
+drwxrwxrwx   0        0        0        0 2023-07-07 05:35:14.126342 ez0th-0.1.2/ez0th.egg-info/
+-rw-rw-rw-   0        0        0    14268 2023-07-07 05:35:13.000000 ez0th-0.1.2/ez0th.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-07-07 05:35:13.000000 ez0th-0.1.2/ez0th.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 05:35:13.000000 ez0th-0.1.2/ez0th.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-07 05:35:13.000000 ez0th-0.1.2/ez0th.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-07 05:35:13.000000 ez0th-0.1.2/ez0th.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-07 05:35:14.128344 ez0th-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      801 2023-07-07 05:35:09.000000 ez0th-0.1.2/setup.py
```

### Comparing `ez0th-0.1.1/PKG-INFO` & `ez0th-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez0th
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Library for Easy Authentication and Authorization
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: # ez0th - Python Library for Easy Authentication and Authorization
         
@@ -97,14 +97,22 @@
             sess_token = sess_token,    # Session token
             new_user_info = new_user_info,  # Updated user information
             db = db,    # Database
         )
         # Check result
         print(success_flag)
         
+        # Get user information (Be cautious as there is no authentication process, which may result in information leakage) [ez0th]
+        info = ez0th.get_info(
+            u_id = "WhiteDog",  # Login ID (Any registered ID can be used)
+            db = db,  # Database
+        )
+        # Check the result
+        print(info)
+        
         # Logout [ez0th]
         success_flag = ez0th.logout(
             sess_token = sess_token,    # Session token
             db = db # Database
         )
         # Check result
         print(success_flag)
@@ -221,14 +229,22 @@
             sess_token = sess_token,    # セッショントークン
             new_user_info = new_user_info,  # 変更後のユーザー情報
             db = db,    # データベース
         )
         # 結果確認
         print(success_flag)
         
+        # ユーザー情報取得 (認可処理は入っていないので、情報漏洩に注意) [ez0th]
+        info = ez0th.get_info(
+            u_id = "WhiteDog",  # ログインid (登録されたいずれのidも可)
+            db = db,    # データベース
+        )
+        # 結果確認
+        print(info)
+        
         # ログアウト [ez0th]
         success_flag = ez0th.logout(
             sess_token = sess_token,    # セッショントークン
             db = db # データベース
         )
         # 結果確認
         print(success_flag)
```

### Comparing `ez0th-0.1.1/README.md` & `ez0th-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,22 @@
     sess_token = sess_token,    # Session token
     new_user_info = new_user_info,  # Updated user information
     db = db,    # Database
 )
 # Check result
 print(success_flag)
 
+# Get user information (Be cautious as there is no authentication process, which may result in information leakage) [ez0th]
+info = ez0th.get_info(
+    u_id = "WhiteDog",  # Login ID (Any registered ID can be used)
+    db = db,  # Database
+)
+# Check the result
+print(info)
+
 # Logout [ez0th]
 success_flag = ez0th.logout(
     sess_token = sess_token,    # Session token
     db = db # Database
 )
 # Check result
 print(success_flag)
@@ -213,14 +221,22 @@
     sess_token = sess_token,    # セッショントークン
     new_user_info = new_user_info,  # 変更後のユーザー情報
     db = db,    # データベース
 )
 # 結果確認
 print(success_flag)
 
+# ユーザー情報取得 (認可処理は入っていないので、情報漏洩に注意) [ez0th]
+info = ez0th.get_info(
+    u_id = "WhiteDog",  # ログインid (登録されたいずれのidも可)
+    db = db,    # データベース
+)
+# 結果確認
+print(info)
+
 # ログアウト [ez0th]
 success_flag = ez0th.logout(
     sess_token = sess_token,    # セッショントークン
     db = db # データベース
 )
 # 結果確認
 print(success_flag)
```

### Comparing `ez0th-0.1.1/ez0th/__init__.py` & `ez0th-0.1.2/ez0th/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -247,7 +247,22 @@
 	try:
 		db["update"](inner_id,
 			{**db["read"](inner_id), "info": new_user_info}
 		)
 		return True
 	except:
 		return False
+
+# ユーザー情報取得 (認可処理は入っていないので、情報漏洩に注意) [ez0th]
+def get_info(
+	u_id,	# ログインid (登録されたいずれのidも可)
+	db,	# データベース
+):
+	if db == "auto": db = json_stock("./__ez0th_user_db__/")
+	# 引数インジェクションチェック (セキュリティー対策; ptnを満たす文字列かどうかをチェック)
+	check_injection(u_id)
+	# アカウント存在確認 [ez0th]
+	if exists(u_id, db) is not True: raise Exception("[ez0th error] No user exists matching the specified u_id.")
+	# ユーザーのinner_idを明らかにする
+	inner_id = db["read"]("id_"+u_id)
+	# ユーザー情報を返す
+	return db["read"](inner_id)
```

### Comparing `ez0th-0.1.1/ez0th/test.py` & `ez0th-0.1.2/ez0th/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,22 @@
 	sess_token = sess_token,	# セッショントークン
 	new_user_info = new_user_info,	# 変更後のユーザー情報
 	db = db,	# データベース
 )
 # 結果確認
 print(success_flag)
 
+# ユーザー情報取得 (認可処理は入っていないので、情報漏洩に注意) [ez0th]
+info = ez0th.get_info(
+	u_id = "WhiteDog",	# ログインid (登録されたいずれのidも可)
+	db = db,	# データベース
+)
+# 結果確認
+print(info)
+
 # ログアウト [ez0th]
 success_flag = ez0th.logout(
 	sess_token = sess_token,	# セッショントークン
 	db = db	# データベース
 )
 # 結果確認
 print(success_flag)
```

### Comparing `ez0th-0.1.1/ez0th.egg-info/PKG-INFO` & `ez0th-0.1.2/ez0th.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez0th
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Library for Easy Authentication and Authorization
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: # ez0th - Python Library for Easy Authentication and Authorization
         
@@ -97,14 +97,22 @@
             sess_token = sess_token,    # Session token
             new_user_info = new_user_info,  # Updated user information
             db = db,    # Database
         )
         # Check result
         print(success_flag)
         
+        # Get user information (Be cautious as there is no authentication process, which may result in information leakage) [ez0th]
+        info = ez0th.get_info(
+            u_id = "WhiteDog",  # Login ID (Any registered ID can be used)
+            db = db,  # Database
+        )
+        # Check the result
+        print(info)
+        
         # Logout [ez0th]
         success_flag = ez0th.logout(
             sess_token = sess_token,    # Session token
             db = db # Database
         )
         # Check result
         print(success_flag)
@@ -221,14 +229,22 @@
             sess_token = sess_token,    # セッショントークン
             new_user_info = new_user_info,  # 変更後のユーザー情報
             db = db,    # データベース
         )
         # 結果確認
         print(success_flag)
         
+        # ユーザー情報取得 (認可処理は入っていないので、情報漏洩に注意) [ez0th]
+        info = ez0th.get_info(
+            u_id = "WhiteDog",  # ログインid (登録されたいずれのidも可)
+            db = db,    # データベース
+        )
+        # 結果確認
+        print(info)
+        
         # ログアウト [ez0th]
         success_flag = ez0th.logout(
             sess_token = sess_token,    # セッショントークン
             db = db # データベース
         )
         # 結果確認
         print(success_flag)
```

### Comparing `ez0th-0.1.1/setup.py` & `ez0th-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 00000080: 205b 657a 7069 705d 0d0a 7769 7468 2065   [ezpip]..with e
 00000090: 7a70 6970 2e70 6163 6b61 6765 7228 6465  zpip.packager(de
 000000a0: 7665 6c6f 705f 6469 7220 3d20 222e 2f5f  velop_dir = "./_
 000000b0: 6465 7665 6c6f 705f 657a 3074 682f 2229  develop_ez0th/")
 000000c0: 2061 7320 703a 0d0a 0973 6574 7570 280d   as p:...setup(.
 000000d0: 0a09 096e 616d 6520 3d20 2265 7a30 7468  ...name = "ez0th
 000000e0: 222c 0d0a 0909 7665 7273 696f 6e20 3d20  ",....version = 
-000000f0: 2230 2e31 2e31 222c 0d0a 0909 6465 7363  "0.1.1",....desc
+000000f0: 2230 2e31 2e32 222c 0d0a 0909 6465 7363  "0.1.2",....desc
 00000100: 7269 7074 696f 6e20 3d20 2250 7974 686f  ription = "Pytho
 00000110: 6e20 4c69 6272 6172 7920 666f 7220 4561  n Library for Ea
 00000120: 7379 2041 7574 6865 6e74 6963 6174 696f  sy Authenticatio
 00000130: 6e20 616e 6420 4175 7468 6f72 697a 6174  n and Authorizat
 00000140: 696f 6e22 2c0d 0a09 0961 7574 686f 7220  ion",....author 
 00000150: 3d20 2262 6962 5f69 6e66 222c 0d0a 0909  = "bib_inf",....
 00000160: 6175 7468 6f72 5f65 6d61 696c 203d 2022  author_email = "
```


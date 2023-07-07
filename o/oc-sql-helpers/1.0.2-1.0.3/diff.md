# Comparing `tmp/oc_sql_helpers-1.0.2-py3-none-any.whl.zip` & `tmp/oc_sql_helpers-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 20127 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 07:46 oc_sql_helpers/__init__.py
--rw-r--r--  2.0 unx    34675 b- defN 23-May-22 07:46 oc_sql_helpers/normalizer.py
--rw-r--r--  2.0 unx     2802 b- defN 23-May-22 07:46 oc_sql_helpers/str_decoder.py
--rw-r--r--  2.0 unx    18181 b- defN 23-May-22 07:46 oc_sql_helpers/wrapper.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-22 07:46 oc_sql_helpers-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      243 b- defN 23-May-22 07:46 oc_sql_helpers-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 07:46 oc_sql_helpers-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-May-22 07:46 oc_sql_helpers-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      756 b- defN 23-May-22 07:46 oc_sql_helpers-1.0.2.dist-info/RECORD
-9 files, 68121 bytes uncompressed, 18817 bytes compressed:  72.4%
+Zip file size: 20217 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-07 11:02 oc_sql_helpers/__init__.py
+-rw-r--r--  2.0 unx    35275 b- defN 23-Jul-07 11:02 oc_sql_helpers/normalizer.py
+-rw-r--r--  2.0 unx     2802 b- defN 23-Jul-07 11:02 oc_sql_helpers/str_decoder.py
+-rw-r--r--  2.0 unx    18181 b- defN 23-Jul-07 11:02 oc_sql_helpers/wrapper.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-07 11:02 oc_sql_helpers-1.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      243 b- defN 23-Jul-07 11:02 oc_sql_helpers-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-07 11:02 oc_sql_helpers-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jul-07 11:02 oc_sql_helpers-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      756 b- defN 23-Jul-07 11:02 oc_sql_helpers-1.0.3.dist-info/RECORD
+9 files, 68721 bytes uncompressed, 18907 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: oc_sql_helpers/str_decoder.py
 Comment: 
 
 Filename: oc_sql_helpers/wrapper.py
 Comment: 
 
-Filename: oc_sql_helpers-1.0.2.dist-info/LICENSE
+Filename: oc_sql_helpers-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: oc_sql_helpers-1.0.2.dist-info/METADATA
+Filename: oc_sql_helpers-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: oc_sql_helpers-1.0.2.dist-info/WHEEL
+Filename: oc_sql_helpers-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: oc_sql_helpers-1.0.2.dist-info/top_level.txt
+Filename: oc_sql_helpers-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: oc_sql_helpers-1.0.2.dist-info/RECORD
+Filename: oc_sql_helpers-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oc_sql_helpers/normalizer.py

```diff
@@ -67,16 +67,32 @@
             "wrapped": [{"start": re.compile(b'(\s|^)wrapped(\s|$)', flags=re.I)}]}
     # these objects are legal in any part of file
     # NOTE: national charset literals may be supported in wrong way by this implementation
     _re_objects_body={
             "object_name": [{"start": re.compile(b'"'), "end": re.compile(b'"')}],
             "literal":[
                 {"start": re.compile(b"q'(.)", flags=re.I), "end": b"%s'", 
-                    "substitutes": {b"[": b"\]", b"{": b"\}", b"<": b"\>", b"(": b"\)", b"?": b"\?", b".": b"\.", b"^": b"\^", b"$": b"\$", b"\\": b"\\\\", b"*": b"\*",
-                        b"+": b"\+", b"|": b"\|"}},
+                    "substitutes": {
+                        b"[": b"\]", 
+                        b"{": b"\}", 
+                        b"<": b"\>", 
+                        b"(": b"\)", 
+                        b"?": b"\?", 
+                        b".": b"\.", 
+                        b"^": b"\^", 
+                        b"$": b"\$", 
+                        b"\\": b"\\\\", 
+                        b"*": b"\*",
+                        b"+": b"\+", 
+                        b"|": b"\|",
+                        # there may be a closing brackets also, we have to escape them too
+                        b"]": b"\]", 
+                        b"}": b"\}", 
+                        b">": b"\>", 
+                        b")": b"\)"}},
                 {"start": re.compile(b"'", flags=re.I), "end": re.compile(b"'")}],
             "comment":[
                 {"start": re.compile(b'(\s|^)\-\-'), "end": re.compile(b'\n')},
                 {"start": re.compile(b'\/\*'), "end": re.compile(b'\*\/')}]}
 
     def _fl_full(self):
         """
@@ -204,14 +220,16 @@
 
                 # here we have a match object
                 # if start posistion is less than one we have now - replace the context key in the result
                 if _result and _match.start() >= _result.get("match").start():
                     # not a first inc, out of interest
                     continue
 
+                logging.log(1, "Found context: [%s], match: [%s]" % (_k, _match))
+
                 _result = {"context": _k, "match": _match, "end": self._make_reg_end(_regx, _match)}
 
         return _result
 
     def _search_declaration_regx(self, line):
         """
         Search 'line' upon declaration regular expressions
```

## Comparing `oc_sql_helpers-1.0.2.dist-info/LICENSE` & `oc_sql_helpers-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `oc_sql_helpers-1.0.2.dist-info/RECORD` & `oc_sql_helpers-1.0.3.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 oc_sql_helpers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-oc_sql_helpers/normalizer.py,sha256=yT7Rbe-vl0ec4oHQ6-oazv-41R5x1IIGfdhcZR41OL4,34675
+oc_sql_helpers/normalizer.py,sha256=BUdmRWfq0bfJ8CJ5quRtpfbHIIOUaSrt27C45xq_DrA,35275
 oc_sql_helpers/str_decoder.py,sha256=zt1fN07fkW55TmLm7Inb-5RTab7UaXiAjxBd-f5vMeU,2802
 oc_sql_helpers/wrapper.py,sha256=GJcu_iS7o9fjBLECv17U1IPecPVt9fy0m89KXWJKywQ,18181
-oc_sql_helpers-1.0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-oc_sql_helpers-1.0.2.dist-info/METADATA,sha256=H6Drxnd-c0FOs3R6JvxeK21i87OkVFd4jxh2BwiYF7o,243
-oc_sql_helpers-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-oc_sql_helpers-1.0.2.dist-info/top_level.txt,sha256=pKp8OXzXLdlZecL-DuIWqY8U4tr1bMLDqK4MOtMdMTU,15
-oc_sql_helpers-1.0.2.dist-info/RECORD,,
+oc_sql_helpers-1.0.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+oc_sql_helpers-1.0.3.dist-info/METADATA,sha256=7e5J7iJ0332Ega5amsygmzIKEWuZcz0cMZqKWpb1qfY,243
+oc_sql_helpers-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+oc_sql_helpers-1.0.3.dist-info/top_level.txt,sha256=pKp8OXzXLdlZecL-DuIWqY8U4tr1bMLDqK4MOtMdMTU,15
+oc_sql_helpers-1.0.3.dist-info/RECORD,,
```


# Comparing `tmp/moordyn-2.1.0.tar.gz` & `tmp/moordyn-2.2.0-cp37-cp37m-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moordyn-2.1.0.tar", last modified: Fri Feb 17 15:06:51 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


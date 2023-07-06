# Comparing `tmp/kenoAPI-4.1.0.tar.gz` & `tmp/kenoAPI-4.9.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kenoAPI-4.1.0.tar", last modified: Thu Aug 12 00:47:54 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


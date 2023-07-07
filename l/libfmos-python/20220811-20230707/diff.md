# Comparing `tmp/libfmos-python-20220811.tar.gz` & `tmp/libfmos_python-20230707-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfmos-python-20220811.tar", last modified: Wed Aug 17 18:18:42 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


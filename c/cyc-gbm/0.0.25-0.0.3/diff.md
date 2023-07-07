# Comparing `tmp/cyc-gbm-0.0.25.tar.gz` & `tmp/cyc_gbm-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyc-gbm-0.0.25.tar", last modified: Mon Jul  3 10:27:57 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


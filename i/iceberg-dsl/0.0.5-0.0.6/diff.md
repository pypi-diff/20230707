# Comparing `tmp/iceberg-dsl-0.0.5.tar.gz` & `tmp/iceberg_dsl-0.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iceberg-dsl-0.0.5.tar", last modified: Thu Jul  6 01:09:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


# Comparing `tmp/dwave-preprocessing-0.6.1.tar.gz` & `tmp/dwave_preprocessing-0.6.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwave-preprocessing-0.6.1.tar", last modified: Thu Jul  6 15:55:21 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


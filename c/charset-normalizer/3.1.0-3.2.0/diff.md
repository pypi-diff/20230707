# Comparing `tmp/charset-normalizer-3.1.0.tar.gz` & `tmp/charset_normalizer-3.2.0-cp37-cp37m-musllinux_1_1_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charset-normalizer-3.1.0.tar", last modified: Mon Mar  6 08:37:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


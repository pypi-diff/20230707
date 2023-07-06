# Comparing `tmp/torch_hep-0.0.3.tar.gz` & `tmp/torch_hep-0.0.4-py3.10.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_hep-0.0.3.tar", last modified: Mon Jun 20 16:08:55 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


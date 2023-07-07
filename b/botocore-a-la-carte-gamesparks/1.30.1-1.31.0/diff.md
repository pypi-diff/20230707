# Comparing `tmp/botocore-a-la-carte-gamesparks-1.30.1.tar.gz` & `tmp/botocore-a-la-carte-gamesparks-1.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-gamesparks-1.30.1.tar", last modified: Thu Jul  6 01:45:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


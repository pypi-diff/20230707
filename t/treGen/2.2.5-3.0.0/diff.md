# Comparing `tmp/treGen-2.2.5.tar.gz` & `tmp/treGen-3.0.0-py3.9.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treGen-2.2.5.tar", last modified: Thu Jul  6 21:33:59 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


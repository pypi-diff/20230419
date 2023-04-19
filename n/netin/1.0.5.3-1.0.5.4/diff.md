# Comparing `tmp/netin-1.0.5.3.tar.gz` & `tmp/netin-1.0.5.4-py3.9.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netin-1.0.5.3.tar", last modified: Mon Apr 17 23:29:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


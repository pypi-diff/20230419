# Comparing `tmp/asyncbg-0.8.0.tar.gz` & `tmp/asyncbg-0.9.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/asyncbg-0.8.0.tar", last modified: Mon Aug  3 10:23:43 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


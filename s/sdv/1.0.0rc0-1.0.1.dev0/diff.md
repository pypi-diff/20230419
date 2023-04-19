# Comparing `tmp/sdv-1.0.0rc0.tar.gz` & `tmp/sdv-1.0.1.dev0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdv-1.0.0rc0.tar", last modified: Tue Mar 28 14:08:32 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


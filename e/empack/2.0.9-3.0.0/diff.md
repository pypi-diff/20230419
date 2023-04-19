# Comparing `tmp/empack-2.0.9.tar.gz` & `tmp/empack-3.0.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empack-2.0.9.tar", last modified: Tue Feb 14 11:00:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


# Comparing `tmp/sextant-0.2.0.tar.gz` & `tmp/sextant-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sextant-0.2.0.tar", last modified: Thu Jan 12 14:51:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


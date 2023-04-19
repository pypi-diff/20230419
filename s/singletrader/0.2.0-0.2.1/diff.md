# Comparing `tmp/singletrader-0.2.0.tar.gz` & `tmp/singletrader-0.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singletrader-0.2.0.tar", last modified: Fri Apr 14 09:17:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


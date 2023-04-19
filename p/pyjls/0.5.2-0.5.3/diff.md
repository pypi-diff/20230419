# Comparing `tmp/pyjls-0.5.2.tar.gz` & `tmp/pyjls-0.5.3-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjls-0.5.2.tar", last modified: Thu Mar 30 20:13:48 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


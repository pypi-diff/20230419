# Comparing `tmp/ifcfg-0.9.3.tar.gz` & `tmp/ifcfg-0.9.4-py2-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ifcfg-0.9.3.tar", last modified: Sun Apr 17 17:06:06 2016, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


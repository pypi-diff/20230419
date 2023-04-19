# Comparing `tmp/shimoku-components-catalog-0.2.tar.gz` & `tmp/shimoku_components_catalog-0.2.1-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shimoku-components-catalog-0.2.tar", last modified: Tue Nov 15 14:09:28 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


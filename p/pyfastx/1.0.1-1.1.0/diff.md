# Comparing `tmp/pyfastx-1.0.1.tar.gz` & `tmp/pyfastx-1.1.0-cp36-cp36m-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfastx-1.0.1.tar", last modified: Tue Mar 28 10:33:14 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


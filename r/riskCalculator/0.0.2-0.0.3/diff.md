# Comparing `tmp/riskCalculator-0.0.2.tar.gz` & `tmp/riskCalculator-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riskCalculator-0.0.2.tar", last modified: Wed Apr 19 04:46:15 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```


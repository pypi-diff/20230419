# Comparing `tmp/mlops_lessons-0.1.dev1-py3-none-any.whl.zip` & `tmp/mlops_lessons-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 2950 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 17:24 mlops_lessons/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 17:24 mlops_lessons/jobs/__init__.py
--rw-r--r--  2.0 unx       49 b- defN 23-Apr-19 17:24 mlops_lessons/jobs/training/__init__.py
--rw-r--r--  2.0 unx     1190 b- defN 23-Apr-19 17:24 mlops_lessons/jobs/training/main.py
--rw-r--r--  2.0 unx      628 b- defN 23-Apr-19 17:24 mlops_lessons-0.1.dev1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 17:24 mlops_lessons-0.1.dev1.dist-info/WHEEL
--rw-r--r--  2.0 unx       63 b- defN 23-Apr-19 17:24 mlops_lessons-0.1.dev1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-19 17:24 mlops_lessons-0.1.dev1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      786 b- defN 23-Apr-19 17:24 mlops_lessons-0.1.dev1.dist-info/RECORD
-9 files, 2822 bytes uncompressed, 1560 bytes compressed:  44.7%
+Zip file size: 3066 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 17:04 mlops_lessons/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-19 17:04 mlops_lessons/version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-19 17:04 mlops_lessons/jobs/__init__.py
+-rw-r--r--  2.0 unx       49 b- defN 23-Apr-19 17:04 mlops_lessons/jobs/training/__init__.py
+-rw-r--r--  2.0 unx     1190 b- defN 23-Apr-19 17:04 mlops_lessons/jobs/training/main.py
+-rw-r--r--  2.0 unx      539 b- defN 23-Apr-19 17:04 mlops_lessons-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 17:04 mlops_lessons-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 23-Apr-19 17:04 mlops_lessons-1.0.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-19 17:04 mlops_lessons-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      850 b- defN 23-Apr-19 17:04 mlops_lessons-1.0.0.dist-info/RECORD
+10 files, 2819 bytes uncompressed, 1582 bytes compressed:  43.9%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: mlops_lessons/__init__.py
 Comment: 
 
+Filename: mlops_lessons/version.py
+Comment: 
+
 Filename: mlops_lessons/jobs/__init__.py
 Comment: 
 
 Filename: mlops_lessons/jobs/training/__init__.py
 Comment: 
 
 Filename: mlops_lessons/jobs/training/main.py
 Comment: 
 
-Filename: mlops_lessons-0.1.dev1.dist-info/METADATA
+Filename: mlops_lessons-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: mlops_lessons-0.1.dev1.dist-info/WHEEL
+Filename: mlops_lessons-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: mlops_lessons-0.1.dev1.dist-info/entry_points.txt
+Filename: mlops_lessons-1.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: mlops_lessons-0.1.dev1.dist-info/top_level.txt
+Filename: mlops_lessons-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mlops_lessons-0.1.dev1.dist-info/RECORD
+Filename: mlops_lessons-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mlops_lessons-0.1.dev1.dist-info/METADATA` & `mlops_lessons-1.0.0.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 Metadata-Version: 2.1
 Name: mlops-lessons
-Version: 0.1.dev1
+Version: 1.0.0
 Summary: Lesons about mlops
 Home-page: https://github.com/vincentvic/MLOps
 Author: VINCENT Victor
 Author-email: vincent.victor206@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: tensorflow
 Requires-Dist: matplotlib
-Requires-Dist: setuptools-scm
 
 # MLOps
 Lessons about MLOPS first part 
 
 #  Create env python = Packaging
 - python -m venv .venv
 - .venv\Script\activate
 - pip install -e .
 - pip freeze > requirements.txt
 
 # create setup.py
-- respect the format
-
-# github workflows
-- wheel python
```


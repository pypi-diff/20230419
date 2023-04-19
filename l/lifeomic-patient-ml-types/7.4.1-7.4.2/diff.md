# Comparing `tmp/lifeomic_patient_ml_types-7.4.1.tar.gz` & `tmp/lifeomic_patient_ml_types-7.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeomic_patient_ml_types-7.4.1.tar", max compression
+gzip compressed data, was "lifeomic_patient_ml_types-7.4.2.tar", max compression
```

## Comparing `lifeomic_patient_ml_types-7.4.1.tar` & `lifeomic_patient_ml_types-7.4.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    13999 2023-04-14 13:46:44.313518 lifeomic_patient_ml_types-7.4.1/lifeomic_patient_ml_types/schemas.py
--rw-r--r--   0        0        0      664 2023-04-14 13:48:13.416859 lifeomic_patient_ml_types-7.4.1/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.4.1/setup.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.4.1/PKG-INFO
+-rw-r--r--   0        0        0    13999 2023-04-19 13:26:32.506832 lifeomic_patient_ml_types-7.4.2/lifeomic_patient_ml_types/schemas.py
+-rw-r--r--   0        0        0      664 2023-04-19 13:28:18.331313 lifeomic_patient_ml_types-7.4.2/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.4.2/setup.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.4.2/PKG-INFO
```

### Comparing `lifeomic_patient_ml_types-7.4.1/lifeomic_patient_ml_types/schemas.py` & `lifeomic_patient_ml_types-7.4.2/lifeomic_patient_ml_types/schemas.py`

 * *Files identical despite different names*

### Comparing `lifeomic_patient_ml_types-7.4.1/pyproject.toml` & `lifeomic_patient_ml_types-7.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lifeomic-patient-ml-types"
-version = "7.4.1"
+version = "7.4.2"
 description = "Shared types for the patient-ml-service repos."
 authors = ["LifeOmic <development@lifeomic.com>"]
 license = "UNLICENSED"
 
 [tool.poe.tasks]
 format = "black lifeomic_patient_ml_types"
 lint = "pyright lifeomic_patient_ml_types"
```

### Comparing `lifeomic_patient_ml_types-7.4.1/setup.py` & `lifeomic_patient_ml_types-7.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['lifeomic_patient_ml_types']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'lifeomic-patient-ml-types',
-    'version': '7.4.1',
+    'version': '7.4.2',
     'description': 'Shared types for the patient-ml-service repos.',
     'long_description': 'None',
     'author': 'LifeOmic',
     'author_email': 'development@lifeomic.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```


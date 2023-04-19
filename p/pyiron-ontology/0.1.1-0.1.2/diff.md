# Comparing `tmp/pyiron_ontology-0.1.1.tar.gz` & `tmp/pyiron_ontology-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_ontology-0.1.1.tar", last modified: Thu Mar 16 22:28:30 2023, max compression
+gzip compressed data, was "pyiron_ontology-0.1.2.tar", last modified: Wed Apr 19 21:32:32 2023, max compression
```

## Comparing `pyiron_ontology-0.1.1.tar` & `pyiron_ontology-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:28:30.793556 pyiron_ontology-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-03-16 22:28:25.000000 pyiron_ontology-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-16 22:28:25.000000 pyiron_ontology-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-16 22:28:30.793556 pyiron_ontology-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13303 2023-03-16 22:28:25.000000 pyiron_ontology-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:28:30.793556 pyiron_ontology-0.1.1/pyiron_ontology/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-16 22:28:25.000000 pyiron_ontology-0.1.1/pyiron_ontology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-16 22:28:30.793556 pyiron_ontology-0.1.1/pyiron_ontology/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:28:30.793556 pyiron_ontology-0.1.1/pyiron_ontology/atomistics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 22:28:25.000000 pyiron_ontology-0.1.1/pyiron_ontology/atomistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-03-16 22:28:25.000000 pyiron_ontology-0.1.1/pyiron_ontology/atomistics/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-03-16 22:28:25.000000 pyiron_ontology-0.1.1/pyiron_ontology/atomistics/reasoning.py
--rw-r--r--   0 runner    (1001) docker     (123)    17649 2023-03-16 22:28:25.000000 pyiron_ontology-0.1.1/pyiron_ontology/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-16 22:28:25.000000 pyiron_ontology-0.1.1/pyiron_ontology/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:28:30.793556 pyiron_ontology-0.1.1/pyiron_ontology/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 22:28:25.000000 pyiron_ontology-0.1.1/pyiron_ontology/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-03-16 22:28:25.000000 pyiron_ontology-0.1.1/pyiron_ontology/example/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-16 22:28:25.000000 pyiron_ontology-0.1.1/pyiron_ontology/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:28:30.793556 pyiron_ontology-0.1.1/pyiron_ontology.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-16 22:28:30.000000 pyiron_ontology-0.1.1/pyiron_ontology.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-16 22:28:30.000000 pyiron_ontology-0.1.1/pyiron_ontology.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 22:28:30.000000 pyiron_ontology-0.1.1/pyiron_ontology.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-16 22:28:30.000000 pyiron_ontology-0.1.1/pyiron_ontology.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-16 22:28:30.000000 pyiron_ontology-0.1.1/pyiron_ontology.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-16 22:28:30.793556 pyiron_ontology-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-03-16 22:28:30.000000 pyiron_ontology-0.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-16 22:28:25.000000 pyiron_ontology-0.1.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:32:32.529369 pyiron_ontology-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-19 21:32:32.529369 pyiron_ontology-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:32:32.529369 pyiron_ontology-0.1.2/pyiron_ontology/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-19 21:32:32.529369 pyiron_ontology-0.1.2/pyiron_ontology/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:32:32.529369 pyiron_ontology-0.1.2/pyiron_ontology/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/atomistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/atomistics/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/atomistics/reasoning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17649 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:32:32.529369 pyiron_ontology-0.1.2/pyiron_ontology/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/example/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/pyiron_ontology/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:32:32.529369 pyiron_ontology-0.1.2/pyiron_ontology.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-19 21:32:32.000000 pyiron_ontology-0.1.2/pyiron_ontology.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-19 21:32:32.000000 pyiron_ontology-0.1.2/pyiron_ontology.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:32:32.000000 pyiron_ontology-0.1.2/pyiron_ontology.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-19 21:32:32.000000 pyiron_ontology-0.1.2/pyiron_ontology.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 21:32:32.000000 pyiron_ontology-0.1.2/pyiron_ontology.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-19 21:32:32.529369 pyiron_ontology-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-19 21:32:32.000000 pyiron_ontology-0.1.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-19 21:32:29.000000 pyiron_ontology-0.1.2/versioneer.py
```

### Comparing `pyiron_ontology-0.1.1/LICENSE` & `pyiron_ontology-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.1/PKG-INFO` & `pyiron_ontology-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_ontology
-Version: 0.1.1
+Version: 0.1.2
 Summary: pyiron_ontology - module extension to pyiron.
 Home-page: https://github.com/pyiron/pyiron_ontology
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: liamhuber@greyhavensolutions.com
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyiron_ontology-0.1.1/README.md` & `pyiron_ontology-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     Generic: is_more_specific_than()
 ```
 
 With the following key relationships:
 
 ```mermaid
 erDiagram
-    Function ||--|{ Input : has_mandatory
+    Function ||--|{ Input : optional_inputs
     Function ||--o{ Input : mandatory_inputs
     Function ||--|{ Output : outputs
     Input |{--|| Generic : generic
     Output |{--|| Generic : generic
     Input ||--o{ Generic: req
     Input ||--o{ Generic: transitive_req
 ```
@@ -336,8 +336,8 @@
 onto = po.dynamic.atomistics()
 reasoner = AtomisticsReasoner(onto) 
 pr = Project('your_project_tree_with_loads_of_data')
 
 reasoner.search_database_for_property(onto.BulkModulus(), pr)
 ```
 
-If you have `Murnaghan` jobs in your project, this will return a nice little dataframe.
+If you have `Murnaghan` jobs in your project, this will return a nice little dataframe.
```

### Comparing `pyiron_ontology-0.1.1/pyiron_ontology/atomistics/constructor.py` & `pyiron_ontology-0.1.2/pyiron_ontology/atomistics/constructor.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.1/pyiron_ontology/atomistics/reasoning.py` & `pyiron_ontology-0.1.2/pyiron_ontology/atomistics/reasoning.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.1/pyiron_ontology/constructor.py` & `pyiron_ontology-0.1.2/pyiron_ontology/constructor.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.1/pyiron_ontology/dynamic.py` & `pyiron_ontology-0.1.2/pyiron_ontology/dynamic.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.1/pyiron_ontology/example/constructor.py` & `pyiron_ontology-0.1.2/pyiron_ontology/example/constructor.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.1/pyiron_ontology/workflow.py` & `pyiron_ontology-0.1.2/pyiron_ontology/workflow.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.1/pyiron_ontology.egg-info/PKG-INFO` & `pyiron_ontology-0.1.2/pyiron_ontology.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron-ontology
-Version: 0.1.1
+Version: 0.1.2
 Summary: pyiron_ontology - module extension to pyiron.
 Home-page: https://github.com/pyiron/pyiron_ontology
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: liamhuber@greyhavensolutions.com
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyiron_ontology-0.1.1/pyiron_ontology.egg-info/SOURCES.txt` & `pyiron_ontology-0.1.2/pyiron_ontology.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.1/setup.py` & `pyiron_ontology-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,12 +28,12 @@
     packages=find_packages(exclude=["*tests*", "*docs*", "*binder*", "*conda*", "*notebooks*", "*.ci_support*"]),
     install_requires=[
         'numpy',
         'owlready2',
         'pandas',
         'pint',
         'pyiron_atomistics>=0.2.63',
-        'sqlalchemy>=1.4.46',
+        'sqlalchemy',
     ],
     cmdclass=versioneer.get_cmdclass(),
 
     )
```

### Comparing `pyiron_ontology-0.1.1/versioneer.py` & `pyiron_ontology-0.1.2/versioneer.py`

 * *Files identical despite different names*


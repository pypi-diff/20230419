# Comparing `tmp/mongo_to_som-1.0.6.tar.gz` & `tmp/mongo_to_som-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_to_som-1.0.6.tar", last modified: Wed Apr 19 18:14:21 2023, max compression
+gzip compressed data, was "mongo_to_som-1.0.7.tar", last modified: Wed Apr 19 18:16:26 2023, max compression
```

## Comparing `mongo_to_som-1.0.6.tar` & `mongo_to_som-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 18:14:21.051728 mongo_to_som-1.0.6/
--rw-rw-rw-   0        0        0     1143 2023-04-19 18:14:21.049720 mongo_to_som-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-04-07 12:24:07.000000 mongo_to_som-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 18:14:21.043720 mongo_to_som-1.0.6/mongo_to_som/
--rw-rw-rw-   0        0        0       49 2023-04-07 14:06:43.000000 mongo_to_som-1.0.6/mongo_to_som/__init__.py
--rw-rw-rw-   0        0        0     7405 2023-04-19 18:13:44.000000 mongo_to_som-1.0.6/mongo_to_som/mongotosom.py
-drwxrwxrwx   0        0        0        0 2023-04-19 18:14:21.048720 mongo_to_som-1.0.6/mongo_to_som.egg-info/
--rw-rw-rw-   0        0        0     1143 2023-04-19 18:14:20.000000 mongo_to_som-1.0.6/mongo_to_som.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-19 18:14:20.000000 mongo_to_som-1.0.6/mongo_to_som.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 18:14:20.000000 mongo_to_som-1.0.6/mongo_to_som.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-19 18:14:20.000000 mongo_to_som-1.0.6/mongo_to_som.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-19 18:14:20.000000 mongo_to_som-1.0.6/mongo_to_som.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 18:14:21.052721 mongo_to_som-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1428 2023-04-19 18:14:03.000000 mongo_to_som-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:16:26.867682 mongo_to_som-1.0.7/
+-rw-rw-rw-   0        0        0     1140 2023-04-19 18:16:26.867682 mongo_to_som-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-04-19 18:15:58.000000 mongo_to_som-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 18:16:26.861684 mongo_to_som-1.0.7/mongo_to_som/
+-rw-rw-rw-   0        0        0       49 2023-04-07 14:06:43.000000 mongo_to_som-1.0.7/mongo_to_som/__init__.py
+-rw-rw-rw-   0        0        0     7405 2023-04-19 18:13:44.000000 mongo_to_som-1.0.7/mongo_to_som/mongotosom.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:16:26.866681 mongo_to_som-1.0.7/mongo_to_som.egg-info/
+-rw-rw-rw-   0        0        0     1140 2023-04-19 18:16:26.000000 mongo_to_som-1.0.7/mongo_to_som.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-04-19 18:16:26.000000 mongo_to_som-1.0.7/mongo_to_som.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 18:16:26.000000 mongo_to_som-1.0.7/mongo_to_som.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-19 18:16:26.000000 mongo_to_som-1.0.7/mongo_to_som.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-19 18:16:26.000000 mongo_to_som-1.0.7/mongo_to_som.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 18:16:26.867682 mongo_to_som-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1428 2023-04-19 18:16:03.000000 mongo_to_som-1.0.7/setup.py
```

### Comparing `mongo_to_som-1.0.6/PKG-INFO` & `mongo_to_som-1.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo_to_som
-Version: 1.0.6
+Version: 1.0.7
 Summary: Library to create Self-Organizing Map from MongoDB collection
 Home-page: UNKNOWN
 Author: Tomáš Peregrín
 Author-email: djtoso@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -28,11 +28,11 @@
 
 ### Get started
 How to use library:
 
 ```Python
 from mongo_to_som import mongotosom
 
-# Instantiate a Multiplication object
+# Instantiate Mongo to Som Library
 mongotosom.mongo_to_som(num_rows, num_cols, max_steps, max_m_distance, max_learning_rate, url, port, db, collection)
 ```
```

### Comparing `mongo_to_som-1.0.6/mongo_to_som/mongotosom.py` & `mongo_to_som-1.0.7/mongo_to_som/mongotosom.py`

 * *Files identical despite different names*

### Comparing `mongo_to_som-1.0.6/mongo_to_som.egg-info/PKG-INFO` & `mongo_to_som-1.0.7/mongo_to_som.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo-to-som
-Version: 1.0.6
+Version: 1.0.7
 Summary: Library to create Self-Organizing Map from MongoDB collection
 Home-page: UNKNOWN
 Author: Tomáš Peregrín
 Author-email: djtoso@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -28,11 +28,11 @@
 
 ### Get started
 How to use library:
 
 ```Python
 from mongo_to_som import mongotosom
 
-# Instantiate a Multiplication object
+# Instantiate Mongo to Som Library
 mongotosom.mongo_to_som(num_rows, num_cols, max_steps, max_m_distance, max_learning_rate, url, port, db, collection)
 ```
```

### Comparing `mongo_to_som-1.0.6/setup.py` & `mongo_to_som-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="mongo_to_som",
     packages=["mongo_to_som"],
     include_package_data=True,
-    version='1.0.6',
+    version='1.0.7',
     description='Library to create Self-Organizing Map from MongoDB collection',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Tomáš Peregrín',
     author_email="djtoso@gmail.com",
     license='MIT',
     classifiers=[
```


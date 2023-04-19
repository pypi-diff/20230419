# Comparing `tmp/modelreport-0.1.tar.gz` & `tmp/modelreport-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelreport-0.1.tar", last modified: Wed Apr 19 11:48:15 2023, max compression
+gzip compressed data, was "modelreport-0.2.tar", last modified: Wed Apr 19 12:07:12 2023, max compression
```

## Comparing `modelreport-0.1.tar` & `modelreport-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 11:48:15.725785 modelreport-0.1/
--rw-rw-rw-   0        0        0     1062 2023-04-19 11:40:22.000000 modelreport-0.1/LICENSE
--rw-rw-rw-   0        0        0     1370 2023-04-19 11:48:15.723794 modelreport-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-04-19 10:42:14.000000 modelreport-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 11:48:15.624256 modelreport-0.1/modelreport/
--rw-rw-rw-   0        0        0      147 2023-04-19 11:39:09.000000 modelreport-0.1/modelreport/_init_.py
--rw-rw-rw-   0        0        0     2852 2023-04-19 11:38:41.000000 modelreport-0.1/modelreport/metric.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:48:15.719902 modelreport-0.1/modelreport.egg-info/
--rw-rw-rw-   0        0        0     1370 2023-04-19 11:48:15.000000 modelreport-0.1/modelreport.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-04-19 11:48:15.000000 modelreport-0.1/modelreport.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 11:48:15.000000 modelreport-0.1/modelreport.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-19 11:48:15.000000 modelreport-0.1/modelreport.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-19 11:48:15.000000 modelreport-0.1/modelreport.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 11:48:15.725785 modelreport-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1286 2023-04-19 11:48:08.000000 modelreport-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:07:12.837107 modelreport-0.2/
+-rw-rw-rw-   0        0        0     1057 2023-04-19 11:49:04.000000 modelreport-0.2/LICENSE
+-rw-rw-rw-   0        0        0     1391 2023-04-19 12:07:12.831423 modelreport-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2023-04-19 11:59:35.000000 modelreport-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 12:07:12.743130 modelreport-0.2/modelreport/
+-rw-rw-rw-   0        0        0      231 2023-04-19 12:06:41.000000 modelreport-0.2/modelreport/_init_.py
+-rw-rw-rw-   0        0        0     2852 2023-04-19 11:38:41.000000 modelreport-0.2/modelreport/metric.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:07:12.829072 modelreport-0.2/modelreport.egg-info/
+-rw-rw-rw-   0        0        0     1391 2023-04-19 12:07:12.000000 modelreport-0.2/modelreport.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-04-19 12:07:12.000000 modelreport-0.2/modelreport.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:07:12.000000 modelreport-0.2/modelreport.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-19 12:07:12.000000 modelreport-0.2/modelreport.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-19 12:07:12.000000 modelreport-0.2/modelreport.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 12:07:12.837720 modelreport-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1286 2023-04-19 12:04:38.000000 modelreport-0.2/setup.py
```

### Comparing `modelreport-0.1/LICENSE` & `modelreport-0.2/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2021 - Donald Buhl-Brown
+Copyright (c) 2023 - Susmit Panda
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `modelreport-0.1/PKG-INFO` & `modelreport-0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelreport
-Version: 0.1
+Version: 0.2
 Summary: A lightweight library to get the all classification metric scores.
 Author: SusmitPanda
 Author-email: susmit.vssut@gmail.com
 License: MIT
 Keywords: accuracy,confusion_matrix,precision_score,recall_score,f1_score,auc,matthews_corrcoef,cohen_kappa_score,classification report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -26,17 +26,17 @@
 
 
     ```pip install -U modelreport```
 
 Example
 ---------
 
-from modelreport import metrics
+from modelreport.metric import result_summary
 
-print(metrics(test data,predicted data))
+print(result_summary(test data,predicted data))
 
 
 `More Updates Coming Soon...` 😄
 
 
 Contact
 ---------
```

### Comparing `modelreport-0.1/modelreport/metric.py` & `modelreport-0.2/modelreport/metric.py`

 * *Files identical despite different names*

### Comparing `modelreport-0.1/modelreport.egg-info/PKG-INFO` & `modelreport-0.2/modelreport.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelreport
-Version: 0.1
+Version: 0.2
 Summary: A lightweight library to get the all classification metric scores.
 Author: SusmitPanda
 Author-email: susmit.vssut@gmail.com
 License: MIT
 Keywords: accuracy,confusion_matrix,precision_score,recall_score,f1_score,auc,matthews_corrcoef,cohen_kappa_score,classification report
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -26,17 +26,17 @@
 
 
     ```pip install -U modelreport```
 
 Example
 ---------
 
-from modelreport import metrics
+from modelreport.metric import result_summary
 
-print(metrics(test data,predicted data))
+print(result_summary(test data,predicted data))
 
 
 `More Updates Coming Soon...` 😄
 
 
 Contact
 ---------
```

### Comparing `modelreport-0.1/setup.py` & `modelreport-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
   name = 'modelreport',         
   packages = ['modelreport'],  
-  version = '0.1',      
+  version = '0.2',      
   license='MIT',        
   description = 'A lightweight library to get the all classification metric scores.',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author = 'SusmitPanda',                   
   author_email = 'susmit.vssut@gmail.com',  
   install_requires=['scikit-learn','pandas'],
```


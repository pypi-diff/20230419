# Comparing `tmp/ifd_python-7.6.4.tar.gz` & `tmp/ifd_python-7.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifd_python-7.6.4.tar", max compression
+gzip compressed data, was "ifd_python-7.6.5.tar", max compression
```

## Comparing `ifd_python-7.6.4.tar` & `ifd_python-7.6.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.6.4/LICENSE
--rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.6.4/README.md
--rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.6.4/ifd/__init__.py
--rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.6.4/ifd/entities/Abstract/ADetection.py
--rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.6.4/ifd/entities/Abstract/__init__.py
--rw-r--r--   0        0        0      734 2023-04-13 09:26:25.358120 ifd_python-7.6.4/ifd/entities/Classification.py
--rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.6.4/ifd/entities/Couleur.py
--rw-r--r--   0        0        0      707 2023-04-13 09:26:25.358120 ifd_python-7.6.4/ifd/entities/Detection.py
--rw-r--r--   0        0        0     2303 2023-04-19 08:19:41.294208 ifd_python-7.6.4/ifd/entities/Image.py
--rw-r--r--   0        0        0     1332 2023-04-19 09:49:38.767857 ifd_python-7.6.4/ifd/entities/LogResult.py
--rw-r--r--   0        0        0      477 2023-04-13 09:26:25.358120 ifd_python-7.6.4/ifd/entities/Modele.py
--rw-r--r--   0        0        0      666 2023-04-14 14:33:26.310964 ifd_python-7.6.4/ifd/entities/OCR.py
--rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.6.4/ifd/entities/RabbitMqMessage.py
--rw-r--r--   0        0        0      709 2023-04-19 08:27:21.531854 ifd_python-7.6.4/ifd/entities/Tag.py
--rw-r--r--   0        0        0      262 2023-04-19 09:19:06.169869 ifd_python-7.6.4/ifd/entities/__init__.py
--rw-r--r--   0        0        0      717 2023-04-13 09:26:25.358120 ifd_python-7.6.4/ifd/entities/bbox.py
--rw-r--r--   0        0        0     2219 2023-04-14 12:09:37.448293 ifd_python-7.6.4/ifd/repository/AmqpImageRepository.py
--rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.6.4/ifd/repository/Interfaces/IImageRepository.py
--rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.6.4/ifd/repository/Interfaces/__init__.py
--rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.6.4/ifd/repository/MemoryImageRepository.py
--rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.6.4/ifd/repository/__init__.py
--rw-r--r--   0        0        0      644 2023-04-17 07:37:46.512419 ifd_python-7.6.4/ifd/spec.py
--rw-r--r--   0        0        0      526 2023-04-19 08:19:41.298208 ifd_python-7.6.4/ifd/tools.py
--rw-r--r--   0        0        0      131 2023-04-14 12:36:19.030168 ifd_python-7.6.4/ifd/usecase/Interfaces/IFonction.py
--rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.6.4/ifd/usecase/Interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 09:49:54.784050 ifd_python-7.6.4/ifd/usecase/__init__.py
--rw-r--r--   0        0        0      329 2023-04-19 09:50:03.936160 ifd_python-7.6.4/pyproject.toml
--rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 ifd_python-7.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.6.5/LICENSE
+-rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.6.5/README.md
+-rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.6.5/ifd/__init__.py
+-rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.6.5/ifd/entities/Abstract/ADetection.py
+-rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.6.5/ifd/entities/Abstract/__init__.py
+-rw-r--r--   0        0        0      734 2023-04-13 09:26:25.358120 ifd_python-7.6.5/ifd/entities/Classification.py
+-rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.6.5/ifd/entities/Couleur.py
+-rw-r--r--   0        0        0      707 2023-04-13 09:26:25.358120 ifd_python-7.6.5/ifd/entities/Detection.py
+-rw-r--r--   0        0        0     2303 2023-04-19 08:19:41.294208 ifd_python-7.6.5/ifd/entities/Image.py
+-rw-r--r--   0        0        0     1341 2023-04-19 10:22:56.432935 ifd_python-7.6.5/ifd/entities/LogResult.py
+-rw-r--r--   0        0        0      477 2023-04-13 09:26:25.358120 ifd_python-7.6.5/ifd/entities/Modele.py
+-rw-r--r--   0        0        0      666 2023-04-14 14:33:26.310964 ifd_python-7.6.5/ifd/entities/OCR.py
+-rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.6.5/ifd/entities/RabbitMqMessage.py
+-rw-r--r--   0        0        0      709 2023-04-19 08:27:21.531854 ifd_python-7.6.5/ifd/entities/Tag.py
+-rw-r--r--   0        0        0      262 2023-04-19 09:19:06.169869 ifd_python-7.6.5/ifd/entities/__init__.py
+-rw-r--r--   0        0        0      717 2023-04-13 09:26:25.358120 ifd_python-7.6.5/ifd/entities/bbox.py
+-rw-r--r--   0        0        0     2219 2023-04-14 12:09:37.448293 ifd_python-7.6.5/ifd/repository/AmqpImageRepository.py
+-rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.6.5/ifd/repository/Interfaces/IImageRepository.py
+-rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.6.5/ifd/repository/Interfaces/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.6.5/ifd/repository/MemoryImageRepository.py
+-rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.6.5/ifd/repository/__init__.py
+-rw-r--r--   0        0        0      644 2023-04-17 07:37:46.512419 ifd_python-7.6.5/ifd/spec.py
+-rw-r--r--   0        0        0      526 2023-04-19 08:19:41.298208 ifd_python-7.6.5/ifd/tools.py
+-rw-r--r--   0        0        0      131 2023-04-14 12:36:19.030168 ifd_python-7.6.5/ifd/usecase/Interfaces/IFonction.py
+-rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.6.5/ifd/usecase/Interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 10:23:12.341137 ifd_python-7.6.5/ifd/usecase/__init__.py
+-rw-r--r--   0        0        0      329 2023-04-19 10:23:21.689256 ifd_python-7.6.5/pyproject.toml
+-rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 ifd_python-7.6.5/PKG-INFO
```

### Comparing `ifd_python-7.6.4/LICENSE` & `ifd_python-7.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.4/README.md` & `ifd_python-7.6.5/README.md`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.4/ifd/entities/Abstract/ADetection.py` & `ifd_python-7.6.5/ifd/entities/Abstract/ADetection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.4/ifd/entities/Classification.py` & `ifd_python-7.6.5/ifd/entities/Classification.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.4/ifd/entities/Detection.py` & `ifd_python-7.6.5/ifd/entities/Detection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.4/ifd/entities/Image.py` & `ifd_python-7.6.5/ifd/entities/Image.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.4/ifd/entities/LogResult.py` & `ifd_python-7.6.5/ifd/entities/LogResult.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,19 +5,19 @@
     startTime : date de début de l'analyse
     stopTime : date de fin de l'analyse
     duration : durée de l'analyse
     result : le résultat de l'analyse; en cas d'erreur, contient le type d'erreur
     message : contient le message d'erreur en cas d'erreur
     """
     step :str
-    startTime :datetime
-    stopTime:datetime
-    duration:float
-    result:str
-    message:str
+    startTime : datetime
+    stopTime : datetime
+    duration : float
+    result : str
+    message : str
 
     def serialize(self):
         return {
             "step": self.step,
             "startTime": self.startTime,
             "stopTime": self.stopTime,
             "duration": self.duration,
```

### Comparing `ifd_python-7.6.4/ifd/entities/OCR.py` & `ifd_python-7.6.5/ifd/entities/OCR.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.4/ifd/entities/RabbitMqMessage.py` & `ifd_python-7.6.5/ifd/entities/RabbitMqMessage.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.4/ifd/entities/Tag.py` & `ifd_python-7.6.5/ifd/entities/Tag.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.4/ifd/entities/bbox.py` & `ifd_python-7.6.5/ifd/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.4/ifd/repository/AmqpImageRepository.py` & `ifd_python-7.6.5/ifd/repository/AmqpImageRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.4/ifd/spec.py` & `ifd_python-7.6.5/ifd/spec.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.4/ifd/tools.py` & `ifd_python-7.6.5/ifd/tools.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.4/PKG-INFO` & `ifd_python-7.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifd-python
-Version: 7.6.4
+Version: 7.6.5
 Summary: 
 Author: Antonin Lemoine
 Author-email: antonin.lemoine@altitudeinfra.fr
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```


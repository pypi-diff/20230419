# Comparing `tmp/ifd_python-7.6.1.tar.gz` & `tmp/ifd_python-7.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifd_python-7.6.1.tar", max compression
+gzip compressed data, was "ifd_python-7.6.2.tar", max compression
```

## Comparing `ifd_python-7.6.1.tar` & `ifd_python-7.6.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.6.1/LICENSE
--rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.6.1/README.md
--rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/__init__.py
--rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/entities/Abstract/ADetection.py
--rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/entities/Abstract/__init__.py
--rw-r--r--   0        0        0      734 2023-04-13 09:26:25.358120 ifd_python-7.6.1/ifd/entities/Classification.py
--rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/entities/Couleur.py
--rw-r--r--   0        0        0      707 2023-04-13 09:26:25.358120 ifd_python-7.6.1/ifd/entities/Detection.py
--rw-r--r--   0        0        0     2045 2023-04-14 12:09:37.448293 ifd_python-7.6.1/ifd/entities/Image.py
--rw-r--r--   0        0        0     1453 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/entities/LogResult.py
--rw-r--r--   0        0        0      477 2023-04-13 09:26:25.358120 ifd_python-7.6.1/ifd/entities/Modele.py
--rw-r--r--   0        0        0      666 2023-04-14 14:33:26.310964 ifd_python-7.6.1/ifd/entities/OCR.py
--rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/entities/RabbitMqMessage.py
--rw-r--r--   0        0        0      208 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/entities/__init__.py
--rw-r--r--   0        0        0      717 2023-04-13 09:26:25.358120 ifd_python-7.6.1/ifd/entities/bbox.py
--rw-r--r--   0        0        0     2219 2023-04-14 12:09:37.448293 ifd_python-7.6.1/ifd/repository/AmqpImageRepository.py
--rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/repository/Interfaces/IImageRepository.py
--rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/repository/Interfaces/__init__.py
--rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/repository/MemoryImageRepository.py
--rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/repository/__init__.py
--rw-r--r--   0        0        0      644 2023-04-17 07:37:46.512419 ifd_python-7.6.1/ifd/spec.py
--rw-r--r--   0        0        0      558 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/tools.py
--rw-r--r--   0        0        0      131 2023-04-14 12:36:19.030168 ifd_python-7.6.1/ifd/usecase/Interfaces/IFonction.py
--rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.6.1/ifd/usecase/Interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 07:38:02.412258 ifd_python-7.6.1/ifd/usecase/__init__.py
--rw-r--r--   0        0        0      329 2023-04-17 07:38:11.740163 ifd_python-7.6.1/pyproject.toml
--rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 ifd_python-7.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.6.2/LICENSE
+-rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.6.2/README.md
+-rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.6.2/ifd/__init__.py
+-rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.6.2/ifd/entities/Abstract/ADetection.py
+-rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.6.2/ifd/entities/Abstract/__init__.py
+-rw-r--r--   0        0        0      734 2023-04-13 09:26:25.358120 ifd_python-7.6.2/ifd/entities/Classification.py
+-rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.6.2/ifd/entities/Couleur.py
+-rw-r--r--   0        0        0      707 2023-04-13 09:26:25.358120 ifd_python-7.6.2/ifd/entities/Detection.py
+-rw-r--r--   0        0        0     2303 2023-04-19 08:19:41.294208 ifd_python-7.6.2/ifd/entities/Image.py
+-rw-r--r--   0        0        0     1453 2023-04-12 12:43:31.521191 ifd_python-7.6.2/ifd/entities/LogResult.py
+-rw-r--r--   0        0        0      477 2023-04-13 09:26:25.358120 ifd_python-7.6.2/ifd/entities/Modele.py
+-rw-r--r--   0        0        0      666 2023-04-14 14:33:26.310964 ifd_python-7.6.2/ifd/entities/OCR.py
+-rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.6.2/ifd/entities/RabbitMqMessage.py
+-rw-r--r--   0        0        0      709 2023-04-19 08:27:21.531854 ifd_python-7.6.2/ifd/entities/Tag.py
+-rw-r--r--   0        0        0      208 2023-04-12 12:43:31.521191 ifd_python-7.6.2/ifd/entities/__init__.py
+-rw-r--r--   0        0        0      717 2023-04-13 09:26:25.358120 ifd_python-7.6.2/ifd/entities/bbox.py
+-rw-r--r--   0        0        0     2219 2023-04-14 12:09:37.448293 ifd_python-7.6.2/ifd/repository/AmqpImageRepository.py
+-rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.6.2/ifd/repository/Interfaces/IImageRepository.py
+-rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.6.2/ifd/repository/Interfaces/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.6.2/ifd/repository/MemoryImageRepository.py
+-rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.6.2/ifd/repository/__init__.py
+-rw-r--r--   0        0        0      644 2023-04-17 07:37:46.512419 ifd_python-7.6.2/ifd/spec.py
+-rw-r--r--   0        0        0      526 2023-04-19 08:19:41.298208 ifd_python-7.6.2/ifd/tools.py
+-rw-r--r--   0        0        0      131 2023-04-14 12:36:19.030168 ifd_python-7.6.2/ifd/usecase/Interfaces/IFonction.py
+-rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.6.2/ifd/usecase/Interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 08:27:37.936052 ifd_python-7.6.2/ifd/usecase/__init__.py
+-rw-r--r--   0        0        0      329 2023-04-19 08:27:47.068163 ifd_python-7.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 ifd_python-7.6.2/PKG-INFO
```

### Comparing `ifd_python-7.6.1/LICENSE` & `ifd_python-7.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.1/README.md` & `ifd_python-7.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.1/ifd/entities/Abstract/ADetection.py` & `ifd_python-7.6.2/ifd/entities/Abstract/ADetection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.1/ifd/entities/Classification.py` & `ifd_python-7.6.2/ifd/entities/Classification.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.1/ifd/entities/Detection.py` & `ifd_python-7.6.2/ifd/entities/Detection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.1/ifd/entities/Image.py` & `ifd_python-7.6.2/ifd/entities/Image.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from .Classification import Classification
 from .Detection import Detection
+from .Tag import Tag
 from .OCR import OCR
 
 class Image():
     id: int = -1
     img_path : str = ""
     img_checksum: str = ""
     classification: Classification = None
     detections: list = []
+    tags: list = []
     rotation: int = 0
     ocr : OCR = None
     is_blur : bool = False
     
     ref_infra_pto : str = ""
 
     def serialize(self):
         return {
             "id": self.id,
             "img_path": self.img_path,
             "img_checksum": self.img_checksum,
             "rotation": self.rotation,
             "classification": self.classification.serialize() if isinstance(self.classification, Classification) else None,
+            "tags": [tag.serialize() if isinstance(tag, Tag) else None for tag in self.tags],
             "detections": [detection.serialize() if isinstance(detection, Detection) else None for detection in self.detections],
             "ocr": self.ocr.serialize() if isinstance(self.ocr,OCR) else None,
             "ref_infra_pto": self.ref_infra_pto,
             "is_blur": self.is_blur
         }
     def deserialize(self, data):
         
@@ -38,14 +41,16 @@
                 self.img_path = data[field]
             elif field == "img_checksum":
                 self.img_checksum = data[field]
             elif field == "classification":
                 self.classification = Classification().deserialize(data[field])
             elif field == "rotation":
                 self.rotation = data[field]
+            elif field == "tags":
+                self.tags = [Tag().deserialize(element) for element in data[field]]
             elif field == "detections":
                 self.detections = [Detection().deserialize(element) for element in data[field]]
             elif field == "ocr":
                 self.ocr = OCR().deserialize(data[field])
             elif field == "ref_infra_pto":
                 self.ref_infra_pto = data[field]
             elif field == "is_blur":
```

### Comparing `ifd_python-7.6.1/ifd/entities/LogResult.py` & `ifd_python-7.6.2/ifd/entities/LogResult.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.1/ifd/entities/OCR.py` & `ifd_python-7.6.2/ifd/entities/OCR.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.1/ifd/entities/RabbitMqMessage.py` & `ifd_python-7.6.2/ifd/entities/RabbitMqMessage.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.1/ifd/entities/bbox.py` & `ifd_python-7.6.2/ifd/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.1/ifd/repository/AmqpImageRepository.py` & `ifd_python-7.6.2/ifd/repository/AmqpImageRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.1/ifd/spec.py` & `ifd_python-7.6.2/ifd/spec.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.1/PKG-INFO` & `ifd_python-7.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifd-python
-Version: 7.6.1
+Version: 7.6.2
 Summary: 
 Author: Antonin Lemoine
 Author-email: antonin.lemoine@altitudeinfra.fr
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```


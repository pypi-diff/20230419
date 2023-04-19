# Comparing `tmp/promsoft_weight_calc_interface-0.1.4.tar.gz` & `tmp/promsoft_weight_calc_interface-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promsoft_weight_calc_interface-0.1.4.tar", max compression
+gzip compressed data, was "promsoft_weight_calc_interface-0.1.5.tar", max compression
```

## Comparing `promsoft_weight_calc_interface-0.1.4.tar` & `promsoft_weight_calc_interface-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      392 2023-04-14 07:41:57.164500 promsoft_weight_calc_interface-0.1.4/README.md
--rw-r--r--   0        0        0       68 2023-04-07 05:47:16.006748 promsoft_weight_calc_interface-0.1.4/promsoft_weight_calc_interface/__init__.py
--rw-r--r--   0        0        0     1533 2023-04-07 05:47:16.010748 promsoft_weight_calc_interface-0.1.4/promsoft_weight_calc_interface/models.py
--rw-r--r--   0        0        0      521 2023-04-14 07:41:57.164500 promsoft_weight_calc_interface-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 promsoft_weight_calc_interface-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      392 2023-04-14 07:41:57.164500 promsoft_weight_calc_interface-0.1.5/README.md
+-rw-r--r--   0        0        0       68 2023-04-07 05:47:16.006748 promsoft_weight_calc_interface-0.1.5/promsoft_weight_calc_interface/__init__.py
+-rw-r--r--   0        0        0     1575 2023-04-19 05:24:09.630483 promsoft_weight_calc_interface-0.1.5/promsoft_weight_calc_interface/models.py
+-rw-r--r--   0        0        0      521 2023-04-19 05:24:09.630483 promsoft_weight_calc_interface-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 promsoft_weight_calc_interface-0.1.5/PKG-INFO
```

### Comparing `promsoft_weight_calc_interface-0.1.4/promsoft_weight_calc_interface/models.py` & `promsoft_weight_calc_interface-0.1.5/promsoft_weight_calc_interface/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from pydantic import BaseModel, validator, Field
 
 
-# класс для входных данных о товарах
 class Entry(BaseModel):
+    """
+    Класс для входных данных о товарах
+    """
+
     id: int = Field(
         default=0,
         title="The idgood of item.",
         description="Needs to be an integer positive number.",
         example=10004,
     )
     cnt: int = Field(
@@ -25,16 +28,19 @@
     @validator("cnt")
     def check_cnt(cls, v):
         if v < 0:
             raise ValueError("cnt must be >= 0")
         return v
 
 
-# класс для входных данных о товарах с возможностью возврата изначальных размеров
 class ComplEntry(BaseModel):
+    """
+        Класс для входных данных о товарах с возможностью возврата изначальных размеров
+    """
+
     items: list[Entry] = []
     return_sizes_goods: bool = Field(
         default=False,
         title="True if you need to see the initial sizes of all items which ids you wrote in 'id' fields.",
         description="Can only be True or False.",
     )
```

### Comparing `promsoft_weight_calc_interface-0.1.4/pyproject.toml` & `promsoft_weight_calc_interface-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promsoft_weight_calc_interface"
-version = "0.1.4"
+version = "0.1.5"
 description = "Интерфейс для сервиса weight_calc."
 authors = ["Alena Chegodaikina <alena@promsoft.ru>"]
 readme = "README.md"
 packages = [{include = "promsoft_weight_calc_interface"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `promsoft_weight_calc_interface-0.1.4/PKG-INFO` & `promsoft_weight_calc_interface-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promsoft-weight-calc-interface
-Version: 0.1.4
+Version: 0.1.5
 Summary: Интерфейс для сервиса weight_calc.
 Author: Alena Chegodaikina
 Author-email: alena@promsoft.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


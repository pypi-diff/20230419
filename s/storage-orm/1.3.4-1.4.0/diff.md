# Comparing `tmp/storage_orm-1.3.4.tar.gz` & `tmp/storage_orm-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storage_orm-1.3.4.tar", last modified: Thu Mar  2 02:53:32 2023, max compression
+gzip compressed data, was "storage_orm-1.4.0.tar", last modified: Wed Apr 19 07:11:40 2023, max compression
```

## Comparing `storage_orm-1.3.4.tar` & `storage_orm-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 02:53:32.894879 storage_orm-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-03-02 02:53:32.894879 storage_orm-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-03-02 02:53:24.000000 storage_orm-1.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 02:53:32.894879 storage_orm-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-02 02:53:24.000000 storage_orm-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 02:53:32.894879 storage_orm-1.3.4/storage_orm/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-02 02:53:24.000000 storage_orm-1.3.4/storage_orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-02 02:53:24.000000 storage_orm-1.3.4/storage_orm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-02 02:53:24.000000 storage_orm-1.3.4/storage_orm/operation_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 02:53:32.894879 storage_orm-1.3.4/storage_orm/redis_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-02 02:53:24.000000 storage_orm-1.3.4/storage_orm/redis_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-03-02 02:53:24.000000 storage_orm-1.3.4/storage_orm/redis_impl/redis_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    19413 2023-03-02 02:53:24.000000 storage_orm-1.3.4/storage_orm/redis_impl/redis_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-03-02 02:53:24.000000 storage_orm-1.3.4/storage_orm/redis_impl/redis_orm.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-02 02:53:24.000000 storage_orm-1.3.4/storage_orm/storage_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-03-02 02:53:24.000000 storage_orm-1.3.4/storage_orm/storage_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-02 02:53:24.000000 storage_orm-1.3.4/storage_orm/storage_orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 02:53:32.894879 storage_orm-1.3.4/storage_orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-03-02 02:53:32.000000 storage_orm-1.3.4/storage_orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-02 02:53:32.000000 storage_orm-1.3.4/storage_orm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 02:53:32.000000 storage_orm-1.3.4/storage_orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-02 02:53:32.000000 storage_orm-1.3.4/storage_orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-02 02:53:32.000000 storage_orm-1.3.4/storage_orm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:11:40.321634 storage_orm-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-04-19 07:11:40.321634 storage_orm-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-04-19 07:11:29.000000 storage_orm-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 07:11:40.321634 storage_orm-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-19 07:11:29.000000 storage_orm-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:11:40.321634 storage_orm-1.4.0/storage_orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/operation_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:11:40.321634 storage_orm-1.4.0/storage_orm/redis_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/redis_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/redis_impl/redis_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/redis_impl/redis_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/redis_impl/redis_orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/storage_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/storage_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-19 07:11:29.000000 storage_orm-1.4.0/storage_orm/storage_orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:11:40.321634 storage_orm-1.4.0/storage_orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-04-19 07:11:40.000000 storage_orm-1.4.0/storage_orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-19 07:11:40.000000 storage_orm-1.4.0/storage_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 07:11:40.000000 storage_orm-1.4.0/storage_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 07:11:40.000000 storage_orm-1.4.0/storage_orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 07:11:40.000000 storage_orm-1.4.0/storage_orm.egg-info/top_level.txt
```

### Comparing `storage_orm-1.3.4/PKG-INFO` & `storage_orm-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storage_orm
-Version: 1.3.4
+Version: 1.4.0
 Summary: Python for using in-memory storage with ORM
 Home-page: https://github.com/CyberPhysics-Platform/storage-orm
 Download-URL: https://github.com/CyberPhysics-Platform/storage-orm/archive/refs/heads/master.zip
 Author: aarekuha
 Author-email: aarekuha@gmail.ru
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `storage_orm-1.3.4/README.md` & `storage_orm-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `storage_orm-1.3.4/setup.py` & `storage_orm-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.3.4/storage_orm/operation_result.py` & `storage_orm-1.4.0/storage_orm/operation_result.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.3.4/storage_orm/redis_impl/redis_frame.py` & `storage_orm-1.4.0/storage_orm/redis_impl/redis_frame.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.3.4/storage_orm/redis_impl/redis_item.py` & `storage_orm-1.4.0/storage_orm/redis_impl/redis_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -231,43 +231,52 @@
         for field in fields:
             with suppress(pickle.UnpicklingError):
                 if field in items and items[field] and pickle.loads(items[field]) is not None:
                     return False
         return True
 
     @classmethod
+    def _get_src_values_for_meta(cls: Type[T], table: str) -> dict:
+        """ Получение значений данных Meta класса"""
+        src_values_for_meta: dict = dict()
+        src_values: list[str] = table.split(".")
+        for key, position in cls._keys_positions.items():
+            src_values_for_meta[key] = int(src_values[position])
+        return src_values_for_meta
+
+    @classmethod
     def _objects_from_db_items(cls: Type[T], items: dict[bytes, bytes]) -> list[T]:
         """ Формирование cls(RedisItem)-объектов из данных базы """
-        # Подготовка базовых данных для формирования объектов из ключей
-        #   (уникальные ключи, без имён полей)
-        tables: set[str] = {
-            str(key).rsplit(KEYS_DELIMITER, 1)[0]
-            for key in items.keys()
-        }
-        result_items: list[T] = []
-        for table in tables:
-            # Отбор полей с префиксом текущей table
-            fields_src: list[bytes] = list(
-                filter(lambda item: str(item).startswith(table), items)
-            )
-            if cls._all_fields_is_empty(items=items, fields=fields_src):
+        class_fields: dict = {}
+        for redis_key, src_value in items.items():
+            # Определение имени таблицы (без имени поля)
+            table = redis_key.decode().rsplit(KEYS_DELIMITER, 1)[0]
+            # Определение имени поля
+            field_name = redis_key.decode().rsplit(KEYS_DELIMITER, 1)[1]
+
+            if cls._all_fields_is_empty(items=items, fields=[redis_key]):
                 continue
-            fields: dict[str, Any] = {}
-            for field in fields_src:
-                # Формирование атрибутов объекта из присутствующих полей
-                key: str = field.decode().rsplit(KEYS_DELIMITER, 1)[1]
-                fields[key] = pickle.loads(items[field])
-
-            # Формирование Meta из table класса и префикса полученных данных
-            table_args: dict = {}
-            src_values: list[str] = table.split('.')
-            for key, position in cls._keys_positions.items():
-                table_args[key] = src_values[position]
 
-            result_items.append(cls(**(fields | table_args)))
+            # Подготовка базовых данных для формирования объекта
+            if not class_fields.get(table):
+                class_fields[table] = {
+                    field_name: pickle.loads(src_value)
+                }
+            else:
+                class_fields[table] |= {
+                    field_name: pickle.loads(src_value)
+                }
+
+        result_items = []
+        for table, class_args in class_fields.items():
+            src_values_for_meta: dict = cls._get_src_values_for_meta(table=table)
+
+            result_items.append(
+                cls(**(class_args | src_values_for_meta))
+            )
 
         return result_items
 
     @staticmethod
     def _get_list_of_prepared_kwargs(**kwargs: dict) -> list[dict]:
         """
             Подготовка списка фильтров из словарей:
```

### Comparing `storage_orm-1.3.4/storage_orm/redis_impl/redis_orm.py` & `storage_orm-1.4.0/storage_orm/redis_impl/redis_orm.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.3.4/storage_orm/storage_frame.py` & `storage_orm-1.4.0/storage_orm/storage_frame.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.3.4/storage_orm/storage_item.py` & `storage_orm-1.4.0/storage_orm/storage_item.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.3.4/storage_orm/storage_orm.py` & `storage_orm-1.4.0/storage_orm/storage_orm.py`

 * *Files identical despite different names*

### Comparing `storage_orm-1.3.4/storage_orm.egg-info/PKG-INFO` & `storage_orm-1.4.0/storage_orm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: storage-orm
-Version: 1.3.4
+Version: 1.4.0
 Summary: Python for using in-memory storage with ORM
 Home-page: https://github.com/CyberPhysics-Platform/storage-orm
 Download-URL: https://github.com/CyberPhysics-Platform/storage-orm/archive/refs/heads/master.zip
 Author: aarekuha
 Author-email: aarekuha@gmail.ru
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
```


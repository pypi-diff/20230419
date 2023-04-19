# Comparing `tmp/aiostorage_orm-1.3.4.tar.gz` & `tmp/aiostorage_orm-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiostorage_orm-1.3.4.tar", last modified: Thu Mar  2 02:54:09 2023, max compression
+gzip compressed data, was "aiostorage_orm-1.4.0.tar", last modified: Wed Apr 19 07:12:35 2023, max compression
```

## Comparing `aiostorage_orm-1.3.4.tar` & `aiostorage_orm-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 02:54:09.319683 aiostorage_orm-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-03-02 02:54:09.319683 aiostorage_orm-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-03-02 02:54:00.000000 aiostorage_orm-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 02:54:09.315683 aiostorage_orm-1.3.4/aiostorage_orm/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-02 02:54:00.000000 aiostorage_orm-1.3.4/aiostorage_orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-02 02:54:00.000000 aiostorage_orm-1.3.4/aiostorage_orm/aiostorage_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-03-02 02:54:00.000000 aiostorage_orm-1.3.4/aiostorage_orm/aiostorage_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-02 02:54:00.000000 aiostorage_orm-1.3.4/aiostorage_orm/aiostorage_orm.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-02 02:54:00.000000 aiostorage_orm-1.3.4/aiostorage_orm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-02 02:54:00.000000 aiostorage_orm-1.3.4/aiostorage_orm/operation_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 02:54:09.319683 aiostorage_orm-1.3.4/aiostorage_orm/redis_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-02 02:54:00.000000 aiostorage_orm-1.3.4/aiostorage_orm/redis_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-03-02 02:54:00.000000 aiostorage_orm-1.3.4/aiostorage_orm/redis_impl/aioredis_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    19712 2023-03-02 02:54:00.000000 aiostorage_orm-1.3.4/aiostorage_orm/redis_impl/aioredis_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-03-02 02:54:00.000000 aiostorage_orm-1.3.4/aiostorage_orm/redis_impl/aioredis_orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 02:54:09.319683 aiostorage_orm-1.3.4/aiostorage_orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-03-02 02:54:09.000000 aiostorage_orm-1.3.4/aiostorage_orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-02 02:54:09.000000 aiostorage_orm-1.3.4/aiostorage_orm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 02:54:09.000000 aiostorage_orm-1.3.4/aiostorage_orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-02 02:54:09.000000 aiostorage_orm-1.3.4/aiostorage_orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-02 02:54:09.000000 aiostorage_orm-1.3.4/aiostorage_orm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 02:54:09.319683 aiostorage_orm-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-02 02:54:00.000000 aiostorage_orm-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:12:35.805313 aiostorage_orm-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-04-19 07:12:35.805313 aiostorage_orm-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:12:35.801313 aiostorage_orm-1.4.0/aiostorage_orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/aiostorage_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/aiostorage_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/aiostorage_orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/operation_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:12:35.805313 aiostorage_orm-1.4.0/aiostorage_orm/redis_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/redis_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/redis_impl/aioredis_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19859 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/redis_impl/aioredis_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/aiostorage_orm/redis_impl/aioredis_orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:12:35.805313 aiostorage_orm-1.4.0/aiostorage_orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-04-19 07:12:35.000000 aiostorage_orm-1.4.0/aiostorage_orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-19 07:12:35.000000 aiostorage_orm-1.4.0/aiostorage_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 07:12:35.000000 aiostorage_orm-1.4.0/aiostorage_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 07:12:35.000000 aiostorage_orm-1.4.0/aiostorage_orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 07:12:35.000000 aiostorage_orm-1.4.0/aiostorage_orm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 07:12:35.805313 aiostorage_orm-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-19 07:12:25.000000 aiostorage_orm-1.4.0/setup.py
```

### Comparing `aiostorage_orm-1.3.4/PKG-INFO` & `aiostorage_orm-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiostorage_orm
-Version: 1.3.4
+Version: 1.4.0
 Summary: Python for using in-memory storage with ORM
 Home-page: https://github.com/CyberPhysics-Platform/aiostorage-orm
 Download-URL: https://github.com/CyberPhysics-Platform/aiostorage-orm/archive/refs/heads/master.zip
 Author: aarekuha
 Author-email: aarekuha@gmail.ru
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiostorage_orm-1.3.4/README.md` & `aiostorage_orm-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.3.4/aiostorage_orm/aiostorage_frame.py` & `aiostorage_orm-1.4.0/aiostorage_orm/aiostorage_frame.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.3.4/aiostorage_orm/aiostorage_item.py` & `aiostorage_orm-1.4.0/aiostorage_orm/aiostorage_item.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.3.4/aiostorage_orm/aiostorage_orm.py` & `aiostorage_orm-1.4.0/aiostorage_orm/aiostorage_orm.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.3.4/aiostorage_orm/operation_result.py` & `aiostorage_orm-1.4.0/aiostorage_orm/operation_result.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.3.4/aiostorage_orm/redis_impl/aioredis_frame.py` & `aiostorage_orm-1.4.0/aiostorage_orm/redis_impl/aioredis_frame.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.3.4/aiostorage_orm/redis_impl/aioredis_item.py` & `aiostorage_orm-1.4.0/aiostorage_orm/redis_impl/aioredis_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -239,43 +239,52 @@
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
-        """ Формирование cls(AIORedisItem)-объектов из данных базы """
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
+        """ Формирование cls(RedisItem)-объектов из данных базы """
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

### Comparing `aiostorage_orm-1.3.4/aiostorage_orm/redis_impl/aioredis_orm.py` & `aiostorage_orm-1.4.0/aiostorage_orm/redis_impl/aioredis_orm.py`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.3.4/aiostorage_orm.egg-info/PKG-INFO` & `aiostorage_orm-1.4.0/aiostorage_orm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiostorage-orm
-Version: 1.3.4
+Version: 1.4.0
 Summary: Python for using in-memory storage with ORM
 Home-page: https://github.com/CyberPhysics-Platform/aiostorage-orm
 Download-URL: https://github.com/CyberPhysics-Platform/aiostorage-orm/archive/refs/heads/master.zip
 Author: aarekuha
 Author-email: aarekuha@gmail.ru
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiostorage_orm-1.3.4/aiostorage_orm.egg-info/SOURCES.txt` & `aiostorage_orm-1.4.0/aiostorage_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiostorage_orm-1.3.4/setup.py` & `aiostorage_orm-1.4.0/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/client_bank_1c-0.2.1.tar.gz` & `tmp/client_bank_1c-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_bank_1c-0.2.1.tar", max compression
+gzip compressed data, was "client_bank_1c-0.2.2.tar", max compression
```

## Comparing `client_bank_1c-0.2.1.tar` & `client_bank_1c-0.2.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1057 2023-04-04 23:35:03.689527 client_bank_1c-0.2.1/LICENSE
--rw-r--r--   0        0        0     4434 2023-04-18 00:28:36.705671 client_bank_1c-0.2.1/client_bank_1c.py
--rw-r--r--   0        0        0      888 2023-04-18 00:53:28.538979 client_bank_1c-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 client_bank_1c-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-04-04 23:35:03.689527 client_bank_1c-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4478 2023-04-19 07:17:04.187385 client_bank_1c-0.2.2/client_bank_1c.py
+-rw-r--r--   0        0        0      888 2023-04-19 07:19:28.631007 client_bank_1c-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 client_bank_1c-0.2.2/PKG-INFO
```

### Comparing `client_bank_1c-0.2.1/LICENSE` & `client_bank_1c-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `client_bank_1c-0.2.1/client_bank_1c.py` & `client_bank_1c-0.2.2/client_bank_1c.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,22 +91,26 @@
                     section_values[key] = value
 
         info, accounts, documents = self._process_result(info, accounts, documents)
         return self.result_class(info, accounts, documents)
 
     def _parse_line(self, line):
         key, value = self.LINE_REGEXP.match(line).groups()
+        if not value:
+            return key, value
+
         if 'Дата' in key:
             value = datetime.datetime.strptime(value, '%d.%m.%Y').date()
         elif 'Время' in key:
             value = datetime.datetime.strptime(value, '%H:%M:%S').time()
         elif key in self.MONEY_FIELDS:
             value = self.money_type(value)
-        elif key in self.NUMBER_FIELDS and value:
+        elif key in self.NUMBER_FIELDS:
             value = int(value)
+
         return key, value
 
     def _process_result(self, info, accounts, documents):
         if self.fill_collected_fields:
             for document in documents:
                 if 'Получатель' not in document:
                     self._fill_collected_field(document, 'Получатель')
```

### Comparing `client_bank_1c-0.2.1/pyproject.toml` & `client_bank_1c-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "client-bank-1c"
-version = "0.2.1"
+version = "0.2.2"
 description = "1C Client Bank Exchange Format"
 authors = ["Dmitry Voronin <dimka665@gmail.com>"]
 
 repository = "https://github.com/odoo-ru/client-bank-1c"
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `client_bank_1c-0.2.1/PKG-INFO` & `client_bank_1c-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: client-bank-1c
-Version: 0.2.1
+Version: 0.2.2
 Summary: 1C Client Bank Exchange Format
 Home-page: https://github.com/odoo-ru/client-bank-1c
 License: MIT
 Author: Dmitry Voronin
 Author-email: dimka665@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Intended Audience :: Developers
```


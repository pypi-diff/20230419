# Comparing `tmp/postgres_data_faker-1.1.1.tar.gz` & `tmp/postgres_data_faker-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgres_data_faker-1.1.1.tar", max compression
+gzip compressed data, was "postgres_data_faker-1.1.2.tar", max compression
```

## Comparing `postgres_data_faker-1.1.1.tar` & `postgres_data_faker-1.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-04-19 14:22:20.355332 postgres_data_faker-1.1.1/postgres_data_faker/__init__.py
--rw-r--r--   0        0        0     3621 2023-04-19 14:27:27.371472 postgres_data_faker-1.1.1/postgres_data_faker/data_faker.py
--rw-r--r--   0        0        0      385 2023-04-19 14:47:17.645102 postgres_data_faker-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      669 2023-04-19 14:44:20.568175 postgres_data_faker-1.1.1/README.md
--rw-r--r--   0        0        0     1360 1970-01-01 00:00:00.000000 postgres_data_faker-1.1.1/setup.py
--rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 postgres_data_faker-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-19 14:59:44.457121 postgres_data_faker-1.1.2/postgres_data_faker/__init__.py
+-rw-r--r--   0        0        0     3621 2023-04-19 14:59:44.457121 postgres_data_faker-1.1.2/postgres_data_faker/data_faker.py
+-rw-r--r--   0        0        0      385 2023-04-19 15:00:10.057988 postgres_data_faker-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      674 2023-04-19 15:00:26.153224 postgres_data_faker-1.1.2/README.md
+-rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 postgres_data_faker-1.1.2/setup.py
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 postgres_data_faker-1.1.2/PKG-INFO
```

### Comparing `postgres_data_faker-1.1.1/postgres_data_faker/data_faker.py` & `postgres_data_faker-1.1.2/postgres_data_faker/data_faker.py`

 * *Files identical despite different names*

### Comparing `postgres_data_faker-1.1.1/README.md` & `postgres_data_faker-1.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Postgres data faker
+# Postgres data faker 🧹
 
 ---
 
 - install package with:
   - pip: `pip install postgres-data-faker`
   - poetry: `poetry add postgres-data-faker`
 - import module with `from postgres_data_faker import data_faker`
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `postgres_data_faker-1.1.1/setup.py` & `postgres_data_faker-1.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['faker>=18.4.0,<19.0.0', 'psycopg2>=2.9.6,<3.0.0']
 
 setup_kwargs = {
     'name': 'postgres-data-faker',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'Dummy and simple faker sensitive data for postgres database',
-    'long_description': '# Postgres data faker\n\n---\n\n- install package with:\n  - pip: `pip install postgres-data-faker`\n  - poetry: `poetry add postgres-data-faker`\n- import module with `from postgres_data_faker import data_faker`\n- using func `data_faker.faking_table(enter name of your table here)`\n---\n- available table names:\n  - customer: will fake columns (**ordered!**):\n    - phone\n    - email\n    - firstname\n    - lastname\n  - recipient: similar to customer\n  - customer address: will fake columns (**also ordered!**):\n    - address_text\n    - postal_code\n---\n\n- connection data stored ad `.env` file, so you must create and fill it with your database parameters',
+    'long_description': '# Postgres data faker 🧹\n\n---\n\n- install package with:\n  - pip: `pip install postgres-data-faker`\n  - poetry: `poetry add postgres-data-faker`\n- import module with `from postgres_data_faker import data_faker`\n- using func `data_faker.faking_table(enter name of your table here)`\n---\n- available table names:\n  - customer: will fake columns (**ordered!**):\n    - phone\n    - email\n    - firstname\n    - lastname\n  - recipient: similar to customer\n  - customer address: will fake columns (**also ordered!**):\n    - address_text\n    - postal_code\n---\n\n- connection data stored ad `.env` file, so you must create and fill it with your database parameters',
     'author': 'Borteq2',
     'author_email': 'borteq2@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `postgres_data_faker-1.1.1/PKG-INFO` & `postgres_data_faker-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: postgres-data-faker
-Version: 1.1.1
+Version: 1.1.2
 Summary: Dummy and simple faker sensitive data for postgres database
 Author: Borteq2
 Author-email: borteq2@yandex.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faker (>=18.4.0,<19.0.0)
 Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
 Description-Content-Type: text/markdown
 
-# Postgres data faker
+# Postgres data faker 🧹
 
 ---
 
 - install package with:
   - pip: `pip install postgres-data-faker`
   - poetry: `poetry add postgres-data-faker`
 - import module with `from postgres_data_faker import data_faker`
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


# Comparing `tmp/postgres_data_faker-1.1.0.tar.gz` & `tmp/postgres_data_faker-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgres_data_faker-1.1.0.tar", max compression
+gzip compressed data, was "postgres_data_faker-1.1.1.tar", max compression
```

## Comparing `postgres_data_faker-1.1.0.tar` & `postgres_data_faker-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-04-19 13:08:30.443772 postgres_data_faker-1.1.0/postgres_data_faker/__init__.py
--rw-r--r--   0        0        0     3619 2023-04-19 14:13:16.377428 postgres_data_faker-1.1.0/postgres_data_faker/main.py
--rw-r--r--   0        0        0      326 2023-04-19 14:13:32.140621 postgres_data_faker-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-19 13:09:23.435917 postgres_data_faker-1.1.0/README.md
--rw-r--r--   0        0        0      632 1970-01-01 00:00:00.000000 postgres_data_faker-1.1.0/setup.py
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 postgres_data_faker-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-19 14:22:20.355332 postgres_data_faker-1.1.1/postgres_data_faker/__init__.py
+-rw-r--r--   0        0        0     3621 2023-04-19 14:27:27.371472 postgres_data_faker-1.1.1/postgres_data_faker/data_faker.py
+-rw-r--r--   0        0        0      385 2023-04-19 14:47:17.645102 postgres_data_faker-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      669 2023-04-19 14:44:20.568175 postgres_data_faker-1.1.1/README.md
+-rw-r--r--   0        0        0     1360 1970-01-01 00:00:00.000000 postgres_data_faker-1.1.1/setup.py
+-rw-r--r--   0        0        0     1129 1970-01-01 00:00:00.000000 postgres_data_faker-1.1.1/PKG-INFO
```

### Comparing `postgres_data_faker-1.1.0/postgres_data_faker/main.py` & `postgres_data_faker-1.1.1/postgres_data_faker/data_faker.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def next_value(lst):
     for tup in lst:
         for value in tup:
             yield value
 
 
-def data_faking(tablename: str):
+def faking_table(tablename: str):
     try:
         with closing(psycopg2.connect(
                 dbname=os.getenv('POSTGRES_DB'),
                 user=os.getenv('POSTGRES_USER'),
                 password=os.getenv('POSTGRES_PASSWORD'),
                 host=os.getenv('POSTGRES_HOST'),
                 port=os.getenv('POSTGRES_PORT')
@@ -89,8 +89,8 @@
 
 
 if __name__ == '__main__':
     # main(tablename='customer')
     # main(tablename='recipient')
     # main(tablename='customer_address')
 
-    data_faking(tablename=input('Table name for faking: '))
+    faking_table(tablename=input('Table name for faking: '))
```


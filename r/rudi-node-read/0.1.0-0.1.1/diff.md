# Comparing `tmp/rudi-node-read-0.1.0.tar.gz` & `tmp/rudi-node-read-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rudi-node-read-0.1.0.tar", last modified: Wed Apr 19 13:04:59 2023, max compression
+gzip compressed data, was "rudi-node-read-0.1.1.tar", last modified: Wed Apr 19 13:19:19 2023, max compression
```

## Comparing `rudi-node-read-0.1.0.tar` & `rudi-node-read-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:04:59.233121 rudi-node-read-0.1.0/
--rw-rw-r--   0 omartine (660741) dept-aac (29120)    13840 2022-03-30 12:00:55.000000 rudi-node-read-0.1.0/LICENCE.md
--rw-rw-r--   0 omartine (660741) dept-aac (29120)     1811 2023-04-19 13:04:59.232725 rudi-node-read-0.1.0/PKG-INFO
--rw-r--r--   0 omartine (660741) dept-aac (29120)      732 2023-04-19 13:01:54.000000 rudi-node-read-0.1.0/README.md
--rw-r--r--   0 omartine (660741) dept-aac (29120)     1269 2023-04-19 13:03:07.000000 rudi-node-read-0.1.0/pyproject.toml
--rw-rw-r--   0 omartine (660741) dept-aac (29120)       38 2023-04-19 13:04:59.233271 rudi-node-read-0.1.0/setup.cfg
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:04:59.220399 rudi-node-read-0.1.0/src/
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:04:59.223110 rudi-node-read-0.1.0/src/rudi_node_read/
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:04:59.226910 rudi-node-read-0.1.0/src/rudi_node_read/connectors/
--rw-r--r--   0 omartine (660741) dept-aac (29120)     5148 2023-04-19 12:30:07.000000 rudi-node-read-0.1.0/src/rudi_node_read/connectors/io_connector.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)     3993 2023-04-19 12:57:38.000000 rudi-node-read-0.1.0/src/rudi_node_read/connectors/io_rudi_api.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)    19661 2023-04-19 12:52:26.000000 rudi-node-read-0.1.0/src/rudi_node_read/rudi_node_reader.py
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:04:59.232008 rudi-node-read-0.1.0/src/rudi_node_read/utils/
--rw-r--r--   0 omartine (660741) dept-aac (29120)     2037 2023-04-19 12:31:16.000000 rudi-node-read-0.1.0/src/rudi_node_read/utils/err.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)      834 2023-03-31 08:32:41.000000 rudi-node-read-0.1.0/src/rudi_node_read/utils/jwt.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)     1355 2023-04-19 12:57:54.000000 rudi-node-read-0.1.0/src/rudi_node_read/utils/log.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)      308 2023-04-04 08:52:42.000000 rudi-node-read-0.1.0/src/rudi_node_read/utils/serializable.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)     8436 2023-04-19 12:31:29.000000 rudi-node-read-0.1.0/src/rudi_node_read/utils/type_dict.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)     2548 2023-04-19 12:31:32.000000 rudi-node-read-0.1.0/src/rudi_node_read/utils/type_string.py
--rw-r--r--   0 omartine (660741) dept-aac (29120)     1495 2023-04-19 12:31:35.000000 rudi-node-read-0.1.0/src/rudi_node_read/utils/types.py
-drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:04:59.225913 rudi-node-read-0.1.0/src/rudi_node_read.egg-info/
--rw-rw-r--   0 omartine (660741) dept-aac (29120)     1811 2023-04-19 13:04:59.000000 rudi-node-read-0.1.0/src/rudi_node_read.egg-info/PKG-INFO
--rw-rw-r--   0 omartine (660741) dept-aac (29120)      623 2023-04-19 13:04:59.000000 rudi-node-read-0.1.0/src/rudi_node_read.egg-info/SOURCES.txt
--rw-rw-r--   0 omartine (660741) dept-aac (29120)        1 2023-04-19 13:04:59.000000 rudi-node-read-0.1.0/src/rudi_node_read.egg-info/dependency_links.txt
--rw-rw-r--   0 omartine (660741) dept-aac (29120)       56 2023-04-19 13:04:59.000000 rudi-node-read-0.1.0/src/rudi_node_read.egg-info/requires.txt
--rw-rw-r--   0 omartine (660741) dept-aac (29120)       15 2023-04-19 13:04:59.000000 rudi-node-read-0.1.0/src/rudi_node_read.egg-info/top_level.txt
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:19:19.817991 rudi-node-read-0.1.1/
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)    13840 2022-03-30 12:00:55.000000 rudi-node-read-0.1.1/LICENCE.md
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     1807 2023-04-19 13:19:19.817659 rudi-node-read-0.1.1/PKG-INFO
+-rw-r--r--   0 omartine (660741) dept-aac (29120)      728 2023-04-19 13:12:30.000000 rudi-node-read-0.1.1/README.md
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     1269 2023-04-19 13:12:52.000000 rudi-node-read-0.1.1/pyproject.toml
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)       38 2023-04-19 13:19:19.818101 rudi-node-read-0.1.1/setup.cfg
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:19:19.805365 rudi-node-read-0.1.1/src/
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:19:19.808069 rudi-node-read-0.1.1/src/rudi_node_read/
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:19:19.811608 rudi-node-read-0.1.1/src/rudi_node_read/connectors/
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     5148 2023-04-19 12:30:07.000000 rudi-node-read-0.1.1/src/rudi_node_read/connectors/io_connector.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     3993 2023-04-19 12:57:38.000000 rudi-node-read-0.1.1/src/rudi_node_read/connectors/io_rudi_api.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)    19661 2023-04-19 12:52:26.000000 rudi-node-read-0.1.1/src/rudi_node_read/rudi_node_reader.py
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:19:19.817049 rudi-node-read-0.1.1/src/rudi_node_read/utils/
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     2037 2023-04-19 12:31:16.000000 rudi-node-read-0.1.1/src/rudi_node_read/utils/err.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)      834 2023-03-31 08:32:41.000000 rudi-node-read-0.1.1/src/rudi_node_read/utils/jwt.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     1355 2023-04-19 12:57:54.000000 rudi-node-read-0.1.1/src/rudi_node_read/utils/log.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)      308 2023-04-04 08:52:42.000000 rudi-node-read-0.1.1/src/rudi_node_read/utils/serializable.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     8436 2023-04-19 12:31:29.000000 rudi-node-read-0.1.1/src/rudi_node_read/utils/type_dict.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     2548 2023-04-19 12:31:32.000000 rudi-node-read-0.1.1/src/rudi_node_read/utils/type_string.py
+-rw-r--r--   0 omartine (660741) dept-aac (29120)     1495 2023-04-19 12:31:35.000000 rudi-node-read-0.1.1/src/rudi_node_read/utils/types.py
+drwxrwxr-x   0 omartine (660741) dept-aac (29120)        0 2023-04-19 13:19:19.810458 rudi-node-read-0.1.1/src/rudi_node_read.egg-info/
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)     1807 2023-04-19 13:19:19.000000 rudi-node-read-0.1.1/src/rudi_node_read.egg-info/PKG-INFO
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)      623 2023-04-19 13:19:19.000000 rudi-node-read-0.1.1/src/rudi_node_read.egg-info/SOURCES.txt
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)        1 2023-04-19 13:19:19.000000 rudi-node-read-0.1.1/src/rudi_node_read.egg-info/dependency_links.txt
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)       56 2023-04-19 13:19:19.000000 rudi-node-read-0.1.1/src/rudi_node_read.egg-info/requires.txt
+-rw-rw-r--   0 omartine (660741) dept-aac (29120)       15 2023-04-19 13:19:19.000000 rudi-node-read-0.1.1/src/rudi_node_read.egg-info/top_level.txt
```

### Comparing `rudi-node-read-0.1.0/LICENCE.md` & `rudi-node-read-0.1.1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.0/PKG-INFO` & `rudi-node-read-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudi-node-read
-Version: 0.1.0
+Version: 0.1.1
 Summary: Use the external API of a RUDI Producer node
 Author-email: Olivier Martineau <olivier.martineau@irisa.fr>
 License: EUPL-1.2
 Project-URL: repository, https://github.com/OlivierMartineau/rudi-node-read
 Project-URL: documentation, https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER
 Project-URL: changelog, https://github.com/OlivierMartineau/rudi-node-read/blob/release/CHANGELOG.md
 Keywords: RUDI,producer node,RUDI node,open-data,Univ. Rennes
@@ -24,15 +24,15 @@
 
 # RUDI Node tools: _rudi-node-read_ library
 
 This library offers tools to take advantage of
 the [external API](https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER) of a RUDI Producer node (also
 referred as RUDI node).
 
-The Jupyter notebook [README.ipynb](doc/README.ipynb) offers an overview of the available functionalities.
+The Jupyter notebook [README.ipynb](README.ipynb) offers an overview of the available functionalities.
 
 ## Installation
 
 ```bash
 $ pip install rudi_node_read
 ```
```

### Comparing `rudi-node-read-0.1.0/README.md` & `rudi-node-read-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # RUDI Node tools: _rudi-node-read_ library
 
 This library offers tools to take advantage of
 the [external API](https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER) of a RUDI Producer node (also
 referred as RUDI node).
 
-The Jupyter notebook [README.ipynb](doc/README.ipynb) offers an overview of the available functionalities.
+The Jupyter notebook [README.ipynb](README.ipynb) offers an overview of the available functionalities.
 
 ## Installation
 
 ```bash
 $ pip install rudi_node_read
 ```
```

### Comparing `rudi-node-read-0.1.0/pyproject.toml` & `rudi-node-read-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rudi-node-read"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name = "Olivier Martineau", email = "olivier.martineau@irisa.fr" }]
 description = "Use the external API of a RUDI Producer node"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "EUPL-1.2" }
 classifiers = ["Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
```

### Comparing `rudi-node-read-0.1.0/src/rudi_node_read/connectors/io_connector.py` & `rudi-node-read-0.1.1/src/rudi_node_read/connectors/io_connector.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.0/src/rudi_node_read/connectors/io_rudi_api.py` & `rudi-node-read-0.1.1/src/rudi_node_read/connectors/io_rudi_api.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.0/src/rudi_node_read/rudi_node_reader.py` & `rudi-node-read-0.1.1/src/rudi_node_read/rudi_node_reader.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.0/src/rudi_node_read/utils/err.py` & `rudi-node-read-0.1.1/src/rudi_node_read/utils/err.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.0/src/rudi_node_read/utils/jwt.py` & `rudi-node-read-0.1.1/src/rudi_node_read/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.0/src/rudi_node_read/utils/log.py` & `rudi-node-read-0.1.1/src/rudi_node_read/utils/log.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.0/src/rudi_node_read/utils/type_dict.py` & `rudi-node-read-0.1.1/src/rudi_node_read/utils/type_dict.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.0/src/rudi_node_read/utils/type_string.py` & `rudi-node-read-0.1.1/src/rudi_node_read/utils/type_string.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.0/src/rudi_node_read/utils/types.py` & `rudi-node-read-0.1.1/src/rudi_node_read/utils/types.py`

 * *Files identical despite different names*

### Comparing `rudi-node-read-0.1.0/src/rudi_node_read.egg-info/PKG-INFO` & `rudi-node-read-0.1.1/src/rudi_node_read.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudi-node-read
-Version: 0.1.0
+Version: 0.1.1
 Summary: Use the external API of a RUDI Producer node
 Author-email: Olivier Martineau <olivier.martineau@irisa.fr>
 License: EUPL-1.2
 Project-URL: repository, https://github.com/OlivierMartineau/rudi-node-read
 Project-URL: documentation, https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER
 Project-URL: changelog, https://github.com/OlivierMartineau/rudi-node-read/blob/release/CHANGELOG.md
 Keywords: RUDI,producer node,RUDI node,open-data,Univ. Rennes
@@ -24,15 +24,15 @@
 
 # RUDI Node tools: _rudi-node-read_ library
 
 This library offers tools to take advantage of
 the [external API](https://app.swaggerhub.com/apis/OlivierMartineau/RUDI-PRODUCER) of a RUDI Producer node (also
 referred as RUDI node).
 
-The Jupyter notebook [README.ipynb](doc/README.ipynb) offers an overview of the available functionalities.
+The Jupyter notebook [README.ipynb](README.ipynb) offers an overview of the available functionalities.
 
 ## Installation
 
 ```bash
 $ pip install rudi_node_read
 ```
```

### Comparing `rudi-node-read-0.1.0/src/rudi_node_read.egg-info/SOURCES.txt` & `rudi-node-read-0.1.1/src/rudi_node_read.egg-info/SOURCES.txt`

 * *Files identical despite different names*


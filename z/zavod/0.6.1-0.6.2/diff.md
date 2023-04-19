# Comparing `tmp/zavod-0.6.1.tar.gz` & `tmp/zavod-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zavod-0.6.1.tar", last modified: Wed Apr  5 17:23:48 2023, max compression
+gzip compressed data, was "zavod-0.6.2.tar", last modified: Wed Apr 19 18:11:30 2023, max compression
```

## Comparing `zavod-0.6.1.tar` & `zavod-0.6.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:23:48.887280 zavod-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-05 17:21:56.000000 zavod-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-05 17:21:56.000000 zavod-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-05 17:23:48.887280 zavod-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-05 17:21:56.000000 zavod-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 17:23:48.887280 zavod-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-05 17:21:56.000000 zavod-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:23:48.883280 zavod-0.6.1/zavod/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:23:48.887280 zavod-0.6.1/zavod/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/parse/addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/parse/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/parse/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:23:48.887280 zavod-0.6.1/zavod/sinks/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/sinks/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/sinks/json_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/sinks/json_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-05 17:21:56.000000 zavod-0.6.1/zavod/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 17:23:48.883280 zavod-0.6.1/zavod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-05 17:23:48.000000 zavod-0.6.1/zavod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-05 17:23:48.000000 zavod-0.6.1/zavod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 17:23:48.000000 zavod-0.6.1/zavod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-05 17:23:48.000000 zavod-0.6.1/zavod.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 17:23:48.000000 zavod-0.6.1/zavod.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 17:23:30.000000 zavod-0.6.1/zavod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-05 17:23:48.000000 zavod-0.6.1/zavod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-05 17:23:48.000000 zavod-0.6.1/zavod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:11:30.937906 zavod-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-19 18:09:39.000000 zavod-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-19 18:09:39.000000 zavod-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-19 18:11:30.937906 zavod-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 18:09:39.000000 zavod-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:11:30.937906 zavod-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-19 18:09:39.000000 zavod-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:11:30.937906 zavod-0.6.2/zavod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:11:30.937906 zavod-0.6.2/zavod/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/parse/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/parse/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/parse/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:11:30.937906 zavod-0.6.2/zavod/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/sinks/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/sinks/json_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/sinks/json_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-19 18:09:39.000000 zavod-0.6.2/zavod/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:11:30.937906 zavod-0.6.2/zavod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-19 18:11:30.000000 zavod-0.6.2/zavod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-19 18:11:30.000000 zavod-0.6.2/zavod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:11:30.000000 zavod-0.6.2/zavod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-19 18:11:30.000000 zavod-0.6.2/zavod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:11:30.000000 zavod-0.6.2/zavod.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:11:13.000000 zavod-0.6.2/zavod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-19 18:11:30.000000 zavod-0.6.2/zavod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 18:11:30.000000 zavod-0.6.2/zavod.egg-info/top_level.txt
```

### Comparing `zavod-0.6.1/LICENSE` & `zavod-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zavod-0.6.1/PKG-INFO` & `zavod-0.6.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zavod
-Version: 0.6.1
+Version: 0.6.2
 Summary: Data factory for followthemoney data.
 Home-page: https://github.com/opensanctions/zavod
 Author: Friedrich Lindenberg
 Author-email: friedrich@opensanctions.org
 License: MIT
 Keywords: data mapping identity followthemoney etl parsing
 Platform: UNKNOWN
```

### Comparing `zavod-0.6.1/setup.py` & `zavod-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="zavod",
-    version="0.6.1",
+    version="0.6.2",
     description="Data factory for followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney etl parsing",
     author="Friedrich Lindenberg",
     author_email="friedrich@opensanctions.org",
     url="https://github.com/opensanctions/zavod",
```

### Comparing `zavod-0.6.1/zavod/__init__.py` & `zavod-0.6.2/zavod/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from zavod import settings
 from zavod.context import GenericZavod
 from zavod.dataset import ZavodDataset, ZD
 from zavod.logs import configure_logging, get_logger
 from zavod.sinks.common import Sink
 from zavod.sinks.json_entity import JSONEntitySink
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 __all__ = [
     "init",
     "context",
     "Zavod",
     "ZavodDataset",
     "ZD",
     "PathLike",
```

### Comparing `zavod-0.6.1/zavod/audit.py` & `zavod-0.6.2/zavod/audit.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.1/zavod/context.py` & `zavod-0.6.2/zavod/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,19 @@
             data_path=self.path,
             auth=auth,
             headers=headers,
         )
 
     def make(self, schema: Union[str, Schema]) -> CE:
         """Make a new entity with some dataset context set."""
-        return self.entity_type(model, {"schema": schema})
+        return self.entity_type(
+            model,
+            {"schema": schema},
+            default_dataset=self.dataset.name,
+        )
 
     def make_slug(
         self, *parts: Optional[str], strict: bool = True, prefix: Optional[str] = None
     ) -> Optional[str]:
         prefix = self.dataset.prefix if prefix is None else prefix
         return join_slug(*parts, prefix=prefix, strict=strict)
```

### Comparing `zavod-0.6.1/zavod/dataset.py` & `zavod-0.6.2/zavod/dataset.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.1/zavod/http.py` & `zavod-0.6.2/zavod/http.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.1/zavod/logs.py` & `zavod-0.6.2/zavod/logs.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.1/zavod/parse/addresses.py` & `zavod-0.6.2/zavod/parse/addresses.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.1/zavod/parse/names.py` & `zavod-0.6.2/zavod/parse/names.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.1/zavod/parse/xml.py` & `zavod-0.6.2/zavod/parse/xml.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.1/zavod/sinks/common.py` & `zavod-0.6.2/zavod/sinks/common.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.1/zavod/util.py` & `zavod-0.6.2/zavod/util.py`

 * *Files identical despite different names*

### Comparing `zavod-0.6.1/zavod.egg-info/PKG-INFO` & `zavod-0.6.2/zavod.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zavod
-Version: 0.6.1
+Version: 0.6.2
 Summary: Data factory for followthemoney data.
 Home-page: https://github.com/opensanctions/zavod
 Author: Friedrich Lindenberg
 Author-email: friedrich@opensanctions.org
 License: MIT
 Keywords: data mapping identity followthemoney etl parsing
 Platform: UNKNOWN
```

### Comparing `zavod-0.6.1/zavod.egg-info/SOURCES.txt` & `zavod-0.6.2/zavod.egg-info/SOURCES.txt`

 * *Files identical despite different names*


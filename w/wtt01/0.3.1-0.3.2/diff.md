# Comparing `tmp/wtt01-0.3.1.tar.gz` & `tmp/wtt01-0.3.2.tar.gz`

## Comparing `wtt01-0.3.1.tar` & `wtt01-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 wtt01-0.3.1/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtt01-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 wtt01-0.3.1/tests/test_load.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 wtt01-0.3.1/wtt01/__about__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wtt01-0.3.1/wtt01/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 wtt01-0.3.1/wtt01/_env.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wtt01-0.3.1/wtt01/cli.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 wtt01-0.3.1/wtt01/main.py
--rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 wtt01-0.3.1/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 wtt01-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wtt01-0.3.1/README.md
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 wtt01-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 wtt01-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 wtt01-0.3.2/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtt01-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 wtt01-0.3.2/tests/test_load.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 wtt01-0.3.2/wtt01/__about__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wtt01-0.3.2/wtt01/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 wtt01-0.3.2/wtt01/_env.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wtt01-0.3.2/wtt01/cli.py
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 wtt01-0.3.2/wtt01/main.py
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 wtt01-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 wtt01-0.3.2/LICENSE.txt
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wtt01-0.3.2/README.md
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 wtt01-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 wtt01-0.3.2/PKG-INFO
```

### Comparing `wtt01-0.3.1/tests/test_load.py` & `wtt01-0.3.2/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `wtt01-0.3.1/wtt01/cli.py` & `wtt01-0.3.2/wtt01/cli.py`

 * *Files identical despite different names*

### Comparing `wtt01-0.3.1/wtt01/main.py` & `wtt01-0.3.2/wtt01/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,45 +22,38 @@
 class WTTException(Exception):
     """Base exception for wtt01."""
 
 
 class WTT01ConfigurationException(WTTException):
     """Exception for wtt01 configuration."""
 
+
 class WTT01QueryException(WTTException):
     """Exception for wtt01 query."""
 
 
 def run_query_file(
-    con: duckdb.DuckDBPyConnection,
-    file_path: Union[Path, str],
-    **template_vars: dict[str,str],
+    con: duckdb.DuckDBPyConnection, file_path: Union[Path, str], **template_vars: dict
 ) -> duckdb.DuckDBPyConnection:
     """Run a query from a file."""
     if isinstance(file_path, str):
         file_path = Path(file_path)
 
     if template_vars:
         try:
             template = Template(file_path.read_text(encoding="utf-8"))
             query = template.substitute(**template_vars)
 
             return con.execute(query)
         except KeyError as exp:
-            raise WTT01QueryException(
-                f"Missing key {exp} in query"
-            ) from exp
+            raise WTT01QueryException(f"Missing key {exp} in query") from exp
         except TypeError as exp:
-            raise WTT01QueryException(
-                f"Invalid query {exp}"
-            ) from exp
+            raise WTT01QueryException(f"Invalid query {exp}") from exp
         except Exception as exp:
-            raise WTT01QueryException(
-                f"Unknown error {exp}"
-            ) from exp
+            raise WTT01QueryException(f"Unknown error {exp}") from exp
 
     else:
         return con.execute(file_path.read_text(encoding="utf-8"))
 
 
 def get_connection(
     database: str = ":memory:",
@@ -74,25 +67,19 @@
     if "WTT_01_LICENSE" not in os.environ:
         raise WTT01ConfigurationException(
             "WTT_01_LICENSE environment variable not set. "
             "Check the docs or email at help@wheretrue.com"
         )
 
     if config is None:
-        config = {
-            "allow_unsigned_extensions": True,
-        }
+        config = {"allow_unsigned_extensions": True}
     else:
         config["allow_unsigned_extensions"] = True
 
-    con = duckdb.connect(
-        database=database,
-        read_only=read_only,
-        config=config,
-    )
+    con = duckdb.connect(database=database, read_only=read_only, config=config)
 
     try:
         con.load_extension(EXTENSION_NAME)
         return con
     except duckdb.IOException as exp:
         extension_path = os.getenv("WTT01_EXTENSION_PATH")
 
@@ -112,16 +99,18 @@
             platform_uname = platform.uname()
             operating_system = platform_uname.system
             architecture = platform_uname.machine
             version = __version__
 
             from wtt01._env import ENVIRONMENT
 
+            env = os.getenv("WTT01_ENVIRONMENT", ENVIRONMENT)
+
             name = "wtt01"
-            bucket = f"wtt-01-dist-{ENVIRONMENT}"
+            bucket = f"wtt-01-dist-{env}"
             filename = f"{name}-{version}-{operating_system}-{architecture}.zip"
 
             full_s3_path = (
                 f"http://{bucket}.s3.amazonaws.com/extension/{name}/{filename}"
             )
 
             with tempfile.TemporaryDirectory() as temp_dir:
```

### Comparing `wtt01-0.3.1/.gitignore` & `wtt01-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `wtt01-0.3.1/LICENSE.txt` & `wtt01-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wtt01-0.3.1/pyproject.toml` & `wtt01-0.3.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,29 @@
 
 [project]
 authors = [
   {name = "Trent Hauck", email = "thauck@wheretrue.com"},
 ]
 classifiers = [
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "duckdb==0.7.1",
 ]
 description = ''
 dynamic = ["version"]
 keywords = []
 license = "MIT"
 name = "wtt01"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 
 [project.scripts]
 wtt01 = "wtt01.cli:main"
 
 [tool.hatch.version]
 path = "wtt01/__about__.py"
 
@@ -37,15 +36,15 @@
   "pytest-cov",
 ]
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=wtt01 --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
-python = ["37", "38", "39", "310", "311"]
+python = ["38", "39", "310", "311"]
 
 [tool.coverage.run]
 branch = true
 omit = [
   "wtt01/__about__.py",
 ]
 parallel = true
```

### Comparing `wtt01-0.3.1/PKG-INFO` & `wtt01-0.3.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: wtt01
-Version: 0.3.1
+Version: 0.3.2
 Author-email: Trent Hauck <thauck@wheretrue.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: duckdb==0.7.1
 Description-Content-Type: text/markdown
 
 # WTT 01
 
 **Table of Contents**
```


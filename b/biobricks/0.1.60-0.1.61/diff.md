# Comparing `tmp/biobricks-0.1.60.tar.gz` & `tmp/biobricks-0.1.61.tar.gz`

## Comparing `biobricks-0.1.60.tar` & `biobricks-0.1.61.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    13118 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks.svg
--rw-r--r--   0        0        0     9430 2020-02-02 00:00:00.000000 biobricks-0.1.60/coverage.xml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 biobricks-0.1.60/requirements.txt
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 biobricks-0.1.60/.github/workflows/biobricks.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.60/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.60/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.60/.pytest_cache/README.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.60/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 biobricks-0.1.60/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.60/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 biobricks-0.1.60/.vscode/tasks.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/__init__.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/api.py
--rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/brick.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/checks.py
--rwxr-xr-x   0        0        0     4514 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/cli.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/config.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/local_bb.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/.pytest_cache/README.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/tests/__init__.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/tests/test_init.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.60/biobricks/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 biobricks-0.1.60/docker/Dockerfile
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.60/docker/test.sh
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 biobricks-0.1.60/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 biobricks-0.1.60/LICENSE
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 biobricks-0.1.60/README.md
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 biobricks-0.1.60/pyproject.toml
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 biobricks-0.1.60/PKG-INFO
+-rw-r--r--   0        0        0    13118 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks.svg
+-rw-r--r--   0        0        0     9430 2020-02-02 00:00:00.000000 biobricks-0.1.61/coverage.xml
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 biobricks-0.1.61/requirements.txt
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 biobricks-0.1.61/.github/workflows/biobricks.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.61/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.61/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.61/.pytest_cache/README.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.61/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 biobricks-0.1.61/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.61/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 biobricks-0.1.61/.vscode/tasks.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/__init__.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/api.py
+-rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/brick.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/checks.py
+-rwxr-xr-x   0        0        0     4653 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/cli.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/config.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/local_bb.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/.pytest_cache/README.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/tests/__init__.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/tests/test_init.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.61/biobricks/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 biobricks-0.1.61/docker/Dockerfile
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.61/docker/test.sh
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 biobricks-0.1.61/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 biobricks-0.1.61/LICENSE
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 biobricks-0.1.61/README.md
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 biobricks-0.1.61/pyproject.toml
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 biobricks-0.1.61/PKG-INFO
```

### Comparing `biobricks-0.1.60/biobricks.svg` & `biobricks-0.1.61/biobricks.svg`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.60/coverage.xml` & `biobricks-0.1.61/coverage.xml`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.60/.github/workflows/biobricks.yml` & `biobricks-0.1.61/.github/workflows/biobricks.yml`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.60/biobricks/api.py` & `biobricks-0.1.61/biobricks/api.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.60/biobricks/brick.py` & `biobricks-0.1.61/biobricks/brick.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.60/biobricks/checks.py` & `biobricks-0.1.61/biobricks/checks.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.60/biobricks/cli.py` & `biobricks-0.1.61/biobricks/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,19 @@
     dotbb = Path(location)
     if dotbb.exists():
         return
     dotbb.mkdir()
     
     with open(dotbb / ".gitignore", "w") as f: 
         f.write("/*/") # ignore all subdirectories
+        
+    # create file dotbb/dependencies.txt with no contents
+    with open(dotbb / "dependencies.txt", "w") as f: 
+        pass
+    
 
 def local_bblib():
     return Path(".bb")
 
 def check_has_local_bblib():
     if not local_bblib().exists():
         raise Exception(".bb not found. run `biobricks init` first.")
```

### Comparing `biobricks-0.1.60/biobricks/config.py` & `biobricks-0.1.61/biobricks/config.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.60/biobricks/local_bb.py` & `biobricks-0.1.61/biobricks/local_bb.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.60/biobricks/tests/test_init.py` & `biobricks-0.1.61/biobricks/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.60/docker/Dockerfile` & `biobricks-0.1.61/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.60/LICENSE` & `biobricks-0.1.61/LICENSE`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.60/README.md` & `biobricks-0.1.61/README.md`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.60/pyproject.toml` & `biobricks-0.1.61/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "biobricks"
-version = "0.1.60"
+version = "0.1.61"
 authors = [
   { name="Jose A. Jaramillo", email="jjv@utp.edu.co" },
   { name="Thomas Luechtefeld", email="tom@insilica.co" }
 ]
 description = "Biobricks automates bioinformatics data."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `biobricks-0.1.60/PKG-INFO` & `biobricks-0.1.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobricks
-Version: 0.1.60
+Version: 0.1.61
 Summary: Biobricks automates bioinformatics data.
 Project-URL: Homepage, https://github.com/biobricks-ai/biobricks
 Project-URL: Bug Tracker, https://github.com/biobricks-ai/biobricks/issues
 Author-email: "Jose A. Jaramillo" <jjv@utp.edu.co>, Thomas Luechtefeld <tom@insilica.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/pdm_conda-0.9.0b1.tar.gz` & `tmp/pdm_conda-0.9.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_conda-0.9.0b1.tar", last modified: Wed Apr 19 18:15:14 2023, max compression
+gzip compressed data, was "pdm_conda-0.9.0b2.tar", last modified: Wed Apr 19 18:21:51 2023, max compression
```

## Comparing `pdm_conda-0.9.0b1.tar` & `pdm_conda-0.9.0b2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.9.0b1/LICENSE
--rw-r--r--   0        0        0     5649 2023-04-19 17:36:40.659039 pdm_conda-0.9.0b1/README.md
--rw-r--r--   0        0        0     1979 2023-04-19 18:15:15.334802 pdm_conda-0.9.0b1/pyproject.toml
--rw-r--r--   0        0        0      595 2023-04-19 18:14:58.819861 pdm_conda-0.9.0b1/src/pdm_conda/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.9.0b1/src/pdm_conda/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.9.0b1/src/pdm_conda/cli/commands/__init__.py
--rw-r--r--   0        0        0     3087 2023-04-19 15:05:35.481829 pdm_conda-0.9.0b1/src/pdm_conda/cli/commands/add.py
--rw-r--r--   0        0        0     1681 2023-04-19 16:32:57.025189 pdm_conda-0.9.0b1/src/pdm_conda/cli/commands/remove.py
--rw-r--r--   0        0        0     2183 2023-04-09 20:29:55.604925 pdm_conda-0.9.0b1/src/pdm_conda/cli/utils.py
--rw-r--r--   0        0        0    14551 2023-04-19 16:29:34.284850 pdm_conda-0.9.0b1/src/pdm_conda/conda.py
--rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.9.0b1/src/pdm_conda/installers/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-09 20:29:55.606525 pdm_conda-0.9.0b1/src/pdm_conda/installers/manager.py
--rw-r--r--   0        0        0     2307 2023-04-18 22:35:19.397503 pdm_conda-0.9.0b1/src/pdm_conda/installers/synchronizers.py
--rw-r--r--   0        0        0     3043 2023-04-18 01:05:14.781588 pdm_conda-0.9.0b1/src/pdm_conda/mapping.py
--rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.9.0b1/src/pdm_conda/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.9.0b1/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
--rw-r--r--   0        0        0     7946 2023-04-18 23:13:02.100650 pdm_conda-0.9.0b1/src/pdm_conda/models/candidates.py
--rw-r--r--   0        0        0     1818 2023-04-18 01:05:14.782254 pdm_conda-0.9.0b1/src/pdm_conda/models/conda.py
--rw-r--r--   0        0        0     8612 2023-04-18 23:02:22.362754 pdm_conda-0.9.0b1/src/pdm_conda/models/config.py
--rw-r--r--   0        0        0     3095 2023-04-19 17:13:01.223457 pdm_conda-0.9.0b1/src/pdm_conda/models/environment.py
--rw-r--r--   0        0        0     6581 2023-04-19 14:41:57.331734 pdm_conda-0.9.0b1/src/pdm_conda/models/repositories.py
--rw-r--r--   0        0        0    11268 2023-04-18 23:02:59.727692 pdm_conda-0.9.0b1/src/pdm_conda/models/requirements.py
--rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.9.0b1/src/pdm_conda/models/setup.py
--rw-r--r--   0        0        0     8311 2023-04-19 18:14:37.792025 pdm_conda-0.9.0b1/src/pdm_conda/project.py
--rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.9.0b1/src/pdm_conda/resolver/__init__.py
--rw-r--r--   0        0        0     2418 2023-04-18 22:33:52.217660 pdm_conda-0.9.0b1/src/pdm_conda/resolver/providers.py
--rw-r--r--   0        0        0     8575 2023-04-19 16:34:29.164097 pdm_conda-0.9.0b1/src/pdm_conda/resolvers.py
--rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.9.0b1/src/pdm_conda/utils.py
--rw-r--r--   0        0        0     7497 1970-01-01 00:00:00.000000 pdm_conda-0.9.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.9.0b2/LICENSE
+-rw-r--r--   0        0        0     5649 2023-04-19 17:36:40.659039 pdm_conda-0.9.0b2/README.md
+-rw-r--r--   0        0        0     1979 2023-04-19 18:21:51.984162 pdm_conda-0.9.0b2/pyproject.toml
+-rw-r--r--   0        0        0      595 2023-04-19 18:21:34.158877 pdm_conda-0.9.0b2/src/pdm_conda/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.9.0b2/src/pdm_conda/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.9.0b2/src/pdm_conda/cli/commands/__init__.py
+-rw-r--r--   0        0        0     3087 2023-04-19 15:05:35.481829 pdm_conda-0.9.0b2/src/pdm_conda/cli/commands/add.py
+-rw-r--r--   0        0        0     1681 2023-04-19 16:32:57.025189 pdm_conda-0.9.0b2/src/pdm_conda/cli/commands/remove.py
+-rw-r--r--   0        0        0     2183 2023-04-09 20:29:55.604925 pdm_conda-0.9.0b2/src/pdm_conda/cli/utils.py
+-rw-r--r--   0        0        0    14710 2023-04-19 18:21:22.125888 pdm_conda-0.9.0b2/src/pdm_conda/conda.py
+-rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.9.0b2/src/pdm_conda/installers/__init__.py
+-rw-r--r--   0        0        0     2482 2023-04-09 20:29:55.606525 pdm_conda-0.9.0b2/src/pdm_conda/installers/manager.py
+-rw-r--r--   0        0        0     2307 2023-04-18 22:35:19.397503 pdm_conda-0.9.0b2/src/pdm_conda/installers/synchronizers.py
+-rw-r--r--   0        0        0     3043 2023-04-18 01:05:14.781588 pdm_conda-0.9.0b2/src/pdm_conda/mapping.py
+-rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.9.0b2/src/pdm_conda/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.9.0b2/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
+-rw-r--r--   0        0        0     7946 2023-04-18 23:13:02.100650 pdm_conda-0.9.0b2/src/pdm_conda/models/candidates.py
+-rw-r--r--   0        0        0     1818 2023-04-18 01:05:14.782254 pdm_conda-0.9.0b2/src/pdm_conda/models/conda.py
+-rw-r--r--   0        0        0     8612 2023-04-18 23:02:22.362754 pdm_conda-0.9.0b2/src/pdm_conda/models/config.py
+-rw-r--r--   0        0        0     3095 2023-04-19 17:13:01.223457 pdm_conda-0.9.0b2/src/pdm_conda/models/environment.py
+-rw-r--r--   0        0        0     6581 2023-04-19 14:41:57.331734 pdm_conda-0.9.0b2/src/pdm_conda/models/repositories.py
+-rw-r--r--   0        0        0    11268 2023-04-18 23:02:59.727692 pdm_conda-0.9.0b2/src/pdm_conda/models/requirements.py
+-rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.9.0b2/src/pdm_conda/models/setup.py
+-rw-r--r--   0        0        0     8311 2023-04-19 18:14:37.792025 pdm_conda-0.9.0b2/src/pdm_conda/project.py
+-rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.9.0b2/src/pdm_conda/resolver/__init__.py
+-rw-r--r--   0        0        0     2418 2023-04-18 22:33:52.217660 pdm_conda-0.9.0b2/src/pdm_conda/resolver/providers.py
+-rw-r--r--   0        0        0     8575 2023-04-19 16:34:29.164097 pdm_conda-0.9.0b2/src/pdm_conda/resolvers.py
+-rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.9.0b2/src/pdm_conda/utils.py
+-rw-r--r--   0        0        0     7497 1970-01-01 00:00:00.000000 pdm_conda-0.9.0b2/PKG-INFO
```

### Comparing `pdm_conda-0.9.0b1/LICENSE` & `pdm_conda-0.9.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/README.md` & `pdm_conda-0.9.0b2/README.md`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/pyproject.toml` & `pdm_conda-0.9.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
     "pdm~=2.4.0",
     "requests>=2.28.1",
 ]
-version = "0.9.0b1"
+version = "0.9.0b2"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/macro128/pdm-conda"
 Changelog = "https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md"
```

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/__init__.py` & `pdm_conda-0.9.0b2/src/pdm_conda/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     core.register_command(AddCommand)
     core.register_command(RemoveCommand)
 
     for name, config in CONFIGS:
         core.add_config(name, config)
 
 
-__version__ = "0.9.0b1"
+__version__ = "0.9.0b2"
```

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/cli/commands/add.py` & `pdm_conda-0.9.0b2/src/pdm_conda/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/cli/commands/remove.py` & `pdm_conda-0.9.0b2/src/pdm_conda/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/cli/utils.py` & `pdm_conda-0.9.0b2/src/pdm_conda/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/conda.py` & `pdm_conda-0.9.0b2/src/pdm_conda/conda.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 from pdm_conda.models.setup import CondaSetupDistribution
 from pdm_conda.project import CondaProject
 from pdm_conda.utils import normalize_name
 
 logger = termui.logger
 
 
+class CondaResolutionError(PdmException):
+    pass
+
+
 @contextlib.contextmanager
 def _optional_temporary_file(environment: dict):
     """
     If environment contains data then creates temporary file else yield None
     :param environment: environment data
     :return: Temporary file or None
     """
@@ -287,16 +291,16 @@
     if channels:
         for c in channels:
             command.extend(["-c", c])
         command.append("--override-channels")
 
     result = run_conda(
         command,
-        exception_cls=VirtualenvCreateError,
-        exception_msg="Error creating environment",
+        exception_cls=CondaResolutionError if dry_run else VirtualenvCreateError,
+        exception_msg=f"Error resolving requirements with {config.runner}" if dry_run else "Error creating environment",
     )
 
     actions = result.get("actions", dict())
     fetch_packages = {pkg["name"]: pkg for pkg in actions.get("FETCH", [])}
     packages = actions.get("LINK", [])
     for i, pkg in enumerate(packages):
         pkg = fetch_packages.get(pkg["name"], pkg)
```

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/installers/manager.py` & `pdm_conda-0.9.0b2/src/pdm_conda/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/installers/synchronizers.py` & `pdm_conda-0.9.0b2/src/pdm_conda/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/mapping.py` & `pdm_conda-0.9.0b2/src/pdm_conda/mapping.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/models/candidates.py` & `pdm_conda-0.9.0b2/src/pdm_conda/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/models/conda.py` & `pdm_conda-0.9.0b2/src/pdm_conda/models/conda.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/models/config.py` & `pdm_conda-0.9.0b2/src/pdm_conda/models/config.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/models/environment.py` & `pdm_conda-0.9.0b2/src/pdm_conda/models/environment.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/models/repositories.py` & `pdm_conda-0.9.0b2/src/pdm_conda/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/models/requirements.py` & `pdm_conda-0.9.0b2/src/pdm_conda/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/models/setup.py` & `pdm_conda-0.9.0b2/src/pdm_conda/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/project.py` & `pdm_conda-0.9.0b2/src/pdm_conda/project.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/resolver/providers.py` & `pdm_conda-0.9.0b2/src/pdm_conda/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/resolvers.py` & `pdm_conda-0.9.0b2/src/pdm_conda/resolvers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/src/pdm_conda/utils.py` & `pdm_conda-0.9.0b2/src/pdm_conda/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b1/PKG-INFO` & `pdm_conda-0.9.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-conda
-Version: 0.9.0b1
+Version: 0.9.0b2
 Summary: A PDM plugin to resolve/install/uninstall project dependencies with Conda
 Keywords: pdm plugin conda
 Author: Marcos Pastorini
 License: MIT License
         
         Copyright (c) 2022 macro128
```


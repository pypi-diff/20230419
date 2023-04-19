# Comparing `tmp/pdm_conda-0.9.0b0.tar.gz` & `tmp/pdm_conda-0.9.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_conda-0.9.0b0.tar", last modified: Wed Apr 19 17:38:17 2023, max compression
+gzip compressed data, was "pdm_conda-0.9.0b1.tar", last modified: Wed Apr 19 18:15:14 2023, max compression
```

## Comparing `pdm_conda-0.9.0b0.tar` & `pdm_conda-0.9.0b1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.9.0b0/LICENSE
--rw-r--r--   0        0        0     5649 2023-04-19 17:36:40.659039 pdm_conda-0.9.0b0/README.md
--rw-r--r--   0        0        0     1979 2023-04-19 17:38:17.553059 pdm_conda-0.9.0b0/pyproject.toml
--rw-r--r--   0        0        0      595 2023-04-19 17:38:08.385052 pdm_conda-0.9.0b0/src/pdm_conda/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.9.0b0/src/pdm_conda/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.9.0b0/src/pdm_conda/cli/commands/__init__.py
--rw-r--r--   0        0        0     3087 2023-04-19 15:05:35.481829 pdm_conda-0.9.0b0/src/pdm_conda/cli/commands/add.py
--rw-r--r--   0        0        0     1681 2023-04-19 16:32:57.025189 pdm_conda-0.9.0b0/src/pdm_conda/cli/commands/remove.py
--rw-r--r--   0        0        0     2183 2023-04-09 20:29:55.604925 pdm_conda-0.9.0b0/src/pdm_conda/cli/utils.py
--rw-r--r--   0        0        0    14551 2023-04-19 16:29:34.284850 pdm_conda-0.9.0b0/src/pdm_conda/conda.py
--rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.9.0b0/src/pdm_conda/installers/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-09 20:29:55.606525 pdm_conda-0.9.0b0/src/pdm_conda/installers/manager.py
--rw-r--r--   0        0        0     2307 2023-04-18 22:35:19.397503 pdm_conda-0.9.0b0/src/pdm_conda/installers/synchronizers.py
--rw-r--r--   0        0        0     3043 2023-04-18 01:05:14.781588 pdm_conda-0.9.0b0/src/pdm_conda/mapping.py
--rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.9.0b0/src/pdm_conda/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.9.0b0/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
--rw-r--r--   0        0        0     7946 2023-04-18 23:13:02.100650 pdm_conda-0.9.0b0/src/pdm_conda/models/candidates.py
--rw-r--r--   0        0        0     1818 2023-04-18 01:05:14.782254 pdm_conda-0.9.0b0/src/pdm_conda/models/conda.py
--rw-r--r--   0        0        0     8612 2023-04-18 23:02:22.362754 pdm_conda-0.9.0b0/src/pdm_conda/models/config.py
--rw-r--r--   0        0        0     3095 2023-04-19 17:13:01.223457 pdm_conda-0.9.0b0/src/pdm_conda/models/environment.py
--rw-r--r--   0        0        0     6581 2023-04-19 14:41:57.331734 pdm_conda-0.9.0b0/src/pdm_conda/models/repositories.py
--rw-r--r--   0        0        0    11268 2023-04-18 23:02:59.727692 pdm_conda-0.9.0b0/src/pdm_conda/models/requirements.py
--rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.9.0b0/src/pdm_conda/models/setup.py
--rw-r--r--   0        0        0     8246 2023-04-19 16:32:27.859361 pdm_conda-0.9.0b0/src/pdm_conda/project.py
--rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.9.0b0/src/pdm_conda/resolver/__init__.py
--rw-r--r--   0        0        0     2418 2023-04-18 22:33:52.217660 pdm_conda-0.9.0b0/src/pdm_conda/resolver/providers.py
--rw-r--r--   0        0        0     8575 2023-04-19 16:34:29.164097 pdm_conda-0.9.0b0/src/pdm_conda/resolvers.py
--rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.9.0b0/src/pdm_conda/utils.py
--rw-r--r--   0        0        0     7497 1970-01-01 00:00:00.000000 pdm_conda-0.9.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.9.0b1/LICENSE
+-rw-r--r--   0        0        0     5649 2023-04-19 17:36:40.659039 pdm_conda-0.9.0b1/README.md
+-rw-r--r--   0        0        0     1979 2023-04-19 18:15:15.334802 pdm_conda-0.9.0b1/pyproject.toml
+-rw-r--r--   0        0        0      595 2023-04-19 18:14:58.819861 pdm_conda-0.9.0b1/src/pdm_conda/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.9.0b1/src/pdm_conda/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.9.0b1/src/pdm_conda/cli/commands/__init__.py
+-rw-r--r--   0        0        0     3087 2023-04-19 15:05:35.481829 pdm_conda-0.9.0b1/src/pdm_conda/cli/commands/add.py
+-rw-r--r--   0        0        0     1681 2023-04-19 16:32:57.025189 pdm_conda-0.9.0b1/src/pdm_conda/cli/commands/remove.py
+-rw-r--r--   0        0        0     2183 2023-04-09 20:29:55.604925 pdm_conda-0.9.0b1/src/pdm_conda/cli/utils.py
+-rw-r--r--   0        0        0    14551 2023-04-19 16:29:34.284850 pdm_conda-0.9.0b1/src/pdm_conda/conda.py
+-rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.9.0b1/src/pdm_conda/installers/__init__.py
+-rw-r--r--   0        0        0     2482 2023-04-09 20:29:55.606525 pdm_conda-0.9.0b1/src/pdm_conda/installers/manager.py
+-rw-r--r--   0        0        0     2307 2023-04-18 22:35:19.397503 pdm_conda-0.9.0b1/src/pdm_conda/installers/synchronizers.py
+-rw-r--r--   0        0        0     3043 2023-04-18 01:05:14.781588 pdm_conda-0.9.0b1/src/pdm_conda/mapping.py
+-rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.9.0b1/src/pdm_conda/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.9.0b1/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
+-rw-r--r--   0        0        0     7946 2023-04-18 23:13:02.100650 pdm_conda-0.9.0b1/src/pdm_conda/models/candidates.py
+-rw-r--r--   0        0        0     1818 2023-04-18 01:05:14.782254 pdm_conda-0.9.0b1/src/pdm_conda/models/conda.py
+-rw-r--r--   0        0        0     8612 2023-04-18 23:02:22.362754 pdm_conda-0.9.0b1/src/pdm_conda/models/config.py
+-rw-r--r--   0        0        0     3095 2023-04-19 17:13:01.223457 pdm_conda-0.9.0b1/src/pdm_conda/models/environment.py
+-rw-r--r--   0        0        0     6581 2023-04-19 14:41:57.331734 pdm_conda-0.9.0b1/src/pdm_conda/models/repositories.py
+-rw-r--r--   0        0        0    11268 2023-04-18 23:02:59.727692 pdm_conda-0.9.0b1/src/pdm_conda/models/requirements.py
+-rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.9.0b1/src/pdm_conda/models/setup.py
+-rw-r--r--   0        0        0     8311 2023-04-19 18:14:37.792025 pdm_conda-0.9.0b1/src/pdm_conda/project.py
+-rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.9.0b1/src/pdm_conda/resolver/__init__.py
+-rw-r--r--   0        0        0     2418 2023-04-18 22:33:52.217660 pdm_conda-0.9.0b1/src/pdm_conda/resolver/providers.py
+-rw-r--r--   0        0        0     8575 2023-04-19 16:34:29.164097 pdm_conda-0.9.0b1/src/pdm_conda/resolvers.py
+-rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.9.0b1/src/pdm_conda/utils.py
+-rw-r--r--   0        0        0     7497 1970-01-01 00:00:00.000000 pdm_conda-0.9.0b1/PKG-INFO
```

### Comparing `pdm_conda-0.9.0b0/LICENSE` & `pdm_conda-0.9.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/README.md` & `pdm_conda-0.9.0b1/README.md`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/pyproject.toml` & `pdm_conda-0.9.0b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
     "pdm~=2.4.0",
     "requests>=2.28.1",
 ]
-version = "0.9.0b0"
+version = "0.9.0b1"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/macro128/pdm-conda"
 Changelog = "https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md"
```

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/__init__.py` & `pdm_conda-0.9.0b1/src/pdm_conda/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     core.register_command(AddCommand)
     core.register_command(RemoveCommand)
 
     for name, config in CONFIGS:
         core.add_config(name, config)
 
 
-__version__ = "0.9.0b0"
+__version__ = "0.9.0b1"
```

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/cli/commands/add.py` & `pdm_conda-0.9.0b1/src/pdm_conda/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/cli/commands/remove.py` & `pdm_conda-0.9.0b1/src/pdm_conda/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/cli/utils.py` & `pdm_conda-0.9.0b1/src/pdm_conda/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/conda.py` & `pdm_conda-0.9.0b1/src/pdm_conda/conda.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/installers/manager.py` & `pdm_conda-0.9.0b1/src/pdm_conda/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/installers/synchronizers.py` & `pdm_conda-0.9.0b1/src/pdm_conda/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/mapping.py` & `pdm_conda-0.9.0b1/src/pdm_conda/mapping.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/models/candidates.py` & `pdm_conda-0.9.0b1/src/pdm_conda/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/models/conda.py` & `pdm_conda-0.9.0b1/src/pdm_conda/models/conda.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/models/config.py` & `pdm_conda-0.9.0b1/src/pdm_conda/models/config.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/models/environment.py` & `pdm_conda-0.9.0b1/src/pdm_conda/models/environment.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/models/repositories.py` & `pdm_conda-0.9.0b1/src/pdm_conda/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/models/requirements.py` & `pdm_conda-0.9.0b1/src/pdm_conda/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/models/setup.py` & `pdm_conda-0.9.0b1/src/pdm_conda/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/project.py` & `pdm_conda-0.9.0b1/src/pdm_conda/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,27 +49,29 @@
         self._conda_mapping: dict[str, str] = dict()
         self._pypi_mapping: dict[str, str] = dict()
         self.conda_config = PluginConfig.load_config(self)
 
     def _check_update_info(self, prop):
         if prop is None:
             self._get_conda_info()
-        return prop
 
     @property
     def virtual_packages(self) -> set[CondaRequirement]:
-        return self._check_update_info(self._virtual_packages)  # type: ignore
+        self._check_update_info(self._virtual_packages)
+        return self._virtual_packages  # type: ignore
 
     @property
     def platform(self) -> str:
-        return self._check_update_info(self._platform)  # type: ignore
+        self._check_update_info(self._platform)
+        return self._platform  # type: ignore
 
     @property
     def default_channels(self) -> list[str]:
-        return self._check_update_info(self._default_channels)  # type: ignore
+        self._check_update_info(self._default_channels)
+        return self._default_channels  # type: ignore
 
     @property
     def locked_repository(self) -> LockedRepository:
         try:
             lockfile = self.lockfile._data.unwrap()
         except ProjectError:
             lockfile = {}
```

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/resolver/providers.py` & `pdm_conda-0.9.0b1/src/pdm_conda/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/resolvers.py` & `pdm_conda-0.9.0b1/src/pdm_conda/resolvers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/src/pdm_conda/utils.py` & `pdm_conda-0.9.0b1/src/pdm_conda/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.0b0/PKG-INFO` & `pdm_conda-0.9.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-conda
-Version: 0.9.0b0
+Version: 0.9.0b1
 Summary: A PDM plugin to resolve/install/uninstall project dependencies with Conda
 Keywords: pdm plugin conda
 Author: Marcos Pastorini
 License: MIT License
         
         Copyright (c) 2022 macro128
```


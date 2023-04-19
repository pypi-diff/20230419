# Comparing `tmp/pysistentclass-0.0.2.tar.gz` & `tmp/pysistentclass-0.0.3.tar.gz`

## Comparing `pysistentclass-0.0.2.tar` & `pysistentclass-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     7819 2020-02-02 00:00:00.000000 pysistentclass-0.0.2/src/pysistentclass/__init__.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pysistentclass-0.0.2/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pysistentclass-0.0.2/LICENSE
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pysistentclass-0.0.2/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pysistentclass-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 pysistentclass-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pysistentclass-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 pysistentclass-0.0.3/src/pysistentclass/__init__.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pysistentclass-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pysistentclass-0.0.3/LICENSE
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pysistentclass-0.0.3/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pysistentclass-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 pysistentclass-0.0.3/PKG-INFO
```

### Comparing `pysistentclass-0.0.2/src/pysistentclass/__init__.py` & `pysistentclass-0.0.3/src/pysistentclass/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from pathlib import Path
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import Dict, List, Union
+from typing import Dict, List, Union, Any
 
 from importlib import import_module
 
 import json
 import yaml
 import toml
 
@@ -71,24 +71,24 @@
     PRIVATE = "private"
 
     class _ScopeRepr:
         def __repr__(self) -> str:
             pass
 
 
-@dataclass
-class Entry:
+def pysistentclass(wrapped_class: type):
     """
-    Entry class
+    pysistentclass decorator
 
-    This is the base class for all entries in the settings file. It
-    should not be used directly, but subclassed.
+    This decorator can be used to mark a class as a pysistentclass.
     """
-    _scope: Scope
-    _class_key: str
+    setattr(wrapped_class, "_scope", Scope.PUBLIC)
+    setattr(wrapped_class, "_class_key", None)
+    wrapped_class = dataclass(wrapped_class)
+    return wrapped_class
 
 
 @dataclass
 class Settings(dict):
     """ Settings class
 
     This is a dataclass that holds the settings for the application. It
@@ -108,21 +108,21 @@
     parameter should be the path to the directory where the settings
     file will be stored.
     """
     settings_dir: Union[Path, str]
 
     _classes: Dict[str, Dict[str, str]] = field(
         default_factory=dict, init=False)
-    _settings: Dict[str, Entry] = field(default_factory=dict, init=False)
+    _settings: Dict[str, object] = field(default_factory=dict, init=False)
 
     module_names: List[str] = field(default_factory=list)
     format: Format = Format.JSON
     logging_level: int = logging.DEBUG
 
-    def json_object_hook(self, obj: dict) -> Entry:
+    def json_object_hook(self, obj: dict) -> object:
         if "_class_key" in obj:
             class_key = obj["_class_key"]
             module = import_module(self._classes[class_key]["module"])
             class_name = self._classes[class_key]["class_name"]
             if not hasattr(module, class_name):
                 raise SettingsAttributeError(
                     f"{module} does not have {class_name}")
@@ -155,16 +155,16 @@
                 module = import_module(mod_name)
             except ModuleNotFoundError as e:
                 LOGGER.error(f"module '{mod_name}' not found")
                 exit(1)
             classes = inspect.getmembers(
                 module,
                 lambda o: inspect.isclass(o)
-                and issubclass(o, Entry)
-                and o is not Entry,
+                and hasattr(o, "_class_key")
+                and hasattr(o, "_scope"),
             )
             for class_name, class_obj in classes:
                 key = f"{mod_name}.{class_name}"
                 key_hash = hashlib.md5(key.encode()).hexdigest()
                 if key_hash in self._classes:
                     LOGGER.debug(f"o {key}")
                 else:
@@ -189,15 +189,15 @@
             instance = class_obj(
                 _class_key=class_key,
                 _scope=scope,
             )
             LOGGER.debug(f"+ instance of {class_obj}")
             self._settings[module_class_dict["class_name"]] = instance
 
-    def get(self, key: str) -> Entry:
+    def get(self, key: str) -> Any:
         return self._settings[key]
 
     def write(self):
         serialized = self.format.serializer(self._settings)
         self.settings_file.write_text(serialized)
 
     def read(self):
```

### Comparing `pysistentclass-0.0.2/LICENSE` & `pysistentclass-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysistentclass-0.0.2/pyproject.toml` & `pysistentclass-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pysistentclass"
-version = "0.0.2"
+version = "0.0.3"
 authors = [{ name = "manjaroman2", email = "manjaroman2@protonmail.com" }]
 description = "A small settings module for python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `pysistentclass-0.0.2/PKG-INFO` & `pysistentclass-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysistentclass
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small settings module for python
 Project-URL: Homepage, https://github.com/manjaroman2/pysistentclass
 Project-URL: Bug Tracker, https://github.com/manjaroman2/pysistentclass/issues
 Author-email: manjaroman2 <manjaroman2@protonmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -15,7 +15,12 @@
 Requires-Dist: toml
 Description-Content-Type: text/markdown
 
 # pysistentclass 
 
 ## A small settings module for python
 
+Found on [pypi](https://pypi.org/project/pysistentclass/)
+
+`
+pip install pysistentclass
+`
```


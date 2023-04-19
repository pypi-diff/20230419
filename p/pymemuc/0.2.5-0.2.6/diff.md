# Comparing `tmp/pymemuc-0.2.5.tar.gz` & `tmp/pymemuc-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemuc-0.2.5.tar", max compression
+gzip compressed data, was "pymemuc-0.2.6.tar", max compression
```

## Comparing `pymemuc-0.2.5.tar` & `pymemuc-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1057 2023-04-15 02:12:52.839467 pymemuc-0.2.5/LICENSE
--rw-r--r--   0        0        0     1580 2023-04-15 02:12:52.839467 pymemuc-0.2.5/README.md
--rw-r--r--   0        0        0      386 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/__init__.py
--rw-r--r--   0        0        0    22754 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/_command.py
--rw-r--r--   0        0        0      465 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/_constants.py
--rw-r--r--   0        0        0     4984 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/_control.py
--rw-r--r--   0        0        0     1150 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/_decorators.py
--rw-r--r--   0        0        0    12663 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/_manage.py
--rw-r--r--   0        0        0     3938 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/_memuc.py
--rw-r--r--   0        0        0      891 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/exceptions.py
--rw-r--r--   0        0        0     2194 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/pymemuc.py
--rw-r--r--   0        0        0      379 2023-04-15 02:12:52.843467 pymemuc-0.2.5/pymemuc/vminfo.py
--rw-r--r--   0        0        0     1655 2023-04-15 02:13:17.667534 pymemuc-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2432 1970-01-01 00:00:00.000000 pymemuc-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-04-19 18:00:35.150590 pymemuc-0.2.6/LICENSE
+-rw-r--r--   0        0        0     1580 2023-04-19 18:00:35.150590 pymemuc-0.2.6/README.md
+-rw-r--r--   0        0        0      386 2023-04-19 18:00:35.154590 pymemuc-0.2.6/pymemuc/__init__.py
+-rw-r--r--   0        0        0    22754 2023-04-19 18:00:35.154590 pymemuc-0.2.6/pymemuc/_command.py
+-rw-r--r--   0        0        0      465 2023-04-19 18:00:35.154590 pymemuc-0.2.6/pymemuc/_constants.py
+-rw-r--r--   0        0        0     4984 2023-04-19 18:00:35.154590 pymemuc-0.2.6/pymemuc/_control.py
+-rw-r--r--   0        0        0     1150 2023-04-19 18:00:35.154590 pymemuc-0.2.6/pymemuc/_decorators.py
+-rw-r--r--   0        0        0    13670 2023-04-19 18:00:35.158590 pymemuc-0.2.6/pymemuc/_manage.py
+-rw-r--r--   0        0        0     3938 2023-04-19 18:00:35.158590 pymemuc-0.2.6/pymemuc/_memuc.py
+-rw-r--r--   0        0        0      891 2023-04-19 18:00:35.158590 pymemuc-0.2.6/pymemuc/exceptions.py
+-rw-r--r--   0        0        0     2216 2023-04-19 18:00:35.158590 pymemuc-0.2.6/pymemuc/pymemuc.py
+-rw-r--r--   0        0        0      379 2023-04-19 18:00:35.158590 pymemuc-0.2.6/pymemuc/vminfo.py
+-rw-r--r--   0        0        0     1655 2023-04-19 18:00:58.818617 pymemuc-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2432 1970-01-01 00:00:00.000000 pymemuc-0.2.6/PKG-INFO
```

### Comparing `pymemuc-0.2.5/LICENSE` & `pymemuc-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.5/README.md` & `pymemuc-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.5/pymemuc/_command.py` & `pymemuc-0.2.6/pymemuc/_command.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.5/pymemuc/_control.py` & `pymemuc-0.2.6/pymemuc/_control.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.5/pymemuc/_decorators.py` & `pymemuc-0.2.6/pymemuc/_decorators.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.5/pymemuc/_manage.py` & `pymemuc-0.2.6/pymemuc/_manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,7 +337,32 @@
         )
     else:
         raise PyMemucIndexError("Please specify either a vm index or a vm name")
     success = status == 0 and output is not None and "SUCCESS" in output
     if not success:
         raise PyMemucError(f"Failed to set VM configuration: {output}")
     return True
+
+
+def randomize_vm(
+    self: "PyMemuc", vm_index: Union[int, None] = None, vm_name: Union[str, None] = None
+) -> Literal[True]:
+    """Randomize a VM, must specify either a vm index or a vm name
+
+    :param vm_index: VM index. Defaults to None.
+    :type vm_index: int, optional
+    :param vm_name: VM name. Defaults to None.
+    :type vm_name: str, optional
+    :raises PyMemucIndexError: an error if neither a vm index or a vm name is specified
+    :return: True if the vm was randomized successfully
+    :rtype: Literal[True]
+    """
+    if vm_index is not None:
+        status, output = self.memuc_run(["-i", str(vm_index), "randomize"])
+    elif vm_name is not None:
+        status, output = self.memuc_run(["-n", vm_name, "randomize"])
+    else:
+        raise PyMemucIndexError("Please specify either a vm index or a vm name")
+    success = status == 0 and output is not None and "SUCCESS" in output
+    if not success:
+        raise PyMemucError(f"Failed to randomize VM: {output}")
+    return True
```

### Comparing `pymemuc-0.2.5/pymemuc/_memuc.py` & `pymemuc-0.2.6/pymemuc/_memuc.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.5/pymemuc/exceptions.py` & `pymemuc-0.2.6/pymemuc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.5/pymemuc/pymemuc.py` & `pymemuc-0.2.6/pymemuc/pymemuc.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         clone_vm,
         create_vm,
         delete_vm,
         export_vm,
         get_configuration_vm,
         import_vm,
         list_vm_info,
+        randomize_vm,
         rename_vm,
         set_configuration_vm,
         vm_is_running,
     )
     from ._memuc import _get_memu_top_level, check_task_status, memuc_run
 
     def __init__(self, memuc_path: Union[str, None] = None, debug=False) -> None:
```

### Comparing `pymemuc-0.2.5/pyproject.toml` & `pymemuc-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pymemuc"
-version = "v0.2.5"
+version = "v0.2.6"
 description = "A Memuc.exe wrapper for Python"
 readme = "README.md"
 authors = ["Martin Miglio <code@martinmiglio.dev>"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pymemuc-0.2.5/PKG-INFO` & `pymemuc-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemuc
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Memuc.exe wrapper for Python
 Home-page: https://github.com/marmig0404/pymemuc
 License: MIT
 Keywords: memu,memuc,wrapper,api
 Author: Martin Miglio
 Author-email: code@martinmiglio.dev
 Requires-Python: >=3.9,<4.0
```


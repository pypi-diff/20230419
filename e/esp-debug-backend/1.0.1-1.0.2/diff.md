# Comparing `tmp/esp-debug-backend-1.0.1.tar.gz` & `tmp/esp-debug-backend-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-debug-backend/esp-debug-backend/dist/.tmp-6o4dae8i/esp-debug-backend-1.0.1.tar", last modified: Thu Jan 19 21:20:28 2023, max compression
+gzip compressed data, was "/home/runner/work/esp-debug-backend/esp-debug-backend/dist/.tmp-9bg99a93/esp-debug-backend-1.0.2.tar", last modified: Wed Apr 19 19:12:26 2023, max compression
```

## Comparing `esp-debug-backend-1.0.1.tar` & `esp-debug-backend-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:20:28.000000 esp-debug-backend-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-19 21:20:12.000000 esp-debug-backend-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-01-19 21:20:28.000000 esp-debug-backend-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-01-19 21:20:12.000000 esp-debug-backend-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-01-19 21:20:12.000000 esp-debug-backend-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 21:20:28.000000 esp-debug-backend-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:20:28.000000 esp-debug-backend-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:20:28.000000 esp-debug-backend-1.0.1/src/esp_debug_backend/
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-01-19 21:20:12.000000 esp-debug-backend-1.0.1/src/esp_debug_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-01-19 21:20:12.000000 esp-debug-backend-1.0.1/src/esp_debug_backend/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28920 2023-01-19 21:20:12.000000 esp-debug-backend-1.0.1/src/esp_debug_backend/gdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-01-19 21:20:12.000000 esp-debug-backend-1.0.1/src/esp_debug_backend/gdb_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:20:28.000000 esp-debug-backend-1.0.1/src/esp_debug_backend/hw_specific/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-19 21:20:12.000000 esp-debug-backend-1.0.1/src/esp_debug_backend/hw_specific/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-01-19 21:20:12.000000 esp-debug-backend-1.0.1/src/esp_debug_backend/hw_specific/esp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-01-19 21:20:12.000000 esp-debug-backend-1.0.1/src/esp_debug_backend/hw_specific/riscv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-01-19 21:20:12.000000 esp-debug-backend-1.0.1/src/esp_debug_backend/hw_specific/xtensa.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-01-19 21:20:12.000000 esp-debug-backend-1.0.1/src/esp_debug_backend/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-01-19 21:20:12.000000 esp-debug-backend-1.0.1/src/esp_debug_backend/oocd.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-01-19 21:20:12.000000 esp-debug-backend-1.0.1/src/esp_debug_backend/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 21:20:28.000000 esp-debug-backend-1.0.1/src/esp_debug_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-01-19 21:20:28.000000 esp-debug-backend-1.0.1/src/esp_debug_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-01-19 21:20:28.000000 esp-debug-backend-1.0.1/src/esp_debug_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 21:20:28.000000 esp-debug-backend-1.0.1/src/esp_debug_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-19 21:20:28.000000 esp-debug-backend-1.0.1/src/esp_debug_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-19 21:20:28.000000 esp-debug-backend-1.0.1/src/esp_debug_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29417 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/gdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/gdb_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/hw_specific/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/hw_specific/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/hw_specific/esp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/hw_specific/riscv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/hw_specific/xtensa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/oocd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/src/esp_debug_backend/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/esp_debug_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/esp_debug_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/esp_debug_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/esp_debug_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/esp_debug_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/src/esp_debug_backend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:12:26.000000 esp-debug-backend-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/tests/test_gdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-19 19:12:09.000000 esp-debug-backend-1.0.2/tests/test_oocd.py
```

### Comparing `esp-debug-backend-1.0.1/LICENSE` & `esp-debug-backend-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.1/PKG-INFO` & `esp-debug-backend-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: esp-debug-backend
-Version: 1.0.1
+Version: 1.0.2
 Summary: This package is a library built on top of pygdbmi providing high-level API for debugging programs using GDB and OpenOCD.
 Author-email: Alexey Gerenkov <alexey.gerenkov@espressif.com>, Andrei Gramakov <andrei.gramakov@espressif.com>
 Project-URL: Homepage, https://github.com/espressif/esp-debug-backend
 Project-URL: Bug Tracker, https://github.com/espressif/esp-debug-backend/issues
+Project-URL: Documentation, https://github.com/espressif/esp-debug-backend/blob/master/README.md
+Project-URL: Changelog, https://github.com/espressif/esp-debug-backend/blob/master/CHANGELOG.md
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `esp-debug-backend-1.0.1/src/esp_debug_backend/__init__.py` & `esp-debug-backend-1.0.2/src/esp_debug_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.1/src/esp_debug_backend/defs.py` & `esp-debug-backend-1.0.2/src/esp_debug_backend/defs.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.1/src/esp_debug_backend/gdb.py` & `esp-debug-backend-1.0.2/src/esp_debug_backend/gdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,18 +223,25 @@
             raise DebuggerError('Unsupported stream type "%s"' % stream_type)
         if handler not in self.stream_handlers[stream_type]:
             return
         self.stream_handlers[stream_type].remove(handler)
 
     def gdb_exit(self, tmo=5):
         """ -gdb-exit ~= quit """
-        self._mi_cmd_run("-gdb-exit", response_on_success=["exit"], tmo=tmo)
-        with self._gdbmi_lock:
-            self._gdbmi.exit()
-            self._gdbmi = None
+        try:
+            self._mi_cmd_run("-gdb-exit", response_on_success=["exit"], tmo=tmo)
+        except NoGdbProcessError:
+            # pygdbmi<=0.10 calls `verify_valid_gdb_subprocess` before reading GDB response,
+            # 1) if after sending `-gdb-exit` to GDB it exits before we call `get_gdb_response` `NoGdbProcessError` is raised. Ignore the exception.
+            # 2) it is also safe to ignore `NoGdbProcessError` if it is raised because GDB has exited before sending `-gdb-exit`.
+            self._logger.warning('GDB had exited before `-gdb-exit` was completely processed!')
+        finally:
+            with self._gdbmi_lock:
+                self._gdbmi.exit()
+                self._gdbmi = None
 
     def console_cmd_run(self, cmd, response_on_success=["done"], tmo=5):
         """
         Execute a command in the console mode
 
         Parameters
         ----------
@@ -655,17 +662,14 @@
         #
         sel_id, ths = self.get_thread_info()
         for th in ths:
             if th['id'] == sel_id:
                 return th
         return None
 
-    def target_program(self):
-        return None
-
     def set_prog_startup_script(self, path):
         """
         Set up a startup command file which will be executed in the beginning of `exec_run` method.
         See : https://sourceware.org/gdb/current/onlinedocs/gdb/Command-Files.html#Command-Files
 
         Parameters
         ----------
```

### Comparing `esp-debug-backend-1.0.1/src/esp_debug_backend/gdb_helpers.py` & `esp-debug-backend-1.0.2/src/esp_debug_backend/gdb_helpers.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.1/src/esp_debug_backend/hw_specific/esp.py` & `esp-debug-backend-1.0.2/src/esp_debug_backend/hw_specific/esp.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.1/src/esp_debug_backend/hw_specific/riscv.py` & `esp-debug-backend-1.0.2/src/esp_debug_backend/hw_specific/riscv.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.1/src/esp_debug_backend/hw_specific/xtensa.py` & `esp-debug-backend-1.0.2/src/esp_debug_backend/hw_specific/xtensa.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.1/src/esp_debug_backend/log.py` & `esp-debug-backend-1.0.2/src/esp_debug_backend/log.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.1/src/esp_debug_backend/oocd.py` & `esp-debug-backend-1.0.2/src/esp_debug_backend/oocd.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.1/src/esp_debug_backend/utils.py` & `esp-debug-backend-1.0.2/src/esp_debug_backend/utils.py`

 * *Files identical despite different names*

### Comparing `esp-debug-backend-1.0.1/src/esp_debug_backend.egg-info/PKG-INFO` & `esp-debug-backend-1.0.2/src/esp_debug_backend.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: esp-debug-backend
-Version: 1.0.1
+Version: 1.0.2
 Summary: This package is a library built on top of pygdbmi providing high-level API for debugging programs using GDB and OpenOCD.
 Author-email: Alexey Gerenkov <alexey.gerenkov@espressif.com>, Andrei Gramakov <andrei.gramakov@espressif.com>
 Project-URL: Homepage, https://github.com/espressif/esp-debug-backend
 Project-URL: Bug Tracker, https://github.com/espressif/esp-debug-backend/issues
+Project-URL: Documentation, https://github.com/espressif/esp-debug-backend/blob/master/README.md
+Project-URL: Changelog, https://github.com/espressif/esp-debug-backend/blob/master/CHANGELOG.md
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `esp-debug-backend-1.0.1/src/esp_debug_backend.egg-info/SOURCES.txt` & `esp-debug-backend-1.0.2/src/esp_debug_backend.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,8 +12,10 @@
 src/esp_debug_backend.egg-info/SOURCES.txt
 src/esp_debug_backend.egg-info/dependency_links.txt
 src/esp_debug_backend.egg-info/requires.txt
 src/esp_debug_backend.egg-info/top_level.txt
 src/esp_debug_backend/hw_specific/__init__.py
 src/esp_debug_backend/hw_specific/esp.py
 src/esp_debug_backend/hw_specific/riscv.py
-src/esp_debug_backend/hw_specific/xtensa.py
+src/esp_debug_backend/hw_specific/xtensa.py
+tests/test_gdb.py
+tests/test_oocd.py
```


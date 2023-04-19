# Comparing `tmp/flytekitplugins-papermill-1.5.0b1.tar.gz` & `tmp/flytekitplugins-papermill-1.6.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-papermill-1.5.0b1.tar", last modified: Wed Mar 29 18:58:42 2023, max compression
+gzip compressed data, was "flytekitplugins-papermill-1.6.0b0.tar", last modified: Wed Apr 19 20:54:34 2023, max compression
```

## Comparing `flytekitplugins-papermill-1.5.0b1.tar` & `flytekitplugins-papermill-1.6.0b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:42.840238 flytekitplugins-papermill-1.5.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-29 18:58:42.840238 flytekitplugins-papermill-1.5.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-29 18:58:20.000000 flytekitplugins-papermill-1.5.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:42.840238 flytekitplugins-papermill-1.5.0b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:42.840238 flytekitplugins-papermill-1.5.0b1/flytekitplugins/papermill/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-29 18:58:20.000000 flytekitplugins-papermill-1.5.0b1/flytekitplugins/papermill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-03-29 18:58:20.000000 flytekitplugins-papermill-1.5.0b1/flytekitplugins/papermill/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:42.840238 flytekitplugins-papermill-1.5.0b1/flytekitplugins_papermill.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-29 18:58:42.000000 flytekitplugins-papermill-1.5.0b1/flytekitplugins_papermill.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-29 18:58:42.000000 flytekitplugins-papermill-1.5.0b1/flytekitplugins_papermill.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 18:58:42.000000 flytekitplugins-papermill-1.5.0b1/flytekitplugins_papermill.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-29 18:58:42.000000 flytekitplugins-papermill-1.5.0b1/flytekitplugins_papermill.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-29 18:58:42.000000 flytekitplugins-papermill-1.5.0b1/flytekitplugins_papermill.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-29 18:58:42.000000 flytekitplugins-papermill-1.5.0b1/flytekitplugins_papermill.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 18:58:42.840238 flytekitplugins-papermill-1.5.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-29 18:58:35.000000 flytekitplugins-papermill-1.5.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:34.055140 flytekitplugins-papermill-1.6.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-19 20:54:34.051140 flytekitplugins-papermill-1.6.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-19 20:54:06.000000 flytekitplugins-papermill-1.6.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:34.051140 flytekitplugins-papermill-1.6.0b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:34.051140 flytekitplugins-papermill-1.6.0b0/flytekitplugins/papermill/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-19 20:54:06.000000 flytekitplugins-papermill-1.6.0b0/flytekitplugins/papermill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-04-19 20:54:06.000000 flytekitplugins-papermill-1.6.0b0/flytekitplugins/papermill/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:34.051140 flytekitplugins-papermill-1.6.0b0/flytekitplugins_papermill.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-19 20:54:34.000000 flytekitplugins-papermill-1.6.0b0/flytekitplugins_papermill.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-19 20:54:34.000000 flytekitplugins-papermill-1.6.0b0/flytekitplugins_papermill.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:54:34.000000 flytekitplugins-papermill-1.6.0b0/flytekitplugins_papermill.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:34.000000 flytekitplugins-papermill-1.6.0b0/flytekitplugins_papermill.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-19 20:54:34.000000 flytekitplugins-papermill-1.6.0b0/flytekitplugins_papermill.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:34.000000 flytekitplugins-papermill-1.6.0b0/flytekitplugins_papermill.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:54:34.055140 flytekitplugins-papermill-1.6.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-19 20:54:25.000000 flytekitplugins-papermill-1.6.0b0/setup.py
```

### Comparing `flytekitplugins-papermill-1.5.0b1/PKG-INFO` & `flytekitplugins-papermill-1.6.0b0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-papermill
-Version: 1.5.0b1
+Version: 1.6.0b0
 Summary: This is the flytekit papermill plugin
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-papermill-1.5.0b1/README.md` & `flytekitplugins-papermill-1.6.0b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-papermill-1.5.0b1/flytekitplugins/papermill/task.py` & `flytekitplugins-papermill-1.6.0b0/flytekitplugins/papermill/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import json
+import logging
 import os
+import sys
 import typing
 from typing import Any
 
 import nbformat
 import papermill as pm
 from flyteidl.core.literals_pb2 import LiteralMap as _pb2_LiteralMap
 from google.protobuf import text_format as _text_format
@@ -82,14 +84,21 @@
     #. It also converts the captured notebook into an ``html`` page, which the FlyteConsole will render called -
        ``out_rendered_nb``. If ``render_deck=True`` is passed, this html content will be inserted into a deck.
 
     .. note:
 
         Users can access these notebooks after execution of the task locally or from remote servers.
 
+    .. note:
+
+        By default, print statements in your notebook won't be transmitted to the pod logs/stdout. If you would
+        like to have logs forwarded as the notebook executes, pass the stream_logs argument. Note that notebook
+        logs can be quite verbose, so ensure you are prepared for any downstream log ingestion costs
+        (e.g., cloudwatch)
+
     .. todo:
 
         Implicit extraction of SparkConfiguration from the notebook is not supported.
 
     .. todo:
 
         Support for remote notebook execution, we can create a custom metadata field that is read by a propeller plugin
@@ -110,14 +119,15 @@
     _IMPLICIT_RENDERED_NOTEBOOK_TYPE = HTMLPage
 
     def __init__(
         self,
         name: str,
         notebook_path: str,
         render_deck: bool = False,
+        stream_logs: bool = False,
         task_config: T = None,
         inputs: typing.Optional[typing.Dict[str, typing.Type]] = None,
         outputs: typing.Optional[typing.Dict[str, typing.Type]] = None,
         **kwargs,
     ):
         # Each instance of NotebookTask instantiates an underlying task with a dummy function that will only be used
         # to run pre- and post- execute functions using the corresponding task plugin.
@@ -131,14 +141,24 @@
         # at serialization time.
         self._config_task_instance._name = f"{PAPERMILL_TASK_PREFIX}.{name}"
         task_type = f"{self._config_task_instance.task_type}"
         task_type_version = self._config_task_instance.task_type_version
         self._notebook_path = os.path.abspath(notebook_path)
 
         self._render_deck = render_deck
+        self._stream_logs = stream_logs
+
+        # Send the papermill logger to stdout so that it appears in pod logs. Note that papermill doesn't allow
+        # injecting a logger, so we cannot redirect logs to the flyte child loggers (e.g., the userspace logger)
+        # and inherit their settings, but we instead must send logs to stdout directly
+        if self._stream_logs:
+            papermill_logger = logging.getLogger("papermill")
+            papermill_logger.addHandler(logging.StreamHandler(sys.stdout))
+            # Papermill leaves the default level of DEBUG. We increase it here.
+            papermill_logger.setLevel(logging.INFO)
 
         if not os.path.exists(self._notebook_path):
             raise ValueError(f"Illegal notebook path passed in {self._notebook_path}")
 
         if outputs:
             outputs.update(
                 {
@@ -232,15 +252,15 @@
         TODO: Figure out how to share FlyteContext ExecutionParameters with the notebook kernel (as notebook kernel
              is executed in a separate python process)
         For Spark, the notebooks today need to use the new_session or just getOrCreate session and get a handle to the
         singleton
         """
         logger.info(f"Hijacking the call for task-type {self.task_type}, to call notebook.")
         # Execute Notebook via Papermill.
-        pm.execute_notebook(self._notebook_path, self.output_notebook_path, parameters=kwargs)  # type: ignore
+        pm.execute_notebook(self._notebook_path, self.output_notebook_path, parameters=kwargs, log_output=self._stream_logs)  # type: ignore
 
         outputs = self.extract_outputs(self.output_notebook_path)
         self.render_nb_html(self.output_notebook_path, self.rendered_output_path)
 
         m = {}
         if outputs:
             m = outputs.literals
```

### Comparing `flytekitplugins-papermill-1.5.0b1/flytekitplugins_papermill.egg-info/PKG-INFO` & `flytekitplugins-papermill-1.6.0b0/flytekitplugins_papermill.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-papermill
-Version: 1.5.0b1
+Version: 1.6.0b0
 Summary: This is the flytekit papermill plugin
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-papermill-1.5.0b1/setup.py` & `flytekitplugins-papermill-1.6.0b0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 plugin_requires = [
     "flytekit>=1.3.0b2,<2.0.0",
     "papermill>=1.2.0",
     "nbconvert>=6.0.7",
     "ipykernel>=5.0.0",
 ]
 
-__version__ = "1.5.0b1"
+__version__ = "1.6.0b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This is the flytekit papermill plugin",
```


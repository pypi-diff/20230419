# Comparing `tmp/gladier-0.8.4.tar.gz` & `tmp/gladier-0.8.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gladier-0.8.4.tar", last modified: Wed Apr 19 21:20:37 2023, max compression
+gzip compressed data, was "gladier-0.8.4b1.tar", last modified: Tue Apr  4 15:55:07 2023, max compression
```

## Comparing `gladier-0.8.4.tar` & `gladier-0.8.4b1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:20:37.185306 gladier-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 21:20:26.000000 gladier-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-19 21:20:26.000000 gladier-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-19 21:20:37.185306 gladier-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-19 21:20:26.000000 gladier-0.8.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:20:37.181306 gladier-0.8.4/gladier/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20592 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:20:37.181306 gladier-0.8.4/gladier/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18333 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/managers/flows_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/managers/funcx_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/managers/login_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/managers/service_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:20:37.181306 gladier-0.8.4/gladier/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/storage/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/storage/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/storage/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:20:37.185306 gladier-0.8.4/gladier/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/utils/automate.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/utils/dynamic_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/utils/flow_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/utils/flow_modifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/utils/flow_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/utils/funcx_login_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/utils/name_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/utils/tool_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/utils/tool_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 21:20:26.000000 gladier-0.8.4/gladier/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:20:37.181306 gladier-0.8.4/gladier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-19 21:20:37.000000 gladier-0.8.4/gladier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-19 21:20:37.000000 gladier-0.8.4/gladier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:20:37.000000 gladier-0.8.4/gladier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 21:20:37.000000 gladier-0.8.4/gladier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 21:20:37.000000 gladier-0.8.4/gladier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 21:20:26.000000 gladier-0.8.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-19 21:20:37.185306 gladier-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-19 21:20:26.000000 gladier-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:55:07.876788 gladier-0.8.4b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-04 15:54:46.000000 gladier-0.8.4b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-04 15:54:46.000000 gladier-0.8.4b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-04 15:55:07.876788 gladier-0.8.4b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-04 15:54:46.000000 gladier-0.8.4b1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:55:07.872788 gladier-0.8.4b1/gladier/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17889 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:55:07.872788 gladier-0.8.4b1/gladier/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20077 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/managers/flows_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/managers/funcx_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/managers/login_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/managers/service_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:55:07.872788 gladier-0.8.4b1/gladier/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/storage/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/storage/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/storage/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:55:07.876788 gladier-0.8.4b1/gladier/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/dynamic_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/flow_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/flow_modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/flow_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/funcx_login_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/name_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/tool_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/utils/tool_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-04 15:54:50.000000 gladier-0.8.4b1/gladier/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 15:55:07.872788 gladier-0.8.4b1/gladier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-04 15:55:07.000000 gladier-0.8.4b1/gladier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-04 15:55:07.000000 gladier-0.8.4b1/gladier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 15:55:07.000000 gladier-0.8.4b1/gladier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-04 15:55:07.000000 gladier-0.8.4b1/gladier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 15:55:07.000000 gladier-0.8.4b1/gladier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-04 15:54:50.000000 gladier-0.8.4b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-04 15:55:07.876788 gladier-0.8.4b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-04 15:54:50.000000 gladier-0.8.4b1/setup.py
```

### Comparing `gladier-0.8.4/LICENSE` & `gladier-0.8.4b1/LICENSE`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/PKG-INFO` & `gladier-0.8.4b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gladier
-Version: 0.8.4
+Version: 0.8.4b1
 Summary: Tooling for rapid deployment of automation tooling.
 Home-page: https://github.com/globus-gladier/gladier
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,14 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Gladier: The Globus Architecture for Data-Intensive Experimental Research.
 ==========================================================================
 |docs|
```

### Comparing `gladier-0.8.4/README.rst` & `gladier-0.8.4b1/README.rst`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/base.py` & `gladier-0.8.4b1/gladier/base.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/client.py` & `gladier-0.8.4b1/gladier/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -255,65 +255,14 @@
                                           '"gladier.GladierBaseTool"')
 
     def sync_flow(self):
         self.flows_manager.flow_definition = self.get_flow_definition()
         self.flows_manager.sync_flow()
 
     def run_flow(self, flow_input=None, use_defaults=True, **flow_kwargs):
-        r"""
-        Start a Globus Automate flow. By default, the flow definiton is checked and synced if it
-        has changed locally or deployed if it does not exist.
-
-        If a group is set, run permissions are updated and applied to the run (includes
-        'run_managers', 'run_monitors').
-
-        Any scope changes required post-deployment/update are propogated through the login_manager
-        and may require an additional login. A new flow checksum/id may be tracked in storage if
-        the flow changed or was newly deployed.
-
-        The run_flow method shadows the globus-automate-client method for running flows documented
-        here: https://globus-automate-client.readthedocs.io/en/latest/python_sdk_reference.html#globus_automate_client.flows_client.FlowsClient.run_flow  # noqa
-        Additional arguments matching the method signature may be added. Common ones include the
-        following:
-
-        * **label** (Optional[str]) An optional label which can be used to identify this run
-        * **tags** (Optional[List[str]]) Tags that will be associated with this Run.
-
-        Example:
-
-        .. code-block:: python
-
-            myinput = {
-                "input": {
-                    "args": "cat /proc/version",
-                    "capture_output": True,
-                    "funcx_endpoint_compute": "4b116d3c-1703-4f8f-9f6f-39921e5864df",
-                }
-            }
-            my_client.run_flow(myinput, label='Check Version', tags=['version', 'POSIX'])
-
-        :param flow_input: A dict of input to be passed to the automate flow. self.check_input()
-                           is called on each tool to ensure basic needs are met for each.
-                           Input MUST be wrapped inside an 'input' dict,
-                           for example {'input': {'foo': 'bar'}}.
-
-        :param use_defaults: Use the result of self.get_input() to populate base input for the
-                             flow. All conflicting input provided by flow_input overrides
-                             values set in use_defaults.
-        :param \**flow_kwargs: Set several keyed arguments that include the label to be used
-                               in the automate app. If no label is passed the standard automate
-                               label is used. Also ensure label <= 64 chars long.
-        :raise: gladier.exc.ConfigException by self.check_input()
-        :raises: gladier.exc.FlowObsolete
-        :raises: gladier.exc.NoFlowRegistered
-        :raises: gladier.exc.RegistrationException
-        :raises: gladier.exc.FunctionObsolete
-        :raises: gladier.exc.AuthException
-        :raises: Any globus_sdk.exc.BaseException
-        """
         combine_flow_input = self.get_input() if use_defaults else dict()
         if flow_input is not None:
             if not flow_input.get('input') or len(flow_input.keys()) != 1:
                 raise gladier.exc.ConfigException(
                     f'Malformed input to flow, all input must be nested under "input", got '
                     f'{flow_input.keys()}')
             combine_flow_input['input'].update(flow_input['input'])
```

### Comparing `gladier-0.8.4/gladier/decorators.py` & `gladier-0.8.4b1/gladier/decorators.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/exc.py` & `gladier-0.8.4b1/gladier/exc.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/managers/flows_manager.py` & `gladier-0.8.4b1/gladier/managers/flows_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -334,14 +334,44 @@
         """
         Remove the stored flow_id and flow_checksum.
         """
         self.storage.del_value('flow_id')
         self.storage.del_value('flow_checksum')
 
     def run_flow(self, **kwargs):
+        r"""
+        Start a Globus Automate flow. By default, the flow definiton is checked and synced if it
+        has changed locally or deployed if it does not exist.
+
+        If a group is set, run permissions are updated and applied to the run (includes
+        'run_managers', 'run_monitors').
+
+        Any scope changes required post-deployment/update are propogated through the login_manager
+        and may require an additional login. A new flow checksum/id may be tracked in storage if
+        the flow changed or was newly deployed.
+
+        :param flow_input: A dict of input to be passed to the automate flow. self.check_input()
+                           is called on each tool to ensure basic needs are met for each.
+                           Input MUST be wrapped inside an 'input' dict,
+                           for example {'input': {'foo': 'bar'}}.
+
+        :param use_defaults: Use the result of self.get_input() to populate base input for the
+                             flow. All conflicting input provided by flow_input overrides
+                             values set in use_defaults.
+        :param \**flow_kwargs: Set several keyed arguments that include the label to be used
+                               in the automate app. If no label is passed the standard automate
+                               label is used. Also ensure label <= 64 chars long.
+        :raise: gladier.exc.ConfigException by self.check_input()
+        :raises: gladier.exc.FlowObsolete
+        :raises: gladier.exc.NoFlowRegistered
+        :raises: gladier.exc.RegistrationException
+        :raises: gladier.exc.FunctionObsolete
+        :raises: gladier.exc.AuthException
+        :raises: Any globus_sdk.exc.BaseException
+        """
         flow_id = self.get_flow_id()
 
         permissions = {
             p_type: self.get_flow_permission(p_type)
             for p_type in ['run_managers', 'run_monitors']
             if self.get_flow_permission(p_type)
         }
```

### Comparing `gladier-0.8.4/gladier/managers/funcx_manager.py` & `gladier-0.8.4b1/gladier/managers/funcx_manager.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/managers/login_manager.py` & `gladier-0.8.4b1/gladier/managers/login_manager.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/managers/service_manager.py` & `gladier-0.8.4b1/gladier/managers/service_manager.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/storage/config.py` & `gladier-0.8.4b1/gladier/storage/config.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/storage/migrations.py` & `gladier-0.8.4b1/gladier/storage/migrations.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/storage/tokens.py` & `gladier-0.8.4b1/gladier/storage/tokens.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/utils/automate.py` & `gladier-0.8.4b1/gladier/utils/automate.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/utils/dynamic_imports.py` & `gladier-0.8.4b1/gladier/utils/dynamic_imports.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/utils/flow_generation.py` & `gladier-0.8.4b1/gladier/utils/flow_generation.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/utils/flow_modifiers.py` & `gladier-0.8.4b1/gladier/utils/flow_modifiers.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/utils/flow_traversal.py` & `gladier-0.8.4b1/gladier/utils/flow_traversal.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/utils/funcx_login_manager.py` & `gladier-0.8.4b1/gladier/utils/funcx_login_manager.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/utils/name_generation.py` & `gladier-0.8.4b1/gladier/utils/name_generation.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/utils/tool_alias.py` & `gladier-0.8.4b1/gladier/utils/tool_alias.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier/utils/tool_chain.py` & `gladier-0.8.4b1/gladier/utils/tool_chain.py`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/gladier.egg-info/PKG-INFO` & `gladier-0.8.4b1/gladier.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gladier
-Version: 0.8.4
+Version: 0.8.4b1
 Summary: Tooling for rapid deployment of automation tooling.
 Home-page: https://github.com/globus-gladier/gladier
 Maintainer: 
 Maintainer-email: 
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,14 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Gladier: The Globus Architecture for Data-Intensive Experimental Research.
 ==========================================================================
 |docs|
```

### Comparing `gladier-0.8.4/gladier.egg-info/SOURCES.txt` & `gladier-0.8.4b1/gladier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gladier-0.8.4/setup.py` & `gladier-0.8.4b1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,10 +39,9 @@
         'Operating System :: MacOS :: MacOS X',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
     ]
 )
```


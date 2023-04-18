# Comparing `tmp/TapisCL-ICICLE-0.0.27.tar.gz` & `tmp/TapisCL-ICICLE-0.0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.27.tar", last modified: Tue Apr 18 02:47:00 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.28.tar", last modified: Tue Apr 18 23:40:11 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.27.tar` & `TapisCL-ICICLE-0.0.28.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 02:47:00.110382 TapisCL-ICICLE-0.0.27/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.27/LICENSE
--rw-rw-rw-   0        0        0    43999 2023-04-18 02:47:00.110382 TapisCL-ICICLE-0.0.27/PKG-INFO
--rw-rw-rw-   0        0        0     2089 2023-04-18 01:25:59.000000 TapisCL-ICICLE-0.0.27/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 02:47:00.100554 TapisCL-ICICLE-0.0.27/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/__main__.py
--rw-rw-rw-   0        0        0     1597 2023-04-18 02:12:46.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/args.py
--rw-rw-rw-   0        0        0    10894 2023-04-18 02:36:57.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/cli.py
--rw-rw-rw-   0        0        0     9161 2023-04-18 02:36:33.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/decorators.py
--rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/exceptions.py
--rw-rw-rw-   0        0        0     5754 2023-04-18 02:23:18.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/helpers.py
--rw-rw-rw-   0        0        0     2023 2023-04-18 02:17:20.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/schemas.py
--rw-rw-rw-   0        0        0    10260 2023-04-18 02:42:20.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/server.py
--rw-rw-rw-   0        0        0     1645 2023-04-18 02:26:10.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/socketOpts.py
--rw-rw-rw-   0        0        0    18892 2023-04-18 02:20:35.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/tapisObjectWrappers.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:47:00.108679 TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    43999 2023-04-18 02:47:00.000000 TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-04-18 02:47:00.000000 TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 02:47:00.000000 TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-18 02:47:00.000000 TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-04-18 02:47:00.000000 TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-18 02:47:00.000000 TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-04-18 02:45:35.000000 TapisCL-ICICLE-0.0.27/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 02:47:00.110382 TapisCL-ICICLE-0.0.27/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 23:40:11.605894 TapisCL-ICICLE-0.0.28/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.28/LICENSE
+-rw-rw-rw-   0        0        0    44210 2023-04-18 23:40:11.605391 TapisCL-ICICLE-0.0.28/PKG-INFO
+-rw-rw-rw-   0        0        0     2300 2023-04-18 23:36:28.000000 TapisCL-ICICLE-0.0.28/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 23:40:11.596109 TapisCL-ICICLE-0.0.28/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/__main__.py
+-rw-rw-rw-   0        0        0     1597 2023-04-18 02:12:46.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/args.py
+-rw-rw-rw-   0        0        0    10894 2023-04-18 02:36:57.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/cli.py
+-rw-rw-rw-   0        0        0     9161 2023-04-18 02:36:33.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/decorators.py
+-rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/exceptions.py
+-rw-rw-rw-   0        0        0     5754 2023-04-18 02:23:18.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/helpers.py
+-rw-rw-rw-   0        0        0     2023 2023-04-18 02:17:20.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/schemas.py
+-rw-rw-rw-   0        0        0    10260 2023-04-18 02:42:20.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/server.py
+-rw-rw-rw-   0        0        0     1645 2023-04-18 02:26:10.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/socketOpts.py
+-rw-rw-rw-   0        0        0    19155 2023-04-18 23:35:02.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/tapisObjectWrappers.py
+drwxrwxrwx   0        0        0        0 2023-04-18 23:40:11.604447 TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    44210 2023-04-18 23:40:11.000000 TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-04-18 23:40:11.000000 TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 23:40:11.000000 TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-18 23:40:11.000000 TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-04-18 23:40:11.000000 TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-18 23:40:11.000000 TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2023-04-18 23:39:28.000000 TapisCL-ICICLE-0.0.28/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 23:40:11.605894 TapisCL-ICICLE-0.0.28/setup.cfg
```

### Comparing `TapisCL-ICICLE-0.0.27/LICENSE` & `TapisCL-ICICLE-0.0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.27/PKG-INFO` & `TapisCL-ICICLE-0.0.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.27
+Version: 0.0.28
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -717,7 +717,11 @@
 
 Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
 
 `python -m TapisCLICICLE pods -c help`
 
 this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
 
+**Scripting**
+
+Python and Bash scripting examples are available [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/Scripting-Examples)
+
```

### Comparing `TapisCL-ICICLE-0.0.27/README.md` & `TapisCL-ICICLE-0.0.28/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -27,7 +27,11 @@
 
 Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
 
 `python -m TapisCLICICLE pods -c help`
 
 this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
 
+**Scripting**
+
+Python and Bash scripting examples are available [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/Scripting-Examples)
+
```

### Comparing `TapisCL-ICICLE-0.0.27/TapisCLICICLE/args.py` & `TapisCL-ICICLE-0.0.28/TapisCLICICLE/args.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.27/TapisCLICICLE/cli.py` & `TapisCL-ICICLE-0.0.28/TapisCLICICLE/cli.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.27/TapisCLICICLE/decorators.py` & `TapisCL-ICICLE-0.0.28/TapisCLICICLE/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.27/TapisCLICICLE/exceptions.py` & `TapisCL-ICICLE-0.0.28/TapisCLICICLE/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.27/TapisCLICICLE/helpers.py` & `TapisCL-ICICLE-0.0.28/TapisCLICICLE/helpers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.27/TapisCLICICLE/schemas.py` & `TapisCL-ICICLE-0.0.28/TapisCLICICLE/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.27/TapisCLICICLE/server.py` & `TapisCL-ICICLE-0.0.28/TapisCLICICLE/server.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.27/TapisCLICICLE/socketOpts.py` & `TapisCL-ICICLE-0.0.28/TapisCLICICLE/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.27/TapisCLICICLE/tapisObjectWrappers.py` & `TapisCL-ICICLE-0.0.28/TapisCLICICLE/tapisObjectWrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,15 @@
     """
     @help: Access Tapis pods through the connected service
     """
     def __init__(self, tapis_instance, username, password, connection=None):
         command_map = {
                 'get_pods':self.get_pods,
                 'create_pod':self.create_pod,
+                'start_pod':self.start_pod,
                 'restart_pod':self.restart_pod,
                 'delete_pod':self.delete_pod,
                 'set_pod_perms':self.set_pod_perms,
                 'stop_pod':self.stop_pod,
                 'delete_pod_perms':self.delete_pod_perms,
                 'get_perms':self.get_perms,
                 'copy_pod_password':self.copy_pod_password,
@@ -249,14 +250,21 @@
         """
         @help: create a new pod on the selected Tapis service
         """
         pod_information = self.t.pods.create_pod(pod_id=id, pod_template=template, description=description)
         if verbose:
             return str(pod_information)
         return pod_information
+    
+    def start_pod(self, id: str):
+        """
+        @help: start the pod specified with ID
+        """
+        return_information = self.t.pods.start_pod(pod_id=id)
+        return str(return_information)
 
     @decorators.NeedsConfirmation
     def restart_pod(self, id: str, verbose: bool) -> str:
         """
         @help: initiate a pod restart
         """
         return_information = self.t.pods.restart_pod(pod_id=id)
```

### Comparing `TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.27
+Version: 0.0.28
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -717,7 +717,11 @@
 
 Alternatively, if you do not want to enter the actual command line environment of the TapisCL-ICICLE application, you can run commands directly from the command line like this:
 
 `python -m TapisCLICICLE pods -c help`
 
 this may still ask you for authentication, however once you are logged in once, you do not need to enter your credentials again unless the 5 minute timeout period passes, in which case the application shuts itself off.
 
+**Scripting**
+
+Python and Bash scripting examples are available [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/Scripting-Examples)
+
```

### Comparing `TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.27/pyproject.toml` & `TapisCL-ICICLE-0.0.28/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.27"
+version = "0.0.28"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```


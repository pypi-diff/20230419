# Comparing `tmp/mojo_testplus-0.0.3.tar.gz` & `tmp/mojo_testplus-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_testplus-0.0.3.tar", max compression
+gzip compressed data, was "mojo_testplus-0.0.4.tar", max compression
```

## Comparing `mojo_testplus-0.0.3.tar` & `mojo_testplus-0.0.4.tar`

### file list

```diff
@@ -1,44 +1,54 @@
--rw-r--r--   0        0        0     1083 2023-03-23 04:58:22.729118 mojo_testplus-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0      195 2023-03-23 07:27:52.484881 mojo_testplus-0.0.3/README.md
--rw-r--r--   0        0        0      685 2023-03-23 07:58:17.846032 mojo_testplus-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      350 2023-03-10 15:49:36.503525 mojo_testplus-0.0.3/source/packages/README.md
--rw-r--r--   0        0        0     1415 2023-03-22 03:44:52.832695 mojo_testplus-0.0.3/source/packages/mojo/testplus/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 04:51:36.888730 mojo_testplus-0.0.3/source/packages/mojo/testplus/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 03:58:12.734868 mojo_testplus-0.0.3/source/packages/mojo/testplus/cli/cmdtree/__init__.py
--rw-r--r--   0        0        0      859 2023-03-23 07:58:00.173924 mojo_testplus-0.0.3/source/packages/mojo/testplus/cli/cmdtree/testing/__init__.py
--rw-r--r--   0        0        0     3165 2023-03-23 04:58:22.729118 mojo_testplus-0.0.3/source/packages/mojo/testplus/cli/cmdtree/testing/constants.py
--rw-r--r--   0        0        0     5783 2023-03-23 07:58:00.177924 mojo_testplus-0.0.3/source/packages/mojo/testplus/cli/cmdtree/testing/jobs.py
--rw-r--r--   0        0        0     3831 2023-03-23 07:58:00.177924 mojo_testplus-0.0.3/source/packages/mojo/testplus/cli/cmdtree/testing/query.py
--rw-r--r--   0        0        0    13280 2023-03-23 07:58:00.177924 mojo_testplus-0.0.3/source/packages/mojo/testplus/cli/cmdtree/testing/run.py
--rw-r--r--   0        0        0     1284 2023-03-23 07:58:00.173924 mojo_testplus-0.0.3/source/packages/mojo/testplus/cli/testpluscommand.py
--rw-r--r--   0        0        0     1941 2023-03-20 23:24:48.709671 mojo_testplus-0.0.3/source/packages/mojo/testplus/constraints.py
--rw-r--r--   0        0        0     4752 2023-03-23 07:58:00.169924 mojo_testplus-0.0.3/source/packages/mojo/testplus/entrypoints.py
--rw-r--r--   0        0        0      714 2023-03-21 17:13:07.396394 mojo_testplus-0.0.3/source/packages/mojo/testplus/exceptions.py
--rw-r--r--   0        0        0     4370 2023-03-20 23:24:48.709671 mojo_testplus-0.0.3/source/packages/mojo/testplus/expressions.py
--rw-r--r--   0        0        0      526 2023-03-20 23:24:48.709671 mojo_testplus-0.0.3/source/packages/mojo/testplus/jsos.py
--rw-r--r--   0        0        0     7424 2023-03-20 23:24:48.701671 mojo_testplus-0.0.3/source/packages/mojo/testplus/markers.py
--rw-r--r--   0        0        0     3988 2023-03-23 07:58:00.173924 mojo_testplus-0.0.3/source/packages/mojo/testplus/parameters.py
--rw-r--r--   0        0        0     3228 2023-03-23 07:58:00.169924 mojo_testplus-0.0.3/source/packages/mojo/testplus/queries.py
--rw-r--r--   0        0        0    13374 2023-03-23 07:58:00.169924 mojo_testplus-0.0.3/source/packages/mojo/testplus/recorders.py
--rw-r--r--   0        0        0     1398 2023-03-20 23:24:48.701671 mojo_testplus-0.0.3/source/packages/mojo/testplus/reflection.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296697 mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/__init__.py
--rw-r--r--   0        0        0      691 2023-03-23 07:58:00.177924 mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/integrationsource.py
--rw-r--r--   0        0        0     2991 2023-03-23 07:58:00.177924 mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/parameterorigin.py
--rw-r--r--   0        0        0    10904 2023-03-23 07:58:00.177924 mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/resourceregistry.py
--rw-r--r--   0        0        0    16262 2023-03-23 07:58:00.177924 mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/resourcescope.py
--rw-r--r--   0        0        0      636 2023-03-23 07:58:00.177924 mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/resourcesource.py
--rw-r--r--   0        0        0      743 2023-03-23 07:58:00.177924 mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/scopesource.py
--rw-r--r--   0        0        0     1575 2023-03-21 17:11:05.906189 mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/sourcebase.py
--rw-r--r--   0        0        0      888 2023-03-23 07:58:00.177924 mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/unknownsource.py
--rw-r--r--   0        0        0      391 2023-03-20 23:24:48.709671 mojo_testplus-0.0.3/source/packages/mojo/testplus/resourcelifespan.py
--rw-r--r--   0        0        0     6916 2023-03-23 07:58:00.169924 mojo_testplus-0.0.3/source/packages/mojo/testplus/resources.py
--rw-r--r--   0        0        0    10718 2023-03-20 23:24:48.705671 mojo_testplus-0.0.3/source/packages/mojo/testplus/results.py
--rwxr-xr-x   0        0        0     9165 2023-03-23 07:58:00.173924 mojo_testplus-0.0.3/source/packages/mojo/testplus/testcollector.py
--rw-r--r--   0        0        0     5047 2023-03-23 07:58:03.641945 mojo_testplus-0.0.3/source/packages/mojo/testplus/testgroup.py
--rwxr-xr-x   0        0        0    17729 2023-03-23 07:58:00.169924 mojo_testplus-0.0.3/source/packages/mojo/testplus/testjob.py
--rwxr-xr-x   0        0        0     4516 2023-03-23 07:58:00.169924 mojo_testplus-0.0.3/source/packages/mojo/testplus/testref.py
--rw-r--r--   0        0        0    38037 2023-03-23 07:58:00.173924 mojo_testplus-0.0.3/source/packages/mojo/testplus/testsequencer.py
--rwxr-xr-x   0        0        0     6040 2023-03-20 23:24:48.685671 mojo_testplus-0.0.3/source/packages/mojo/testplus/utilities.py
--rw-r--r--   0        0        0    17493 2023-03-21 17:13:07.396394 mojo_testplus-0.0.3/source/packages/mojo/testplus/verification.py
--rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 mojo_testplus-0.0.3/setup.py
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 mojo_testplus-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-03-23 04:58:22.729118 mojo_testplus-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0      195 2023-03-23 07:27:52.484881 mojo_testplus-0.0.4/README.md
+-rw-r--r--   0        0        0      696 2023-04-19 06:06:27.030557 mojo_testplus-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      551 2023-03-23 14:26:34.599237 mojo_testplus-0.0.4/source/packages/mojo/factories/testplusfactory.py
+-rw-r--r--   0        0        0     1415 2023-03-22 03:44:52.832695 mojo_testplus-0.0.4/source/packages/mojo/testplus/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-23 04:51:36.888730 mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-22 03:58:12.734868 mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-23 07:58:00.173924 mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/__init__.py
+-rw-r--r--   0        0        0     3165 2023-03-23 04:58:22.729118 mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/constants.py
+-rw-r--r--   0        0        0     6102 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/jobs.py
+-rw-r--r--   0        0        0     4130 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/query.py
+-rw-r--r--   0        0        0    13150 2023-04-19 06:05:41.489797 mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/run.py
+-rw-r--r--   0        0        0     1421 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/testplus_command.py
+-rw-r--r--   0        0        0     1941 2023-03-20 23:24:48.709671 mojo_testplus-0.0.4/source/packages/mojo/testplus/constraints.py
+-rw-r--r--   0        0        0      556 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/diagnostics.py
+-rw-r--r--   0        0        0     5089 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/entrypoints.py
+-rw-r--r--   0        0        0      714 2023-03-21 17:13:07.396394 mojo_testplus-0.0.4/source/packages/mojo/testplus/exceptions.py
+-rw-r--r--   0        0        0     4370 2023-03-20 23:24:48.709671 mojo_testplus-0.0.4/source/packages/mojo/testplus/expressions.py
+-rw-r--r--   0        0        0      352 2023-03-23 14:25:46.434788 mojo_testplus-0.0.4/source/packages/mojo/testplus/extensionpoints.py
+-rw-r--r--   0        0        0     1225 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/initialize.py
+-rw-r--r--   0        0        0      526 2023-03-20 23:24:48.709671 mojo_testplus-0.0.4/source/packages/mojo/testplus/jsos.py
+-rw-r--r--   0        0        0     7403 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/markers.py
+-rw-r--r--   0        0        0     3988 2023-03-23 07:58:00.173924 mojo_testplus-0.0.4/source/packages/mojo/testplus/parameters.py
+-rw-r--r--   0        0        0     3228 2023-03-23 07:58:00.169924 mojo_testplus-0.0.4/source/packages/mojo/testplus/queries.py
+-rw-r--r--   0        0        0    13374 2023-03-23 07:58:00.169924 mojo_testplus-0.0.4/source/packages/mojo/testplus/recorders.py
+-rw-r--r--   0        0        0     1398 2023-03-20 23:24:48.701671 mojo_testplus-0.0.4/source/packages/mojo/testplus/reflection.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296697 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/__init__.py
+-rw-r--r--   0        0        0      691 2023-03-23 07:58:00.177924 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/integrationsource.py
+-rw-r--r--   0        0        0     2991 2023-03-23 07:58:00.177924 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/parameterorigin.py
+-rw-r--r--   0        0        0    10904 2023-03-23 07:58:00.177924 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/resourceregistry.py
+-rw-r--r--   0        0        0    16262 2023-03-23 07:58:00.177924 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/resourcescope.py
+-rw-r--r--   0        0        0      636 2023-03-23 07:58:00.177924 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/resourcesource.py
+-rw-r--r--   0        0        0      743 2023-03-23 07:58:00.177924 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/scopesource.py
+-rw-r--r--   0        0        0     1575 2023-03-21 17:11:05.906189 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/sourcebase.py
+-rw-r--r--   0        0        0      888 2023-03-23 07:58:00.177924 mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/unknownsource.py
+-rw-r--r--   0        0        0      391 2023-03-20 23:24:48.709671 mojo_testplus-0.0.4/source/packages/mojo/testplus/resourcelifespan.py
+-rw-r--r--   0        0        0     6916 2023-03-23 07:58:00.169924 mojo_testplus-0.0.4/source/packages/mojo/testplus/resources.py
+-rw-r--r--   0        0        0    10718 2023-03-20 23:24:48.705671 mojo_testplus-0.0.4/source/packages/mojo/testplus/results.py
+-rwxr-xr-x   0        0        0      959 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/__init__.py
+-rw-r--r--   0        0        0    10399 2023-04-19 05:52:19.472744 mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/static/v0/testsummary.css
+-rw-r--r--   0        0        0    38006 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/static/v0/testsummary.js
+-rw-r--r--   0        0        0    23424 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/static/v0/w3.css
+-rw-r--r--   0        0        0     3190 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/tabs/tab-images.html
+-rw-r--r--   0        0        0     3385 2023-04-08 22:20:18.965889 mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/tabs/tab-sounds.html
+-rwxr-xr-x   0        0        0     6714 2023-04-19 05:52:19.472744 mojo_testplus-0.0.4/source/packages/mojo/testplus/templates/testsummary.html
+-rwxr-xr-x   0        0        0     9165 2023-03-23 07:58:00.173924 mojo_testplus-0.0.4/source/packages/mojo/testplus/testcollector.py
+-rw-r--r--   0        0        0     5047 2023-03-23 07:58:03.641945 mojo_testplus-0.0.4/source/packages/mojo/testplus/testgroup.py
+-rwxr-xr-x   0        0        0    17780 2023-04-08 22:20:18.969889 mojo_testplus-0.0.4/source/packages/mojo/testplus/testjob.py
+-rwxr-xr-x   0        0        0     4516 2023-03-23 07:58:00.169924 mojo_testplus-0.0.4/source/packages/mojo/testplus/testref.py
+-rw-r--r--   0        0        0    37901 2023-04-08 22:20:18.969889 mojo_testplus-0.0.4/source/packages/mojo/testplus/testsequencer.py
+-rwxr-xr-x   0        0        0     6040 2023-03-20 23:24:48.685671 mojo_testplus-0.0.4/source/packages/mojo/testplus/utilities.py
+-rw-r--r--   0        0        0    17353 2023-04-08 22:20:18.969889 mojo_testplus-0.0.4/source/packages/mojo/testplus/verification.py
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 mojo_testplus-0.0.4/setup.py
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 mojo_testplus-0.0.4/PKG-INFO
```

### Comparing `mojo_testplus-0.0.3/LICENSE.txt` & `mojo_testplus-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/pyproject.toml` & `mojo_testplus-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "mojo-testplus"
 description = "Automation Mojo TestPlus Test Framework"
-version = "0.0.3"
+version = "0.0.4"
 authors = []
 readme = "README.md"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
 ]
 keywords = [
     "python"
 ]
-packages = [{include = "source/packages"}]
+packages = [{include="mojo", from="source/packages"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 debugpy = "^1.6.5"
 click = "^8.1.3"
-mojo-runtime = "^0.0.14"
+mojo-runtime = "^0.0.19"
 
 [tool.poetry.group.dev.dependencies]
 myst-parser = "^0.18.1"
 sphinx = ">=1.6,<6"
 sphinx-rtd-theme = "^1.1.1"
 
 [build-system]
```

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/__init__.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/cli/cmdtree/testing/__init__.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/cli/cmdtree/testing/constants.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/constants.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/cli/cmdtree/testing/jobs.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/jobs.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
     # We do the imports of the automation framework code inside the action functions because
     # we don't want to startup loggin and the processing of inputs and environment variables
     # until we have entered an action method.  Thats way we know how to setup the environment.
 
     # IMPORTANT: We need to load the context first because it will trigger the loading
     # of the default user configuration
+
     from mojo.xmods.xcollections.context import Context
 
     from mojo.xmods.ximport import import_by_name
     from mojo.xmods.xpython import extend_path
 
     try:
         ctx = Context()
@@ -86,26 +87,34 @@
         # Make sure we extend PATH to include the test root
         extend_path(test_root)
 
         # We perform activation a little later in the testrunner.py file so we can
         # handle exceptions in the context of testrunner_main function
         import mojo.runtime.activation.testrun
 
-        from mojo.xmods.xlogging.foundations import logging_initialize
+        from mojo.testplus.initialize import initialize_testplus_results
+        initialize_testplus_results()
 
         # Initialize logging
+        from mojo.xmods.xlogging.foundations import logging_initialize
         logging_initialize()
+
         logger = logging.getLogger()
 
-        from mojo.testplus.extensionpoints import testplusExtensionPoints
-        akep = testplusExtensionPoints()
+        tpmod = sys.modules["mojo.testplus"]
+        tpmod.logger = logger
+
+
+        from mojo.xmods.wellknown.singletons import SuperFactorySinglton
+        from mojo.testplus.extensionpoints import TestPlusExtensionPoints
 
         # At this point in the code, we either lookup an existing test job or we create a test job
         # from the includes, excludes or test_module
-        TestJobType = akep.get_testplus_default_job_type()
+        sfactory = SuperFactorySinglton()
+        TestJobType = sfactory.get_override_types_by_order(TestPlusExtensionPoints.get_testplus_default_job_type)
 
         if job is not None:
             job_parts = job.split("@")
             if len(job_parts) != 2:
                 errmsg = "A --job parameter must be of the form 'package.module@JobClass'"
                 raise click.UsageError(errmsg)
```

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/cli/cmdtree/testing/query.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/query.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
     # We do the imports of the automation framework code inside the action functions because
     # we don't want to startup loggin and the processing of inputs and environment variables
     # until we have entered an action method.  Thats way we know how to setup the environment.
 
     # IMPORTANT: We need to load the context first because it will trigger the loading
     # of the default user configuration
+
     from mojo.xmods.xcollections.context import Context
     from mojo.xmods.xpython import extend_path
 
     from mojo.runtime.variables import MOJO_RUNTIME_VARIABLES
 
     ctx = Context()
     env = ctx.lookup("/environment")
@@ -64,26 +65,34 @@
 
     # Make sure we extend PATH to include the test root
     extend_path(test_root)
 
     # We use console activation because all our input output is going through the terminal
     import mojo.runtime.activation.console
 
-    from mojo.xmods.xlogging.foundations import logging_initialize
+    from mojo.testplus.initialize import initialize_testplus_results
+    initialize_testplus_results()
+
+    from mojo.xmods.wellknown.singletons import SuperFactorySinglton
+    from mojo.testplus.extensionpoints import TestPlusExtensionPoints
 
     # Initialize logging
+    from mojo.xmods.xlogging.foundations import logging_initialize
     logging_initialize()
+
     logger = logging.getLogger()
 
-    from mojo.testplus.extensionpoints import testplusExtensionPoints
-    akep = testplusExtensionPoints()
+    tpmod = sys.modules["mojo.testplus"]
+    tpmod.logger = logger
+
+    sfactory = SuperFactorySinglton()
+    TestJobType = sfactory.get_override_types_by_order(TestPlusExtensionPoints.get_testplus_default_job_type)
 
     # At this point in the code, we either lookup an existing test job or we create a test job
     # from the includes, excludes or test_module
-    TestJobType = akep.get_testplus_default_job_type()
 
     result_code = 0
     with TestJobType(logger, test_root, includes=includes, excludes=excludes) as tjob:
         query_results = tjob.query()
 
         test_names = [tn for tn in query_results.keys()]
         test_names.sort()
```

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/cli/cmdtree/testing/run.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/cmdtree/testing/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,16 +44,14 @@
     HELP_TOPOLOGY_NAMES,
     HELP_TOPOLOGY_PATH,
     HELP_RUNID,
     HELP_CONSOLE_LOG_LEVEL,
     HELP_FILE_LOG_LEVEL,
     HELP_DEBUGGER,
     HELP_BREAKPOINT,
-    HELP_TIMETRAVEL,
-    HELP_TIMEPORTAL,
     HELP_PRERUN_DIAGNOSTIC,
     HELP_POSTRUN_DIAGNOSTIC,
     HELP_INCLUDE_MARKER_EXP,
     HELP_EXCLUDE_MARKER_EXP
 )
 
 @click.command("run", help="Command used to run collections of tests.")
@@ -67,68 +65,70 @@
 @click.option("--build", default=None, required=False, help=HELP_BUILD)
 @click.option("--flavor", default=None, required=False, help=HELP_FLAVOR)
 @click.option("--job-initiator", default=None, required=False, help=HELP_JOB_INITIATOR)
 @click.option("--job-label", default=None, required=False, help=HELP_JOB_LABEL)
 @click.option("--job-name", default=None, required=False, help=HELP_JOB_NAME)
 @click.option("--job-owner", default=None, required=False, help=HELP_JOB_OWNER)
 @click.option("--credential", "credential_files", multiple=True, default=None, required=False, help=HELP_CREDENTIAL)
-@click.option("--credential-name", "credential_names", default=None, required=False, help=HELP_CREDENTIAL_NAMES)
+@click.option("--credential-name", "credential_names", multiple=True, default=None, required=False, help=HELP_CREDENTIAL_NAMES)
 @click.option("--credential-path", "credential_path", default=None, required=False, help=HELP_CREDENTIAL_PATH)
 @click.option("--landscape", "landscape_files", multiple=True, default=None, required=False, help=HELP_LANDSCAPE)
-@click.option("--landscape-name", "landscape_names", default=None, required=False, help=HELP_LANDSCAPE_NAMES)
+@click.option("--landscape-name", "landscape_names", multiple=True, default=None, required=False, help=HELP_LANDSCAPE_NAMES)
 @click.option("--landscape-path", "landscape_path", default=None, required=False, help=HELP_LANDSCAPE_PATH)
 @click.option("--runtime", "runtime_files", multiple=True, default=None, required=False, help=HELP_RUNTIME)
 @click.option("--runtime-name", "runtime_names", default=None, required=False, help=HELP_RUNTIME_NAMES)
 @click.option("--runtime-path", "runtime_path", default=None, required=False, help=HELP_RUNTIME_PATH)
 @click.option("--topology", "topology_files", multiple=True, default=None, required=False, help=HELP_TOPOLOGY)
-@click.option("--topology-name", "topology_names", default=None, required=False, help=HELP_TOPOLOGY_NAMES)
+@click.option("--topology-name", "topology_names", multiple=True, default=None, required=False, help=HELP_TOPOLOGY_NAMES)
 @click.option("--topology-path", "topology_path", default=None, required=False, help=HELP_TOPOLOGY_PATH)
 @click.option("--console-level", default=None, required=False, type=click.Choice(LOG_LEVEL_NAMES, case_sensitive=False), help=HELP_CONSOLE_LOG_LEVEL)
 @click.option("--logfile-level", default=None, required=False, type=click.Choice(LOG_LEVEL_NAMES, case_sensitive=False), help=HELP_FILE_LOG_LEVEL)
 @click.option("--debugger", default=None, required=False, type=click.Choice(['pdb', 'debugpy']), help=HELP_DEBUGGER)
 @click.option("--breakpoint", "breakpoints", default=None, required=False, multiple=True, type=click.Choice(['test-discovery', 'testrun-start']), help=HELP_BREAKPOINT)
-@click.option("--time-travel", is_flag=True, default=False, required=False, help=HELP_TIMETRAVEL)
-@click.option("--time-portal", "timeportals", default=None, required=False, multiple=True, help=HELP_TIMEPORTAL)
 @click.option("--prerun-diagnostic", is_flag=True, default=False, required=False, help=HELP_PRERUN_DIAGNOSTIC)
 @click.option("--postrun-diagnostic", is_flag=True, default=False, required=False, help=HELP_POSTRUN_DIAGNOSTIC)
 @click.option("--include-marker-exp", required=False, multiple=True, help=HELP_INCLUDE_MARKER_EXP)
 @click.option("--exclude-marker-exp", required=False, multiple=True, help=HELP_EXCLUDE_MARKER_EXP)
 def command_testplus_testing_run(root, includes, excludes, output, start, runid, branch, build, flavor, job_initiator,
-                        job_label, job_name, job_owner, credentials_files, credential_names, credential_path,
+                        job_label, job_name, job_owner, credential_files, credential_names, credential_path,
                         landscape_files, landscape_names, landscape_path, runtime_files, runtime_names, runtime_path,
                         topology_files, topology_names, topology_path, console_level, logfile_level,
-                        debugger, breakpoints, time_travel, timeportals, prerun_diagnostic,
-                        postrun_diagnostic, include_marker_exp, exclude_marker_exp):
+                        debugger, breakpoints, prerun_diagnostic, postrun_diagnostic, include_marker_exp,
+                        exclude_marker_exp):
 
     # pylint: disable=unused-import,import-outside-toplevel
 
     # We do the imports of the automation framework code inside the action functions because
     # we don't want to startup loggin and the processing of inputs and environment variables
     # until we have entered an action method.  Thats way we know how to setup the environment.
 
     # IMPORTANT: We need to load the context first because it will trigger the loading
     # of the default user configuration
+
     from mojo.xmods.xcollections.context import Context, ContextPaths
     from mojo.xmods.xpython import extend_path
 
     from mojo.runtime.variables import JobType, MOJO_RUNTIME_VARIABLES
     
     from mojo.runtime import optionoverrides
 
+    # We perform activation a little later in the testrunner.py file so we can
+    # handle exceptions in the context of testrunner_main function
+    import mojo.runtime.activation.testrun
+
+    from mojo.testplus.initialize import initialize_runtime, initialize_testplus_results
+    initialize_runtime()
+
     ctx = Context()
     env = ctx.lookup("/environment")
 
     # We need to set the job type before we trigger activation.
     env["jobtype"] = JobType.TestRun
 
-    # We perform activation a little later in the testrunner.py file so we can
-    # handle exceptions in the context of testrunner_main function
-    import mojo.runtime.activation.testrun
-
-    from mojo.xmods.xlogging.foundations import logging_initialize
+    initialize_testplus_results()
 
     from mojo.testplus.markers import MetaFilter, parse_marker_expression
 
     if branch is not None:
         optionoverrides.override_build_branch(branch)
 
     if build is not None:
@@ -145,62 +145,62 @@
     
     if job_name is not None:
         optionoverrides.override_job_name(job_name)
 
     if job_owner is not None:
         optionoverrides.override_job_owner(job_owner)
 
-    if credentials_files is not None:
-        optionoverrides.override_config_credential_files(credentials_files)
+    if len(credential_files) > 0:
+        optionoverrides.override_config_credential_files(credential_files)
 
-    if landscape_files is not None and landscape_names is not None:
+    if len(landscape_files) > 0 and len(landscape_names) > 0:
         errmsg = "The '--landscape-file' and '--landscape-name' options should not be used together."
         raise click.BadOptionUsage("landscape-name", errmsg)
 
-    if landscape_files is not None:
+    if len(landscape_files) > 0:
         optionoverrides.override_config_landscape_files(landscape_files)
 
-    if landscape_names is not None:
+    if len(landscape_names) > 0:
         optionoverrides.override_config_landscape_names(landscape_names)
 
-    if landscape_files is not None or landscape_names is not None:
+    if len(landscape_files) > 0 or len(landscape_names) > 0:
         landscape_filenames = MOJO_RUNTIME_VARIABLES.MJR_CONFIG_LANDSCAPE_FILES
         option_name = "landscape" if landscape_files is not None else "landscape-names"
         if not os.path.exists(landscape_filenames):
             errmsg = "The specified landscape file does not exist. filename={}".format(landscape_filenames)
             raise click.BadOptionUsage(option_name, errmsg)
 
-    if runtime_files is not None and runtime_names is not None:
+    if len(runtime_files) > 0 and len(runtime_names) > 0:
         errmsg = "The '--runtime-file' and '--runtime-name' options should not be used together."
         raise click.BadOptionUsage("runtime-name", errmsg)
 
-    if runtime_files is not None:
+    if len(runtime_files) > 0:
         optionoverrides.override_config_runtime_files(runtime_files)
     
-    if runtime_names is not None:
+    if len(runtime_names) > 0:
         optionoverrides.override_config_runtime_names(runtime_names)
     
-    if runtime_files is not None or runtime_names is not None:
+    if len(runtime_files) > 0 or len(runtime_names) > 0:
         runtime_filename = MOJO_RUNTIME_VARIABLES.MJR_CONFIG_RUNTIME_FILES
         option_name = "runtime" if runtime_files is not None else "runtime-names"
         if not os.path.exists(runtime_filename):
             errmsg = "The specified runtime file does not exist. filename={}".format(runtime_filename)
             raise click.BadOptionUsage(option_name, errmsg)
 
-    if topology_files is not None and topology_names is not None:
+    if len(topology_files) > 0 and len(topology_names) > 0:
         errmsg = "The '--topology-file' and '--topology-name' options should not be used together."
         raise click.BadOptionUsage("option_name", errmsg)
 
-    if topology_files is not None:
+    if len(topology_files) > 0:
         optionoverrides.override_config_topology_files(topology_files)
     
-    if topology_names is not None:
+    if len(topology_names) > 0:
         optionoverrides.override_config_topology_names(topology_names)
 
-    if topology_files is not None or topology_names is not None:
+    if len(topology_files) > 0 or len(topology_names) > 0:
         topology_filename = MOJO_RUNTIME_VARIABLES.MJR_CONFIG_TOPOLOGY_FILES
         option_name = "topology" if topology_files is not None else "topology-names"
         if not os.path.exists(topology_filename):
             errmsg = "The specified topology file does not exist. filename={}".format(topology_filename)
             raise click.BadOptionUsage(option_name, errmsg)
 
     if console_level is not None:
@@ -227,20 +227,14 @@
         # default debugger.
         if debugger is None:
             optionoverrides.override_debug_debugger('debugpy')
 
     if debugger is not None:
         optionoverrides.override_debug_debugger('debugpy')
 
-    if time_travel is not None:
-        optionoverrides.override_timetravel(time_travel)
-
-    if timeportals is not None:
-        optionoverrides.override_timeportals(timeportals)
-
     if prerun_diagnostic:
         ctx.insert("/configuration/diagnostics/prerun-diagnostic", {})
     
     if postrun_diagnostic:
         ctx.insert("/configuration/diagnostics/postrun-diagnostic", {})
 
     if root is None:
@@ -275,23 +269,30 @@
     for exmexp in exclude_marker_exp:
         exmexp = exmexp.strip("\"")
         imexp = imexp.strip("'")
         mfilter = parse_marker_expression("-" + imexp)
         metafilters.append(mfilter)
 
     # Initialize logging
+    from mojo.xmods.xlogging.foundations import logging_initialize
     logging_initialize()
+
     logger = logging.getLogger()
 
-    from mojo.testplus.extensionpoints import TestplusExtensionPoints
-    akep = TestplusExtensionPoints()
+    tpmod = sys.modules["mojo.testplus"]
+    tpmod.logger = logger
+
+    from mojo.xmods.wellknown.singletons import SuperFactorySinglton
+    from mojo.testplus.extensionpoints import TestPlusExtensionPoints
 
     # At this point in the code, we either lookup an existing test job or we create a test job
     # from the includes, excludes or test_module
-    TestJobType = akep.get_testplus_default_job_type()
+    sfactory = SuperFactorySinglton()
+    TestJobType = sfactory.get_override_types_by_order(TestPlusExtensionPoints.get_testplus_default_job_type)
+
     result_code = 0
     with TestJobType(logger, test_root, includes=includes, excludes=excludes, metafilters=metafilters) as tjob:
         result_code = tjob.execute()
 
     sys.exit(result_code)
 
     return
```

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/cli/testpluscommand.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/cli/testplus_command.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 
 #!/usr/bin/env python3
 """
-.. module:: akitcommand
+.. module:: testplus_command
     :platform: Darwin, Linux, Unix, Windows
-    :synopsis: The script entrypoint for the 'akit' command.
+    :synopsis: The script entrypoint for the 'testplus' command.
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
@@ -16,19 +16,19 @@
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
 import click
 
-from mojo.testplus.cli.cmdtree.testing import group_akit_testing
+from mojo.testplus.cli.cmdtree.testing import group_testplus_testing
 
-@click.group("akit")
+@click.group("testplus")
 @click.option('-v', '--verbose', count=True)
-def akit_root_command(verbose):
+def testplus_root_command(verbose):
 
     from mojo.runtime.variables import MOJO_RUNTIME_VARIABLES
 
     if verbose == 0:
         MOJO_RUNTIME_VARIABLES.MJR_INTERACTIVE_CONSOLE = True
     else:
         MOJO_RUNTIME_VARIABLES.MJR_INTERACTIVE_CONSOLE = False
@@ -36,13 +36,16 @@
         if verbose == 1:
             MOJO_RUNTIME_VARIABLES.MJR_LOG_LEVEL_CONSOLE = "INFO"
         elif verbose == 2:
             MOJO_RUNTIME_VARIABLES.MJR_LOG_LEVEL_CONSOLE = "DEBUG"
         elif verbose > 2:
             MOJO_RUNTIME_VARIABLES.MJR_LOG_LEVEL_CONSOLE = "NOTSET"
 
+    from mojo.testplus.initialize import initialize_testplus_runtime
+    initialize_testplus_runtime()
+
     return
 
-akit_root_command.add_command(group_akit_testing)
+testplus_root_command.add_command(group_testplus_testing)
 
 if __name__ == '__main__':
-    akit_root_command()
+    testplus_root_command()
```

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/constraints.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/constraints.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/entrypoints.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/entrypoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 .. module:: entrypoints
     :platform: Darwin, Linux, Unix, Windows
     :synopsis: A set of standaridized entry point functions that provide standardized test environment
-               startup and test run commencement utilizing the :class:`akit.testing.unittest.testsequencer.TestSequencer`
+               startup and test run commencement utilizing the :class:`mojo.testplus.testsequencer.TestSequencer`
                object.
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
@@ -33,27 +33,30 @@
 from mojo.runtime.paths import get_path_for_testresults
 from mojo.xmods.xlogging.foundations import logging_initialize
 
 from mojo.testplus.utilities import find_testmodule_root, find_testmodule_fullname
 from mojo.testplus.testjob import DefaultTestJob
 from mojo.testplus.registration.resourceregistry import ResourceRegistry
 
-logger = logging.getLogger()
-
 def generic_test_entrypoint():
     """
         This is the generic test entry point for test modules.  It provides a standardized set of
         commanline parameters that can be used to run test files as scripts.
 
     .. note::
        The `generic_test_entrypoint` is a useful tool to place at the bottom of test files to allow
        them to easily be run for debugging purposes.
     """
+    from mojo.testplus.initialize import initialize_testplus_runtime, initialize_testplus_results
+    initialize_testplus_runtime()
+
     import mojo.runtime.activation.testrun
 
+    initialize_testplus_results()
+
     # We must exit with a result code, initialize it to 0 here
     result_code = 0
 
     base_parser = argparse.ArgumentParser()
 
     base_parser.add_argument("-i", "--include", dest="includes", action="append", default=[], help="Add an include search statement.")
     base_parser.add_argument("-x", "--exclude", dest="excludes", action="append", default=[], help="Add an exclude filter statement.")
@@ -69,14 +72,20 @@
     env["jobtype"] = "testrun"
 
     test_results_dir = get_path_for_testresults()
     if not os.path.exists(test_results_dir):
         os.makedirs(test_results_dir)
     env["output_directory"] = test_results_dir
 
+    from mojo.xmods.xlogging.foundations import logging_initialize
+    logging_initialize()
+
+    tpmod = sys.modules["mojo.testplus"]
+    tpmod.logger = logging.getLogger()
+
     testroot = find_testmodule_root(test_module)
     module_fullname = find_testmodule_fullname(test_module, testroot=testroot)
     
     module_lastdot = module_fullname.rfind('.')
     if module_lastdot > -1:
         # We need to import every module up to the test module
         parent_module_name = module_fullname[:module_lastdot]
@@ -107,14 +116,15 @@
 
         resource_registry = ResourceRegistry()
         resource_registry.rename_resource_origins_from_main(module_fullname)
 
     args = base_parser.parse_args()
 
     logging_initialize()
+    logger = logging.getLogger()
 
     includes = args.includes
     excludes = args.excludes
     if len(includes) == 0:
         includes.append("*")
 
     result_code = 0
```

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/exceptions.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/exceptions.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/expressions.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/expressions.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/jsos.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/jsos.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/markers.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/markers.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 __license__ = "MIT"
 
 from typing import Any, Callable, Dict, List
 
 import inspect
 
 
-from mojo.xmods.exceptions import SemanticError, NotImplementedError
+from mojo.xmods.exceptions import SemanticError
 
 
 def mark_categories(*, categories: List[str]):
     """
         Used to mark a test with category markers.
     """
```

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/parameters.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/parameters.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/queries.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/queries.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/recorders.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/recorders.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/reflection.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/reflection.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/integrationsource.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/integrationsource.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/parameterorigin.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/parameterorigin.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/resourceregistry.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/resourceregistry.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/resourcescope.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/resourcescope.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/resourcesource.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/resourcesource.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/scopesource.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/scopesource.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/sourcebase.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/sourcebase.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/registration/unknownsource.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/registration/unknownsource.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/resources.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/resources.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/results.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/results.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/testcollector.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/testcollector.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/testgroup.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/testgroup.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/testjob.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/testjob.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,32 +12,29 @@
 __credits__ = []
 __version__ = "1.0.0"
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
-from typing import List, Optional
+from typing import List, Optional, Protocol
 
 import os
 import traceback
 
-from mojo.xmods.xcollections.context import ContextUser
+from mojo.xmods.xcollections.context import ContextUser, ContextPaths
+from mojo.xmods.wellknown.singletons import LandscapeSingleton
+from mojo.xmods.xformatting import CommandOutputFormat
+from mojo.xmods.xdebugger import WELLKNOWN_BREAKPOINTS, debugger_wellknown_breakpoint_entry
 
 from mojo.runtime.variables import MOJO_RUNTIME_VARIABLES
 
-
 from mojo.testplus.recorders import JsonResultRecorder
-
-from mojo.xmods.wellknown.singletons import LandscapeSingleton
-from mojo.xmods.xformatting import CommandOutputFormat
-
 from mojo.testplus.testsequencer import TestSequencer
 
-from mojo.xmods.xdebugger import WELLKNOWN_BREAKPOINTS, debugger_wellknown_breakpoint_entry
 
 class TestJob(ContextUser):
     """
         The :class:`TestJob` spans the execution of all :class:`TestPack` and organizes the
         flow of execution of test packs.  It allows for the sequencing of the execution of test
         packs so as to optimize the time test runs spend performing setup and tearnown tasks.  This
         allows for the optimization of infrastructure resources.
@@ -81,15 +78,14 @@
             self.includes = includes
             self.excludes = excludes
 
         self.metafilters = metafilters
 
         self._test_module = test_module
         self._parser = parser
-        self._runid = None
         self._starttime = None
 
         self._test_results_dir = None
         self._result_filename = None
         self._summary_filename = None
         self._import_errors_filename = None
 
@@ -98,14 +94,15 @@
         self._apod = MOJO_RUNTIME_VARIABLES.MJR_AUTOMATION_POD
         self._branch = MOJO_RUNTIME_VARIABLES.MJR_BUILD_BRANCH
         self._build = MOJO_RUNTIME_VARIABLES.MJR_BUILD_NAME
         self._flavor = MOJO_RUNTIME_VARIABLES.MJR_BUILD_FLAVOR
         self._build_url = MOJO_RUNTIME_VARIABLES.MJR_BUILD_URL
 
         self._job_initiator = MOJO_RUNTIME_VARIABLES.MJR_JOB_INITIATOR
+        self._job_id = MOJO_RUNTIME_VARIABLES.MJR_JOB_ID
         self._job_label = MOJO_RUNTIME_VARIABLES.MJR_JOB_LABEL
         self._job_name = MOJO_RUNTIME_VARIABLES.MJR_JOB_NAME
         self._job_owner = MOJO_RUNTIME_VARIABLES.MJR_JOB_OWNER
         self._job_type = MOJO_RUNTIME_VARIABLES.MJR_JOB_TYPE
 
         self._import_errors = []
 
@@ -124,19 +121,20 @@
         return self._import_errors
 
     def begin(self):
         """
             Called at the beginning of a test job in order to setup the recording of test results.
         """
 
+        
+
         env = self.context.lookup("/environment")
 
         self._test_results_dir = env["output_directory"]
         self._starttime = env["starttime"]
-        self._runid = env["runid"]
 
         self._result_filename = os.path.join(self._test_results_dir, "testrun_results.jsos")
         self._summary_filename = os.path.join(self._test_results_dir, "testrun_summary.json")
         self._import_errors_filename = os.path.join(self._test_results_dir, "import_errors.jsos")
         self._testrun_sequence_filename = os.path.join(self._test_results_dir, "testrun_sequence.py")
         
         return
@@ -149,17 +147,16 @@
 
         with self._create_sequencer() as tseq:
             # IMPORTANT: The ordering of the automation sequence is extremely important.  Proper
             # ordering of these steps ensures that the correct things are happening in the correct
             # order in the automation code and that we provide the ability for configuration
             # issues to be discovered as early as possible.
 
-            env = self.context.lookup("/environment")
-            debugger = env["debugger"]
-            breakpoints = env["breakpoints"]
+            debugger = self.context.lookup(ContextPaths.DEBUG_DEBUGGER, None)
+            breakpoints = self.context.lookup(ContextPaths.DEBUG_BREAKPOINTS, None)
 
             # STEP 1: We discover the tests first so we can build a listing of the
             # Integration and Scope couplings.  We don't want to execute any test code, setup,
             # or teardown code at this point.  We want to seperate out the integration
             # code from the test code and run the integration code first so we can discover
             # integration issues independant of the test code itself.
             self._logger.section("Discovery")
@@ -241,15 +238,15 @@
                 tseq.expand_test_tree_based_on_query()
 
                 self._logger.section("Generating Test Run Sequence")
                 # STEP 10: Generate the test run sequence document that will be used or the run.
                 tseq.generate_testrun_sequence_document(self._testrun_sequence_filename)
 
                 title = self.title
-                runid = self._runid
+                runid = self._job_id
                 start = str(self._starttime)
                 sum_file = self._summary_filename
                 res_file = self._result_filename
                 apod = self._apod
                 branch = self._branch
                 build = self._build
                 flavor = self._flavor
```

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/testref.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/testref.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/testsequencer.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/testsequencer.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 import json
 import logging
 import os
 import sys
 import uuid
 
 from mojo.xmods.xcollections.context import ContextUser
-from mojo.xmods.exceptions import SemanticError, format_exception
+from mojo.xmods.exceptions import SemanticError
 from mojo.xmods.ximport import import_file
-
-from akit.xconfiguration import DiagnosticLabel, RuntimeConfigPaths
+from mojo.xmods.xtraceback import format_exception
 
 from mojo.runtime.paths import get_path_for_diagnostics, get_path_for_output
 
+from mojo.testplus.diagnostics import DiagnosticLabel, RuntimeConfigPaths
 from mojo.testplus.exceptions import SkitTestError
 from mojo.testplus.jsos import CHAR_RECORD_SEPERATOR
 from mojo.testplus.results import ResultCode, ResultContainer, ResultNode, ResultType
 from mojo.testplus.recorders import ResultRecorder
 
 from mojo.testplus.constraints import Constraints
 from mojo.testplus.testcollector import TestCollector
@@ -58,17 +58,17 @@
     This is a code generated execution sequence document, do not manually edit this document.  The 'testplus'
     test framework generates this document in order to layout the test run scopes, parameter creations, and
     test calls in a user ledgible way which is easy to read and also to debug.
 """
 
 __traceback_format_policy__ = "Brief"
 
-from akit.xlogging.foundations import getAutomatonKitLogger
+import logging
 
-logger = getAutomatonKitLogger()
+logger = logging.getLogger()
 
 {}
 
 {}
 
 '''.format(CONSTRAINT_IMPORT_INSERTION_POINT, FACTORY_IMPORT_INSERTION_POINT)
 
@@ -763,16 +763,14 @@
             '{}"""'.format(current_indent),
             '{}This is the entry point for the test run sequence document.'.format(indent_space),
             '{}"""'.format(current_indent)
         ]
 
         debugger_wellknown_breakpoint_code_append(WELLKNOWN_BREAKPOINTS.TESTRUN_START, method_lines, current_indent)
 
-        current_indent += timemachine_timeportal_code_append(WELLKNOWN_PORTALS.TESTRUN_START, method_lines, current_indent)
-
         method_lines.append('')
         method_lines.append('{}with sequencer.enter_session_scope_context() as ssc:'.format(current_indent))
         method_lines.append('')
 
         current_indent = current_indent + indent_space
 
         this_scope = root_node.get_resource_scope()
```

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/utilities.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/utilities.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.3/source/packages/mojo/testplus/verification.py` & `mojo_testplus-0.0.4/source/packages/mojo/testplus/verification.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,32 +13,32 @@
 import os
 import re
 
 from pprint import pformat
 
 from mojo.xmods.xformatting import indent_lines
 
-from mojo.xmods.exceptions import AKitAssertionError, TracebackFormatPolicy
+from mojo.xmods.xtraceback import TracebackFormatPolicy
 
 __traceback_format_policy__ = TracebackFormatPolicy.Hide
 
 PREFIX_STD = "Result"
 PREFIX_API = "'{}' API result"
 
 def assert_dict_response_has_keys(to_inspect: dict, expected_keys: List[str], api: Optional[str] = None):
     """
         Verifies that the specified return result from the specified API has the specified expected keys.  If the
-        verification fails then an :class:`AKitAssertionError` is created and return, otherwise None is returned. It
+        verification fails then an :class:`AssertionError` is created and return, otherwise None is returned. It
         is the resposibility of the calling test to raise the returned error.
 
         :param to_inspect: The dictionary being inspected
         :param expected_keys: The list of expected keys
         :param api: The optional name of the API that returned the result being inspected.
         
-        :returns: None or an :class:`AKitAssertionError` for the caller to raise.
+        :returns: None or an :class:`AssertionError` for the caller to raise.
     """
 
     template = "    '{}' key not found."
 
     content_errors = verify_dict_has_keys(to_inspect, expected_keys, template)
     if len(content_errors) > 0:
 
@@ -48,29 +48,29 @@
             "{} verification failed with the following errors:".format(msg_prefix)
         ]
 
         for nxtce in content_errors:
             err_msg_lines.append(nxtce)
 
         errmsg = os.linesep.join(err_msg_lines)
-        raise AKitAssertionError(errmsg)
+        raise AssertionError(errmsg)
 
     return
 
 def assert_dict_response_has_paths(to_inspect: dict, expected_paths: List[str], api: Optional[str] = None):
     """
         Verifies that the specified return result from the specified API has the specified expected paths.  If the
-        verification fails then an :class:`AKitAssertionError` is created and return, otherwise None is returned. It
+        verification fails then an :class:`AssertionError` is created and return, otherwise None is returned. It
         is the resposibility of the calling test to raise the returned error.
 
         :param to_inspect: The dictionary being inspected
         :param expected_keys: The list of expected keys
         :param api: The name of the API that returned the result being inspected.
         
-        :returns: None or an :class:`AKitAssertionError` for the caller to raise.
+        :returns: None or an :class:`AssertionError` for the caller to raise.
     """
 
     template = "    '{}' path not found."
 
     content_errors = verify_dict_has_paths(to_inspect, expected_paths, template)
     if len(content_errors) > 0:
 
@@ -80,30 +80,30 @@
             "{} verification failed with the following errors:".format(msg_prefix)
         ]
 
         for nxtce in content_errors:
             err_msg_lines.append(nxtce)
 
         errmsg = os.linesep.join(err_msg_lines)
-        raise AKitAssertionError(errmsg)
+        raise AssertionError(errmsg)
 
     return
 
 
 def assert_equal(found: Any, expected: Any, api: Optional[str] = None):
     """
         Verifies that the specified return result from the specified API has the specified expected value.
-        If the verification fails then an :class:`AKitAssertionError` is created and returned, otherwise None
+        If the verification fails then an :class:`AssertionError` is created and returned, otherwise None
         is returned. It is the resposibility of the calling test to raise the returned error.
 
         :param found: The value to be compared
         :param expected: The expected value
         :param api: The name of the API that returned the result being inspected.
         
-        :returns: None or an :class:`AKitAssertionError` for the caller to raise.
+        :returns: None or an :class:`AssertionError` for the caller to raise.
     """
 
     if found != expected:
 
         msg_prefix = PREFIX_STD if api is None else PREFIX_API.format(api)
 
         err_msg_lines = [
@@ -124,29 +124,29 @@
             err_msg_lines.append("FOUND: {}".format(found_format_lines[0]))
         elif len(found_format_lines) > 1:
             err_msg_lines.append("FOUND:")
             found_format_lines = indent_lines(found_format_lines, 1)
             err_msg_lines.extend(found_format_lines)
 
         errmsg = os.linesep.join(err_msg_lines)
-        raise AKitAssertionError(errmsg)
+        raise AssertionError(errmsg)
 
     return
 
 def assert_expression(found: str, expr: Union[str, re.Pattern], api: Optional[str] = None):
     """
         Verifies that the specified return result from the specified API has the specified expected value.
-        If the verification fails then an :class:`AKitAssertionError` is created and returned, otherwise None
+        If the verification fails then an :class:`AssertionError` is created and returned, otherwise None
         is returned. It is the resposibility of the calling test to raise the returned error.
 
         :param found: The value to be compared
         :param expr: An expression to match with the found value.
         :param api: The name of the API that returned the result being inspected.
         
-        :returns: None or an :class:`AKitAssertionError` for the caller to raise.
+        :returns: None or an :class:`AssertionError` for the caller to raise.
     """
 
     if not isinstance(expr, re.Pattern):
         expr = re.compile(expr)
 
     mobj = expr.match(found)
     if mobj is None:
@@ -156,30 +156,30 @@
         err_msg_lines = [
             "{} verification failed because the found value did not match expression provided.".format(msg_prefix),
             "FOUND: {}".format(found),
             "EXPR: {}".format(expr)
         ]
 
         errmsg = os.linesep.join(err_msg_lines)
-        raise AKitAssertionError(errmsg)
+        raise AssertionError(errmsg)
 
     return
 
 def assert_greater(found: Any, boundary: Any, api: Optional[str] = None):
     """
         Verifies that the specified return result from the specified API has a value greater than the
-        boundary specified. If the verification fails then an :class:`AKitAssertionError` is created
+        boundary specified. If the verification fails then an :class:`AssertionError` is created
         and returned, otherwise None is returned. It is the resposibility of the calling test to raise
         the returned error.
 
         :param found: The value being compared
         :param boundry: The boundary value being compared against
         :param api: The name of the API that returned the result being inspected.
         
-        :returns: None or an :class:`AKitAssertionError` for the caller to raise.
+        :returns: None or an :class:`AssertionError` for the caller to raise.
     """
 
     if not found > boundary:
 
         msg_prefix = PREFIX_STD if api is None else PREFIX_API.format(api)
 
         err_msg_lines = [
@@ -199,30 +199,30 @@
             err_msg_lines.append("FOUND: {}".format(found_format_lines[0]))
         elif len(found_format_lines) > 1:
             err_msg_lines.append("FOUND:")
             found_format_lines = indent_lines(found_format_lines, 1)
             err_msg_lines.extend(found_format_lines)
 
         errmsg = os.linesep.join(err_msg_lines)
-        raise AKitAssertionError(errmsg)
+        raise AssertionError(errmsg)
 
     return
 
 def assert_lessthan(found: Any, boundary: Any, api: Optional[str] = None):
     """
         Verifies that the specified return result from the specified API has a value less than the
-        boundary specified. If the verification fails then an :class:`AKitAssertionError` is created
+        boundary specified. If the verification fails then an :class:`AssertionError` is created
         and returned, otherwise None is returned. It is the resposibility of the calling test to raise
         the returned error.
 
         :param found: The value being compared
         :param boundry: The boundary value being compared against
         :param api: The name of the API that returned the result being inspected.
         
-        :returns: None or an :class:`AKitAssertionError` for the caller to raise.
+        :returns: None or an :class:`AssertionError` for the caller to raise.
     """
 
     if not found < boundary:
 
         msg_prefix = PREFIX_STD if api is None else PREFIX_API.format(api)
 
         err_msg_lines = [
@@ -242,30 +242,30 @@
             err_msg_lines.append("FOUND: {}".format(found_format_lines[0]))
         elif len(found_format_lines) > 1:
             err_msg_lines.append("FOUND:")
             found_format_lines = indent_lines(found_format_lines, 1)
             err_msg_lines.extend(found_format_lines)
 
         errmsg = os.linesep.join(err_msg_lines)
-        raise AKitAssertionError(errmsg)
+        raise AssertionError(errmsg)
 
     return
 
 
 def assert_list_length(to_inspect: List, expected_len: int, api: Optional[str] = None):
     """
         Verifies that the specified return result from the specified API has the specified expected number of items.
-        If the verification fails then an :class:`AKitAssertionError` is created and returned, otherwise None
+        If the verification fails then an :class:`AssertionError` is created and returned, otherwise None
         is returned. It is the resposibility of the calling test to raise the returned error.
 
         :param to_inspect: The list being inspected
         :param expected_len: The expected length of the list
         :param api: The name of the API that returned the result being inspected.
         
-        :returns: None or an :class:`AKitAssertionError` for the caller to raise.
+        :returns: None or an :class:`AssertionError` for the caller to raise.
     """
 
     found_len = len(to_inspect)
     if found_len != expected_len:
 
         msg_prefix = PREFIX_STD if api is None else PREFIX_API.format(api)
 
@@ -276,29 +276,29 @@
         ]
 
         for fitem in to_inspect:
             err_msg_lines.append("    {}".format(fitem))
         err_msg_lines.append("")
 
         errmsg = os.linesep.join(err_msg_lines)
-        raise AKitAssertionError(errmsg)
+        raise AssertionError(errmsg)
 
     return
 
 def assert_list_length_greater(to_inspect: List, boundary_len: int, api: Optional[str] = None):
     """
         Verifies that the specified return result from the specified API has more items than the specified expected
-        number of items.  If the verification fails then an :class:`AKitAssertionError` is created and returned,
+        number of items.  If the verification fails then an :class:`AssertionError` is created and returned,
         otherwise None is returned. It is the resposibility of the calling test to raise the returned error.
 
         :param to_inspect: The list being inspected
         :param boundary_len: The boundary that the list length should exceed.
         :param api: The name of the API that returned the result being inspected.
         
-        :returns: None or an :class:`AKitAssertionError` for the caller to raise.
+        :returns: None or an :class:`AssertionError` for the caller to raise.
     """
 
     found_len = len(to_inspect)
     if not found_len > boundary_len:
 
         msg_prefix = PREFIX_STD if api is None else PREFIX_API.format(api)
 
@@ -309,29 +309,29 @@
         ]
 
         for fitem in to_inspect:
             err_msg_lines.append("    {}".format(fitem))
         err_msg_lines.append("")
 
         errmsg = os.linesep.join(err_msg_lines)
-        raise AKitAssertionError(errmsg)
+        raise AssertionError(errmsg)
 
     return
 
 def assert_list_length_less(to_inspect: List, boundary_len: int, api: Optional[str] = None):
     """
         Verifies that the specified return result from the specified API has less items than the specified expected
-        number of items.  If the verification fails then an :class:`AKitAssertionError` is created and returned,
+        number of items.  If the verification fails then an :class:`AssertionError` is created and returned,
         otherwise None is returned. It is the resposibility of the calling test to raise the returned error.
 
         :param to_inspect: The list being inspected
         :param boundary_len: The boundary the list length should not exceed
         :param api: The name of the API that returned the result being inspected.
         
-        :returns: None or an :class:`AKitAssertionError` for the caller to raise.
+        :returns: None or an :class:`AssertionError` for the caller to raise.
     """
     
     found_len = len(to_inspect)
     if not found_len < boundary_len:
 
         msg_prefix = PREFIX_STD if api is None else PREFIX_API.format(api)
         
@@ -342,44 +342,44 @@
         ]
 
         for fitem in to_inspect:
             err_msg_lines.append("    {}".format(fitem))
         err_msg_lines.append("")
 
         errmsg = os.linesep.join(err_msg_lines)
-        raise AKitAssertionError(errmsg)
+        raise AssertionError(errmsg)
 
     return
 
 
 def assert_type(found: Any, exp_type: Type, api: Optional[str] = None):
     """
         Verifies that the specified return result from the specified API has the specified expected value type.
-        If the verification fails then an :class:`AKitAssertionError` is created and returned, otherwise None
+        If the verification fails then an :class:`AssertionError` is created and returned, otherwise None
         is returned. It is the resposibility of the calling test to raise the returned error.
 
         :param found: The value to check the type of
         :param exp_type: The expected value type
         :param api: The name of the API that returned the result being inspected.
         
-        :returns: None or an :class:`AKitAssertionError` for the caller to raise.
+        :returns: None or an :class:`AssertionError` for the caller to raise.
     """
 
     found_type = type(found)
     if found_type != exp_type:
 
         msg_prefix = PREFIX_STD if api is None else PREFIX_API.format(api)
 
         err_msg_lines = [
             "{} verification failed because the found value did not the expected type={}.".format(msg_prefix, exp_type),
             "FOUND_TYPE: {}".format(found_type)
         ]
 
         errmsg = os.linesep.join(err_msg_lines)
-        raise AKitAssertionError(errmsg)
+        raise AssertionError(errmsg)
 
     return
 
 
 def verify_dict_has_keys(to_inspect: dict, expected_keys: List[str], template: Optional[str]=None) -> List[str]:
     """
         Verifies that the expected keys are found in the dictionary provided.  Returns a list of
```

### Comparing `mojo_testplus-0.0.3/PKG-INFO` & `mojo_testplus-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-testplus
-Version: 0.0.3
+Version: 0.0.4
 Summary: Automation Mojo TestPlus Test Framework
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: debugpy (>=1.6.5,<2.0.0)
-Requires-Dist: mojo-runtime (>=0.0.14,<0.0.15)
+Requires-Dist: mojo-runtime (>=0.0.19,<0.0.20)
 Description-Content-Type: text/markdown
 
 # Automation Mojo - Testplus 
 This is preliminary release of the 'testplus' automation framework in a separate package from
 the AutomationKit.  This release is not ready for public consumption.
```


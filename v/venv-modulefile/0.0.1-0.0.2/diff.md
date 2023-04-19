# Comparing `tmp/venv-modulefile-0.0.1.tar.gz` & `tmp/venv-modulefile-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/extend_python_venv_with_environment_modules/dist/tmpm4a6u9ix/venv-modulefile-0.0.1.ta", last modified: Wed Apr 19 16:45:48 2023, max compression
+gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/extend_python_venv_with_environment_modules/dist/tmp3h54xkcm/venv-modulefile-0.0.2.ta", last modified: Wed Apr 19 17:39:53 2023, max compression
```

## Comparing `venv-modulefile-0.0.1.tar` & `venv-modulefile-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-04-19 16:45:48.000000 venv-modulefile-0.0.1/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1188 2023-04-19 16:45:48.000000 venv-modulefile-0.0.1/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-04-19 16:42:52.000000 venv-modulefile-0.0.1/pyproject.toml
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2023-04-19 16:45:48.000000 venv-modulefile-0.0.1/setup.cfg
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       22 2023-04-19 16:42:18.000000 venv-modulefile-0.0.1/MANIFEST.in
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      909 2023-04-18 14:24:37.000000 venv-modulefile-0.0.1/README.md
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9512 2023-04-19 16:34:34.000000 venv-modulefile-0.0.1/setup.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-04-19 16:45:48.000000 venv-modulefile-0.0.1/src/
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-04-19 16:45:48.000000 venv-modulefile-0.0.1/src/venvmod/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-04-19 16:37:23.000000 venv-modulefile-0.0.1/src/venvmod/VERSION
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       45 2023-04-19 16:36:02.000000 venv-modulefile-0.0.1/src/venvmod/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1666 2023-04-19 15:36:05.000000 venv-modulefile-0.0.1/src/venvmod/tools.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-04-19 16:45:48.000000 venv-modulefile-0.0.1/src/venvmod/commands/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1236 2023-04-19 11:41:45.000000 venv-modulefile-0.0.1/src/venvmod/commands/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2894 2023-04-19 16:35:42.000000 venv-modulefile-0.0.1/src/venvmod/commands/create_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4654 2023-04-19 16:34:49.000000 venv-modulefile-0.0.1/src/venvmod/commands/append_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    10971 2023-04-19 15:26:15.000000 venv-modulefile-0.0.1/src/venvmod/modulefile.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       47 2023-04-19 09:35:41.000000 venv-modulefile-0.0.1/src/README.md
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-04-19 16:45:48.000000 venv-modulefile-0.0.1/src/venv_modulefile.egg-info/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      744 2023-04-19 16:45:48.000000 venv-modulefile-0.0.1/src/venv_modulefile.egg-info/entry_points.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2023-04-19 16:45:48.000000 venv-modulefile-0.0.1/src/venv_modulefile.egg-info/top_level.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      530 2023-04-19 16:45:48.000000 venv-modulefile-0.0.1/src/venv_modulefile.egg-info/SOURCES.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1188 2023-04-19 16:45:48.000000 venv-modulefile-0.0.1/src/venv_modulefile.egg-info/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2023-04-19 16:45:48.000000 venv-modulefile-0.0.1/src/venv_modulefile.egg-info/dependency_links.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      229 2023-04-19 16:45:48.000000 venv-modulefile-0.0.1/src/venv_modulefile.egg-info/requires.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-04-18 14:24:37.000000 venv-modulefile-0.0.1/LICENSE.md
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1188 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-04-19 16:42:52.000000 venv-modulefile-0.0.2/pyproject.toml
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/setup.cfg
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       22 2023-04-19 16:42:18.000000 venv-modulefile-0.0.2/MANIFEST.in
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      909 2023-04-18 14:24:37.000000 venv-modulefile-0.0.2/README.md
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9590 2023-04-19 17:34:33.000000 venv-modulefile-0.0.2/setup.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venvmod/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-04-19 17:38:08.000000 venv-modulefile-0.0.2/src/venvmod/VERSION
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       45 2023-04-19 16:36:02.000000 venv-modulefile-0.0.2/src/venvmod/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1666 2023-04-19 15:36:05.000000 venv-modulefile-0.0.2/src/venvmod/tools.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venvmod/commands/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1336 2023-04-19 17:34:50.000000 venv-modulefile-0.0.2/src/venvmod/commands/test_imports.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1236 2023-04-19 11:41:45.000000 venv-modulefile-0.0.2/src/venvmod/commands/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2894 2023-04-19 16:35:42.000000 venv-modulefile-0.0.2/src/venvmod/commands/create_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4578 2023-04-19 17:36:07.000000 venv-modulefile-0.0.2/src/venvmod/commands/append_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    10971 2023-04-19 15:26:15.000000 venv-modulefile-0.0.2/src/venvmod/modulefile.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       47 2023-04-19 09:35:41.000000 venv-modulefile-0.0.2/src/README.md
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venv_modulefile.egg-info/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      809 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venv_modulefile.egg-info/entry_points.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venv_modulefile.egg-info/top_level.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      567 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venv_modulefile.egg-info/SOURCES.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1188 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venv_modulefile.egg-info/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venv_modulefile.egg-info/dependency_links.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      229 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venv_modulefile.egg-info/requires.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-04-18 14:24:37.000000 venv-modulefile-0.0.2/LICENSE.md
```

### Comparing `venv-modulefile-0.0.1/PKG-INFO` & `venv-modulefile-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-modulefile
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python venv extension using Modulefile
 Home-page: https://github.com/roland-lenain/venv-modulefile
 Author: R. Lenain
 Author-email: roland.lenain@cea.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/roland-lenain/venv-modulefile/issues
 Project-URL: Doc, https://icoco-python.readthedocs.io/en/latest/index.html
```

### Comparing `venv-modulefile-0.0.1/README.md` & `venv-modulefile-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.0.1/setup.py` & `venv-modulefile-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,23 +169,24 @@
     },
     # Entry points. The following would provide a command called `sample` which
     # executes the function `main` from this package when invoked:
     entry_points={  # Optional
         "console_scripts": [
             "venvmod-initialize=venvmod.commands.create_module:initialize",
             "venvmod-add-appli=venvmod.commands.create_module:add_appli",
-            "venvmod-cmd-read_env=venvmod.commands.append_module:read_env",
+            "venvmod-cmd-read-env=venvmod.commands.append_module:read_env",
             "venvmod-cmd-module-use=venvmod.commands.append_module:module_use",
             "venvmod-cmd-module-load=venvmod.commands.append_module:module_load",
             "venvmod-cmd-source-sh=venvmod.commands.append_module:source_sh",
             "venvmod-cmd-prepend-path=venvmod.commands.append_module:prepend_path",
             "venvmod-cmd-append-path=venvmod.commands.append_module:append_path",
             "venvmod-cmd-setenv=venvmod.commands.append_module:setenv",
             "venvmod-cmd-remove-path=venvmod.commands.append_module:remove_path",
             "venvmod-cmd-set-aliases=venvmod.commands.append_module:set_aliases",
+            "venvmod-test-import=venvmod.commands.test_imports:test_imports",
         ],
     },
     # List additional URLs that are relevant to your project as a dict.
     #
     # This field corresponds to the "Project-URL" metadata fields:
     # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
     #
```

### Comparing `venv-modulefile-0.0.1/src/venvmod/tools.py` & `venv-modulefile-0.0.2/src/venvmod/tools.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.0.1/src/venvmod/commands/__init__.py` & `venv-modulefile-0.0.2/src/venvmod/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.0.1/src/venvmod/commands/create_module.py` & `venv-modulefile-0.0.2/src/venvmod/commands/create_module.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.0.1/src/venvmod/commands/append_module.py` & `venv-modulefile-0.0.2/src/venvmod/commands/append_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,35 +89,37 @@
                              with_appli=True)
         appli = options.appli if options.appli else options.virtual_env
         appli = str(Path(appli).stem)  #virtual_env may be a path
         virtual_env = options.virtual_env
     else:
         virtual_env, appli = arguments
 
-        path_to_prepend = ["LD_LIBRARY_PATH", "PATH", "PYTHONPATH"]
-        for envvar, value in os.environ.items():
-            if not envvar.lower().startswith(appli.lower()):
-                continue
-            for path in path_to_prepend:
-                if envvar.endswith(path):
-                    prepend_path(arguments=(virtual_env, appli, path + " " + value.replace(":", " ")))
-
-            if envvar.endswith("MODULE_USE"):
-                module_use(arguments=(virtual_env, appli, value))
-
-            if envvar.endswith("MODULEFILES"):
-                module_load(arguments=(virtual_env, appli, value))
-
-            if envvar.endswith("SOURCEFILES"):
-                source_sh(arguments=(virtual_env, appli, value))
-
-            if envvar.endswith("ADDITIONAL_EXPORTS"):
-                for var in value.split():
-                    setenv(arguments=(virtual_env, appli, var.replace("=", " ")))
-
-            if envvar.endswith("ALIASES"):
-                for var in value.split():
-                    set_aliases(arguments=(virtual_env, appli, var.replace("=", " ")))
-
-            if envvar.endswith("REMOVE_PATHS"):
-                for var in value.split():
-                    remove_path(arguments=(virtual_env, appli, var.replace("=", " ")))
+    path_to_prepend = ["LD_LIBRARY_PATH", "PYTHONPATH", "PATH"]
+    for envvar, value in os.environ.items():
+        if not envvar.lower().startswith(appli.lower()):
+            continue
+
+        for path in path_to_prepend:
+            if envvar.endswith(path):
+                prepend_path(arguments=(virtual_env, appli, path + " " + value.replace(":", " ")))
+                break
+
+        if envvar.endswith("MODULE_USE"):
+            module_use(arguments=(virtual_env, appli, value))
+
+        if envvar.endswith("MODULEFILES"):
+            module_load(arguments=(virtual_env, appli, value))
+
+        if envvar.endswith("SOURCEFILES"):
+            source_sh(arguments=(virtual_env, appli, value))
+
+        if envvar.endswith("EXPORTS"):
+            for var in value.split():
+                setenv(arguments=(virtual_env, appli, var.replace("=", " ")))
+
+        if envvar.endswith("ALIASES"):
+            for var in value.split():
+                set_aliases(arguments=(virtual_env, appli, var.replace("=", " ")))
+
+        if envvar.endswith("REMOVE_PATHS"):
+            for var in value.split():
+                remove_path(arguments=(virtual_env, appli, var.replace("=", " ")))
```

### Comparing `venv-modulefile-0.0.1/src/venvmod/modulefile.py` & `venv-modulefile-0.0.2/src/venvmod/modulefile.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.0.1/src/venv_modulefile.egg-info/entry_points.txt` & `venv-modulefile-0.0.2/src/venv_modulefile.egg-info/entry_points.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [console_scripts]
 venvmod-add-appli = venvmod.commands.create_module:add_appli
 venvmod-cmd-append-path = venvmod.commands.append_module:append_path
 venvmod-cmd-module-load = venvmod.commands.append_module:module_load
 venvmod-cmd-module-use = venvmod.commands.append_module:module_use
 venvmod-cmd-prepend-path = venvmod.commands.append_module:prepend_path
-venvmod-cmd-read_env = venvmod.commands.append_module:read_env
+venvmod-cmd-read-env = venvmod.commands.append_module:read_env
 venvmod-cmd-remove-path = venvmod.commands.append_module:remove_path
 venvmod-cmd-set-aliases = venvmod.commands.append_module:set_aliases
 venvmod-cmd-setenv = venvmod.commands.append_module:setenv
 venvmod-cmd-source-sh = venvmod.commands.append_module:source_sh
 venvmod-initialize = venvmod.commands.create_module:initialize
+venvmod-test-import = venvmod.commands.test_imports:test_imports
```

### Comparing `venv-modulefile-0.0.1/src/venv_modulefile.egg-info/SOURCES.txt` & `venv-modulefile-0.0.2/src/venv_modulefile.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 src/venv_modulefile.egg-info/top_level.txt
 src/venvmod/VERSION
 src/venvmod/__init__.py
 src/venvmod/modulefile.py
 src/venvmod/tools.py
 src/venvmod/commands/__init__.py
 src/venvmod/commands/append_module.py
-src/venvmod/commands/create_module.py
+src/venvmod/commands/create_module.py
+src/venvmod/commands/test_imports.py
```

### Comparing `venv-modulefile-0.0.1/src/venv_modulefile.egg-info/PKG-INFO` & `venv-modulefile-0.0.2/src/venv_modulefile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-modulefile
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python venv extension using Modulefile
 Home-page: https://github.com/roland-lenain/venv-modulefile
 Author: R. Lenain
 Author-email: roland.lenain@cea.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/roland-lenain/venv-modulefile/issues
 Project-URL: Doc, https://icoco-python.readthedocs.io/en/latest/index.html
```

### Comparing `venv-modulefile-0.0.1/LICENSE.md` & `venv-modulefile-0.0.2/LICENSE.md`

 * *Files identical despite different names*


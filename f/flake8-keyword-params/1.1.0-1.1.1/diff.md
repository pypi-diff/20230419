# Comparing `tmp/flake8-keyword-params-1.1.0.tar.gz` & `tmp/flake8-keyword-params-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-keyword-params-1.1.0.tar", last modified: Tue Apr 18 01:43:36 2023, max compression
+gzip compressed data, was "flake8-keyword-params-1.1.1.tar", last modified: Wed Apr 19 20:43:04 2023, max compression
```

## Comparing `flake8-keyword-params-1.1.0.tar` & `flake8-keyword-params-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:43:36.611959 flake8-keyword-params-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.0/.editorconfig
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.0/.gitlab-ci.env
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.0/.gitlab-ci.yaml
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.0/.yamllint.yaml
--rw-r--r--   0 root         (0) root         (0)     3475 2023-04-18 01:43:36.611959 flake8-keyword-params-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2392 2023-04-18 01:40:25.000000 flake8-keyword-params-1.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.0/flake8-keyword-params.sublime-project
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:43:36.607959 flake8-keyword-params-1.1.0/flake8_keyword_params/
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.0/flake8_keyword_params/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7182 2023-04-18 01:40:25.000000 flake8-keyword-params-1.1.0/flake8_keyword_params/checker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:43:36.611959 flake8-keyword-params-1.1.0/flake8_keyword_params.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3475 2023-04-18 01:43:36.000000 flake8-keyword-params-1.1.0/flake8_keyword_params.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-04-18 01:43:36.000000 flake8-keyword-params-1.1.0/flake8_keyword_params.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 01:43:36.000000 flake8-keyword-params-1.1.0/flake8_keyword_params.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-04-18 01:43:36.000000 flake8-keyword-params-1.1.0/flake8_keyword_params.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      465 2023-04-18 01:43:36.000000 flake8-keyword-params-1.1.0/flake8_keyword_params.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-18 01:43:36.000000 flake8-keyword-params-1.1.0/flake8_keyword_params.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2293 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 01:43:36.611959 flake8-keyword-params-1.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:04.403443 flake8-keyword-params-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.1/.editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.1/.gitlab-ci.env
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.1/.gitlab-ci.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      260 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.1/.yamllint.yaml
+-rw-r--r--   0 root         (0) root         (0)     3475 2023-04-19 20:43:04.403443 flake8-keyword-params-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2392 2023-04-18 01:40:25.000000 flake8-keyword-params-1.1.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.1/flake8-keyword-params.sublime-project
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:04.399443 flake8-keyword-params-1.1.1/flake8_keyword_params/
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.1/flake8_keyword_params/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7111 2023-04-19 20:37:26.000000 flake8-keyword-params-1.1.1/flake8_keyword_params/checker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:43:04.403443 flake8-keyword-params-1.1.1/flake8_keyword_params.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3475 2023-04-19 20:43:04.000000 flake8-keyword-params-1.1.1/flake8_keyword_params.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-04-19 20:43:04.000000 flake8-keyword-params-1.1.1/flake8_keyword_params.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 20:43:04.000000 flake8-keyword-params-1.1.1/flake8_keyword_params.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-04-19 20:43:04.000000 flake8-keyword-params-1.1.1/flake8_keyword_params.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      465 2023-04-19 20:43:04.000000 flake8-keyword-params-1.1.1/flake8_keyword_params.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-19 20:43:04.000000 flake8-keyword-params-1.1.1/flake8_keyword_params.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2293 2023-04-16 00:54:26.000000 flake8-keyword-params-1.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 20:43:04.403443 flake8-keyword-params-1.1.1/setup.cfg
```

### Comparing `flake8-keyword-params-1.1.0/PKG-INFO` & `flake8-keyword-params-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-keyword-params
-Version: 1.1.0
+Version: 1.1.1
 Summary: Flake8 keyword parameter validation
 Author-email: Peter Linss <pypi@linss.com>
 License: GNU Lesser General Public License v3
 Project-URL: homepage, https://github.com/plinss/flake8-keyword-params
 Keywords: flake8,noqa
 Classifier: Framework :: Flake8
 Classifier: Environment :: Console
```

### Comparing `flake8-keyword-params-1.1.0/README.md` & `flake8-keyword-params-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `flake8-keyword-params-1.1.0/flake8_keyword_params/checker.py` & `flake8-keyword-params-1.1.1/flake8_keyword_params/checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 		self.generic_visit(function)
 		safe_params: list[re.Pattern] = []
 		for func, params in self.safelist.items():
 			if (func.match(function.name)):
 				safe_params += params
 
 		arguments = function.args
-		defaults = (arguments.defaults[len(arguments.posonlyargs):] if (hasattr(arguments, 'posonlyargs')) else arguments.defaults)
+		defaults = arguments.defaults[-len(arguments.args):]
 		if (defaults):
 			for arg in arguments.args[-len(defaults):]:
 				for safe_param in safe_params:
 					if (safe_param.match(arg.arg)):
 						break
 				else:
 					self.violations.append((arg, Message.NON_KEWORD_OPTIONAL, {'param': arg.arg}))
```

### Comparing `flake8-keyword-params-1.1.0/flake8_keyword_params.egg-info/PKG-INFO` & `flake8-keyword-params-1.1.1/flake8_keyword_params.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-keyword-params
-Version: 1.1.0
+Version: 1.1.1
 Summary: Flake8 keyword parameter validation
 Author-email: Peter Linss <pypi@linss.com>
 License: GNU Lesser General Public License v3
 Project-URL: homepage, https://github.com/plinss/flake8-keyword-params
 Keywords: flake8,noqa
 Classifier: Framework :: Flake8
 Classifier: Environment :: Console
```

### Comparing `flake8-keyword-params-1.1.0/pyproject.toml` & `flake8-keyword-params-1.1.1/pyproject.toml`

 * *Files identical despite different names*


# Comparing `tmp/ssss-0.0.1.tar.gz` & `tmp/ssss-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssss-0.0.1.tar", max compression
+gzip compressed data, was "ssss-1.0.0.tar", max compression
```

## Comparing `ssss-0.0.1.tar` & `ssss-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2023-04-16 16:24:53.028655 ssss-0.0.1/LICENSE
--rw-r--r--   0        0        0      941 2023-04-17 18:36:21.891584 ssss-0.0.1/README.md
--rw-r--r--   0        0        0      707 2023-04-17 18:54:54.959858 ssss-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      395 2023-04-17 18:14:01.315294 ssss-0.0.1/ssss/__init__.py
--rw-r--r--   0        0        0       90 2023-04-16 16:24:53.038655 ssss-0.0.1/ssss/common/__init__.py
--rw-r--r--   0        0        0      119 2023-04-16 16:24:53.038655 ssss-0.0.1/ssss/common/application/__init__.py
--rw-r--r--   0        0        0     1823 2023-04-17 18:55:21.082440 ssss-0.0.1/ssss/common/application/variables.py
--rw-r--r--   0        0        0      187 2023-04-16 16:24:53.038655 ssss-0.0.1/ssss/common/fs/__init__.py
--rw-r--r--   0        0        0      933 2023-04-16 16:24:53.052655 ssss-0.0.1/ssss/common/fs/directory.py
--rw-r--r--   0        0        0     1152 2023-04-16 16:24:53.052655 ssss-0.0.1/ssss/common/fs/file.py
--rw-r--r--   0        0        0       52 2023-04-16 16:24:53.028655 ssss-0.0.1/ssss/common/md/__init__.py
--rw-r--r--   0        0        0      799 2023-04-16 16:24:53.050655 ssss-0.0.1/ssss/common/md/info.py
--rw-r--r--   0        0        0     1418 2023-04-16 16:24:53.052655 ssss-0.0.1/ssss/common/md/render.py
--rw-r--r--   0        0        0       75 2023-04-16 16:24:53.040655 ssss-0.0.1/ssss/configuration/__init__.py
--rw-r--r--   0        0        0     4898 2023-04-17 18:17:16.598103 ssss-0.0.1/ssss/configuration/application.py
--rw-r--r--   0        0        0      470 2023-04-16 16:24:53.048655 ssss-0.0.1/ssss/configuration/arguments.py
--rw-r--r--   0        0        0      381 2023-04-16 16:24:53.038655 ssss-0.0.1/ssss/configuration/default.py
--rw-r--r--   0        0        0       31 2023-04-16 16:24:53.041655 ssss-0.0.1/ssss/generate/__init__.py
--rw-r--r--   0        0        0      371 2023-04-16 16:24:53.044655 ssss-0.0.1/ssss/generate/site.py
--rw-r--r--   0        0        0     1702 1970-01-01 00:00:00.000000 ssss-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-16 16:24:53.028655 ssss-1.0.0/LICENSE
+-rw-r--r--   0        0        0      941 2023-04-19 17:37:33.344836 ssss-1.0.0/README.md
+-rw-r--r--   0        0        0      702 2023-04-19 11:27:02.015562 ssss-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      395 2023-04-19 17:16:03.361405 ssss-1.0.0/ssss/__init__.py
+-rw-r--r--   0        0        0       91 2023-04-19 12:48:25.202327 ssss-1.0.0/ssss/common/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-16 16:24:53.038655 ssss-1.0.0/ssss/common/application/__init__.py
+-rw-r--r--   0        0        0     1868 2023-04-19 16:26:15.888986 ssss-1.0.0/ssss/common/application/variables.py
+-rw-r--r--   0        0        0      187 2023-04-16 16:24:53.038655 ssss-1.0.0/ssss/common/fs/__init__.py
+-rw-r--r--   0        0        0      933 2023-04-19 18:43:37.988627 ssss-1.0.0/ssss/common/fs/directory.py
+-rw-r--r--   0        0        0     1199 2023-04-19 18:43:37.988627 ssss-1.0.0/ssss/common/fs/file.py
+-rw-r--r--   0        0        0       57 2023-04-19 16:39:41.191763 ssss-1.0.0/ssss/common/md/__init__.py
+-rw-r--r--   0        0        0     1147 2023-04-19 16:39:41.105764 ssss-1.0.0/ssss/common/md/context.py
+-rw-r--r--   0        0        0      843 2023-04-19 16:39:41.216762 ssss-1.0.0/ssss/common/md/rule.py
+-rw-r--r--   0        0        0       75 2023-04-16 16:24:53.040655 ssss-1.0.0/ssss/configuration/__init__.py
+-rw-r--r--   0        0        0     5248 2023-04-19 18:43:37.988627 ssss-1.0.0/ssss/configuration/application.py
+-rw-r--r--   0        0        0      470 2023-04-16 16:24:53.048655 ssss-1.0.0/ssss/configuration/arguments.py
+-rw-r--r--   0        0        0      381 2023-04-16 16:24:53.038655 ssss-1.0.0/ssss/configuration/default.py
+-rw-r--r--   0        0        0       31 2023-04-16 16:24:53.041655 ssss-1.0.0/ssss/generate/__init__.py
+-rw-r--r--   0        0        0      545 2023-04-19 17:40:24.681085 ssss-1.0.0/ssss/generate/site.py
+-rw-r--r--   0        0        0     1697 1970-01-01 00:00:00.000000 ssss-1.0.0/PKG-INFO
```

### Comparing `ssss-0.0.1/LICENSE` & `ssss-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssss-0.0.1/README.md` & `ssss-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ssss-0.0.1/pyproject.toml` & `ssss-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "ssss"
-version = "0.0.1"
+version = "1.0.0"
 description = "ssss, short for Super Simple Static Site, is a static site generator that leverages Jinja and Markdown for creating templates and content. It generates static HTML files for an efficient and lightweight website."
 authors = ["Magnus Åberg <himself@magnusaberg.me>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 markdown = "^3.4.3"
-staticjinja = "^4.1.3"
 pyyaml = "^6.0"
 argparse = "^1.4.0"
 importlib-metadata = "^6.3.0"
+jinja2 = "^3.1.2"
 
 [tool.poetry.scripts]
 ssss = "ssss:main"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
```

### Comparing `ssss-0.0.1/ssss/common/application/variables.py` & `ssss-1.0.0/ssss/common/application/variables.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import importlib.metadata
+import os
 
 
 def application_name() -> str:
     return "ssss"
 
 
 def application_description() -> str:
@@ -12,15 +13,15 @@
 
 
 def application_version() -> str:
     return application_name() + " " + importlib.metadata.version(application_name())
 
 
 def application_default_template_path() -> str:
-    return "_templates/"
+    return "_templates"
 
 
 def application_default_template_name() -> str:
     return "default"
 
 
 def application_default_template_extension() -> str:
@@ -32,23 +33,27 @@
 
 
 def application_default_encoding() -> str:
     return "utf8"
 
 
 def application_default_data() -> str:
-    return r".*\.md"
+    return "*.md"
+
+
+def application_default_rule() -> str:
+    return "*" + application_default_template_extension()
 
 
 def application_default_output() -> str:
-    return "site/build"
+    return "site" + os.sep + "build"
 
 
 def application_default_source() -> str:
-    return "site/source"
+    return "site" + os.sep + "source"
 
 
 def application_default_followlinks() -> bool:
     return True
 
 
 def application_default_filters() -> dict:
@@ -62,20 +67,19 @@
         "author": "Site Author",
         "url": "https://example.com",
         "email": "asssa@example.com",
     }
 
 
 def application_default_template_file() -> str:
-    return application_default_template_path() \
-        + application_default_template_name() \
+    return application_default_template_name() \
         + application_default_template_extension()
 
 
 def application_default_base_html() -> str:
-    return application_default_template_path() + "base.html"
+    return "base.html"
 
 
 def application_default_config_data() -> dict:
     return {
         "site": application_default_site(),
     }
```

### Comparing `ssss-0.0.1/ssss/common/fs/directory.py` & `ssss-1.0.0/ssss/common/fs/directory.py`

 * *Files identical despite different names*

### Comparing `ssss-0.0.1/ssss/common/fs/file.py` & `ssss-1.0.0/ssss/common/fs/file.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,10 +34,13 @@
     for directory in directories:
         found = search_config_in_dir(directory)
         if found is not None:
             return found
     return None
 
 
-def touch_if_not_exists(path):
-    if not os.path.exists(path):
+def touch_if_not_exists(path) -> bool:
+    exists = os.path.exists(path)
+    if not exists:
         Path(path).touch()
+
+    return exists
```

### Comparing `ssss-0.0.1/ssss/common/md/info.py` & `ssss-1.0.0/ssss/common/md/context.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 from pathlib import Path
 
 import markdown
 
 
-def variables(template):
-    md = markdown.Markdown(extensions=["meta"])
-    markdown_content = Path(template.filename).read_text()
-    returned_variables = {"content": md.convert(markdown_content)} | md.Meta
+def variables(match_value, search_path):
+    source = Path(search_path)
+    returned_variables = []
+
+    for file in source.iterdir():
+        if file.match(match_value):
+            print("Baking " + str(file) + "...")
+            returned_variables.append(parse(file))
+
+    return returned_variables
 
+
+def parse(context_file):
+    file_path = Path(context_file)
+    md = markdown.Markdown(extensions=["meta"])
+    markdown_content = file_path.read_text()
+    returned_variables = {"content": md.convert(markdown_content), "file_path": file_path} | md.Meta
     for key, value in returned_variables.items():
         if isinstance(value, list) and len(value) == 1:
             returned_variables[key] = value[0]
 
     returned_variables["content"] = handle_meta_variables(returned_variables, returned_variables["content"], md=md)
 
     return returned_variables
```

### Comparing `ssss-0.0.1/ssss/configuration/application.py` & `ssss-1.0.0/ssss/configuration/application.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 from pathlib import Path
 
 import yaml
 
 from ssss.common.application import application_default_config_data
 from ssss.common.application.variables import application_default_template_path, application_default_template_file, \
     application_default_base_html, application_default_source, application_default_output, application_default_data, \
-    application_default_encoding, application_default_followlinks, application_default_filters, application_default_site
+    application_default_encoding, application_default_followlinks, application_default_filters, \
+    application_default_site, application_default_rule
 from ssss.common.fs import find_config
 from ssss.common.fs.directory import get_full_path, create_directory_if_not_exists, have_write_permission
 from ssss.common.fs.file import touch_if_not_exists
-from ssss.common.md import variables, render
+from ssss.common.md import variables, rule
 from ssss.configuration.arguments import Arguments
 from ssss.configuration.default import config_file_path
 
 
 class Application(Arguments):
 
     def __init__(self):
@@ -69,25 +70,29 @@
             site_data = self.data.get("site", {}) | yaml_data.get("site", {})
             site_filters = self.data.get("filters", {}) | yaml_data.get("filters", {})
             self.data = self.data | yaml_data
             self.data["site"] = site_data
             self.data["filters"] = site_filters
 
             self.set_config()
-            self.create_structure()
+
+            if self.__init_config:
+                self.create_structure()
 
         else:
             raise NotImplementedError
 
     def set_config(self):
         self.data = {k: v for k, v in self.data.items() if v}
         self.config["searchpath"] = get_full_path(self.data.get("source", application_default_source()))
         self.config["outpath"] = get_full_path(self.data.get("output", application_default_output()))
+        self.config["templates"] = get_full_path(
+            self.data.get("templates", os.path.join(application_default_source(), application_default_template_path())))
         self.config["contexts"] = [(self.data.get("data", application_default_data()), variables)]
-        self.config["rules"] = [(self.data.get("data", application_default_data()), render.run)]
+        self.config["rules"] = [(self.data.get("data", application_default_rule()), rule.execute)]
         self.config["encoding"] = str(self.data.get("encoding", application_default_encoding()))
         self.config["followlinks"] = str(self.data.get("followlinks", application_default_followlinks()))
         self.config["filters"] = dict(self.data.get("filters", application_default_filters()))
         self.config["env_globals"] = dict(self.data.get("site", application_default_site()))
 
     def init_config(self):
 
@@ -105,36 +110,37 @@
         else:
             raise PermissionError
 
     def __getitem__(self, item):
         return self.config[item]
 
     def create_structure(self):
-        create_directory_if_not_exists(self.config["outpath"])
-        create_directory_if_not_exists(self.config["searchpath"])
-
-        create_directory_if_not_exists(
-            os.path.join(
-                self.config["searchpath"],
-                application_default_template_path()
-            )
+        base_html = os.path.join(
+            self.config["searchpath"],
+            application_default_template_path(),
+            application_default_base_html()
         )
 
-        touch_if_not_exists(
-            os.path.join(self.config["searchpath"],
-                         application_default_base_html()
-                         )
+        default_template = os.path.join(
+            self.config["searchpath"],
+            application_default_template_path(),
+            application_default_template_file()
         )
-        touch_if_not_exists(
+
+        index_md = os.path.join(
             os.path.join(
                 self.config["searchpath"],
-                application_default_template_file()
+                "index.md"
             )
         )
-        touch_if_not_exists(
-            os.path.join(
-                os.path.join(
-                    self.config["searchpath"],
-                    "index.md"
-                )
-            )
+
+        default_template_path = os.path.join(
+            self.config["searchpath"],
+            application_default_template_path()
         )
+
+        create_directory_if_not_exists(self.config["outpath"])
+        create_directory_if_not_exists(self.config["searchpath"])
+        create_directory_if_not_exists(default_template_path)
+        touch_if_not_exists(default_template)
+        touch_if_not_exists(index_md)
+        touch_if_not_exists(base_html)
```

### Comparing `ssss-0.0.1/PKG-INFO` & `ssss-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ssss
-Version: 0.0.1
+Version: 1.0.0
 Summary: ssss, short for Super Simple Static Site, is a static site generator that leverages Jinja and Markdown for creating templates and content. It generates static HTML files for an efficient and lightweight website.
 Author: Magnus Åberg
 Author-email: himself@magnusaberg.me
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: importlib-metadata (>=6.3.0,<7.0.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: markdown (>=3.4.3,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: staticjinja (>=4.1.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Super Simple Static Site (ssss)
 
 ssss, short for Super Simple Static Site, is a static site generator that leverages Jinja and Markdown for creating
 templates and content. It generates static HTML files for an efficient and lightweight website.
```


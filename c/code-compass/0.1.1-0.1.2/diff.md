# Comparing `tmp/code_compass-0.1.1.tar.gz` & `tmp/code_compass-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_compass-0.1.1.tar", max compression
+gzip compressed data, was "code_compass-0.1.2.tar", max compression
```

## Comparing `code_compass-0.1.1.tar` & `code_compass-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1329 2023-04-19 16:18:39.945858 code_compass-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-19 16:18:39.945858 code_compass-0.1.1/code_compass/__init__.py
--rw-r--r--   0        0        0    17183 2023-04-19 17:13:37.462247 code_compass-0.1.1/code_compass/app.py
--rw-r--r--   0        0        0     3468 2023-04-19 16:18:39.945858 code_compass-0.1.1/code_compass/category.py
--rw-r--r--   0        0        0      777 2023-04-19 16:18:39.945858 code_compass-0.1.1/code_compass/config.py
--rw-r--r--   0        0        0      108 2023-04-19 16:18:39.945858 code_compass-0.1.1/code_compass/config.yaml
--rw-r--r--   0        0        0     1042 2023-04-19 16:18:39.945858 code_compass-0.1.1/code_compass/db.py
--rw-r--r--   0        0        0     3769 2023-04-19 16:18:39.945858 code_compass-0.1.1/code_compass/project.py
--rw-r--r--   0        0        0    12288 2023-01-14 18:54:55.231408 code_compass-0.1.1/code_compass/~/.config/charm_runner/data.db
--rw-r--r--   0        0        0      600 2023-04-19 17:13:20.726385 code_compass-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 code_compass-0.1.1/setup.py
--rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 code_compass-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1329 2023-04-19 16:18:39.945858 code_compass-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 16:18:39.945858 code_compass-0.1.2/code_compass/__init__.py
+-rw-r--r--   0        0        0    17165 2023-04-19 17:26:18.021077 code_compass-0.1.2/code_compass/app.py
+-rw-r--r--   0        0        0     3468 2023-04-19 16:18:39.945858 code_compass-0.1.2/code_compass/category.py
+-rw-r--r--   0        0        0      777 2023-04-19 16:18:39.945858 code_compass-0.1.2/code_compass/config.py
+-rw-r--r--   0        0        0      108 2023-04-19 16:18:39.945858 code_compass-0.1.2/code_compass/config.yaml
+-rw-r--r--   0        0        0     1042 2023-04-19 16:18:39.945858 code_compass-0.1.2/code_compass/db.py
+-rw-r--r--   0        0        0     3769 2023-04-19 16:18:39.945858 code_compass-0.1.2/code_compass/project.py
+-rw-r--r--   0        0        0    12288 2023-01-14 18:54:55.231408 code_compass-0.1.2/code_compass/~/.config/charm_runner/data.db
+-rw-r--r--   0        0        0      600 2023-04-19 17:26:25.825031 code_compass-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 code_compass-0.1.2/setup.py
+-rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 code_compass-0.1.2/PKG-INFO
```

### Comparing `code_compass-0.1.1/README.md` & `code_compass-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `code_compass-0.1.1/code_compass/app.py` & `code_compass-0.1.2/code_compass/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self.db = DB()
         Category.create_default_if_db_is_empty(self.db)
 
         # Set the table headers
         self.table_headers = ["Name", "Path", "Days Since Last Access"]
 
         # Initialize the main window
-        self.setWindowTitle(f"Code Compass {self.font_size}")
+        self.setWindowTitle("Code Compass")
         self.setLayout(QHBoxLayout())
 
         # Render sections
         self.render_left_section()
         self.render_right_section()
 
         # add on close event
```

### Comparing `code_compass-0.1.1/code_compass/category.py` & `code_compass-0.1.2/code_compass/category.py`

 * *Files identical despite different names*

### Comparing `code_compass-0.1.1/code_compass/config.py` & `code_compass-0.1.2/code_compass/config.py`

 * *Files identical despite different names*

### Comparing `code_compass-0.1.1/code_compass/db.py` & `code_compass-0.1.2/code_compass/db.py`

 * *Files identical despite different names*

### Comparing `code_compass-0.1.1/code_compass/project.py` & `code_compass-0.1.2/code_compass/project.py`

 * *Files identical despite different names*

### Comparing `code_compass-0.1.1/code_compass/~/.config/charm_runner/data.db` & `code_compass-0.1.2/code_compass/~/.config/charm_runner/data.db`

 * *Files identical despite different names*

### Comparing `code_compass-0.1.1/pyproject.toml` & `code_compass-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "code-compass"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Roman <roman-right@protonmail.com>"]
 readme = "README.md"
 packages = [{ include = "code_compass" }]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `code_compass-0.1.1/setup.py` & `code_compass-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['cookiecutter>=2.1.1,<3.0.0', 'pyside6>=6.5.0,<7.0.0']
 
 entry_points = \
 {'console_scripts': ['code-compass = code_compass.app:run']}
 
 setup_kwargs = {
     'name': 'code-compass',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': '# Code Compass\n\n![Screenshot](assets/screenshot-1.png)\n\nA simple and intuitive desktop application to manage your coding projects, built with Python and Qt (using PySide6).\n\n## Features\n\n* Organize projects into categories.\n* Quickly access project information, such as project name, path, and last opened date.\n* Easily add, create, delete, and run projects with built-in buttons.\n* Customize your project\'s attributes like name, path, and category.\n* Choose between different IDEs, such as PyCharm and Visual Studio Code.\n* Tab-based navigation for easy access to different project categories.\n\n## Installation\n\n```shell\npip install code-compass\n```\n\n## Usage\n\n```shell\ncode-compass\n```\n\n## Configuration\n\nCode Compass uses a configuration file to store your preferences. The configuration file is located at `~/.config/code_compass/config.yaml`.\n\n### Example\n\n```yaml\n\n# IDE commands to run when clicking the "Run" button.\nide_commands:\n  - pycharm\n  - code\n\n# Default path to start browsing when adding or creating a new project.\nprojects_path: /home/username/Projects\n\n# Cookiecutter template to use when creating a new project.\ncookiecutter: https://github.com/roman-right/py-template\n\n```\n\n## Contributing\n\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n',
     'author': 'Roman',
     'author_email': 'roman-right@protonmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `code_compass-0.1.1/PKG-INFO` & `code_compass-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-compass
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Roman
 Author-email: roman-right@protonmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


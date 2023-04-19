# Comparing `tmp/code_compass-0.1.0.tar.gz` & `tmp/code_compass-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_compass-0.1.0.tar", max compression
+gzip compressed data, was "code_compass-0.1.1.tar", max compression
```

## Comparing `code_compass-0.1.0.tar` & `code_compass-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      625 2023-04-19 15:37:15.725224 code_compass-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-01-12 11:27:19.048059 code_compass-0.1.0/code_compass/__init__.py
--rw-r--r--   0        0        0    16569 2023-04-19 15:52:10.904061 code_compass-0.1.0/code_compass/app.py
--rw-r--r--   0        0        0     3468 2023-04-19 15:36:12.613618 code_compass-0.1.0/code_compass/category.py
--rw-r--r--   0        0        0      520 2023-04-19 15:49:52.660828 code_compass-0.1.0/code_compass/config.py
--rw-r--r--   0        0        0     1042 2023-04-19 15:36:12.625618 code_compass-0.1.0/code_compass/db.py
--rw-r--r--   0        0        0     3769 2023-04-19 15:36:12.617618 code_compass-0.1.0/code_compass/project.py
--rw-r--r--   0        0        0    12288 2023-01-14 18:54:55.231408 code_compass-0.1.0/code_compass/~/.config/charm_runner/data.db
--rw-r--r--   0        0        0      600 2023-04-19 15:45:48.646199 code_compass-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1433 1970-01-01 00:00:00.000000 code_compass-0.1.0/setup.py
--rw-r--r--   0        0        0     1053 1970-01-01 00:00:00.000000 code_compass-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1329 2023-04-19 16:18:39.945858 code_compass-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 16:18:39.945858 code_compass-0.1.1/code_compass/__init__.py
+-rw-r--r--   0        0        0    17183 2023-04-19 17:13:37.462247 code_compass-0.1.1/code_compass/app.py
+-rw-r--r--   0        0        0     3468 2023-04-19 16:18:39.945858 code_compass-0.1.1/code_compass/category.py
+-rw-r--r--   0        0        0      777 2023-04-19 16:18:39.945858 code_compass-0.1.1/code_compass/config.py
+-rw-r--r--   0        0        0      108 2023-04-19 16:18:39.945858 code_compass-0.1.1/code_compass/config.yaml
+-rw-r--r--   0        0        0     1042 2023-04-19 16:18:39.945858 code_compass-0.1.1/code_compass/db.py
+-rw-r--r--   0        0        0     3769 2023-04-19 16:18:39.945858 code_compass-0.1.1/code_compass/project.py
+-rw-r--r--   0        0        0    12288 2023-01-14 18:54:55.231408 code_compass-0.1.1/code_compass/~/.config/charm_runner/data.db
+-rw-r--r--   0        0        0      600 2023-04-19 17:13:20.726385 code_compass-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 code_compass-0.1.1/setup.py
+-rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 code_compass-0.1.1/PKG-INFO
```

### Comparing `code_compass-0.1.0/code_compass/app.py` & `code_compass-0.1.1/code_compass/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 import venv
 from datetime import datetime
 from pathlib import Path
 
 from PySide6 import QtWidgets
 from PySide6.QtCore import Qt
+from PySide6.QtGui import QCursor, QGuiApplication
 from PySide6.QtWidgets import (
     QApplication,
     QDialog,
     QVBoxLayout,
     QTabWidget,
     QTableWidget,
     QTableWidgetItem,
@@ -32,28 +33,42 @@
 from code_compass.project import Project
 
 
 class ProjectManager(QDialog):
     def __init__(self):
         super().__init__()
 
+        # Calculate the width based on the current screen resolution
+        cursor_position = QCursor.pos()
+        current_screen = QGuiApplication.screenAt(cursor_position)
+        self.screen_resolution = current_screen.size()
+
+        self.font_size = (
+            self.screen_resolution.width() + self.screen_resolution.height()
+        ) // 250
+
+        # Initialize the database
         self.db = DB()
         Category.create_default_if_db_is_empty(self.db)
 
+        # Set the table headers
         self.table_headers = ["Name", "Path", "Days Since Last Access"]
 
-        self.setWindowTitle("Code Compass")
+        # Initialize the main window
+        self.setWindowTitle(f"Code Compass {self.font_size}")
         self.setLayout(QHBoxLayout())
 
+        # Render sections
         self.render_left_section()
         self.render_right_section()
 
         # add on close event
         self.finished.connect(self.on_close)
 
+        # Render the data
         self.rerender_table()
 
     # HELPERS
 
     def add_button(self, label, callback=None, parent_layout=None):
         button = QPushButton(label)
         if callback:
@@ -91,15 +106,18 @@
         self.categories = Category.all(self.db)
 
     # RENDERS
 
     def render_left_section(self):
         # Left section - Tabs for project categories
         wrapper = QWidget()
-        wrapper.setFixedWidth(1200)
+
+        wrapper_width = self.screen_resolution.width() // 3
+        wrapper.setFixedWidth(wrapper_width)
+
         self.left_layout = QVBoxLayout()
         self.tabs = QTabWidget()
         self.tabs.currentChanged.connect(self.rerender_table)
         self.left_layout.addWidget(self.tabs)
         wrapper.setLayout(self.left_layout)
         self.layout().addWidget(wrapper)
 
@@ -276,16 +294,15 @@
         add_dialog.layout().addWidget(category_combo)
 
         add_button = QPushButton("Add")
 
         def add_project():
             category = Category(id=None, name=category_combo.currentText())
             project_name = (
-                project_name_edit.text()
-                or Path(project_path_edit.text()).name
+                project_name_edit.text() or Path(project_path_edit.text()).name
             )
             project = Project(
                 name=project_name,
                 path=project_path_edit.text(),
                 last_opened=datetime.now(),
                 category=category,
             )
@@ -342,18 +359,15 @@
         create_dialog.layout().addWidget(category_label)
         create_dialog.layout().addWidget(category_combo)
 
         create_button = QPushButton("Create")
 
         def create_project():
             path = Path(project_path_edit.text())
-            project_name = (
-                project_name_edit.text()
-                or path.name
-            )
+            project_name = project_name_edit.text() or path.name
             cookiecutter(
                 COOKIECUTTER,
                 no_input=True,
                 output_dir=str(project_path_edit.text()),
                 extra_context={"project_name": project_name},
                 overwrite_if_exists=True,
             )
@@ -505,22 +519,23 @@
         for project in projects:
             project.delete(self.db)
         self.rerender_table()
 
 
 def run():
     app = QApplication(sys.argv)
+    project_manager = ProjectManager()
     app.setStyleSheet(
-        """
-        QWidget {
+        f"""
+        QWidget {{
             font-family: "Roboto";
-            font-size: 24px;
-        }
+            font-size: {project_manager.font_size}px;
+        }}
         """
     )
-    project_manager = ProjectManager()
+
     project_manager.show()
     sys.exit(app.exec())
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `code_compass-0.1.0/code_compass/category.py` & `code_compass-0.1.1/code_compass/category.py`

 * *Files identical despite different names*

### Comparing `code_compass-0.1.0/code_compass/config.py` & `code_compass-0.1.1/code_compass/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,29 @@
+import shutil
 from pathlib import Path
 
 import yaml
 
 BASE_DIR = Path.home() / ".config" / "code_compass"
 DB_PATH = BASE_DIR / "data.db"
 CONFIG_PATH = BASE_DIR / "config.yaml"
+TEMPLATE_CONFIG_PATH = Path(__file__).parent / "config.yaml"
+
 
 config_src = {}
-if CONFIG_PATH.is_file():
-    with CONFIG_PATH.open() as f:
-        config_src = yaml.safe_load(f.read())
-
-IDE_COMMANDS = config_src.get("IDE_COMMANDS", ["pycharm"])
-PROJECTS_PATH = str(
-    Path(config_src.get("PROJECTS_PATH", Path.home()))
-)
-COOKIECUTTER = config_src.get(
-    "COOKIECUTTER", "https://github.com/roman-right/py-template"
-)
+if not CONFIG_PATH.is_file():
+    BASE_DIR.mkdir(parents=True, exist_ok=True)
+    shutil.copyfile(TEMPLATE_CONFIG_PATH, CONFIG_PATH)
+
+with CONFIG_PATH.open() as f:
+    config_src = yaml.safe_load(f.read())
+
+IDE_COMMANDS = config_src.get("ide_commands", ["pycharm"])
+
+projects_path = config_src.get("projects_path", Path.home())
+if projects_path in ["~", "HOME"]:
+    projects_path = Path.home()
+else:
+    projects_path = Path(projects_path)
+
+PROJECTS_PATH = str(projects_path)
+COOKIECUTTER = config_src.get("cookiecutter")
```

### Comparing `code_compass-0.1.0/code_compass/db.py` & `code_compass-0.1.1/code_compass/db.py`

 * *Files identical despite different names*

### Comparing `code_compass-0.1.0/code_compass/project.py` & `code_compass-0.1.1/code_compass/project.py`

 * *Files identical despite different names*

### Comparing `code_compass-0.1.0/code_compass/~/.config/charm_runner/data.db` & `code_compass-0.1.1/code_compass/~/.config/charm_runner/data.db`

 * *Files identical despite different names*

### Comparing `code_compass-0.1.0/pyproject.toml` & `code_compass-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "code-compass"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Roman <roman-right@protonmail.com>"]
 readme = "README.md"
 packages = [{ include = "code_compass" }]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```


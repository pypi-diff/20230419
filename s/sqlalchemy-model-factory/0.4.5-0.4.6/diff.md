# Comparing `tmp/sqlalchemy-model-factory-0.4.5.tar.gz` & `tmp/sqlalchemy-model-factory-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-model-factory-0.4.5.tar", max compression
+gzip compressed data, was "sqlalchemy-model-factory-0.4.6.tar", max compression
```

## Comparing `sqlalchemy-model-factory-0.4.5.tar` & `sqlalchemy-model-factory-0.4.6.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      717 2022-12-21 02:12:08.355737 sqlalchemy-model-factory-0.4.5/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2022-12-21 02:12:08.355737 sqlalchemy-model-factory-0.4.5/LICENSE
--rw-r--r--   0        0        0     3381 2022-12-21 02:12:08.355737 sqlalchemy-model-factory-0.4.5/README.md
--rw-r--r--   0        0        0     1200 2022-12-21 02:12:08.355737 sqlalchemy-model-factory-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      447 2022-12-21 02:12:08.355737 sqlalchemy-model-factory-0.4.5/src/sqlalchemy_model_factory/__init__.py
--rw-r--r--   0        0        0     7703 2022-12-21 02:12:08.355737 sqlalchemy-model-factory-0.4.5/src/sqlalchemy_model_factory/base.py
--rw-r--r--   0        0        0     5448 2022-12-21 02:12:08.355737 sqlalchemy-model-factory-0.4.5/src/sqlalchemy_model_factory/declarative.py
--rw-r--r--   0        0        0     2019 2022-12-21 02:12:08.355737 sqlalchemy-model-factory-0.4.5/src/sqlalchemy_model_factory/pytest.py
--rw-r--r--   0        0        0     1817 2022-12-21 02:12:08.355737 sqlalchemy-model-factory-0.4.5/src/sqlalchemy_model_factory/registry.py
--rw-r--r--   0        0        0     6275 2022-12-21 02:12:08.355737 sqlalchemy-model-factory-0.4.5/src/sqlalchemy_model_factory/utils.py
--rw-r--r--   0        0        0     4496 1970-01-01 00:00:00.000000 sqlalchemy-model-factory-0.4.5/setup.py
--rw-r--r--   0        0        0     4304 1970-01-01 00:00:00.000000 sqlalchemy-model-factory-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      717 2023-04-19 14:26:22.431859 sqlalchemy-model-factory-0.4.6/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-04-19 14:26:22.431859 sqlalchemy-model-factory-0.4.6/LICENSE
+-rw-r--r--   0        0        0     3381 2023-04-19 14:26:22.435859 sqlalchemy-model-factory-0.4.6/README.md
+-rw-r--r--   0        0        0     1216 2023-04-19 14:26:22.435859 sqlalchemy-model-factory-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      451 2023-04-19 14:26:22.435859 sqlalchemy-model-factory-0.4.6/src/sqlalchemy_model_factory/__init__.py
+-rw-r--r--   0        0        0     7703 2023-04-19 14:26:22.435859 sqlalchemy-model-factory-0.4.6/src/sqlalchemy_model_factory/base.py
+-rw-r--r--   0        0        0     5448 2023-04-19 14:26:22.435859 sqlalchemy-model-factory-0.4.6/src/sqlalchemy_model_factory/declarative.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:26:22.435859 sqlalchemy-model-factory-0.4.6/src/sqlalchemy_model_factory/py.typed
+-rw-r--r--   0        0        0     2019 2023-04-19 14:26:22.435859 sqlalchemy-model-factory-0.4.6/src/sqlalchemy_model_factory/pytest.py
+-rw-r--r--   0        0        0     1817 2023-04-19 14:26:22.435859 sqlalchemy-model-factory-0.4.6/src/sqlalchemy_model_factory/registry.py
+-rw-r--r--   0        0        0     6275 2023-04-19 14:26:22.435859 sqlalchemy-model-factory-0.4.6/src/sqlalchemy_model_factory/utils.py
+-rw-r--r--   0        0        0     4496 1970-01-01 00:00:00.000000 sqlalchemy-model-factory-0.4.6/setup.py
+-rw-r--r--   0        0        0     4304 1970-01-01 00:00:00.000000 sqlalchemy-model-factory-0.4.6/PKG-INFO
```

### Comparing `sqlalchemy-model-factory-0.4.5/CHANGELOG.md` & `sqlalchemy-model-factory-0.4.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy-model-factory-0.4.5/LICENSE` & `sqlalchemy-model-factory-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-model-factory-0.4.5/README.md` & `sqlalchemy-model-factory-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy-model-factory-0.4.5/pyproject.toml` & `sqlalchemy-model-factory-0.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "sqlalchemy-model-factory"
-version = "0.4.5"
+version = "0.4.6"
 description = "A library to assist in generating models from a central location."
 authors = ["Dan Cardin <ddcardin@gmail.com>"]
 license = "Apache-2.0"
 keywords = [ "sqlalchemy", "model", "factory", "pytest" ]
 repository = "https://github.com/dancardin/sqlalchemy-model-factory"
 packages = [
     { include = "sqlalchemy_model_factory", from = "src" },
 ]
 readme = 'README.md'
 include = [
     "*.md",
+    "py.typed",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.6.2,<4"
 
 sqlalchemy = "*"
 typing_extensions = ">=3.10"
```

### Comparing `sqlalchemy-model-factory-0.4.5/src/sqlalchemy_model_factory/base.py` & `sqlalchemy-model-factory-0.4.6/src/sqlalchemy_model_factory/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-model-factory-0.4.5/src/sqlalchemy_model_factory/declarative.py` & `sqlalchemy-model-factory-0.4.6/src/sqlalchemy_model_factory/declarative.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-model-factory-0.4.5/src/sqlalchemy_model_factory/pytest.py` & `sqlalchemy-model-factory-0.4.6/src/sqlalchemy_model_factory/pytest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-model-factory-0.4.5/src/sqlalchemy_model_factory/registry.py` & `sqlalchemy-model-factory-0.4.6/src/sqlalchemy_model_factory/registry.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-model-factory-0.4.5/src/sqlalchemy_model_factory/utils.py` & `sqlalchemy-model-factory-0.4.6/src/sqlalchemy_model_factory/utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-model-factory-0.4.5/setup.py` & `sqlalchemy-model-factory-0.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 {'pytest': ['pytest>=1.0']}
 
 entry_points = \
 {'pytest11': ['model_manager = sqlalchemy_model_factory.pytest']}
 
 setup_kwargs = {
     'name': 'sqlalchemy-model-factory',
-    'version': '0.4.5',
+    'version': '0.4.6',
     'description': 'A library to assist in generating models from a central location.',
     'long_description': '[![Actions Status](https://github.com/dancardin/sqlalchemy-model-factory/workflows/build/badge.svg)](https://github.com/dancardin/sqlalchemy-model-factory/actions) [![codecov](https://codecov.io/gh/DanCardin/sqlalchemy-model-factory/branch/main/graph/badge.svg)](https://codecov.io/gh/DanCardin/sqlalchemy-model-factory) [![Documentation Status](https://readthedocs.org/projects/sqlalchemy-model-factory/badge/?version=latest)](https://sqlalchemy-model-factory.readthedocs.io/en/latest/?badge=latest)\n\nsqlalchemy-model-factory aims to make it easy to write factory functions for sqlalchemy\nmodels, particularly for use in testing.\n\nIt should make it easy to define as many factories as you might want, with as little\nboilerplate as possible, while remaining as unopinionated as possible about the behavior\ngoing in your factories.\n\n## Installation\n\n```python\npip install sqlalchemy-model-factory\n```\n\n## Usage\n\nSuppose you\'ve defined a `Widget` model, and for example you want to test some API code\nthat queries for `Widget` instances. Couple of factory functions might look like so:\n\n```python\n# tests/test_example_which_uses_pytest\nfrom sqlalchemy_model_factory import autoincrement, register_at\nfrom . import models\n\n@register_at(\'widget\')\ndef new_widget(name, weight, color, size, **etc):\n    """My goal is to allow you to specify *all* the options a widget might require.\n    """\n    return Widget(name, weight, color, size, **etc)\n\n@register_at(\'widget\', name=\'default\')\n@autoincrement\ndef new_default_widget(autoincrement=1):\n    """My goal is to give you a widget with as little input as possible.\n    """\n    # I\'m gonna call the other factory function...because i can!\n    return new_widget(\n        f\'default_name{autoincrement}\',\n        weight=autoincrement,\n        color=\'rgb({0}, {0}, {0})\'.format(autoincrement),\n        size=autoincrement,\n    )\n```\n\nWhat this does, is register those functions to the registry of factory functions, within\nthe "widget" namespace, at the `name` (defaults to `new`) location in the namespace.\n\nSo when I go to write a test, all I need to do is accept the `mf` fixture (and lets say\na `session` db connection fixture to make assertions against) and I can call all the\nfactories that have been registered.\n\n```python\ndef test_example_model(mf, session):\n    widget1 = mf.widget.new(\'name\', 1, \'rgb(0, 0, 0)\', 1)\n    widget2 = mf.widget.default()\n    widget3 = mf.widget.default()\n    widget4 = mf.widget.default()\n\n    widgets = session.query(Widget).all()\n    assert len(widgets) == 4\n    assert widgets[0].name == \'name\'\n    assert widgets[1].id == widget2.id\n    assert widgets[2].name == widget3.name\n    assert widgets[3].color == \'rgb(3, 3, 3)\'\n```\n\nIn a simple toy example, where you don\'t gain much on the calls themselves the benefits\nare primarily:\n\n- The instances are automatically put into the database and cleaned up after the test.\n- You can make assertions without hardcoding the values, because you get back a handle on the object.\n\nBut as the graph of models required to set up a particular scenario grows:\n\n- You can define factories as complex as you want\n  - They can create related objects and assign them to relationships\n  - They can be given sources of randomness or uniqueness to not violate constraints\n  - They can compose with eachother (when called normally, they\'re the same as the original function).\n',
     'author': 'Dan Cardin',
     'author_email': 'ddcardin@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dancardin/sqlalchemy-model-factory',
```

### Comparing `sqlalchemy-model-factory-0.4.5/PKG-INFO` & `sqlalchemy-model-factory-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-model-factory
-Version: 0.4.5
+Version: 0.4.6
 Summary: A library to assist in generating models from a central location.
 Home-page: https://github.com/dancardin/sqlalchemy-model-factory
 License: Apache-2.0
 Keywords: sqlalchemy,model,factory,pytest
 Author: Dan Cardin
 Author-email: ddcardin@gmail.com
 Requires-Python: >=3.6.2,<4
```


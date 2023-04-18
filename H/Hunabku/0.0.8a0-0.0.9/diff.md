# Comparing `tmp/Hunabku-0.0.8a0.tar.gz` & `tmp/Hunabku-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hunabku-0.0.8a0.tar", last modified: Wed Feb  8 21:09:04 2023, max compression
+gzip compressed data, was "Hunabku-0.0.9.tar", last modified: Thu Mar  9 03:38:13 2023, max compression
```

## Comparing `Hunabku-0.0.8a0.tar` & `Hunabku-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:09:04.086246 Hunabku-0.0.8a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:09:04.082246 Hunabku-0.0.8a0/Hunabku.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-02-08 21:09:03.000000 Hunabku-0.0.8a0/Hunabku.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-08 21:09:04.000000 Hunabku-0.0.8a0/Hunabku.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 21:09:03.000000 Hunabku-0.0.8a0/Hunabku.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-08 21:09:03.000000 Hunabku-0.0.8a0/Hunabku.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-08 21:09:03.000000 Hunabku-0.0.8a0/Hunabku.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-02-08 21:09:04.086246 Hunabku-0.0.8a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:09:04.086246 Hunabku-0.0.8a0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/bin/hunabku_loader
--rwxr-xr-x   0 runner    (1001) docker     (123)     1121 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/bin/hunabku_server
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:09:04.086246 Hunabku-0.0.8a0/hunabku/
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/Hunabku.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/HunabkuBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/HunabkuLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:09:04.086246 Hunabku-0.0.8a0/hunabku/config/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/config/apidoc-header.md
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/config/apidoc.json
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/config/errors.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:09:04.086246 Hunabku-0.0.8a0/hunabku/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/plugins/ApiDoc.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/plugins/Hello.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/plugins/MoaiGSCites.py
--rw-r--r--   0 runner    (1001) docker     (123)    10450 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/plugins/MoaiGSLookUp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/plugins/MoaiGSProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/plugins/MoaiGSQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/plugins/MoaiGSStage.py
--rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/plugins/Scienti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:09:04.086246 Hunabku-0.0.8a0/hunabku/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/hunabku/templates/apidoc.html
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 21:09:04.086246 Hunabku-0.0.8a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-02-08 21:08:43.000000 Hunabku-0.0.8a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:38:13.711538 Hunabku-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:38:13.711538 Hunabku-0.0.9/Hunabku.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-09 03:38:13.000000 Hunabku-0.0.9/Hunabku.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-09 03:38:13.000000 Hunabku-0.0.9/Hunabku.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 03:38:13.000000 Hunabku-0.0.9/Hunabku.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-09 03:38:13.000000 Hunabku-0.0.9/Hunabku.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-09 03:38:13.000000 Hunabku-0.0.9/Hunabku.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-03-09 03:38:04.000000 Hunabku-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-09 03:38:04.000000 Hunabku-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-09 03:38:13.711538 Hunabku-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-03-09 03:38:04.000000 Hunabku-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:38:13.711538 Hunabku-0.0.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2103 2023-03-09 03:38:04.000000 Hunabku-0.0.9/bin/hunabku_server
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:38:13.711538 Hunabku-0.0.9/hunabku/
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10606 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/Hunabku.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/HunabkuBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/PluginGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:38:13.711538 Hunabku-0.0.9/hunabku/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/config/apidoc-header.md
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/config/apidoc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/config/errors.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:38:13.711538 Hunabku-0.0.9/hunabku/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/templates/apidoc.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:38:13.707538 Hunabku-0.0.9/hunabku/templates/plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:38:13.711538 Hunabku-0.0.9/hunabku/templates/plugin/HunabKu_template/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/templates/plugin/HunabKu_template/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/templates/plugin/HunabKu_template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:38:13.711538 Hunabku-0.0.9/hunabku/templates/plugin/HunabKu_template/hunabku_template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/templates/plugin/HunabKu_template/hunabku_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/templates/plugin/HunabKu_template/hunabku_template/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:38:13.711538 Hunabku-0.0.9/hunabku/templates/plugin/HunabKu_template/hunabku_template/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/templates/plugin/HunabKu_template/hunabku_template/endpoints/Hello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-03-09 03:38:04.000000 Hunabku-0.0.9/hunabku/templates/plugin/HunabKu_template/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 03:38:13.711538 Hunabku-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-03-09 03:38:04.000000 Hunabku-0.0.9/setup.py
```

### Comparing `Hunabku-0.0.8a0/Hunabku.egg-info/PKG-INFO` & `Hunabku-0.0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,29 @@
-Metadata-Version: 2.1
-Name: Hunabku
-Version: 0.0.8a0
-Summary: Papers database endpoint API
-Home-page: https://github.com/colav/Hunabku
-Author: Colav
-Author-email: colav@udea.edu.co
-License: BSD
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <center><img src="https://raw.githubusercontent.com/colav/colav.github.io/master/img/Logo.png"/></center>
 
 # HunabKu  
-Data Server Gateway/  Maya - father of all gods
+Modular APIs creation using plugins system/  Maya - father of all gods
 
 # Description
-Package to load data in MongoDB and to serve the data from mongodb on endpoints using flask. 
+Package to create APIs endpoints using flask behind.
 The package is handling the endpoints  using a customized plugin system designed by us.
 
+# Plugin
+Take a look on plugins examples in the repository
+https://github.com/colav/HunabKu_plugins 
 
 # Installation
 
 ## Dependencies
 * Install nodejs >=10.x.x ex: 10.13.0
     * Debian based system: `apt-get install nodejs`
     * Redhat based system: `yum install nodejs`
     * Conda: `conda install nodejs==10.13.0`
-* Install Apidocjs `npm install -g apidoc@0.29.0` as root!
+* Install Apidocjs `npm install -g apidoc` as root!
 * The other dependecies can be installed with pip installing this package.
-* Install MongoDB
-    * Debian based system: `apt-get install mongodb`
-    * Redhat based system instructions [here](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-red-hat/)
-    * Conda: `conda install mongodb mongo-tools`
 
 NOTE:
 
 To start mongodb server on conda please run the next steps
 
 `
 mkdir -p $HOME/data/db 
@@ -45,24 +33,25 @@
 mongodb mongod --dbpath $HOME/data/db/
 `
 
 ## Package
 `pip install hunabku`
 
 # Usage
-Let's start the server executing
+
+Let's start creating a config file
 ```.sh
-hunabku_server
+hunabku_server --generate_config config.py --overwrite
 ```
-Or using some command line options
+
+Let's start the server executing
 ```.sh
-hunabku_server --port 8080 --db_ip x.x.x.x
+hunabku_server --config config.py
 ```
 
-where x.x.x.x is your mongodb ip
 
 you can access to the apidoc documentation for the endpoints for example on: http://127.0.1.1:8888/apidoc/index.html
 
 if depends of the ip and port that you are providing to hunabku.
 
 
 # License
```

### Comparing `Hunabku-0.0.8a0/LICENSE` & `Hunabku-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Hunabku-0.0.8a0/hunabku/Hunabku.py` & `Hunabku-0.0.9/hunabku/Hunabku.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,78 @@
 from flask import (
     Flask
 )
 
-from pymongo import MongoClient
-
 import logging
 
 import os
+from hunabku.HunabkuBase import HunabkuPluginBase
+from hunabku.Config import ConfigGenerator, Config
 from hunabku._version import get_version
 from shutil import rmtree
 from distutils.dir_util import copy_tree
 import subprocess
+import inspect
 import glob
 import time
 import pathlib
 import sys
 import importlib
 import json
 
+import pkgutil
+
 
 class Hunabku:
     """
-    Class to serve papers information store in a mongodb database throught an API using flask.
+    Class to serve papers information store in a mongodb database through an API using flask.
 
     example:
     http://0.0.0.0:5000/data/redalyc?init=1&end&apikey=pl0ok9ij8uh7yg
     """
-
-    def __init__(
-            self,
-            apikey,
-            dburi='mongodb://localhost:27017/',
-            ip='127.0.0.1',
-            port=8080,
-            log_file='hunabku.log',
-            info_level=logging.DEBUG):
+    config = ConfigGenerator.config
+    
+    def __init__(self, config:Config):
         """
         Contructor to initialize configuration options.
 
         Args:
             apikey: apikey to access the data
             ip (str): ip to start the server
             port (int): port for the server
             info_level (logging.DEBUG/INFO etc..): enable/disable debug mode with extra messages output.
         """
-        self.dburi = dburi
-        self.dbclient = MongoClient(dburi)
-        self.ip = ip
-        self.port = port
-        self.info_level = info_level
-        self.apikey = apikey
-        self.apidoc_dir = 'hunabku_website'
+        self.config.update(config)
+        self.plugin_prefix = "hunabku"
+        self.apidoc_dir = self.config.apidoc
         self.apidoc_static_dir = self.apidoc_dir + '/static'
         self.apidoc_output_dir = self.apidoc_dir + '/static/apidoc'
         self.apidoc_templates_dir = self.apidoc_dir + '/templates'
         self.apidoc_config_dir = self.apidoc_dir + '/config'
         self.apidoc_config_data = {}
         self.apidoc_config_data['url'] = 'http://' + \
-            ip + ':' + str(port) + '/apidoc'
-        self.apidoc_config_data['sampleUrl'] = 'http://' + ip + ':' + str(port)
+            config.host + ':' + str(config.port)
+        self.apidoc_config_data['sampleUrl'] = 'http://' + \
+            config.host + ':' + str(config.port)
         self.apidoc_config_data['header'] = {}
         self.apidoc_config_data['header']['filename'] = self.apidoc_config_dir + \
             '/apidoc-header.md'
         self.apidoc_config_data['version'] = get_version()
         self.pkg_config_dir = str(
             pathlib.Path(__file__).parent.absolute()) + '/config/'
         self.pkg_templates_dir = str(
             pathlib.Path(__file__).parent.absolute()) + '/templates/'
         self.plugins = []
-        self.log_file = log_file
         self.logger = logging.getLogger(__name__)
-        self.set_info_level(info_level)
+        self.set_info_level(config["info_level"])
         self.app = Flask(
             'hanubku',
             static_folder=self.apidoc_static_dir,
             static_url_path='/',
             template_folder=self.apidoc_templates_dir)
-        self.apidoc_setup()
-        self.load_plugins()
-        self.generate_doc()
 
     def apidoc_setup(self):
         """
         creates an ApiDoc folder to dump configuration and documentation of the APIs
         """
         try:
             os.makedirs(self.apidoc_dir, exist_ok=True)
@@ -156,70 +146,103 @@
         copy_tree(self.pkg_templates_dir, self.apidoc_templates_dir)
 
     def set_info_level(self, info_level):
         """
         Information level for debug or verbosity of the application (https://docs.python.org/3.1/library/logging.html)
         """
         if info_level != logging.DEBUG:
-            logging.basicConfig(filename=self.log_file, level=info_level)
-        self.info_level = info_level
+            logging.basicConfig(
+                filename=self.config["log_file"], level=info_level)
+        self.config["info_level"] = info_level
 
-    def load_plugins(self):
+    def load_plugins(self, verbose=True):
         """
         This method return the plugins found in the folder plugins.
         """
-        self.logger.warning('-----------------------')
-        self.logger.warning('------ Loagind Plugins:')
-        for path in glob.glob(
-                str(pathlib.Path(__file__).parent.absolute()) + "/plugins/*.py"):
-            name = path.split(os.path.sep)[-1].replace('.py', '')
-            print('------ Loading plugin: ' + name)
-            spec = importlib.util.spec_from_file_location(name, path)
-            module = spec.loader.load_module()
-            plugin_class = getattr(module, name)
-            instance = plugin_class(self)
-            instance.register_endpoints()
-            plugin = {}
-            plugin['name'] = name
-            plugin['path'] = path
-            plugin['spec'] = spec
-            plugin['instance'] = instance
-            self.plugins.append(plugin)
+        if verbose:
+            self.logger.warning('-----------------------')
+            self.logger.warning('------ Loagind Plugins:')
+        discovered_plugins = {
+            name: importlib.import_module(name)
+            for finder, name, ispkg
+            in pkgutil.iter_modules()
+            if name.startswith(self.plugin_prefix + '_')
+        }
+        for discovered_plugin in discovered_plugins:
+            for path in glob.glob(
+                    str(discovered_plugins[discovered_plugin].__path__[0]) + "/endpoints/*.py"):
+                mname = path.split(os.path.sep)[-1].replace('.py', '')
+                if verbose:
+                    self.logger.warning(
+                        f'------ Loading plugin module: {discovered_plugin} {mname}')
+                spec = importlib.util.spec_from_file_location(mname, path)
+                module = spec.loader.load_module()
+                for cname, plugin_class in inspect.getmembers(module):
+                    if inspect.isclass(plugin_class) and issubclass(plugin_class, HunabkuPluginBase) and cname.startswith(mname):
+                        if verbose:
+                            self.logger.warning(
+                                f'------ Registering plugin class: {mname}.{cname}')
+                        instance = plugin_class(self)
+                        instance.register_endpoints()
+                        plugin = {}
+
+                        plugin['package'] = discovered_plugin
+                        plugin['mod_name'] = mname
+                        plugin['class'] = plugin_class
+                        plugin['class_name'] = cname
+                        plugin['name'] = f"{discovered_plugin}.{mname}.{cname}"
+                        plugin['path'] = path
+                        plugin['spec'] = spec
+                        plugin['instance'] = instance
+                        if discovered_plugin in self.config.keys():
+                            if mname in self.config[discovered_plugin].keys():
+                                if cname in self.config[discovered_plugin][mname].keys():
+                                    instance.config.update(self.config[discovered_plugin][mname][cname])
+                        self.plugins.append(plugin)
+                        if verbose:
+                            self.logger.warning(
+                                f'------ Registered plugin class: {mname}.{cname}  DONE')
+                        
 
     def check_apidoc_syntax(self, plugin_file):
         """
         Allows to check in the syntaxis in the docstring comment is right
         for apidoc  files generation.
         The the syntax is wrong, the Hunabku server can not start.
         """
-        args = ['apidoc', '-c', self.apidoc_config_dir, '-i',
-                str(pathlib.Path(__file__).parent.absolute()) + '/plugins/',
-                '--simulate',
+        args = ['apidoc', '-c', self.apidoc_config_dir + os.path.sep + "apidoc.json", '-i',
+                str(pathlib.Path(plugin_file).parent.absolute()),
+                '--dry-run',
                 '-f',
                 plugin_file]
         process = subprocess.run(args,
                                  stdout=subprocess.PIPE)
         if process.returncode != 0:
-            self.logger.error('------ERROR: parsing docstring for apidocs in plugin ' + plugin_file)
-            self.logger.error('             server can not start until apidocs syntax is fixed')
+            self.logger.error(
+                '------ERROR: parsing docstring for apidocs in plugin ' + plugin_file)
+            self.logger.error(
+                '             server can not start until apidocs syntax is fixed')
+            self.logger.error(process)
             sys.exit(1)
 
     def generate_doc(self, timeout=1, maxtries=5):
         """
         this method allows to generated apidocs documentation parsing plugin files
         """
         self.logger.warning('-----------------------')
         self.logger.warning('------ Creating documentation')
 
         rmtree(self.apidoc_static_dir, ignore_errors=True)
-        args = ['apidoc', '-c', self.apidoc_config_dir, '-i',
-                str(pathlib.Path(__file__).parent.absolute()) + '/plugins/']
+        args = ['apidoc', '-c', self.apidoc_config_dir +
+                os.path.sep + "apidoc.json"]
 
         for plugin in self.plugins:
             self.check_apidoc_syntax(plugin['path'])
+            args.append('-i')
+            args.append(str(pathlib.Path(plugin['path']).parent.absolute()))
             args.append('-f')
             args.append(plugin['path'])
         args.append('-o')
         args.append(self.apidoc_output_dir)
         process = subprocess.Popen(args,
                                    stdout=subprocess.PIPE,
                                    stderr=subprocess.STDOUT)
@@ -227,14 +250,15 @@
         while process.poll() is None:
             time.sleep(timeout)
             counter = counter + 1
             if counter == maxtries:
                 process.kill()
                 break
         self.logger.warning(
-            '------ Apidocs at http://{}:{}/apidoc/index.html'.format(self.ip, self.port))
+            '------ Apidocs at http://{}:{}/apidoc/index.html'.format(self.config.host, self.config.port))
 
     def start(self):
         """
         Method to start server
         """
-        self.app.run(host=self.ip, port=self.port, debug=True)
+        self.app.run(host=self.config.host, port=self.config.port,
+                     debug=True, use_reloader=self.config.use_reloader)
```

### Comparing `Hunabku-0.0.8a0/hunabku/HunabkuBase.py` & `Hunabku-0.0.9/hunabku/HunabkuBase.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 from flask import (
     json,
     request
 )
 from bson import ObjectId
 from functools import wraps
-
+from hunabku.Config import Config
 
 class HunabkuJsonEncoder(json.JSONEncoder):
     """
     Custom JSON encoder for Hunabku,
     all the customized stuff for encoding required for our endpoints
     can be handle in this class
     """
@@ -17,15 +17,19 @@
     def default(self, o):
         if isinstance(o, ObjectId):
             return str(o)
         return json.JSONEncoder.default(self, o)
 
 
 _endpoints = {}  # global hidden dictionary to register every endpoint by plugin
+_verbose = True
 
+def set_verbose(status):
+    global _verbose
+    _verbose = status
 
 def endpoint(path, methods):
     """
     Specilaized decorator to use in the methods of the class that inherit from  HunabkuPluginBase
     this decorator allows to register the path and methods [GET,POST,DELETE,PUT]
     in the flask app.
 
@@ -45,47 +49,47 @@
             return response
         else:
             return self.send_apikey_error()
 
     """
     def wrapper(func):
         global _endpoints
-        print('------ Adding endpoint ' + path + ' with methods' + str(methods))
+        global _verbose
+        if _verbose:
+            print('------ Adding endpoint ' + path + ' with methods' + str(methods))
         class_name, func_name = func.__qualname__.split('.')
         if class_name not in _endpoints:
             _endpoints[class_name] = []
         _endpoints[class_name].append(
             {'path': path, 'methods': methods, 'func_name': func_name})
 
         @wraps(func)
         def _impl(self, *method_args, **method_kwargs):
-            response = func(self)
+            response = func(self, *method_args, **method_kwargs)
             return response
+        _impl.__name__ = func.__qualname__ ##WARNING: this is required to avoid overwrite methods in the class
         return _impl
     return wrapper
 
 
-class HunabkuPluginBase:
+class HunabkuPluginBase(object):
+    config = Config()
+
     def __init__(self, hunabku):
         """
         Base class to handle the plugins.
         Allows to have access to the MondoDB object, custom json methods
         with our encoders, utility functions to check apikeys and send default messages
         in case of error.
 
         This class allows to register the endpoints setting a decorator in the method
         that is going to hanlde the endpoint.
 
         """
-        self.dburi = hunabku.dburi
-        self.dbclient = hunabku.dbclient
-        self.ip = hunabku.ip
-        self.port = hunabku.port
-        self.info_level = hunabku.info_level
-        self.apikey = hunabku.apikey
+        self.global_config = hunabku.config
         self.app = hunabku.app
         self.request = request
         self.json = json
         self.logger = hunabku.logger
         self.hunabku = hunabku
         _dumps = self.json.dumps
         _dump = self.json.dump
@@ -148,42 +152,72 @@
             response=self.json.dumps(
                 {'msg': 'The HTTP 401 Unauthorized invalid authentication apikey for the target resource.'}),
             status=401,
             mimetype='application/json'
         )
         return response
 
+    def badrequest_error(self):
+        """
+        return defualt bad request error
+        """
+        data = {"error": "Bad Request",
+                "message": "Invalid parameters passed. Please fix your request with valid parameters."}
+        response = self.app.response_class(response=self.json.dumps(data),
+                                            status=400,
+                                            mimetype='application/json')
+        return response
+
     def valid_apikey(self):
-        apikey = self.request.args.get('apikey')
-        if self.apikey == apikey:
+        if self.request.method == 'POST':
+            apikey = self.request.form.get('apikey')
+        else:
+            apikey = self.request.args.get('apikey')
+        if self.global_config["apikey"] == apikey:
             return True
         else:
             return False
 
     def register_endpoints(self):
         """
         Method to register all the endpoints in flask's app
         """
         global _endpoints
-        if self.is_valid_endpoints():
+        if self.has_valid_endpoints():
             for endpoint_data in _endpoints[type(self).__name__]:
                 path = endpoint_data['path']
                 func_name = endpoint_data['func_name']
                 methods = endpoint_data['methods']
                 func = getattr(self, func_name)
                 self.app.add_url_rule(path, view_func=func, methods=methods)
 
-    def get_global_endpoints(self):
+    def valid_parameters(self, params):
+        """
+        Method to check is the parameters passed to the endpoint are valid,
+        if unkown parameter is passed, a bad request is returned.
+        """
+        if self.request.method == 'POST':
+            args = self.request.form
+        else:
+            args = self.request.args
+
+        for rarg in args:
+            if rarg not in params:
+                return False
+        return True
+
+    @classmethod
+    def get_global_endpoints(cls):
         """
         Method to return the global dictionary with all
         the registers  loaded
         """
         return _endpoints
 
-    def is_valid_endpoints(self):
+    def has_valid_endpoints(self):
         """
         This method checks before to load the plugin if any paths in the endpoint is repeated.
         this platform does not allows overwrite endpoint paths.
         """
         plugins = list(_endpoints.keys())
         current = type(self).__name__
         plugins.remove(current)
```

### Comparing `Hunabku-0.0.8a0/setup.py` & `Hunabku-0.0.9/hunabku/templates/plugin/HunabKu_template/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,48 +47,45 @@
     warning = "WARNING: Windows is not officially supported"
     print(warning, file=sys.stderr)
 
 
 def main():
     setup(
         # Application name:
-        name="Hunabku",
+        name="Hunabku_template",
 
         # Version number (initial):
-        version=get_version('hunabku/_version.py'),
+        version=get_version('hunabku_template/_version.py'),
 
         # Application author details:
         author="Colav",
         author_email="colav@udea.edu.co",
 
         # Packages
         packages=find_packages(exclude=['tests']),
 
         # Include additional files into the package
         include_package_data=True,
 
         # Details
-        url="https://github.com/colav/Hunabku",
-        scripts=['bin/hunabku_server', 'bin/hunabku_loader'],
+        url="https://github.com/colav/Hunabku_plugins",
         #
         license="BSD",
 
-        description="Papers database endpoint API",
+        description="Hunabku plguin",
 
         long_description=open("README.md").read(),
 
         long_description_content_type="text/markdown",
 
         # Dependent packages (distributions)
+        # put you packages here
         install_requires=[
-            'pymongo>=3.10.1',
             'flask>=1.1.2',
-            'pandas',
-            'numpy',
             'requests>=2.22.0',
-            'joblib>=0.14.1'
+            'hunabku'
         ],
     )
 
 
 if __name__ == "__main__":
     main()
```


# Comparing `tmp/di_registry-0.4.6.tar.gz` & `tmp/di_registry-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/di_registry-0.4.6.tar", last modified: Wed Jan  4 21:45:41 2023, max compression
+gzip compressed data, was "dist/di_registry-0.4.7.tar", last modified: Wed Apr 19 18:36:35 2023, max compression
```

## Comparing `di_registry-0.4.6.tar` & `di_registry-0.4.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 21:45:41.000000 di_registry-0.4.6/
--rw-r--r--   0 root         (0) root         (0)      504 2023-01-04 21:45:41.000000 di_registry-0.4.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-01-04 21:45:33.000000 di_registry-0.4.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 21:45:41.000000 di_registry-0.4.6/di_registry/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-01-04 21:45:33.000000 di_registry-0.4.6/di_registry/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-04 21:45:33.000000 di_registry-0.4.6/di_registry/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    18465 2023-01-04 21:45:33.000000 di_registry-0.4.6/di_registry/abc.py
--rw-rw-rw-   0 root         (0) root         (0)    15049 2023-01-04 21:45:33.000000 di_registry-0.4.6/di_registry/registry.py
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-01-04 21:45:33.000000 di_registry-0.4.6/di_registry/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 21:45:41.000000 di_registry-0.4.6/di_registry.egg-info/
--rw-r--r--   0 root         (0) root         (0)      504 2023-01-04 21:45:40.000000 di_registry-0.4.6/di_registry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      306 2023-01-04 21:45:41.000000 di_registry-0.4.6/di_registry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-04 21:45:40.000000 di_registry-0.4.6/di_registry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-01-04 21:45:40.000000 di_registry-0.4.6/di_registry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-01-04 21:45:40.000000 di_registry-0.4.6/di_registry.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-04 21:45:41.000000 di_registry-0.4.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-01-04 21:45:33.000000 di_registry-0.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:36:35.000000 di_registry-0.4.7/
+-rw-r--r--   0 root         (0) root         (0)      504 2023-04-19 18:36:35.000000 di_registry-0.4.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-19 18:36:27.000000 di_registry-0.4.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:36:35.000000 di_registry-0.4.7/di_registry/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-19 18:36:27.000000 di_registry-0.4.7/di_registry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-19 18:36:27.000000 di_registry-0.4.7/di_registry/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18465 2023-04-19 18:36:27.000000 di_registry-0.4.7/di_registry/abc.py
+-rw-rw-rw-   0 root         (0) root         (0)    15836 2023-04-19 18:36:27.000000 di_registry-0.4.7/di_registry/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-04-19 18:36:27.000000 di_registry-0.4.7/di_registry/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:36:35.000000 di_registry-0.4.7/di_registry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      504 2023-04-19 18:36:35.000000 di_registry-0.4.7/di_registry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      306 2023-04-19 18:36:35.000000 di_registry-0.4.7/di_registry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 18:36:35.000000 di_registry-0.4.7/di_registry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-04-19 18:36:35.000000 di_registry-0.4.7/di_registry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-19 18:36:35.000000 di_registry-0.4.7/di_registry.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 18:36:35.000000 di_registry-0.4.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2023-04-19 18:36:27.000000 di_registry-0.4.7/setup.py
```

### Comparing `di_registry-0.4.6/di_registry/abc.py` & `di_registry-0.4.7/di_registry/abc.py`

 * *Files identical despite different names*

### Comparing `di_registry-0.4.6/di_registry/registry.py` & `di_registry-0.4.7/di_registry/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,21 +98,24 @@
         return Registry._default_registry
 
     def __init__(self,
                  config_path: Optional[str] = None,
                  configuration: Optional[ConfigurationType] = None,
                  factories: Optional[Dict[str, FactoryType]] = None,
                  objects: Optional[Dict[str, Any]] = None,
-                 set_default: bool = True):
+                 set_default: bool = True,
+                 http_timeout: Optional[float] = 2.,
+                 ):
         self.config_path = config_path
         self.configuration = configuration or {}
         self.configurations = [configuration] if configuration else []
         self.factories = factories or {}
         self.factory_types = {val: key for key, val in self.factories.items()}
         self.objects = objects or {}
+        self.http_timeout = http_timeout
 
         if set_default and Registry._default_registry is None:
             Registry._default_registry = self
 
         if self.config_path is not None:
             self.load_configuration()
 
@@ -147,26 +150,32 @@
         if 'configuration_url' not in registry_config:
             raise RegistryError(f'Cannot use `http_configure`, "$registry.configuration_url" not available in configuration')
 
         for name in names:
             config_url = registry_config['configuration_url'] + '/' + name
             self.configure(config_url, ignore_missing=ignore_missing)
 
-    def save_http_configuration(self, name: str, data: Dict[str, Any]):
+    def save_http_configuration(self, name: str, data: Dict[str, Any], timeout: Optional[float] = 'default'):
+        """
+        Saves the named configuration as a dictionary to the configuration URL
+        """
         registry_config = self.registry_configuration()
 
         if 'configuration_url' not in registry_config:
             raise RegistryError(f'Cannot use `http_configure`, "$registry.configuration_url" not available in configuration')
 
         config_url = registry_config['configuration_url'] + '/' + name
-
+        # 'default' is a sentinel value to allow the user to specify None or a value
+        timeout = self.http_timeout if timeout == 'default' else timeout
         try:
-            response = requests.put(config_url, json=data)
+            response = requests.put(config_url, json=data, timeout=timeout)
         except requests.ConnectionError:
             raise RegistryError(f'Cannot save parameters to "{config_url}", error connecting to server')
+        except TimeoutError:
+            raise RegistryError(f'Cannot save parameters to "{config_url}", timeout when communicating with server')
 
         if not response.ok:
             raise RegistryError(f'Cannot save parameters to "{config_url}", response status: {response.status_code}')
 
     def reconfigure(self):
         self.configuration = {}
 
@@ -193,17 +202,19 @@
             if config_type == 'json':
                 self.merge_configuration(json.load(config_file))
             elif config_type == 'yaml':
                 self.merge_configuration(yaml.safe_load(config_file))
             else:
                 raise RegistryError(f'Invalid config file format, must be "json" or "yaml": {config_type}')
 
-    def load_http_configuration(self, config_url, ignore_missing: bool = False):
+    def load_http_configuration(self, config_url, ignore_missing: bool = False, timeout: Optional[float] = 'default'):
+        # 'default' is a sentinel value to allow the user to specify None or a value
+        timeout = self.http_timeout if timeout == 'default' else timeout
         try:
-            response = requests_session().get(config_url)
+            response = requests_session().get(config_url, timeout=timeout)
         except requests.ConnectionError:
             raise RegistryError(f'Cannot read configuration from "{config_url}", error connecting to server')
 
         if not response.ok:
             if response.status_code == 404 and ignore_missing:
                 return
```

### Comparing `di_registry-0.4.6/di_registry/test.py` & `di_registry-0.4.7/di_registry/test.py`

 * *Files identical despite different names*

### Comparing `di_registry-0.4.6/setup.py` & `di_registry-0.4.7/setup.py`

 * *Files identical despite different names*


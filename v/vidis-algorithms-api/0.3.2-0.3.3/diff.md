# Comparing `tmp/vidis_algorithms_api-0.3.2.tar.gz` & `tmp/vidis_algorithms_api-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidis_algorithms_api-0.3.2.tar", last modified: Sun Apr  9 12:53:05 2023, max compression
+gzip compressed data, was "vidis_algorithms_api-0.3.3.tar", last modified: Wed Apr 19 13:26:22 2023, max compression
```

## Comparing `vidis_algorithms_api-0.3.2.tar` & `vidis_algorithms_api-0.3.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1370 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/examples/dummy_example/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 12:49:15.000000 vidis_algorithms_api-0.3.2/examples/dummy_example/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      528 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.2/examples/dummy_example/algorithm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/examples/neural_network/
--rw-rw-rw-   0 root         (0) root         (0)     3626 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.2/examples/neural_network/algorithm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/examples/neural_network/model/
--rw-rw-rw-   0 root         (0) root         (0)     3737 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.2/examples/neural_network/model/model.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2023-04-09 12:49:15.000000 vidis_algorithms_api-0.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-04-09 12:49:15.000000 vidis_algorithms_api-0.3.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/vidis_algorithms_api/
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     1091 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api/Task.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-07 07:06:59.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/vidis_algorithms_api/core/
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api/core/Settings.py
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/vidis_algorithms_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-09 12:53:05.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      566 2023-04-09 12:53:05.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 12:53:05.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-09 12:53:05.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-09 12:53:05.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 13:26:22.524507 vidis_algorithms_api-0.3.3/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-19 13:26:22.524507 vidis_algorithms_api-0.3.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 13:26:22.524507 vidis_algorithms_api-0.3.3/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 13:26:22.524507 vidis_algorithms_api-0.3.3/examples/dummy_example/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 12:49:15.000000 vidis_algorithms_api-0.3.3/examples/dummy_example/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      528 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.3/examples/dummy_example/algorithm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 13:26:22.524507 vidis_algorithms_api-0.3.3/examples/neural_network/
+-rw-rw-rw-   0 root         (0) root         (0)     3626 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.3/examples/neural_network/algorithm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 13:26:22.524507 vidis_algorithms_api-0.3.3/examples/neural_network/model/
+-rw-rw-rw-   0 root         (0) root         (0)     3737 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.3/examples/neural_network/model/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-04-19 13:18:03.000000 vidis_algorithms_api-0.3.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 13:26:22.524507 vidis_algorithms_api-0.3.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-04-19 13:18:03.000000 vidis_algorithms_api-0.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 13:26:22.524507 vidis_algorithms_api-0.3.3/vidis_algorithms_api/
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.3/vidis_algorithms_api/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-04-19 13:18:03.000000 vidis_algorithms_api-0.3.3/vidis_algorithms_api/Task.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-07 07:06:59.000000 vidis_algorithms_api-0.3.3/vidis_algorithms_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 13:26:22.524507 vidis_algorithms_api-0.3.3/vidis_algorithms_api/core/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.3/vidis_algorithms_api/core/Settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.3/vidis_algorithms_api/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 13:26:22.524507 vidis_algorithms_api-0.3.3/vidis_algorithms_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-19 13:26:22.000000 vidis_algorithms_api-0.3.3/vidis_algorithms_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      566 2023-04-19 13:26:22.000000 vidis_algorithms_api-0.3.3/vidis_algorithms_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 13:26:22.000000 vidis_algorithms_api-0.3.3/vidis_algorithms_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-19 13:26:22.000000 vidis_algorithms_api-0.3.3/vidis_algorithms_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-04-19 13:26:22.000000 vidis_algorithms_api-0.3.3/vidis_algorithms_api.egg-info/top_level.txt
```

### Comparing `vidis_algorithms_api-0.3.2/README.md` & `vidis_algorithms_api-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.3.2/examples/dummy_example/algorithm.py` & `vidis_algorithms_api-0.3.3/examples/dummy_example/algorithm.py`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.3.2/examples/neural_network/algorithm.py` & `vidis_algorithms_api-0.3.3/examples/neural_network/algorithm.py`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.3.2/examples/neural_network/model/model.py` & `vidis_algorithms_api-0.3.3/examples/neural_network/model/model.py`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.3.2/setup.py` & `vidis_algorithms_api-0.3.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 requirements = [
     'pydantic==1.10.2',
     'loguru==0.6.0',
     'numpy==1.24.1',
     'celery[amqp,redis]==5.2.7',
+    'redis==4.5.4'
 ]
 
 with open('README.md', 'r') as f:
     description = f.read()
 
 
 def setup_package():
-    __version__ = '0.3.2'
+    __version__ = '0.3.3'
     url = 'https://github.com/Banayaki'
 
     setup(name='vidis_algorithms_api',
           description=description,
           version=__version__,
           url=url,
           license='MIT',
```

### Comparing `vidis_algorithms_api-0.3.2/vidis_algorithms_api/Main.py` & `vidis_algorithms_api-0.3.3/vidis_algorithms_api/Main.py`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.3.2/vidis_algorithms_api/Task.py` & `vidis_algorithms_api-0.3.3/vidis_algorithms_api/Task.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def _save_task_result(self, layer_data: np.ndarray, hypespecter_path: str):
         path_to_save = os.path.join(settings.DATA_PATH, hypespecter_path,
                                     settings.CUSTOM_LAYER_FOLDER, f'{self.name}_{datetime.now()}.npy')
         os.makedirs(os.path.dirname(path_to_save), exist_ok=True)
         np.save(path_to_save, layer_data)
 
     def run(self, hypespecter_path, **kwargs):
-        data = np.load(os.path.join(settings.DATA_PATH, hypespecter_path), mmap_mode="r")
+        data = np.load(os.path.join(settings.DATA_PATH, hypespecter_path, "hsi.npy"), mmap_mode="r")
         result = self.task(hyperspecter=data, **kwargs)
         assert result.ndim == 2, "Result should have two dimensions (height x width)"
         self._save_task_result(result, hypespecter_path)
     
     @abstractmethod
     def task(self, hyperspecter: np.ndarray, **kwargs) -> np.ndarray:
         pass
```

### Comparing `vidis_algorithms_api-0.3.2/vidis_algorithms_api.egg-info/SOURCES.txt` & `vidis_algorithms_api-0.3.3/vidis_algorithms_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*


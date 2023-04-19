# Comparing `tmp/plico_interferometer-0.0.4.tar.gz` & `tmp/plico_interferometer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plico_interferometer-0.0.4.tar", last modified: Thu Dec 30 18:51:58 2021, max compression
+gzip compressed data, was "plico_interferometer-0.1.0.tar", last modified: Wed Apr 19 16:34:33 2023, max compression
```

## Comparing `plico_interferometer-0.0.4.tar` & `plico_interferometer-0.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-30 18:51:58.931950 plico_interferometer-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2021-12-30 18:51:58.931950 plico_interferometer-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      848 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-30 18:51:58.927950 plico_interferometer-0.0.4/plico_interferometer/
--rw-r--r--   0 runner    (1001) docker     (121)      877 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/plico_interferometer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/plico_interferometer/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-30 18:51:58.931950 plico_interferometer-0.0.4/plico_interferometer/client/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/plico_interferometer/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1840 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/plico_interferometer/client/abstract_interferometer_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2362 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/plico_interferometer/client/interferometer_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      910 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/plico_interferometer/client/simulated_interferometer_client.py
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/plico_interferometer/client/snapshot_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-30 18:51:58.931950 plico_interferometer-0.0.4/plico_interferometer/types/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/plico_interferometer/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      324 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/plico_interferometer/types/interferometer_status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-30 18:51:58.931950 plico_interferometer-0.0.4/plico_interferometer/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/plico_interferometer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      163 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/plico_interferometer/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/plico_interferometer/utils/timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-30 18:51:58.931950 plico_interferometer-0.0.4/plico_interferometer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2021-12-30 18:51:58.000000 plico_interferometer-0.0.4/plico_interferometer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      968 2021-12-30 18:51:58.000000 plico_interferometer-0.0.4/plico_interferometer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-30 18:51:58.000000 plico_interferometer-0.0.4/plico_interferometer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-12-30 18:51:58.000000 plico_interferometer-0.0.4/plico_interferometer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-30 18:51:58.000000 plico_interferometer-0.0.4/plico_interferometer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-12-30 18:51:58.000000 plico_interferometer-0.0.4/plico_interferometer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-30 18:51:58.931950 plico_interferometer-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2895 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-30 18:51:58.931950 plico_interferometer-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/test/fake_time_mod.py
--rw-r--r--   0 runner    (1001) docker     (121)    16662 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/test/test_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-30 18:51:58.931950 plico_interferometer-0.0.4/test/types/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/test/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      563 2021-12-30 18:51:46.000000 plico_interferometer-0.0.4/test/types/interferometer_status_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:33.659877 plico_interferometer-0.1.0/plico_interferometer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/plico_interferometer/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/client/abstract_interferometer_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/client/interferometer_WCF_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/client/interferometer_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/client/simulated_interferometer_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/client/snapshot_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/plico_interferometer/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/types/interferometer_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/plico_interferometer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/utils/timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/plico_interferometer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-19 16:34:33.000000 plico_interferometer-0.1.0/plico_interferometer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-19 16:34:33.000000 plico_interferometer-0.1.0/plico_interferometer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:34:33.000000 plico_interferometer-0.1.0/plico_interferometer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 16:34:33.000000 plico_interferometer-0.1.0/plico_interferometer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-19 16:34:33.000000 plico_interferometer-0.1.0/plico_interferometer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/test/fake_time_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/test/test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/test/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/test/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/test/types/interferometer_status_test.py
```

### Comparing `plico_interferometer-0.0.4/LICENSE` & `plico_interferometer-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plico_interferometer-0.0.4/PKG-INFO` & `plico_interferometer-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: plico_interferometer
-Version: 0.0.4
+Version: 0.1.0
 Summary: interferometer controller with PLICO
 Home-page: https://github.com/ArcetriAdaptiveOptics/plico_interferometer
 Author: Lorenzo Busoni, Alfio Puglisi
 Author-email: lorenzo.busoni@inaf.it
 License: MIT
 Keywords: plico,interferometer,laboratory,instrumentation control
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # plico_interferometer
 
 client of an interferometer controlled under the plico environment 
@@ -26,9 +24,7 @@
  [![Documentation Status](https://readthedocs.org/projects/plico_interferometer/badge/?version=latest)](https://plico_interferometer.readthedocs.io/en/latest/?badge=latest)
  [![PyPI version](https://badge.fury.io/py/plico-interferometer.svg)](https://badge.fury.io/py/plico-interferometer)
 
 
 plico_interferometer is an application to control motors under the [plico][plico] environment.
 
 [plico]: https://github.com/ArcetriAdaptiveOptics/plico
-
-
```

### Comparing `plico_interferometer-0.0.4/README.md` & `plico_interferometer-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `plico_interferometer-0.0.4/plico_interferometer/__init__.py` & `plico_interferometer-0.1.0/plico_interferometer/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,17 +9,49 @@
     return cfgFileMgr.getConfigFilePath()
 
 
 default_config_file_path = _getDefaultConfigFilePath()
 
 
 def interferometer(hostname, port):
+    '''
+    create client of plico interferometer server
 
-    from plico_interferometer.client.interferometer_client import InterferometerClient
+    Parameters
+    ----------
+    hostname: string
+        ip address of the computer running the plico interferometer server
+
+    port: integer
+        port of the plico interferometer server, specified in the
+        config file on the plico interferometer server. Typical = 7300
+    '''
+
+    from plico_interferometer.client.interferometer_client import \
+        InterferometerClient
     from plico.rpc.zmq_remote_procedure_call import ZmqRemoteProcedureCall
     from plico.rpc.zmq_ports import ZmqPorts
     from plico.rpc.sockets import Sockets
 
     rpc = ZmqRemoteProcedureCall()
     zmqPorts = ZmqPorts(hostname, port)
     sockets = Sockets(zmqPorts, rpc)
     return InterferometerClient(rpc, sockets)
+
+
+def interferometer_4SightFocus_client(hostname, port):
+    '''
+    create client of 4SightFocus
+
+    Parameters
+    ----------
+    hostname: string
+        ip address of the computer running the 4SightFocus software
+
+    port: integer
+        port of the 4SightFocus software
+    '''
+    from plico_interferometer.client.interferometer_WCF_client import \
+        InterferometerWCFClient
+
+    interferometer = InterferometerWCFClient(hostname, port)
+    return interferometer
```

### Comparing `plico_interferometer-0.0.4/plico_interferometer/client/abstract_interferometer_client.py` & `plico_interferometer-0.1.0/plico_interferometer/client/abstract_interferometer_client.py`

 * *Files identical despite different names*

### Comparing `plico_interferometer-0.0.4/plico_interferometer/client/interferometer_client.py` & `plico_interferometer-0.1.0/plico_interferometer/client/interferometer_client.py`

 * *Files identical despite different names*

### Comparing `plico_interferometer-0.0.4/plico_interferometer/client/simulated_interferometer_client.py` & `plico_interferometer-0.1.0/plico_interferometer/client/simulated_interferometer_client.py`

 * *Files identical despite different names*

### Comparing `plico_interferometer-0.0.4/plico_interferometer.egg-info/PKG-INFO` & `plico_interferometer-0.1.0/plico_interferometer.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: plico-interferometer
-Version: 0.0.4
+Version: 0.1.0
 Summary: interferometer controller with PLICO
 Home-page: https://github.com/ArcetriAdaptiveOptics/plico_interferometer
 Author: Lorenzo Busoni, Alfio Puglisi
 Author-email: lorenzo.busoni@inaf.it
 License: MIT
 Keywords: plico,interferometer,laboratory,instrumentation control
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # plico_interferometer
 
 client of an interferometer controlled under the plico environment 
@@ -26,9 +24,7 @@
  [![Documentation Status](https://readthedocs.org/projects/plico_interferometer/badge/?version=latest)](https://plico_interferometer.readthedocs.io/en/latest/?badge=latest)
  [![PyPI version](https://badge.fury.io/py/plico-interferometer.svg)](https://badge.fury.io/py/plico-interferometer)
 
 
 plico_interferometer is an application to control motors under the [plico][plico] environment.
 
 [plico]: https://github.com/ArcetriAdaptiveOptics/plico
-
-
```

### Comparing `plico_interferometer-0.0.4/plico_interferometer.egg-info/SOURCES.txt` & `plico_interferometer-0.1.0/plico_interferometer.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 README.md
 setup.py
 plico_interferometer/__init__.py
 plico_interferometer/__version__.py
 plico_interferometer.egg-info/PKG-INFO
 plico_interferometer.egg-info/SOURCES.txt
 plico_interferometer.egg-info/dependency_links.txt
-plico_interferometer.egg-info/entry_points.txt
 plico_interferometer.egg-info/requires.txt
 plico_interferometer.egg-info/top_level.txt
 plico_interferometer/client/__init__.py
 plico_interferometer/client/abstract_interferometer_client.py
+plico_interferometer/client/interferometer_WCF_client.py
 plico_interferometer/client/interferometer_client.py
 plico_interferometer/client/simulated_interferometer_client.py
 plico_interferometer/client/snapshot_entry.py
 plico_interferometer/types/__init__.py
 plico_interferometer/types/interferometer_status.py
 plico_interferometer/utils/__init__.py
 plico_interferometer/utils/constants.py
```

### Comparing `plico_interferometer-0.0.4/setup.py` & `plico_interferometer-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,62 +35,53 @@
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
         try:
-            self.status('Removing previous builds…')
+            self.status('Removing previous builds...')
             rmtree(os.path.join(here, 'dist'))
         except OSError:
             pass
 
-        self.status('Building Source and Wheel (universal) distribution…')
+        self.status('Building Source and Wheel (universal) distribution...')
         os.system(
             '{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
 
-        self.status('Uploading the package to PyPI via Twine…')
+        self.status('Uploading the package to PyPI via Twine...')
         os.system('twine upload dist/*')
 
-        self.status('Pushing git tags…')
+        self.status('Pushing git tags...')
         os.system('git tag v{0}'.format(about['__version__']))
         os.system('git push --tags')
 
         sys.exit()
 
 
 setup(name=NAME,
       description=DESCRIPTION,
       version=about['__version__'],
       classifiers=['Development Status :: 4 - Beta',
                    'Operating System :: POSIX :: Linux',
                    'Programming Language :: Python :: 3',
-                   'Programming Language :: Python :: 2.6',
                    'Programming Language :: Python :: 2.7',
                    ],
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       url=URL,
       author_email=EMAIL,
       author=AUTHOR,
       license=LICENSE,
       keywords=KEYWORDS,
       packages=['plico_interferometer',
                 'plico_interferometer.client',
                 'plico_interferometer.types',
                 'plico_interferometer.utils',
                 ],
-      entry_points={
-          'gui_scripts': [
-              'plico_interferometer_gui=plico_interferometer.gui.plico_interferometer_gui:main',
-          ],
-      },
-      package_data={
-          'plico_interferometer': ['conf/plico_interferometer.conf'],
-      },
       install_requires=["plico>=0.18",
                         "numpy",
                         ],
       include_package_data=True,
       test_suite='test',
       cmdclass={'upload': UploadCommand, },
       )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `plico_interferometer-0.0.4/test/fake_time_mod.py` & `plico_interferometer-0.1.0/test/fake_time_mod.py`

 * *Files identical despite different names*

### Comparing `plico_interferometer-0.0.4/test/test_helper.py` & `plico_interferometer-0.1.0/test/test_helper.py`

 * *Files identical despite different names*

### Comparing `plico_interferometer-0.0.4/test/types/interferometer_status_test.py` & `plico_interferometer-0.1.0/test/types/interferometer_status_test.py`

 * *Files identical despite different names*


# Comparing `tmp/bernhard-py3-1.0.tar.gz` & `tmp/bernhard-py3-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bernhard-py3-1.0.tar", last modified: Tue Apr 18 15:26:26 2017, max compression
+gzip compressed data, was "bernhard-py3-1.0.1.tar", last modified: Wed Apr 19 09:05:55 2023, max compression
```

## Comparing `bernhard-py3-1.0.tar` & `bernhard-py3-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2017-04-18 15:26:26.000000 bernhard-py3-1.0/
--rw-r--r--   0 brute     (1000) brute     (1000)       53 2017-04-18 15:19:52.000000 bernhard-py3-1.0/MANIFEST.in
--rw-r--r--   0 brute     (1000) brute     (1000)      788 2017-04-18 15:19:52.000000 bernhard-py3-1.0/README.md
-drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2017-04-18 15:26:26.000000 bernhard-py3-1.0/bernhard_py3.egg-info/
--rw-r--r--   0 brute     (1000) brute     (1000)     1904 2017-04-18 15:26:26.000000 bernhard-py3-1.0/bernhard_py3.egg-info/PKG-INFO
--rw-r--r--   0 brute     (1000) brute     (1000)       24 2017-04-18 15:26:26.000000 bernhard-py3-1.0/bernhard_py3.egg-info/requires.txt
--rw-r--r--   0 brute     (1000) brute     (1000)        1 2017-04-18 15:26:26.000000 bernhard-py3-1.0/bernhard_py3.egg-info/dependency_links.txt
--rw-r--r--   0 brute     (1000) brute     (1000)        1 2017-04-18 15:26:26.000000 bernhard-py3-1.0/bernhard_py3.egg-info/not-zip-safe
--rw-r--r--   0 brute     (1000) brute     (1000)        9 2017-04-18 15:26:26.000000 bernhard-py3-1.0/bernhard_py3.egg-info/top_level.txt
--rw-r--r--   0 brute     (1000) brute     (1000)      299 2017-04-18 15:26:26.000000 bernhard-py3-1.0/bernhard_py3.egg-info/SOURCES.txt
--rw-r--r--   0 brute     (1000) brute     (1000)     1904 2017-04-18 15:26:26.000000 bernhard-py3-1.0/PKG-INFO
--rw-r--r--   0 brute     (1000) brute     (1000)       38 2017-04-18 15:26:26.000000 bernhard-py3-1.0/setup.cfg
--rw-r--r--   0 brute     (1000) brute     (1000)     1178 2017-04-18 15:26:09.000000 bernhard-py3-1.0/setup.py
--rw-r--r--   0 brute     (1000) brute     (1000)       38 2017-04-18 15:19:52.000000 bernhard-py3-1.0/.gitignore
-drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2017-04-18 15:26:26.000000 bernhard-py3-1.0/bernhard/
--rw-r--r--   0 brute     (1000) brute     (1000)    13784 2017-04-18 15:19:52.000000 bernhard-py3-1.0/bernhard/pb.py
--rw-r--r--   0 brute     (1000) brute     (1000)     8318 2017-04-18 15:23:53.000000 bernhard-py3-1.0/bernhard/__init__.py
--rw-r--r--   0 brute     (1000) brute     (1000)    11189 2017-04-18 15:19:52.000000 bernhard-py3-1.0/LICENSE
+drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2023-04-19 09:05:55.230094 bernhard-py3-1.0.1/
+-rw-r--r--   0 brute     (1000) brute     (1000)       42 2017-04-19 06:05:44.000000 bernhard-py3-1.0.1/.gitignore
+-rw-r--r--   0 brute     (1000) brute     (1000)    11189 2017-04-18 15:19:52.000000 bernhard-py3-1.0.1/LICENSE
+-rw-r--r--   0 brute     (1000) brute     (1000)       53 2017-04-18 15:19:52.000000 bernhard-py3-1.0.1/MANIFEST.in
+-rw-r--r--   0 brute     (1000) brute     (1000)     1455 2023-04-19 09:05:55.226760 bernhard-py3-1.0.1/PKG-INFO
+-rw-r--r--   0 brute     (1000) brute     (1000)      656 2017-04-19 06:04:48.000000 bernhard-py3-1.0.1/README.md
+drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2023-04-19 09:05:55.226760 bernhard-py3-1.0.1/bernhard/
+-rw-r--r--   0 brute     (1000) brute     (1000)     8316 2023-04-19 09:02:21.000000 bernhard-py3-1.0.1/bernhard/__init__.py
+-rw-r--r--   0 brute     (1000) brute     (1000)    13784 2017-04-18 15:19:52.000000 bernhard-py3-1.0.1/bernhard/pb.py
+drwxr-xr-x   0 brute     (1000) brute     (1000)        0 2023-04-19 09:05:55.226760 bernhard-py3-1.0.1/bernhard_py3.egg-info/
+-rw-r--r--   0 brute     (1000) brute     (1000)     1455 2023-04-19 09:05:55.000000 bernhard-py3-1.0.1/bernhard_py3.egg-info/PKG-INFO
+-rw-r--r--   0 brute     (1000) brute     (1000)      299 2023-04-19 09:05:55.000000 bernhard-py3-1.0.1/bernhard_py3.egg-info/SOURCES.txt
+-rw-r--r--   0 brute     (1000) brute     (1000)        1 2023-04-19 09:05:55.000000 bernhard-py3-1.0.1/bernhard_py3.egg-info/dependency_links.txt
+-rw-r--r--   0 brute     (1000) brute     (1000)        1 2017-04-18 15:26:26.000000 bernhard-py3-1.0.1/bernhard_py3.egg-info/not-zip-safe
+-rw-r--r--   0 brute     (1000) brute     (1000)       22 2023-04-19 09:05:55.000000 bernhard-py3-1.0.1/bernhard_py3.egg-info/requires.txt
+-rw-r--r--   0 brute     (1000) brute     (1000)        9 2023-04-19 09:05:55.000000 bernhard-py3-1.0.1/bernhard_py3.egg-info/top_level.txt
+-rw-r--r--   0 brute     (1000) brute     (1000)       38 2023-04-19 09:05:55.230094 bernhard-py3-1.0.1/setup.cfg
+-rw-r--r--   0 brute     (1000) brute     (1000)     1206 2023-04-19 09:05:49.000000 bernhard-py3-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bernhard-py3-1.0/README.md` & `bernhard-py3-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Bernhard
 
-A simple Python client for [Riemann](http://github.com/aphyr/riemann). Usage:
+A simple Python3 client for [Riemann](http://github.com/aphyr/riemann). Usage:
 
 ```python
 import bernhard
 
 c = bernhard.Client()
 c.send({'host': 'myhost.foobar.com', 'service': 'myservice', 'metric': 12})
 q = c.query('true')
@@ -29,13 +29,9 @@
     print "Host:", e.host, "State:", e.state
 ```
 
 
 ## Installing
 
 ```bash
-pip install bernhard
+pip install bernhard-py3
 ```
-
-You may encounter issues with the `protobuf` dependency; if so, just run `pip
-install protobuf` manually, then `pip install bernhard`.
-
```

### Comparing `bernhard-py3-1.0/bernhard_py3.egg-info/PKG-INFO` & `bernhard-py3-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,59 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: bernhard-py3
-Version: 1.0
+Version: 1.0.1
 Summary: Python3 client for Riemann
 Home-page: http://github.com/brutasse/bernhard.git
 Author: Benjamin Anderspn
-Author-email: UNKNOWN
 License: ASF2.0
-Description: # Bernhard
-        
-        A simple Python client for [Riemann](http://github.com/aphyr/riemann). Usage:
-        
-        ```python
-        import bernhard
-        
-        c = bernhard.Client()
-        c.send({'host': 'myhost.foobar.com', 'service': 'myservice', 'metric': 12})
-        q = c.query('true')
-        ```
-        
-        Bernhard supports custom attributes with the syntax:
-        ```python
-        import bernhard
-        
-        c = bernhard.Client()
-        
-        c.send({'host': 'awesome.host.com', 'attributes': {'sky': 'sunny', 'sea': 'agitated'}})
-        ```
-        
-        Querying the index is as easy as:
-        ```python
-        import bernhard
-        
-        c = bernhard.Client()
-        q = c.query('true')
-        for e in q:
-            print "Host:", e.host, "State:", e.state
-        ```
-        
-        
-        ## Installing
-        
-        ```bash
-        pip install bernhard
-        ```
-        
-        You may encounter issues with the `protobuf` dependency; if so, just run `pip
-        install protobuf` manually, then `pip install bernhard`.
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Networking :: Monitoring
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Bernhard
+
+A simple Python3 client for [Riemann](http://github.com/aphyr/riemann). Usage:
+
+```python
+import bernhard
+
+c = bernhard.Client()
+c.send({'host': 'myhost.foobar.com', 'service': 'myservice', 'metric': 12})
+q = c.query('true')
+```
+
+Bernhard supports custom attributes with the syntax:
+```python
+import bernhard
+
+c = bernhard.Client()
+
+c.send({'host': 'awesome.host.com', 'attributes': {'sky': 'sunny', 'sea': 'agitated'}})
+```
+
+Querying the index is as easy as:
+```python
+import bernhard
+
+c = bernhard.Client()
+q = c.query('true')
+for e in q:
+    print "Host:", e.host, "State:", e.state
+```
+
+
+## Installing
+
+```bash
+pip install bernhard-py3
+```
```

### Comparing `bernhard-py3-1.0/PKG-INFO` & `bernhard-py3-1.0.1/bernhard_py3.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,59 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: bernhard-py3
-Version: 1.0
+Version: 1.0.1
 Summary: Python3 client for Riemann
 Home-page: http://github.com/brutasse/bernhard.git
 Author: Benjamin Anderspn
-Author-email: UNKNOWN
 License: ASF2.0
-Description: # Bernhard
-        
-        A simple Python client for [Riemann](http://github.com/aphyr/riemann). Usage:
-        
-        ```python
-        import bernhard
-        
-        c = bernhard.Client()
-        c.send({'host': 'myhost.foobar.com', 'service': 'myservice', 'metric': 12})
-        q = c.query('true')
-        ```
-        
-        Bernhard supports custom attributes with the syntax:
-        ```python
-        import bernhard
-        
-        c = bernhard.Client()
-        
-        c.send({'host': 'awesome.host.com', 'attributes': {'sky': 'sunny', 'sea': 'agitated'}})
-        ```
-        
-        Querying the index is as easy as:
-        ```python
-        import bernhard
-        
-        c = bernhard.Client()
-        q = c.query('true')
-        for e in q:
-            print "Host:", e.host, "State:", e.state
-        ```
-        
-        
-        ## Installing
-        
-        ```bash
-        pip install bernhard
-        ```
-        
-        You may encounter issues with the `protobuf` dependency; if so, just run `pip
-        install protobuf` manually, then `pip install bernhard`.
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Networking :: Monitoring
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Bernhard
+
+A simple Python3 client for [Riemann](http://github.com/aphyr/riemann). Usage:
+
+```python
+import bernhard
+
+c = bernhard.Client()
+c.send({'host': 'myhost.foobar.com', 'service': 'myservice', 'metric': 12})
+q = c.query('true')
+```
+
+Bernhard supports custom attributes with the syntax:
+```python
+import bernhard
+
+c = bernhard.Client()
+
+c.send({'host': 'awesome.host.com', 'attributes': {'sky': 'sunny', 'sea': 'agitated'}})
+```
+
+Querying the index is as easy as:
+```python
+import bernhard
+
+c = bernhard.Client()
+q = c.query('true')
+for e in q:
+    print "Host:", e.host, "State:", e.state
+```
+
+
+## Installing
+
+```bash
+pip install bernhard-py3
+```
```

### Comparing `bernhard-py3-1.0/setup.py` & `bernhard-py3-1.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,39 +2,40 @@
 
 import codecs
 import io
 import os
 
 from setuptools import setup
 
-with io.open(os.path.join(os.path.dirname(__file__), 'README.md'),
-          encoding='utf-8') as f:
+with io.open(
+    os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8"
+) as f:
     long_description = f.read()
 
 setup(
-    name = 'bernhard-py3',
-    version = '1.0',
-    description = 'Python3 client for Riemann',
-    long_description = long_description,
-    author = 'Benjamin Anderspn',
-    license = 'ASF2.0',
-    url = 'http://github.com/brutasse/bernhard.git',
-
-    classifiers = [
-        'Development Status :: 4 - Beta',
-        'Environment :: Other Environment',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: Apache Software License',
-        'Operating System :: MacOS :: MacOS X',
-        'Operating System :: POSIX',
-        'Operating System :: Unix',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3 :: Only',
-        'Topic :: Internet :: Log Analysis',
-        'Topic :: Utilities',
-        'Topic :: System :: Networking :: Monitoring'
+    name="bernhard-py3",
+    version="1.0.1",
+    description="Python3 client for Riemann",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    author="Benjamin Anderspn",
+    license="ASF2.0",
+    url="http://github.com/brutasse/bernhard.git",
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Environment :: Other Environment",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: POSIX",
+        "Operating System :: Unix",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3 :: Only",
+        "Topic :: Internet :: Log Analysis",
+        "Topic :: Utilities",
+        "Topic :: System :: Networking :: Monitoring",
     ],
-    zip_safe = False,
-    packages = ['bernhard'],
-    include_package_data = True,
-    install_requires=['python3-protobuf >= 2.4']
+    zip_safe=False,
+    packages=["bernhard"],
+    include_package_data=True,
+    install_requires=["python3-protobuf >= 2.4"],
 )
```

### Comparing `bernhard-py3-1.0/bernhard/pb.py` & `bernhard-py3-1.0.1/bernhard/pb.py`

 * *Files identical despite different names*

### Comparing `bernhard-py3-1.0/bernhard/__init__.py` & `bernhard-py3-1.0.1/bernhard/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
         TCPTransport.__init__(self, host, port)
 
         self.sock = ssl.wrap_socket(self.sock,
                                     keyfile=keyfile,
                                     certfile=certfile,
                                     cert_reqs=ssl.CERT_REQUIRED,
-                                    ssl_version=ssl.PROTOCOL_TLSv1,
+                                    ssl_version=ssl.PROTOCOL_TLS,
                                     ca_certs=ca_certs)
 
 
 class UDPTransport(object):
     def __init__(self, host, port):
         log.debug("Using UDP Transport")
```

### Comparing `bernhard-py3-1.0/LICENSE` & `bernhard-py3-1.0.1/LICENSE`

 * *Files identical despite different names*


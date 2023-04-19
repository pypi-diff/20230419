# Comparing `tmp/resend-0.1.0.tar.gz` & `tmp/resend-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/resend-0.1.0.tar", last modified: Tue Jan 17 03:14:55 2023, max compression
+gzip compressed data, was "dist/resend-0.1.1.tar", last modified: Wed Apr 19 01:41:15 2023, max compression
```

## Comparing `resend-0.1.0.tar` & `resend-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-01-17 03:14:55.000000 resend-0.1.0/
--rw-r--r--   0 derich     (501) staff       (20)     2414 2023-01-17 03:14:55.000000 resend-0.1.0/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)     1253 2023-01-16 19:07:03.000000 resend-0.1.0/README.md
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-01-17 03:14:55.000000 resend-0.1.0/resend/
--rw-r--r--   0 derich     (501) staff       (20)       94 2023-01-16 19:05:17.000000 resend-0.1.0/resend/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)     2209 2023-01-16 19:05:30.000000 resend-0.1.0/resend/api.py
--rw-r--r--   0 derich     (501) staff       (20)     3386 2023-01-16 19:08:15.000000 resend-0.1.0/resend/exceptions.py
--rw-r--r--   0 derich     (501) staff       (20)      163 2022-12-09 00:47:56.000000 resend-0.1.0/resend/version.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-01-17 03:14:55.000000 resend-0.1.0/resend.egg-info/
--rw-r--r--   0 derich     (501) staff       (20)     2414 2023-01-17 03:14:55.000000 resend-0.1.0/resend.egg-info/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)      278 2023-01-17 03:14:55.000000 resend-0.1.0/resend.egg-info/SOURCES.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2023-01-17 03:14:55.000000 resend-0.1.0/resend.egg-info/dependency_links.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2023-01-17 03:14:55.000000 resend-0.1.0/resend.egg-info/not-zip-safe
--rw-r--r--   0 derich     (501) staff       (20)        9 2023-01-17 03:14:55.000000 resend-0.1.0/resend.egg-info/requires.txt
--rw-r--r--   0 derich     (501) staff       (20)        7 2023-01-17 03:14:55.000000 resend-0.1.0/resend.egg-info/top_level.txt
--rw-r--r--   0 derich     (501) staff       (20)       67 2023-01-17 03:14:55.000000 resend-0.1.0/setup.cfg
--rw-r--r--   0 derich     (501) staff       (20)     1151 2023-01-16 19:07:15.000000 resend-0.1.0/setup.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-04-19 01:41:15.000000 resend-0.1.1/
+-rw-r--r--   0 derich     (501) staff       (20)     1070 2022-12-09 00:15:03.000000 resend-0.1.1/LICENSE.md
+-rw-r--r--   0 derich     (501) staff       (20)     2383 2023-04-19 01:41:15.000000 resend-0.1.1/PKG-INFO
+-rw-r--r--   0 derich     (501) staff       (20)     1263 2023-04-19 01:08:50.000000 resend-0.1.1/README.md
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-04-19 01:41:15.000000 resend-0.1.1/resend/
+-rw-r--r--   0 derich     (501) staff       (20)       94 2023-04-19 00:43:26.000000 resend-0.1.1/resend/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)     2209 2023-04-19 00:43:26.000000 resend-0.1.1/resend/api.py
+-rw-r--r--   0 derich     (501) staff       (20)     3385 2023-04-19 01:11:35.000000 resend-0.1.1/resend/exceptions.py
+-rw-r--r--   0 derich     (501) staff       (20)      163 2023-04-19 01:14:46.000000 resend-0.1.1/resend/version.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2023-04-19 01:41:15.000000 resend-0.1.1/resend.egg-info/
+-rw-r--r--   0 derich     (501) staff       (20)     2383 2023-04-19 01:41:15.000000 resend-0.1.1/resend.egg-info/PKG-INFO
+-rw-r--r--   0 derich     (501) staff       (20)      289 2023-04-19 01:41:15.000000 resend-0.1.1/resend.egg-info/SOURCES.txt
+-rw-r--r--   0 derich     (501) staff       (20)        1 2023-04-19 01:41:15.000000 resend-0.1.1/resend.egg-info/dependency_links.txt
+-rw-r--r--   0 derich     (501) staff       (20)        1 2023-04-19 01:30:00.000000 resend-0.1.1/resend.egg-info/not-zip-safe
+-rw-r--r--   0 derich     (501) staff       (20)       17 2023-04-19 01:41:15.000000 resend-0.1.1/resend.egg-info/requires.txt
+-rw-r--r--   0 derich     (501) staff       (20)        7 2023-04-19 01:41:15.000000 resend-0.1.1/resend.egg-info/top_level.txt
+-rw-r--r--   0 derich     (501) staff       (20)       67 2023-04-19 01:41:15.000000 resend-0.1.1/setup.cfg
+-rw-r--r--   0 derich     (501) staff       (20)     1103 2023-04-19 01:26:20.000000 resend-0.1.1/setup.py
```

### Comparing `resend-0.1.0/PKG-INFO` & `resend-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 0.1.0
+Version: 0.1.1
 Summary: Resend Python SDK
 Home-page: https://github.com/drish/resend-py
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 License: UNKNOWN
 Description: # Resend Python SDK
         
@@ -33,14 +33,15 @@
         
         client = Resend(api_key="kl_123")
         ```
         
         ## Example
         
         ```py
+        import os
         from resend import Resend
         
         client = Resend(api_key=os.environ["RESEND_API_KEY"])
         
         client.send_email(
             to="to@email.com",
             sender="from@email.com",
@@ -55,14 +56,13 @@
 Keywords: email,email platform
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >3.7.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `resend-0.1.0/README.md` & `resend-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 client = Resend(api_key="kl_123")
 ```
 
 ## Example
 
 ```py
+import os
 from resend import Resend
 
 client = Resend(api_key=os.environ["RESEND_API_KEY"])
 
 client.send_email(
     to="to@email.com",
     sender="from@email.com",
```

### Comparing `resend-0.1.0/resend/api.py` & `resend-0.1.1/resend/api.py`

 * *Files identical despite different names*

### Comparing `resend-0.1.0/resend/exceptions.py` & `resend-0.1.1/resend/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,14 @@
     "422": {"missing_required_fields": MissingRequiredFieldsError},
     "401": {"missing_api_key": MissingApiKeyError},
     "403": {"invalid_api_key": InvalidApiKeyError},
 }
 
 
 def raise_for_code_and_type(code, error_type, message: str) -> ResendError:
-
     # Handle the case where the error might be unknown
     if ERRORS.get(code).get(error_type) is None:
         raise ResendError()
 
     # Raise error from errors list
     error: ResendError = ERRORS.get(code).get(error_type)
     raise error(code=code, message=message, error_type=error_type)
```

### Comparing `resend-0.1.0/resend.egg-info/PKG-INFO` & `resend-0.1.1/resend.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 0.1.0
+Version: 0.1.1
 Summary: Resend Python SDK
 Home-page: https://github.com/drish/resend-py
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 License: UNKNOWN
 Description: # Resend Python SDK
         
@@ -33,14 +33,15 @@
         
         client = Resend(api_key="kl_123")
         ```
         
         ## Example
         
         ```py
+        import os
         from resend import Resend
         
         client = Resend(api_key=os.environ["RESEND_API_KEY"])
         
         client.send_email(
             to="to@email.com",
             sender="from@email.com",
@@ -55,14 +56,13 @@
 Keywords: email,email platform
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >3.7.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `resend-0.1.0/setup.py` & `resend-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,22 +15,21 @@
     author="Derich Pacheco",
     author_email="carlosderich@gmail.com",
     url="https://github.com/drish/resend-py",
     packages=["resend"],
     include_package_data=True,
     install_requires=install_requires,
     zip_safe=False,
-    python_requires=">3.7.5",
+    python_requires=">=3.7",
     keywords=["email", "email platform"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
 )
```


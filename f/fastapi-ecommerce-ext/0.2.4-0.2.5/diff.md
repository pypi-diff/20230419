# Comparing `tmp/fastapi_ecommerce_ext-0.2.4.tar.gz` & `tmp/fastapi_ecommerce_ext-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_ecommerce_ext-0.2.4.tar", last modified: Wed Apr 19 15:53:09 2023, max compression
+gzip compressed data, was "fastapi_ecommerce_ext-0.2.5.tar", last modified: Wed Apr 19 15:54:28 2023, max compression
```

## Comparing `fastapi_ecommerce_ext-0.2.4.tar` & `fastapi_ecommerce_ext-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 15:53:09.295595 fastapi_ecommerce_ext-0.2.4/
--rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.2.4/LICENSE.txt
--rw-rw-rw-   0        0        0      383 2023-04-19 15:53:09.295595 fastapi_ecommerce_ext-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 15:53:09.283595 fastapi_ecommerce_ext-0.2.4/fastapi_ecommerce_ext/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:53:09.294596 fastapi_ecommerce_ext-0.2.4/fastapi_ecommerce_ext/logger/
--rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.2.4/fastapi_ecommerce_ext/logger/__init__.py
--rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi_ecommerce_ext-0.2.4/fastapi_ecommerce_ext/logger/configure.py
--rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi_ecommerce_ext-0.2.4/fastapi_ecommerce_ext/logger/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:53:09.292593 fastapi_ecommerce_ext-0.2.4/fastapi_ecommerce_ext.egg-info/
--rw-rw-rw-   0        0        0      383 2023-04-19 15:53:09.000000 fastapi_ecommerce_ext-0.2.4/fastapi_ecommerce_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-04-19 15:53:09.000000 fastapi_ecommerce_ext-0.2.4/fastapi_ecommerce_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 15:53:09.000000 fastapi_ecommerce_ext-0.2.4/fastapi_ecommerce_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-19 15:53:09.000000 fastapi_ecommerce_ext-0.2.4/fastapi_ecommerce_ext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-19 15:53:09.000000 fastapi_ecommerce_ext-0.2.4/fastapi_ecommerce_ext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      142 2023-04-19 15:53:09.296594 fastapi_ecommerce_ext-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1124 2023-04-19 15:53:08.000000 fastapi_ecommerce_ext-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:54:28.324943 fastapi_ecommerce_ext-0.2.5/
+-rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      383 2023-04-19 15:54:28.325944 fastapi_ecommerce_ext-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 15:54:28.313946 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext/
+drwxrwxrwx   0        0        0        0 2023-04-19 15:54:28.324943 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext/logger/
+-rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext/logger/__init__.py
+-rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext/logger/configure.py
+-rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext/logger/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:54:28.322944 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext.egg-info/
+-rw-rw-rw-   0        0        0      383 2023-04-19 15:54:28.000000 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-04-19 15:54:28.000000 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 15:54:28.000000 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-19 15:54:28.000000 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-19 15:54:28.000000 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      142 2023-04-19 15:54:28.326451 fastapi_ecommerce_ext-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1170 2023-04-19 15:54:27.000000 fastapi_ecommerce_ext-0.2.5/setup.py
```

### Comparing `fastapi_ecommerce_ext-0.2.4/LICENSE.txt` & `fastapi_ecommerce_ext-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.2.4/fastapi_ecommerce_ext/logger/configure.py` & `fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext/logger/configure.py`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.2.4/fastapi_ecommerce_ext/logger/middleware.py` & `fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext/logger/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.2.4/setup.py` & `fastapi_ecommerce_ext-0.2.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,24 +10,29 @@
         from pip._internal.download import PipSession  # noqa
         from pip._internal.req import parse_requirements  # noqa
     except ImportError:
         # pip <= 9.0.3
         from pip.download import PipSession  # noqa
         from pip.req import parse_requirements  # noqa
 
-version = 'v0.2.4'
-package_name = 'fastapi_ecommerce_ext'
-url = f'https://github.com/coolworld2049/fastapi-ecommerce/pypi/{package_name}'
+version = "v0.2.5"
+package_name = "fastapi_ecommerce_ext"
+url = f"https://github.com/coolworld2049/fastapi-ecommerce/pypi/{package_name}"
 
-install_requires = [str(x.requirement) for x in parse_requirements("requirements.txt", PipSession())]
+install_requires = [
+    str(x.requirement)
+    for x in parse_requirements(
+        f"{package_name}/requirements.txt", PipSession()
+    )
+]
 print(install_requires)
 setup(
     name=package_name,
     version=version,
-    packages=['fastapi_ecommerce_ext.logger'],
+    packages=["fastapi_ecommerce_ext.logger"],
     install_requires=install_requires,
     url=url,
-    download_url=f'{url}-{version}.tar.gz',
-    license='MIT',
-    author='coolworld2049',
-    description='logging extension for fastapi-microservices'
+    download_url=f"{url}-{version}.tar.gz",
+    license="MIT",
+    author="coolworld2049",
+    description="logging extension for fastapi-microservices",
 )
```


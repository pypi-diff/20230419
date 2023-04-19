# Comparing `tmp/hspylib-vault-0.9.81.tar.gz` & `tmp/hspylib-vault-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-vault-0.9.81.tar", last modified: Wed Apr 19 19:05:55 2023, max compression
+gzip compressed data, was "hspylib-vault-0.9.9.tar", last modified: Tue Feb 22 20:01:27 2022, max compression
```

## Comparing `hspylib-vault-0.9.81.tar` & `hspylib-vault-0.9.9.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:55.454501 hspylib-vault-0.9.81/
--rw-r--r--   0 hjunior    (504) staff       (20)       96 2022-06-17 15:16:57.000000 hspylib-vault-0.9.81/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1543 2023-04-19 19:05:55.453829 hspylib-vault-0.9.81/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      675 2023-04-19 19:05:54.000000 hspylib-vault-0.9.81/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:55.429048 hspylib-vault-0.9.81/hspylib_vault.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1543 2023-04-19 19:05:55.000000 hspylib-vault-0.9.81/hspylib_vault.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      585 2023-04-19 19:05:55.000000 hspylib-vault-0.9.81/hspylib_vault.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-04-19 19:05:55.000000 hspylib-vault-0.9.81/hspylib_vault.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       73 2023-04-19 19:05:55.000000 hspylib-vault-0.9.81/hspylib_vault.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-04-19 19:05:55.000000 hspylib-vault-0.9.81/hspylib_vault.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-04-19 19:05:55.454642 hspylib-vault-0.9.81/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     1855 2023-04-05 21:45:26.000000 hspylib-vault-0.9.81/setup.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:55.435317 hspylib-vault-0.9.81/vault/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-04-19 19:05:54.000000 hspylib-vault-0.9.81/vault/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      716 2022-12-23 00:36:17.000000 hspylib-vault-0.9.81/vault/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      215 2023-04-19 19:05:54.000000 hspylib-vault-0.9.81/vault/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5147 2023-04-18 23:04:17.000000 hspylib-vault-0.9.81/vault/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:55.443631 hspylib-vault-0.9.81/vault/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      219 2023-04-19 19:05:54.000000 hspylib-vault-0.9.81/vault/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)    13133 2023-04-18 23:04:16.000000 hspylib-vault-0.9.81/vault/core/vault.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1400 2023-03-06 16:46:30.000000 hspylib-vault-0.9.81/vault/core/vault_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1809 2023-04-18 23:04:17.000000 hspylib-vault-0.9.81/vault/core/vault_repository.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2373 2023-04-18 23:04:16.000000 hspylib-vault-0.9.81/vault/core/vault_service.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:55.447614 hspylib-vault-0.9.81/vault/domain/
--rw-r--r--   0 hjunior    (504) staff       (20)      165 2023-04-19 19:05:54.000000 hspylib-vault-0.9.81/vault/domain/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3474 2023-04-18 23:04:16.000000 hspylib-vault-0.9.81/vault/domain/vault_entry.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:55.451289 hspylib-vault-0.9.81/vault/exception/
--rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-04-19 19:05:54.000000 hspylib-vault-0.9.81/vault/exception/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      839 2022-12-22 23:18:22.000000 hspylib-vault-0.9.81/vault/exception/exceptions.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:05:55.452799 hspylib-vault-0.9.81/vault/resources/
--rw-r--r--   0 hjunior    (504) staff       (20)       69 2022-11-12 19:14:13.000000 hspylib-vault-0.9.81/vault/resources/application.properties
--rw-r--r--   0 hjunior    (504) staff       (20)      168 2022-02-18 20:29:20.000000 hspylib-vault-0.9.81/vault/welcome.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.651843 hspylib-vault-0.9.9/
+-rw-r--r--   0 hjunior    (504) staff       (20)      125 2022-02-18 20:26:39.000000 hspylib-vault-0.9.9/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)      662 2022-02-22 20:01:27.650723 hspylib-vault-0.9.9/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)       41 2022-02-13 18:46:58.000000 hspylib-vault-0.9.9/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.604944 hspylib-vault-0.9.9/hspylib_vault.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)      662 2022-02-22 20:01:27.000000 hspylib-vault-0.9.9/hspylib_vault.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      704 2022-02-22 20:01:27.000000 hspylib-vault-0.9.9/hspylib_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2022-02-22 20:01:27.000000 hspylib-vault-0.9.9/hspylib_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       57 2022-02-22 20:01:27.000000 hspylib-vault-0.9.9/hspylib_vault.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2022-02-22 20:01:27.000000 hspylib-vault-0.9.9/hspylib_vault.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2022-02-22 20:01:27.651948 hspylib-vault-0.9.9/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     1557 2022-02-15 20:32:21.000000 hspylib-vault-0.9.9/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.615812 hspylib-vault-0.9.9/vault/
+-rw-r--r--   0 hjunior    (504) staff       (20)        5 2022-02-22 20:01:25.000000 hspylib-vault-0.9.9/vault/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      193 2022-02-22 19:09:15.000000 hspylib-vault-0.9.9/vault/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4384 2022-02-18 21:07:53.000000 hspylib-vault-0.9.9/vault/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.624864 hspylib-vault-0.9.9/vault/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      217 2022-02-22 19:09:15.000000 hspylib-vault-0.9.9/vault/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     8712 2022-02-22 08:50:25.000000 hspylib-vault-0.9.9/vault/core/vault.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1315 2022-02-15 20:32:21.000000 hspylib-vault-0.9.9/vault/core/vault_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2160 2022-02-22 08:50:25.000000 hspylib-vault-0.9.9/vault/core/vault_repository.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1089 2022-02-22 08:50:25.000000 hspylib-vault-0.9.9/vault/core/vault_service.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.628367 hspylib-vault-0.9.9/vault/entity/
+-rw-r--r--   0 hjunior    (504) staff       (20)      179 2022-02-22 19:09:15.000000 hspylib-vault-0.9.9/vault/entity/__init__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.631698 hspylib-vault-0.9.9/vault/entity/validator/
+-rw-r--r--   0 hjunior    (504) staff       (20)      177 2022-02-22 19:09:15.000000 hspylib-vault-0.9.9/vault/entity/validator/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2231 2022-02-22 08:50:25.000000 hspylib-vault-0.9.9/vault/entity/validator/entry_validator.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2128 2022-02-15 20:32:21.000000 hspylib-vault-0.9.9/vault/entity/vault_entry.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.634841 hspylib-vault-0.9.9/vault/exception/
+-rw-r--r--   0 hjunior    (504) staff       (20)      165 2022-02-22 19:09:15.000000 hspylib-vault-0.9.9/vault/exception/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      627 2022-02-11 19:26:38.000000 hspylib-vault-0.9.9/vault/exception/exceptions.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.642361 hspylib-vault-0.9.9/vault/resources/
+-rw-r--r--   0 hjunior    (504) staff       (20)       69 2022-02-15 20:32:21.000000 hspylib-vault-0.9.9/vault/resources/application.properties
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 20:01:27.649219 hspylib-vault-0.9.9/vault/resources/log/
+-rw-r--r--   0 hjunior    (504) staff       (20)        0 2022-02-02 16:37:07.000000 hspylib-vault-0.9.9/vault/resources/log/.gitkeep
+-rw-r--r--   0 hjunior    (504) staff       (20)     2572 2022-02-21 23:29:30.000000 hspylib-vault-0.9.9/vault/resources/log/application.log
+-rw-r--r--   0 hjunior    (504) staff       (20)      168 2022-02-18 20:29:20.000000 hspylib-vault-0.9.9/vault/welcome.txt
```

### Comparing `hspylib-vault-0.9.81/hspylib_vault.egg-info/SOURCES.txt` & `hspylib-vault-0.9.9/hspylib_vault.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 setup.py
 hspylib_vault.egg-info/PKG-INFO
 hspylib_vault.egg-info/SOURCES.txt
 hspylib_vault.egg-info/dependency_links.txt
 hspylib_vault.egg-info/requires.txt
 hspylib_vault.egg-info/top_level.txt
 vault/.version
-vault/__classpath__.py
 vault/__init__.py
 vault/__main__.py
 vault/welcome.txt
 vault/core/__init__.py
 vault/core/vault.py
 vault/core/vault_config.py
 vault/core/vault_repository.py
 vault/core/vault_service.py
-vault/domain/__init__.py
-vault/domain/vault_entry.py
+vault/entity/__init__.py
+vault/entity/vault_entry.py
+vault/entity/validator/__init__.py
+vault/entity/validator/entry_validator.py
 vault/exception/__init__.py
 vault/exception/exceptions.py
-vault/resources/application.properties
+vault/resources/application.properties
+vault/resources/log/.gitkeep
+vault/resources/log/application.log
```

### Comparing `hspylib-vault-0.9.81/setup.py` & `hspylib-vault-0.9.9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,56 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib-Vault
+   TODO Purpose of the file
+   @project: HSPyLib
       @file: setup.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2021, HSPyLib team
 """
 
 import pathlib
 
 import setuptools
 
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # The version of the package
-VERSION = (HERE / "vault/.version").read_text().strip()
+VERSION = (HERE / "vault/.version").read_text()
 
 # The package requirements
 REQUIREMENTS = list(filter(None, (HERE / "requirements.txt").read_text().splitlines()))
 
 # This call to setup() does all the work
 setuptools.setup(
-    name="hspylib-vault",
+    name='hspylib-vault',
     version=VERSION,
-    description="HSPyLib - Secrets Vault",
-    author="Hugo Saporetti Junior",
-    author_email="yorevs@hotmail.com",
+    description='HomeSetup vault',
+    author='Hugo Saporetti Junior',
+    author_email='yorevs@hotmail.com',
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/yorevs/hspylib",
-    project_urls={"GitHub": "https://github.com/yorevs/hspylib", "PyPi": "https://pypi.org/project/hspylib-vault/"},
-    license="MIT",
-    license_files="LICENSE.md",
-    packages=setuptools.find_namespace_packages(),
+    license='MIT',
+    packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
-        "Operating System :: Unix",
-        "Development Status :: 3 - Alpha",
-        "Environment :: Console",
-        "Natural Language :: English",
-        "Topic :: Terminals",
+        "Operating System :: Unix"
+
     ],
-    python_requires=">=3.10",
+    python_requires='>=3.7',
     install_requires=REQUIREMENTS,
-    keywords="secrets,passwords,safe,vault,manager,application",
-    platforms="Darwin,Linux",
 )
```

### Comparing `hspylib-vault-0.9.81/vault/exception/exceptions.py` & `hspylib-vault-0.9.9/vault/exception/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib-Vault
-   @package: vault.exception
+   TODO Purpose of the file
+   @project: HSPyLib
+   hspylib.app.vault.exception
       @file: exceptions.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2021, HSPyLib team
 """
 from hspylib.core.exception.exceptions import HSBaseException
 
 
 class VaultCloseError(HSBaseException):
     """Raised when closing the vault"""
 
 
 class VaultOpenError(HSBaseException):
     """Raised when opening the vault"""
-
-
-class VaultSecurityException(HSBaseException):
-    """Raised when something unexpected happened to vault file"""
-
-
-class VaultExecutionException(HSBaseException):
-    """Raised when something unexpected happened to vault execution"""
```


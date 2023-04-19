# Comparing `tmp/Musicreater-0.3.2.tar.gz` & `tmp/Musicreater-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Musicreater-0.3.2.tar", last modified: Sun Feb 12 09:38:13 2023, max compression
+gzip compressed data, was "Musicreater-0.4.0.tar", last modified: Wed Apr 19 13:14:24 2023, max compression
```

## Comparing `Musicreater-0.3.2.tar` & `Musicreater-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 09:38:13.847583 Musicreater-0.3.2/
--rw-rw-rw-   0        0        0    13085 2023-02-12 08:13:49.000000 Musicreater-0.3.2/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-02-12 09:38:13.839576 Musicreater-0.3.2/Musicreater/
--rw-rw-rw-   0        0        0      899 2023-02-12 09:37:40.000000 Musicreater-0.3.2/Musicreater/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-02-12 08:13:49.000000 Musicreater-0.3.2/Musicreater/exceptions.py
--rw-rw-rw-   0        0        0     4847 2023-02-12 08:13:49.000000 Musicreater-0.3.2/Musicreater/instConstants.py
--rw-rw-rw-   0        0        0     7611 2023-02-12 08:13:49.000000 Musicreater-0.3.2/Musicreater/magicmain.py
--rw-rw-rw-   0        0        0    67997 2023-02-12 09:37:40.000000 Musicreater-0.3.2/Musicreater/main.py
--rw-rw-rw-   0        0        0     6643 2023-02-12 08:13:49.000000 Musicreater-0.3.2/Musicreater/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-12 09:38:13.844584 Musicreater-0.3.2/Musicreater.egg-info/
--rw-rw-rw-   0        0        0     6321 2023-02-12 09:38:13.000000 Musicreater-0.3.2/Musicreater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-02-12 09:38:13.000000 Musicreater-0.3.2/Musicreater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-12 09:38:13.000000 Musicreater-0.3.2/Musicreater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-02-12 09:38:13.000000 Musicreater-0.3.2/Musicreater.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-12 09:38:13.000000 Musicreater-0.3.2/Musicreater.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6321 2023-02-12 09:38:13.845577 Musicreater-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     5252 2023-02-12 08:13:49.000000 Musicreater-0.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-02-12 09:38:13.847583 Musicreater-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1533 2023-02-12 08:24:01.000000 Musicreater-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 13:14:24.544093 Musicreater-0.4.0/
+-rw-rw-rw-   0        0        0    13085 2023-02-12 08:13:49.000000 Musicreater-0.4.0/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-04-19 13:14:24.530093 Musicreater-0.4.0/Musicreater/
+-rw-rw-rw-   0        0        0      899 2023-04-19 13:14:14.000000 Musicreater-0.4.0/Musicreater/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-02-12 08:13:49.000000 Musicreater-0.4.0/Musicreater/exceptions.py
+-rw-rw-rw-   0        0        0     4847 2023-02-12 08:13:49.000000 Musicreater-0.4.0/Musicreater/instConstants.py
+-rw-rw-rw-   0        0        0     7611 2023-02-12 08:13:49.000000 Musicreater-0.4.0/Musicreater/magicmain.py
+-rw-rw-rw-   0        0        0    67997 2023-02-12 09:37:40.000000 Musicreater-0.4.0/Musicreater/main.py
+-rw-rw-rw-   0        0        0     6643 2023-02-12 08:13:49.000000 Musicreater-0.4.0/Musicreater/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 13:14:24.541094 Musicreater-0.4.0/Musicreater.egg-info/
+-rw-rw-rw-   0        0        0     6321 2023-04-19 13:14:23.000000 Musicreater-0.4.0/Musicreater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-19 13:14:24.000000 Musicreater-0.4.0/Musicreater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 13:14:23.000000 Musicreater-0.4.0/Musicreater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-19 13:14:23.000000 Musicreater-0.4.0/Musicreater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-19 13:14:23.000000 Musicreater-0.4.0/Musicreater.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6321 2023-04-19 13:14:24.543094 Musicreater-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5252 2023-02-12 08:13:49.000000 Musicreater-0.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 13:14:24.545093 Musicreater-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1533 2023-02-12 08:24:01.000000 Musicreater-0.4.0/setup.py
```

### Comparing `Musicreater-0.3.2/LICENSE.md` & `Musicreater-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Musicreater-0.3.2/Musicreater/__init__.py` & `Musicreater-0.4.0/Musicreater/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 # 音·创 开发交流群 861684859
 # Email EillesWan2006@163.com W-YI_DoctorYI@outlook.com EillesWan@outlook.com
 # 版权所有 金羿("Eilles Wan") & 诸葛亮与八卦阵("bgArray") & 鸣凤鸽子("MingFengPigeon")
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 from .main import *
 
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 __all__ = []
 __author__ = (("金羿", "Eilles Wan"), ("诸葛亮与八卦阵", "bgArray"))
```

### Comparing `Musicreater-0.3.2/Musicreater/exceptions.py` & `Musicreater-0.4.0/Musicreater/exceptions.py`

 * *Files identical despite different names*

### Comparing `Musicreater-0.3.2/Musicreater/instConstants.py` & `Musicreater-0.4.0/Musicreater/instConstants.py`

 * *Files identical despite different names*

### Comparing `Musicreater-0.3.2/Musicreater/magicmain.py` & `Musicreater-0.4.0/Musicreater/magicmain.py`

 * *Files identical despite different names*

### Comparing `Musicreater-0.3.2/Musicreater/main.py` & `Musicreater-0.4.0/Musicreater/main.py`

 * *Files identical despite different names*

### Comparing `Musicreater-0.3.2/Musicreater/utils.py` & `Musicreater-0.4.0/Musicreater/utils.py`

 * *Files identical despite different names*

### Comparing `Musicreater-0.3.2/Musicreater.egg-info/PKG-INFO` & `Musicreater-0.4.0/Musicreater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Musicreater
-Version: 0.3.2
+Version: 0.4.0
 Summary: 一款免费开源的 《我的世界》 mid音乐转换库。
 Home-page: https://github.com/TriM-Organization/Musicreater
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `Musicreater-0.3.2/PKG-INFO` & `Musicreater-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Musicreater
-Version: 0.3.2
+Version: 0.4.0
 Summary: 一款免费开源的 《我的世界》 mid音乐转换库。
 Home-page: https://github.com/TriM-Organization/Musicreater
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `Musicreater-0.3.2/README.md` & `Musicreater-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `Musicreater-0.3.2/setup.py` & `Musicreater-0.4.0/setup.py`

 * *Files identical despite different names*


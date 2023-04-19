# Comparing `tmp/jcmutils-1.3.6.tar.gz` & `tmp/jcmutils-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.3.6.tar", last modified: Wed Apr 19 06:58:17 2023, max compression
+gzip compressed data, was "jcmutils-1.3.7.tar", last modified: Wed Apr 19 07:20:45 2023, max compression
```

## Comparing `jcmutils-1.3.6.tar` & `jcmutils-1.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 06:58:17.125664 jcmutils-1.3.6/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.3.6/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-19 06:58:17.125664 jcmutils-1.3.6/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.3.6/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 06:58:17.125664 jcmutils-1.3.6/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.3.6/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2620 2023-04-19 06:57:08.000000 jcmutils-1.3.6/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.3.6/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.3.6/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8002 2023-04-19 01:54:58.000000 jcmutils-1.3.6/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 06:58:17.125664 jcmutils-1.3.6/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-19 06:58:17.000000 jcmutils-1.3.6/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-04-19 06:58:17.000000 jcmutils-1.3.6/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-04-19 06:58:17.000000 jcmutils-1.3.6/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       31 2023-04-19 06:58:17.000000 jcmutils-1.3.6/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-04-19 06:58:17.000000 jcmutils-1.3.6/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-04-19 06:58:17.125664 jcmutils-1.3.6/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      530 2023-04-19 06:56:55.000000 jcmutils-1.3.6/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 07:20:45.910784 jcmutils-1.3.7/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.3.7/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-19 07:20:45.910784 jcmutils-1.3.7/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.3.7/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 07:20:45.910784 jcmutils-1.3.7/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.3.7/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2613 2023-04-19 07:20:15.000000 jcmutils-1.3.7/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.3.7/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.3.7/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8002 2023-04-19 01:54:58.000000 jcmutils-1.3.7/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 07:20:45.910784 jcmutils-1.3.7/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-19 07:20:45.000000 jcmutils-1.3.7/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-04-19 07:20:45.000000 jcmutils-1.3.7/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-04-19 07:20:45.000000 jcmutils-1.3.7/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       31 2023-04-19 07:20:45.000000 jcmutils-1.3.7/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-04-19 07:20:45.000000 jcmutils-1.3.7/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-04-19 07:20:45.910784 jcmutils-1.3.7/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      530 2023-04-19 07:20:18.000000 jcmutils-1.3.7/setup.py
```

### Comparing `jcmutils-1.3.6/LICENSE` & `jcmutils-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.6/README.md` & `jcmutils-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.6/jcmutils/dataset_utils.py` & `jcmutils-1.3.7/jcmutils/dataset_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         vmaxa = np.max(total_results) if vmax is None else vmax
         afield = (total_results/ vmaxa)*235
         afield = np.rot90(afield)
 
         # 通过每个像素点代表的实际物理尺寸来计算缩放比比例
         scale_factor =source_density*1.0/target_density
         # 缩放电场/光强场到对应的大小
-        scaled_field = cv2.resize(total_results, None, fx=scale_factor,# type: ignore
+        scaled_field = cv2.resize(afield, None, fx=scale_factor,# type: ignore
                                   fy=scale_factor, interpolation=cv2.INTER_LINEAR)  
 
 
         # 绘图
         logger.debug(f"printing max value of results:{np.max(total_results)}")
         cv2.imwrite(target_filename,scaled_field)
         logger.info("all target image saved completed!")
```

### Comparing `jcmutils-1.3.6/jcmutils/gen_sources.py` & `jcmutils-1.3.7/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.6/jcmutils/logger.py` & `jcmutils-1.3.7/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.6/jcmutils/solver.py` & `jcmutils-1.3.7/jcmutils/solver.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.6/setup.py` & `jcmutils-1.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.3.6'
+VERSION = '1.3.7'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```


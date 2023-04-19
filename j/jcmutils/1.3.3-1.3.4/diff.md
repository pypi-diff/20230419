# Comparing `tmp/jcmutils-1.3.3.tar.gz` & `tmp/jcmutils-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.3.3.tar", last modified: Tue Apr 18 08:17:11 2023, max compression
+gzip compressed data, was "jcmutils-1.3.4.tar", last modified: Wed Apr 19 01:48:37 2023, max compression
```

## Comparing `jcmutils-1.3.3.tar` & `jcmutils-1.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-18 08:17:11.149205 jcmutils-1.3.3/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.3.3/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-18 08:17:11.149205 jcmutils-1.3.3/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.3.3/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-18 08:17:11.149205 jcmutils-1.3.3/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.3.3/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2677 2023-04-18 07:46:32.000000 jcmutils-1.3.3/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.3.3/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.3.3/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     7997 2023-04-18 08:15:38.000000 jcmutils-1.3.3/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-18 08:17:11.149205 jcmutils-1.3.3/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-18 08:17:11.000000 jcmutils-1.3.3/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-04-18 08:17:11.000000 jcmutils-1.3.3/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-04-18 08:17:11.000000 jcmutils-1.3.3/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       31 2023-04-18 08:17:11.000000 jcmutils-1.3.3/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-04-18 08:17:11.000000 jcmutils-1.3.3/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-04-18 08:17:11.149205 jcmutils-1.3.3/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      530 2023-04-18 08:16:50.000000 jcmutils-1.3.3/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 01:48:37.545003 jcmutils-1.3.4/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.3.4/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-19 01:48:37.545003 jcmutils-1.3.4/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.3.4/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 01:48:37.541003 jcmutils-1.3.4/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.3.4/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2677 2023-04-18 07:46:32.000000 jcmutils-1.3.4/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.3.4/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.3.4/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8002 2023-04-19 01:47:03.000000 jcmutils-1.3.4/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 01:48:37.545003 jcmutils-1.3.4/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-19 01:48:37.000000 jcmutils-1.3.4/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-04-19 01:48:37.000000 jcmutils-1.3.4/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-04-19 01:48:37.000000 jcmutils-1.3.4/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       31 2023-04-19 01:48:37.000000 jcmutils-1.3.4/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-04-19 01:48:37.000000 jcmutils-1.3.4/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-04-19 01:48:37.545003 jcmutils-1.3.4/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      530 2023-04-19 01:48:13.000000 jcmutils-1.3.4/setup.py
```

### Comparing `jcmutils-1.3.3/LICENSE` & `jcmutils-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.3/README.md` & `jcmutils-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.3/jcmutils/dataset_utils.py` & `jcmutils-1.3.4/jcmutils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.3/jcmutils/gen_sources.py` & `jcmutils-1.3.4/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.3/jcmutils/logger.py` & `jcmutils-1.3.4/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.3/jcmutils/solver.py` & `jcmutils-1.3.4/jcmutils/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,41 +131,43 @@
         field = (temp_result[num_of_result]['field'][0].conj() *
                  temp_result[num_of_result]['field'][0]).sum(axis=2).real
         total_results = np.zeros(field.shape)
         logger.debug(f"total_result shape defined as {total_results.shape}")
 
         # 开始逐个提取结果
         for key in self.keys:
+            # 目录检查
+            if not os.path.exists(target_directory):
+                logger.debug("target directory dosen't exist,creating...")
+                os.makedirs(target_directory)
+            file_name = target_directory.rstrip(
+                '/') + '/' + self.__solve_dict(key) + ".jpg"
+
+            # 获得结果
             result = self.resultbag.get_result(key)
             field = (result[num_of_result]['field'][0].conj() *
                      result[num_of_result]['field'][0]).sum(axis=2).real
             if is_light_intense:
                 field = np.power(field, 2)
-            total_results += field
 
-            if not os.path.exists(target_directory):
-                logger.debug("target directory dosen't exist,creating...")
-                os.makedirs(target_directory)
-            file_name = target_directory.rstrip(
-                '/') + '/' + self.__solve_dict(key) + ".jpg"
-            vmaxa = np.max(field) if vmax is None else vmax
             field = np.rot90(field)
-            save_field = (field / vmaxa)*255
+            save_field = (field / np.max(field))*255
             cv2.imwrite(file_name,save_field)
             logger.debug(f"key {key} successfully saved")
+            total_results += field
             if is_symmetry and not (key['thetaphi'][0] == 0 and key['thetaphi'][1] == 0):
                 field = np.rot90(field, 2)
                 total_results += field
                 logger.debug("key was rotated for symmetry")
 
         logger.debug(f"printing max value of results:{np.max(total_results)}")
         vmaxa = np.max(total_results) if vmax is None else vmax
-        field = (total_results/ vmaxa)*255
+        sfield = (total_results/ vmaxa)*255
         file_name = target_directory.rstrip('/') + '/' + "total_result.jpg"
-        cv2.imwrite(file_name,field)
+        cv2.imwrite(file_name,sfield)
         logger.info("all target image saved completed!")
 
     def __solve_dict(self, target_dict):
         res = ""
         for key, value in target_dict.items():
             res += key + "-"
             if isinstance(value, list):
```

### Comparing `jcmutils-1.3.3/setup.py` & `jcmutils-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.3.3'
+VERSION = '1.3.4'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```


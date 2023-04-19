# Comparing `tmp/jcmutils-1.3.4.tar.gz` & `tmp/jcmutils-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.3.4.tar", last modified: Wed Apr 19 01:48:37 2023, max compression
+gzip compressed data, was "jcmutils-1.3.5.tar", last modified: Wed Apr 19 03:10:58 2023, max compression
```

## Comparing `jcmutils-1.3.4.tar` & `jcmutils-1.3.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 01:48:37.545003 jcmutils-1.3.4/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.3.4/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-19 01:48:37.545003 jcmutils-1.3.4/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.3.4/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 01:48:37.541003 jcmutils-1.3.4/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.3.4/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2677 2023-04-18 07:46:32.000000 jcmutils-1.3.4/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.3.4/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.3.4/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8002 2023-04-19 01:47:03.000000 jcmutils-1.3.4/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 01:48:37.545003 jcmutils-1.3.4/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-19 01:48:37.000000 jcmutils-1.3.4/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-04-19 01:48:37.000000 jcmutils-1.3.4/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-04-19 01:48:37.000000 jcmutils-1.3.4/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       31 2023-04-19 01:48:37.000000 jcmutils-1.3.4/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-04-19 01:48:37.000000 jcmutils-1.3.4/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-04-19 01:48:37.545003 jcmutils-1.3.4/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      530 2023-04-19 01:48:13.000000 jcmutils-1.3.4/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 03:10:58.554613 jcmutils-1.3.5/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.3.5/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-19 03:10:58.554613 jcmutils-1.3.5/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.3.5/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 03:10:58.554613 jcmutils-1.3.5/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.3.5/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2620 2023-04-19 03:09:36.000000 jcmutils-1.3.5/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.3.5/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.3.5/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8002 2023-04-19 01:54:58.000000 jcmutils-1.3.5/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 03:10:58.554613 jcmutils-1.3.5/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-19 03:10:58.000000 jcmutils-1.3.5/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-04-19 03:10:58.000000 jcmutils-1.3.5/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-04-19 03:10:58.000000 jcmutils-1.3.5/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       31 2023-04-19 03:10:58.000000 jcmutils-1.3.5/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-04-19 03:10:58.000000 jcmutils-1.3.5/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-04-19 03:10:58.554613 jcmutils-1.3.5/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      530 2023-04-19 03:10:06.000000 jcmutils-1.3.5/setup.py
```

### Comparing `jcmutils-1.3.4/LICENSE` & `jcmutils-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.4/README.md` & `jcmutils-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.4/jcmutils/dataset_utils.py` & `jcmutils-1.3.5/jcmutils/dataset_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,22 +39,22 @@
                 field = np.power(field, 2)
             total_results += field
             if is_symmetry and not (key['thetaphi'][0] == 0 and key['thetaphi'][1] == 0):
                 field = np.rot90(field, 2)
                 total_results += field
                 logger.debug("key was rotated for symmetry")
 
-        # 通过每个像素点代表的实际物理尺寸来计算缩放比比例
-        scale_factor = source_density*1.0/target_density
         vmaxa = np.max(total_results) if vmax is None else vmax
-        field = (total_results/ vmaxa)*255
-        field = np.rot90(field)
+        afield = (total_results/ vmaxa)*235
+        afield = np.rot90(afield)
 
+        # 通过每个像素点代表的实际物理尺寸来计算缩放比比例
+        scale_factor =target_density*1.0/source_density
         # 缩放电场/光强场到对应的大小
-        scaled_field = cv2.resize(field, None, fx=scale_factor,# type: ignore
+        scaled_field = cv2.resize(total_results, None, fx=scale_factor,# type: ignore
                                   fy=scale_factor, interpolation=cv2.INTER_LINEAR)  
 
+
         # 绘图
         logger.debug(f"printing max value of results:{np.max(total_results)}")
-        file_name =target_filename.rstrip('/') + '/' + "total_result.jpg"
-        cv2.imwrite(file_name,scaled_field)
+        cv2.imwrite(target_filename,scaled_field)
         logger.info("all target image saved completed!")
```

### Comparing `jcmutils-1.3.4/jcmutils/gen_sources.py` & `jcmutils-1.3.5/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.4/jcmutils/logger.py` & `jcmutils-1.3.5/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.4/jcmutils/solver.py` & `jcmutils-1.3.5/jcmutils/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         # 开始提取
         result = self.resultbag.get_result(key)
         field = (result[num_of_result]['field'][0].conj() *
                  result[num_of_result]['field'][0]).sum(axis=2).real
         if is_light_intense:
             field = np.power(field, 2)
         vmaxa = np.max(field) if vmax is None else vmax
-        field = (field / vmaxa)*255
+        field = (field / vmaxa)*235
         field = np.rot90(field)
         cv2.imshow("image",field)
 
     def get_result(self, key):
         return self.resultbag.get_result(key)
 
     def save_image(self, target_directory, key, num_of_result, is_light_intense=False,vmax=None):
@@ -111,15 +111,15 @@
                  result[num_of_result]['field'][0]).sum(axis=2).real
         if is_light_intense:
             field = np.power(field, 2)
         if not os.path.exists(target_directory):
             logger.debug("target directory dosen't exist,creating...")
             os.makedirs(target_directory)
         vmaxa = np.max(field) if vmax is None else vmax
-        field = (field / vmaxa)*255
+        field = (field / vmaxa)*235
         field = np.rot90(field)
         cv2.imwrite(target_directory.rstrip("/")+"output.jpg",field)
 
     def save_all_image(self, num_of_result, target_directory, is_light_intense=False, is_symmetry=False,vmax=None):
         if not self.resultbag.check_result(self.keys[0]):
             logger.error("get result failed! target key not find")
             logger.error(f"the key is : {self.keys[0]}")
@@ -146,26 +146,26 @@
             result = self.resultbag.get_result(key)
             field = (result[num_of_result]['field'][0].conj() *
                      result[num_of_result]['field'][0]).sum(axis=2).real
             if is_light_intense:
                 field = np.power(field, 2)
 
             field = np.rot90(field)
-            save_field = (field / np.max(field))*255
+            save_field = (field / np.max(field))*235
             cv2.imwrite(file_name,save_field)
             logger.debug(f"key {key} successfully saved")
             total_results += field
             if is_symmetry and not (key['thetaphi'][0] == 0 and key['thetaphi'][1] == 0):
                 field = np.rot90(field, 2)
                 total_results += field
                 logger.debug("key was rotated for symmetry")
 
         logger.debug(f"printing max value of results:{np.max(total_results)}")
         vmaxa = np.max(total_results) if vmax is None else vmax
-        sfield = (total_results/ vmaxa)*255
+        sfield = (total_results/ vmaxa)*235
         file_name = target_directory.rstrip('/') + '/' + "total_result.jpg"
         cv2.imwrite(file_name,sfield)
         logger.info("all target image saved completed!")
 
     def __solve_dict(self, target_dict):
         res = ""
         for key, value in target_dict.items():
```

### Comparing `jcmutils-1.3.4/setup.py` & `jcmutils-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.3.4'
+VERSION = '1.3.5'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```


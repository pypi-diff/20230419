# Comparing `tmp/easierfile-1.0.1.tar.gz` & `tmp/easierfile-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easierfile-1.0.1.tar", max compression
+gzip compressed data, was "easierfile-1.1.0.tar", max compression
```

## Comparing `easierfile-1.0.1.tar` & `easierfile-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       32 2023-04-10 13:57:24.548112 easierfile-1.0.1/easierfile/__init__.py
--rw-r--r--   0        0        0     1171 2023-04-11 04:45:40.722039 easierfile-1.0.1/easierfile/file.py
--rw-r--r--   0        0        0     1092 2023-04-11 00:52:37.919987 easierfile-1.0.1/LICENSE
--rw-r--r--   0        0        0      556 2023-04-11 05:01:13.479904 easierfile-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      934 2023-04-11 01:32:23.623996 easierfile-1.0.1/README.md
--rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 easierfile-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       32 2023-04-10 13:57:24.548112 easierfile-1.1.0/easierfile/__init__.py
+-rw-r--r--   0        0        0     1700 2023-04-19 05:38:18.190568 easierfile-1.1.0/easierfile/file.py
+-rw-r--r--   0        0        0     1092 2023-04-11 00:52:37.919987 easierfile-1.1.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-04-19 04:54:06.663354 easierfile-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      934 2023-04-11 01:32:23.623996 easierfile-1.1.0/README.md
+-rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 easierfile-1.1.0/PKG-INFO
```

### Comparing `easierfile-1.0.1/easierfile/file.py` & `easierfile-1.1.0/easierfile/file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,50 @@
 import os
 
 class File:
-    def __init__(self, filePath):
-        self.__m_filePath = filePath
-        self.__m_dirPath = os.path.dirname(self.__m_filePath)
-        if os.path.exists(self.__m_dirPath) == False:  # If the directory of the file path does not exist, it will be created.
-            os.mkdir(self.__m_dirPath)
+    def __init__(self, file_path):
+        self.__m_file_path = file_path
+        self.__m_file_full_name = os.path.basename(self.__m_file_path)
+        self.__m_file_name, self.__m_file_extension = os.path.splitext(self.__m_file_full_name)
+        self.__m_dir_path = os.path.dirname(self.__m_file_path)
+
+        if os.path.exists(self.__m_dir_path) == False:  # If the directory of the file path does not exist, it will be created.
+            os.mkdir(self.__m_dir_path)
         try:  # If the file does not exist, it will be created.
-            self.__m_file = open(self.__m_filePath, "x")
-        except:
-            pass
+            self.__m_file = open(self.__m_file_path, "x")
+        except FileExistsError:
+            pass  # Indicates that the file exists and no further exception handling is required.
         else:
             self.__m_file.close()
 
     @property
     def content(self):
-        self.__m_file = open(self.__m_filePath, "r")
+        self.__m_file = open(self.__m_file_path, "r")
         self.__m_content = self.__m_file.read()
         self.__m_file.close()
         return self.__m_content
 
-    def Rewrite(self,content):
-        self.__m_file = open(self.__m_filePath, "w")
+    @property
+    def full_name(self):
+        return self.__m_file_full_name
+
+    @property
+    def name(self):
+        return self.__m_file_name
+
+    @property
+    def ext(self):
+        return self.__m_file_extension.split(".")[-1]
+
+    def rewrite(self,content):
+        self.__m_file = open(self.__m_file_path, "w")
         self.__m_file.write(content)
         self.__m_file.close()
 
-    def Append(self,content):
-        self.__m_file = open(self.__m_filePath, "a")
+    def append(self,content):
+        self.__m_file = open(self.__m_file_path, "a")
         self.__m_file.write(content)
         self.__m_file.close()
 
-    def Delete(self):
-        if os.path.exists(self.__m_filePath):
-            os.remove(self.__m_filePath)
+    def delete(self):
+        if os.path.exists(self.__m_file_path):
+            os.remove(self.__m_file_path)
```

### Comparing `easierfile-1.0.1/LICENSE` & `easierfile-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easierfile-1.0.1/pyproject.toml` & `easierfile-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easierfile"
-version = "1.0.1"
+version = "1.1.0"
 description = "A simple Python package that object-oriented encapsulates Python traditional built-in file operations."
 license = "MIT"
 authors = ["leoweyr <leoweyr@foxmail.com>"]
 readme = "README.md"
 repository = "https://github.com/leoweyr/Python-Easierfile"
 classifiers = [
     "Development Status :: 3 - Alpha"
```

### Comparing `easierfile-1.0.1/README.md` & `easierfile-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `easierfile-1.0.1/PKG-INFO` & `easierfile-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easierfile
-Version: 1.0.1
+Version: 1.1.0
 Summary: A simple Python package that object-oriented encapsulates Python traditional built-in file operations.
 Home-page: https://github.com/leoweyr/Python-Easierfile
 License: MIT
 Author: leoweyr
 Author-email: leoweyr@foxmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```


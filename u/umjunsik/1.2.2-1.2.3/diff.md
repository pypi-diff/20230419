# Comparing `tmp/umjunsik-1.2.2.tar.gz` & `tmp/umjunsik-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umjunsik-1.2.2.tar", last modified: Wed Apr 19 13:12:00 2023, max compression
+gzip compressed data, was "umjunsik-1.2.3.tar", last modified: Wed Apr 19 13:16:16 2023, max compression
```

## Comparing `umjunsik-1.2.2.tar` & `umjunsik-1.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 13:12:00.995867 umjunsik-1.2.2/
--rw-r--r--   0 hiyabye    (501) staff       (20)     1062 2023-04-18 14:04:33.000000 umjunsik-1.2.2/LICENSE
--rw-r--r--   0 hiyabye    (501) staff       (20)      643 2023-04-19 13:12:00.995924 umjunsik-1.2.2/PKG-INFO
--rw-r--r--   0 hiyabye    (501) staff       (20)    17050 2023-04-17 07:54:45.000000 umjunsik-1.2.2/README.md
--rw-r--r--   0 hiyabye    (501) staff       (20)      103 2023-04-19 13:12:00.996105 umjunsik-1.2.2/setup.cfg
--rw-r--r--   0 hiyabye    (501) staff       (20)      730 2023-04-19 13:11:20.000000 umjunsik-1.2.2/setup.py
-drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 13:12:00.995331 umjunsik-1.2.2/umjunsik/
--rw-r--r--   0 hiyabye    (501) staff       (20)     2928 2023-04-19 12:55:10.000000 umjunsik-1.2.2/umjunsik/runtime.py
-drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 13:12:00.995755 umjunsik-1.2.2/umjunsik.egg-info/
--rw-r--r--   0 hiyabye    (501) staff       (20)      643 2023-04-19 13:12:00.000000 umjunsik-1.2.2/umjunsik.egg-info/PKG-INFO
--rw-r--r--   0 hiyabye    (501) staff       (20)      184 2023-04-19 13:12:00.000000 umjunsik-1.2.2/umjunsik.egg-info/SOURCES.txt
--rw-r--r--   0 hiyabye    (501) staff       (20)        1 2023-04-19 13:12:00.000000 umjunsik-1.2.2/umjunsik.egg-info/dependency_links.txt
--rw-r--r--   0 hiyabye    (501) staff       (20)        9 2023-04-19 13:12:00.000000 umjunsik-1.2.2/umjunsik.egg-info/top_level.txt
+drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 13:16:16.534371 umjunsik-1.2.3/
+-rw-r--r--   0 hiyabye    (501) staff       (20)     1062 2023-04-18 14:04:33.000000 umjunsik-1.2.3/LICENSE
+-rw-r--r--   0 hiyabye    (501) staff       (20)      643 2023-04-19 13:16:16.534423 umjunsik-1.2.3/PKG-INFO
+-rw-r--r--   0 hiyabye    (501) staff       (20)    17050 2023-04-17 07:54:45.000000 umjunsik-1.2.3/README.md
+-rw-r--r--   0 hiyabye    (501) staff       (20)      103 2023-04-19 13:16:16.534596 umjunsik-1.2.3/setup.cfg
+-rw-r--r--   0 hiyabye    (501) staff       (20)      730 2023-04-19 13:15:39.000000 umjunsik-1.2.3/setup.py
+drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 13:16:16.533749 umjunsik-1.2.3/umjunsik/
+-rw-r--r--   0 hiyabye    (501) staff       (20)     3116 2023-04-19 13:15:29.000000 umjunsik-1.2.3/umjunsik/runtime.py
+drwxr-xr-x   0 hiyabye    (501) staff       (20)        0 2023-04-19 13:16:16.534262 umjunsik-1.2.3/umjunsik.egg-info/
+-rw-r--r--   0 hiyabye    (501) staff       (20)      643 2023-04-19 13:16:16.000000 umjunsik-1.2.3/umjunsik.egg-info/PKG-INFO
+-rw-r--r--   0 hiyabye    (501) staff       (20)      184 2023-04-19 13:16:16.000000 umjunsik-1.2.3/umjunsik.egg-info/SOURCES.txt
+-rw-r--r--   0 hiyabye    (501) staff       (20)        1 2023-04-19 13:16:16.000000 umjunsik-1.2.3/umjunsik.egg-info/dependency_links.txt
+-rw-r--r--   0 hiyabye    (501) staff       (20)        9 2023-04-19 13:16:16.000000 umjunsik-1.2.3/umjunsik.egg-info/top_level.txt
```

### Comparing `umjunsik-1.2.2/LICENSE` & `umjunsik-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `umjunsik-1.2.2/PKG-INFO` & `umjunsik-1.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umjunsik
-Version: 1.2.2
+Version: 1.2.3
 Summary: Umjunsik programming language
 Home-page: https://github.com/rycont/umjunsik-lang
 Author: rycont
 Author-email: rycont@outlook.kr
 License: MIT
 Keywords: ESOLANG
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `umjunsik-1.2.2/README.md` & `umjunsik-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `umjunsik-1.2.2/setup.py` & `umjunsik-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
   name = 'umjunsik',
   packages = ['umjunsik'],
-  version = '1.2.2',
+  version = '1.2.3',
   license = 'MIT',
   description = 'Umjunsik programming language',
   author = 'rycont',
   author_email = 'rycont@outlook.kr',
   url = 'https://github.com/rycont/umjunsik-lang',
   include_dirs = ['umjunsik'],
   keywords = ['ESOLANG'],
```

### Comparing `umjunsik-1.2.2/umjunsik/runtime.py` & `umjunsik-1.2.3/umjunsik/runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,8 +77,17 @@
             error += 1
             if error == errors:
                 raise RecursionError(str(errorline+1) + '번째 줄에서 무한 루프가 감지되었습니다.')
 
     def compilePath(self, path):
         with open(path) as file:
             code = ''.join(file.readlines())
-            self.compile(code)
+            self.compile(code)
+        
+if __name__ == '__main__':
+    if len(sys.argv) < 2:
+        print("Usage: umjunsik [file]")
+        sys.exit()
+
+    path = sys.argv[1]
+    u = Umjunsik()
+    u.compilePath(path)
```

### Comparing `umjunsik-1.2.2/umjunsik.egg-info/PKG-INFO` & `umjunsik-1.2.3/umjunsik.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umjunsik
-Version: 1.2.2
+Version: 1.2.3
 Summary: Umjunsik programming language
 Home-page: https://github.com/rycont/umjunsik-lang
 Author: rycont
 Author-email: rycont@outlook.kr
 License: MIT
 Keywords: ESOLANG
 Classifier: Development Status :: 5 - Production/Stable
```


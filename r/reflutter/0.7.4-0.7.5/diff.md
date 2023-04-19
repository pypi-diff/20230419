# Comparing `tmp/reflutter-0.7.4.tar.gz` & `tmp/reflutter-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflutter-0.7.4.tar", last modified: Tue Apr 18 22:54:16 2023, max compression
+gzip compressed data, was "reflutter-0.7.5.tar", last modified: Wed Apr 19 20:32:05 2023, max compression
```

## Comparing `reflutter-0.7.4.tar` & `reflutter-0.7.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-04-18 22:54:16.950120 reflutter-0.7.4/
--rw-r--r--   0 jay        (501) staff       (20)    35149 2023-04-10 12:02:01.000000 reflutter-0.7.4/LICENSE
--rw-r--r--   0 jay        (501) staff       (20)     8721 2023-04-18 22:54:16.949929 reflutter-0.7.4/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)     7739 2023-04-18 22:53:30.000000 reflutter-0.7.4/README.md
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-04-18 22:54:16.944775 reflutter-0.7.4/reflutter.egg-info/
--rw-r--r--   0 jay        (501) staff       (20)     8721 2023-04-18 22:54:16.000000 reflutter-0.7.4/reflutter.egg-info/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      210 2023-04-18 22:54:16.000000 reflutter-0.7.4/reflutter.egg-info/SOURCES.txt
--rw-r--r--   0 jay        (501) staff       (20)        1 2023-04-18 22:54:16.000000 reflutter-0.7.4/reflutter.egg-info/dependency_links.txt
--rw-r--r--   0 jay        (501) staff       (20)       48 2023-04-18 22:54:16.000000 reflutter-0.7.4/reflutter.egg-info/entry_points.txt
--rw-r--r--   0 jay        (501) staff       (20)        4 2023-04-18 22:54:16.000000 reflutter-0.7.4/reflutter.egg-info/top_level.txt
--rw-r--r--   0 jay        (501) staff       (20)       38 2023-04-18 22:54:16.950161 reflutter-0.7.4/setup.cfg
--rw-r--r--   0 jay        (501) staff       (20)     1401 2023-04-18 22:53:36.000000 reflutter-0.7.4/setup.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-04-18 22:54:16.944909 reflutter-0.7.4/src/
--rw-r--r--   0 jay        (501) staff       (20)    44261 2023-04-16 07:07:28.000000 reflutter-0.7.4/src/__init__.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-04-19 20:32:05.297359 reflutter-0.7.5/
+-rw-r--r--   0 jay        (501) staff       (20)    35149 2023-04-10 12:02:01.000000 reflutter-0.7.5/LICENSE
+-rw-r--r--   0 jay        (501) staff       (20)     8721 2023-04-19 20:32:05.297207 reflutter-0.7.5/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)     7739 2023-04-19 20:28:57.000000 reflutter-0.7.5/README.md
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-04-19 20:32:05.292181 reflutter-0.7.5/reflutter.egg-info/
+-rw-r--r--   0 jay        (501) staff       (20)     8721 2023-04-19 20:32:05.000000 reflutter-0.7.5/reflutter.egg-info/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)      210 2023-04-19 20:32:05.000000 reflutter-0.7.5/reflutter.egg-info/SOURCES.txt
+-rw-r--r--   0 jay        (501) staff       (20)        1 2023-04-19 20:32:05.000000 reflutter-0.7.5/reflutter.egg-info/dependency_links.txt
+-rw-r--r--   0 jay        (501) staff       (20)       48 2023-04-19 20:32:05.000000 reflutter-0.7.5/reflutter.egg-info/entry_points.txt
+-rw-r--r--   0 jay        (501) staff       (20)        4 2023-04-19 20:32:05.000000 reflutter-0.7.5/reflutter.egg-info/top_level.txt
+-rw-r--r--   0 jay        (501) staff       (20)       38 2023-04-19 20:32:05.297400 reflutter-0.7.5/setup.cfg
+-rw-r--r--   0 jay        (501) staff       (20)     1401 2023-04-19 20:26:46.000000 reflutter-0.7.5/setup.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-04-19 20:32:05.292315 reflutter-0.7.5/src/
+-rw-r--r--   0 jay        (501) staff       (20)    44409 2023-04-19 20:24:30.000000 reflutter-0.7.5/src/__init__.py
```

### Comparing `reflutter-0.7.4/LICENSE` & `reflutter-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reflutter-0.7.4/PKG-INFO` & `reflutter-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflutter
-Version: 0.7.4
+Version: 0.7.5
 Summary: Reverse Flutter
 Home-page: https://github.com/Impact-I/reFlutter
 Author: impact
 Author-email: routeros7.1@gmail.com
 License: GPLv3+
 Keywords: distutils setuptools egg pip requirements
 Platform: any
@@ -42,15 +42,15 @@
 ### Supported engines
 - Android: arm64, arm32;
 - iOS: arm64;
 - Release: Stable, Beta
 ### Install
 ```
 # Linux, Windows, MacOS
-pip3 install reflutter==0.7.4
+pip3 install reflutter==0.7.5
 ```
 ### Usage
 ```console
 impact@f:~$ reflutter main.apk
 
 Please enter your Burp Suite IP: <input_ip>
```

### Comparing `reflutter-0.7.4/README.md` & `reflutter-0.7.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ### Supported engines
 - Android: arm64, arm32;
 - iOS: arm64;
 - Release: Stable, Beta
 ### Install
 ```
 # Linux, Windows, MacOS
-pip3 install reflutter==0.7.4
+pip3 install reflutter==0.7.5
 ```
 ### Usage
 ```console
 impact@f:~$ reflutter main.apk
 
 Please enter your Burp Suite IP: <input_ip>
```

### Comparing `reflutter-0.7.4/reflutter.egg-info/PKG-INFO` & `reflutter-0.7.5/reflutter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflutter
-Version: 0.7.4
+Version: 0.7.5
 Summary: Reverse Flutter
 Home-page: https://github.com/Impact-I/reFlutter
 Author: impact
 Author-email: routeros7.1@gmail.com
 License: GPLv3+
 Keywords: distutils setuptools egg pip requirements
 Platform: any
@@ -42,15 +42,15 @@
 ### Supported engines
 - Android: arm64, arm32;
 - iOS: arm64;
 - Release: Stable, Beta
 ### Install
 ```
 # Linux, Windows, MacOS
-pip3 install reflutter==0.7.4
+pip3 install reflutter==0.7.5
 ```
 ### Usage
 ```console
 impact@f:~$ reflutter main.apk
 
 Please enter your Burp Suite IP: <input_ip>
```

### Comparing `reflutter-0.7.4/setup.py` & `reflutter-0.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: Implementation :: PyPy',
     'Topic :: Software Development :: Build Tools',
 ]
 
 setuptools.setup(
     name='reflutter',
-    version='0.7.4',
+    version='0.7.5',
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author='impact',
     author_email='routeros7.1@gmail.com',
     url='https://github.com/Impact-I/reFlutter',
     packages=setuptools.find_packages(),
```

### Comparing `reflutter-0.7.4/src/__init__.py` & `reflutter-0.7.5/src/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 libAppArm64 = '', ''
 libAppArm = '', ''
 libAppX64 = '', ''
 libAppX86 = '', ''
 libios = '', ''
 libappHash = ''
 ZIPSTORED = False
+engineHashFile = 'enginehash.tmp.csv'
 
 
 def patchLibrary():
     if len(libios[1]) != 0:
         buffer = open('Flutter', 'rb').read().replace(b'192.168.133.104', IPBurp.encode('ascii'))
         open('Flutter', 'wb').write(buffer)
     if len(libAppArm64[1]) != 0:
@@ -447,18 +448,22 @@
         if sys.argv[1].lower().endswith('.apk') or sys.argv[1].lower().endswith('.ipa'):
             extractZip(sys.argv[1])
             libappHash = ELFF(sys.argv[1])
             shutil.rmtree('libappTmp')
         else:
             libappHash = sys.argv[1]
 
-        if not os.path.exists("enginehash.csv"):
-            urlretrieve("https://raw.githubusercontent.com/Impact-I/reFlutter/main/enginehash.csv", "enginehash.csv")
+        # remove existing enginehash file
+        if os.path.isfile(engineHashFile):
+            os.remove(engineHashFile)
 
-        with open("enginehash.csv") as f_obj:
+        # fetch the latest enginehash file
+        urlretrieve("https://raw.githubusercontent.com/Impact-I/reFlutter/main/enginehash.csv", engineHashFile)
+
+        with open(engineHashFile) as f_obj:
             replaceFileText('src/src/flutter/BUILD.gn',
                             '  if (is_android) {\n    public_deps +=\n        [ "//flutter/shell/platform/android:flutter_shell_native_unittests" ]\n  }',
                             '')
             read = csv.DictReader(f_obj, delimiter=',')
             row_count = sum(1 for _ in read)
             f_obj.seek(0)
             reader = csv.DictReader(f_obj, delimiter=',')
```


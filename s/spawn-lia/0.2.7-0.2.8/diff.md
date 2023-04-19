# Comparing `tmp/spawn-lia-0.2.7.tar.gz` & `tmp/spawn-lia-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spawn-lia-0.2.7.tar", last modified: Wed Apr 19 19:31:04 2023, max compression
+gzip compressed data, was "spawn-lia-0.2.8.tar", last modified: Wed Apr 19 19:36:45 2023, max compression
```

## Comparing `spawn-lia-0.2.7.tar` & `spawn-lia-0.2.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/
--rw-r--r--   0 developer  (1001) developer  (1001)    34693 2023-04-19 19:30:54.000000 spawn-lia-0.2.7/LICENSE.txt
--rw-r--r--   0 developer  (1001) developer  (1001)     5125 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)     4659 2023-04-19 19:30:12.000000 spawn-lia-0.2.7/README.md
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.156620 spawn-lia-0.2.7/lia/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/__init__.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/lia/bounty/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/bounty/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     4814 2023-04-19 19:30:55.000000 spawn-lia-0.2.7/lia/bounty/heal.py
--rw-r--r--   0 developer  (1001) developer  (1001)      554 2023-04-15 20:42:23.000000 spawn-lia-0.2.7/lia/bounty/testing.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/lia/conversation/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/conversation/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1028 2023-04-19 19:30:55.000000 spawn-lia-0.2.7/lia/conversation/ask_to_proceed.py
--rw-r--r--   0 developer  (1001) developer  (1001)      103 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/conversation/decision.py
--rw-r--r--   0 developer  (1001) developer  (1001)      960 2023-04-15 20:42:23.000000 spawn-lia-0.2.7/lia/conversation/emojis.py
--rw-r--r--   0 developer  (1001) developer  (1001)      395 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/conversation/end_message.py
--rw-r--r--   0 developer  (1001) developer  (1001)      506 2023-04-15 20:42:23.000000 spawn-lia-0.2.7/lia/conversation/get_input.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1015 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/conversation/start_message.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2218 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/conversation/virtualenv.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/lia/git_operations/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/git_operations/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1546 2023-04-19 19:30:55.000000 spawn-lia-0.2.7/lia/git_operations/push.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1486 2023-04-19 19:30:55.000000 spawn-lia-0.2.7/lia/git_operations/verify_branch.py
--rw-r--r--   0 developer  (1001) developer  (1001)      608 2023-04-15 20:42:23.000000 spawn-lia-0.2.7/lia/main.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/lia/simplify/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/simplify/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1768 2023-04-19 19:30:55.000000 spawn-lia-0.2.7/lia/simplify/create_venv.py
--rw-r--r--   0 developer  (1001) developer  (1001)      246 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/simplify/verify_package.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/lia/support/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/support/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1260 2023-04-15 19:23:40.000000 spawn-lia-0.2.7/lia/support/deploy.py
--rw-r--r--   0 developer  (1001) developer  (1001)       38 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/setup.cfg
--rw-r--r--   0 developer  (1001) developer  (1001)     1156 2023-04-19 19:30:21.000000 spawn-lia-0.2.7/setup.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/spawn_lia.egg-info/
--rw-r--r--   0 developer  (1001) developer  (1001)     5125 2023-04-19 19:31:04.000000 spawn-lia-0.2.7/spawn_lia.egg-info/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)      894 2023-04-19 19:31:04.000000 spawn-lia-0.2.7/spawn_lia.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-19 19:31:04.000000 spawn-lia-0.2.7/spawn_lia.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       40 2023-04-19 19:31:04.000000 spawn-lia-0.2.7/spawn_lia.egg-info/entry_points.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       96 2023-04-19 19:31:04.000000 spawn-lia-0.2.7/spawn_lia.egg-info/requires.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        4 2023-04-19 19:31:04.000000 spawn-lia-0.2.7/spawn_lia.egg-info/top_level.txt
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/tests/
--rw-r--r--   0 developer  (1001) developer  (1001)      626 2023-04-07 19:00:56.000000 spawn-lia-0.2.7/tests/test_deploy.py
--rw-r--r--   0 developer  (1001) developer  (1001)     5018 2023-04-19 19:25:28.000000 spawn-lia-0.2.7/tests/test_git_operations.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1140 2023-04-12 17:06:07.000000 spawn-lia-0.2.7/tests/test_heal.py
--rw-r--r--   0 developer  (1001) developer  (1001)      885 2023-04-15 20:42:23.000000 spawn-lia-0.2.7/tests/test_venv.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/
+-rw-r--r--   0 developer  (1001) developer  (1001)    34693 2023-04-19 19:36:37.000000 spawn-lia-0.2.8/LICENSE.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)     5125 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)     4659 2023-04-19 19:34:22.000000 spawn-lia-0.2.8/README.md
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/lia/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/__init__.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/lia/bounty/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/bounty/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     4814 2023-04-19 19:36:37.000000 spawn-lia-0.2.8/lia/bounty/heal.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      554 2023-04-15 20:42:23.000000 spawn-lia-0.2.8/lia/bounty/testing.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/lia/conversation/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/conversation/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1028 2023-04-19 19:36:37.000000 spawn-lia-0.2.8/lia/conversation/ask_to_proceed.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      103 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/conversation/decision.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      960 2023-04-15 20:42:23.000000 spawn-lia-0.2.8/lia/conversation/emojis.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      395 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/conversation/end_message.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      506 2023-04-15 20:42:23.000000 spawn-lia-0.2.8/lia/conversation/get_input.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1015 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/conversation/start_message.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2218 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/conversation/virtualenv.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/lia/git_operations/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/git_operations/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1546 2023-04-19 19:36:37.000000 spawn-lia-0.2.8/lia/git_operations/push.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1486 2023-04-19 19:36:37.000000 spawn-lia-0.2.8/lia/git_operations/verify_branch.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      608 2023-04-15 20:42:23.000000 spawn-lia-0.2.8/lia/main.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/lia/simplify/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/simplify/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1768 2023-04-19 19:36:37.000000 spawn-lia-0.2.8/lia/simplify/create_venv.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      246 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/simplify/verify_package.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/lia/support/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.8/lia/support/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1260 2023-04-15 19:23:40.000000 spawn-lia-0.2.8/lia/support/deploy.py
+-rw-r--r--   0 developer  (1001) developer  (1001)       38 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/setup.cfg
+-rw-r--r--   0 developer  (1001) developer  (1001)     1156 2023-04-19 19:36:35.000000 spawn-lia-0.2.8/setup.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/spawn_lia.egg-info/
+-rw-r--r--   0 developer  (1001) developer  (1001)     5125 2023-04-19 19:36:45.000000 spawn-lia-0.2.8/spawn_lia.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)      894 2023-04-19 19:36:45.000000 spawn-lia-0.2.8/spawn_lia.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-19 19:36:45.000000 spawn-lia-0.2.8/spawn_lia.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)       40 2023-04-19 19:36:45.000000 spawn-lia-0.2.8/spawn_lia.egg-info/entry_points.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)       96 2023-04-19 19:36:45.000000 spawn-lia-0.2.8/spawn_lia.egg-info/requires.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        4 2023-04-19 19:36:45.000000 spawn-lia-0.2.8/spawn_lia.egg-info/top_level.txt
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:36:45.771975 spawn-lia-0.2.8/tests/
+-rw-r--r--   0 developer  (1001) developer  (1001)      626 2023-04-07 19:00:56.000000 spawn-lia-0.2.8/tests/test_deploy.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     5114 2023-04-19 19:36:03.000000 spawn-lia-0.2.8/tests/test_git_operations.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1140 2023-04-12 17:06:07.000000 spawn-lia-0.2.8/tests/test_heal.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      885 2023-04-15 20:42:23.000000 spawn-lia-0.2.8/tests/test_venv.py
```

### Comparing `spawn-lia-0.2.7/LICENSE.txt` & `spawn-lia-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.7/PKG-INFO` & `spawn-lia-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spawn-lia
-Version: 0.2.7
+Version: 0.2.8
 Summary: The most wanted support
 Home-page: https://codeberg.org/cap_jmk/lia
 Author: Julian M. Kleber
 Author-email: julian.kleber@sail.black
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `spawn-lia-0.2.7/README.md` & `spawn-lia-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.7/lia/bounty/heal.py` & `spawn-lia-0.2.8/lia/bounty/heal.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.7/lia/bounty/testing.py` & `spawn-lia-0.2.8/lia/bounty/testing.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.7/lia/conversation/ask_to_proceed.py` & `spawn-lia-0.2.8/lia/conversation/ask_to_proceed.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.7/lia/conversation/emojis.py` & `spawn-lia-0.2.8/lia/conversation/emojis.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.7/lia/conversation/start_message.py` & `spawn-lia-0.2.8/lia/conversation/start_message.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.7/lia/conversation/virtualenv.py` & `spawn-lia-0.2.8/lia/conversation/virtualenv.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.7/lia/git_operations/push.py` & `spawn-lia-0.2.8/lia/git_operations/push.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.7/lia/git_operations/verify_branch.py` & `spawn-lia-0.2.8/lia/git_operations/verify_branch.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.7/lia/main.py` & `spawn-lia-0.2.8/lia/main.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.7/lia/simplify/create_venv.py` & `spawn-lia-0.2.8/lia/simplify/create_venv.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.7/lia/support/deploy.py` & `spawn-lia-0.2.8/lia/support/deploy.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.7/setup.py` & `spawn-lia-0.2.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="spawn-lia",
-    version="0.2.7",
+    version="0.2.8",
     packages=find_packages(include=["lia*"]),
     include_package_data=True,
     install_requires=[
         "Click",
         "black",
         "autopep8",
         "mypy",
```

### Comparing `spawn-lia-0.2.7/spawn_lia.egg-info/PKG-INFO` & `spawn-lia-0.2.8/spawn_lia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spawn-lia
-Version: 0.2.7
+Version: 0.2.8
 Summary: The most wanted support
 Home-page: https://codeberg.org/cap_jmk/lia
 Author: Julian M. Kleber
 Author-email: julian.kleber@sail.black
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `spawn-lia-0.2.7/spawn_lia.egg-info/SOURCES.txt` & `spawn-lia-0.2.8/spawn_lia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.7/tests/test_deploy.py` & `spawn-lia-0.2.8/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.7/tests/test_git_operations.py` & `spawn-lia-0.2.8/tests/test_git_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,14 +112,17 @@
 
     subprocess.run(["git checkout dev"], shell=True, check=True)
    """  # -> can only implement after merge
 
 def test_push(): 
 
     #switch to temporary branch to avoid contaminations
+    subprocess.run(["git checkout dev"], check = True, shell=True)
+    subprocess.run(["git branch -D test_branch"], check = True, shell = True)
+
     out = subprocess.run(["git status"], check=True, shell=True, capture_output=True)
     out2 = subprocess.run(["git branch"], check=True, shell=True, capture_output=True)
     if b"On branch test_branch" not in out.stdout:
         if "test_branch" not in out2.stdout.decode("utf-8"):
             subprocess.run(["git checkout -b test_branch"], check=True, shell=True)
         else: 
             subprocess.run(["git checkout test_branch"], check=True, shell=True)
@@ -128,16 +131,15 @@
         ["lia", "push"], stdin=PIPE, stdout=PIPE
     )
 
     out.stdin.write(b"push done by test\n")
     outputlog, errorlog = out.communicate()
 
     out.stdin.close()
-    assert 1 == 2, str(outputlog) +" - " + str(errorlog)
-    subprocess.run["git checkout dev"]
+    subprocess.run(["git checkout dev"], check = True, shell=True)
     out = subprocess.Popen(
         ["python", "./lia/git_operations/verify_branch.py"], stdin=PIPE, stdout=PIPE
     )
     
     outputlog, errorlog = out.communicate()
     out.stdin.close()
-    assert outputlog == b"You are on the master branch but we agreed to only use main... \xf0\x9f\x98\xa1\nPlease rename the branch, darling \xf0\x9f\x98\x98\n"
+    assert outputlog == b"It seems like you are on a good branch.\nThe way is free for you to go ahead \xf0\x9f\xaa\x84 \xf0\x9f\x98\xbd\n"
```

### Comparing `spawn-lia-0.2.7/tests/test_heal.py` & `spawn-lia-0.2.8/tests/test_heal.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.7/tests/test_venv.py` & `spawn-lia-0.2.8/tests/test_venv.py`

 * *Files identical despite different names*


# Comparing `tmp/fooder-0.0.2.tar.gz` & `tmp/fooder-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fooder-0.0.2.tar", last modified: Tue Apr 18 10:08:23 2023, max compression
+gzip compressed data, was "fooder-0.0.3.tar", last modified: Wed Apr 19 16:41:50 2023, max compression
```

## Comparing `fooder-0.0.2.tar` & `fooder-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-04-18 10:08:23.731690 fooder-0.0.2/
--rw-r--r--   0 doman      (501) staff       (20)    35149 2023-04-17 21:36:03.000000 fooder-0.0.2/LICENSE
--rw-r--r--   0 doman      (501) staff       (20)     2134 2023-04-18 10:08:23.731737 fooder-0.0.2/PKG-INFO
-drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-04-18 10:08:23.730249 fooder-0.0.2/fooder.egg-info/
--rw-r--r--   0 doman      (501) staff       (20)     2134 2023-04-18 10:08:23.000000 fooder-0.0.2/fooder.egg-info/PKG-INFO
--rw-r--r--   0 doman      (501) staff       (20)      375 2023-04-18 10:08:23.000000 fooder-0.0.2/fooder.egg-info/SOURCES.txt
--rw-r--r--   0 doman      (501) staff       (20)        1 2023-04-18 10:08:23.000000 fooder-0.0.2/fooder.egg-info/dependency_links.txt
--rw-r--r--   0 doman      (501) staff       (20)       49 2023-04-18 10:08:23.000000 fooder-0.0.2/fooder.egg-info/entry_points.txt
--rw-r--r--   0 doman      (501) staff       (20)       40 2023-04-18 10:08:23.000000 fooder-0.0.2/fooder.egg-info/requires.txt
--rw-r--r--   0 doman      (501) staff       (20)       11 2023-04-18 10:08:23.000000 fooder-0.0.2/fooder.egg-info/top_level.txt
-drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-04-18 10:08:23.731463 fooder-0.0.2/fooder_cli/
--rw-r--r--   0 doman      (501) staff       (20)        0 2023-04-17 21:36:03.000000 fooder-0.0.2/fooder_cli/__init__.py
--rw-r--r--   0 doman      (501) staff       (20)       63 2023-04-17 21:36:03.000000 fooder-0.0.2/fooder_cli/__main__.py
--rw-r--r--   0 doman      (501) staff       (20)     9704 2023-04-18 10:04:23.000000 fooder-0.0.2/fooder_cli/client.py
--rw-r--r--   0 doman      (501) staff       (20)     1626 2023-04-18 10:06:34.000000 fooder-0.0.2/fooder_cli/diary.py
--rw-r--r--   0 doman      (501) staff       (20)      675 2023-04-18 10:04:11.000000 fooder-0.0.2/fooder_cli/entry.py
--rw-r--r--   0 doman      (501) staff       (20)     2992 2023-04-17 21:36:03.000000 fooder-0.0.2/fooder_cli/main.py
--rw-r--r--   0 doman      (501) staff       (20)      719 2023-04-18 10:04:56.000000 fooder-0.0.2/fooder_cli/meal.py
--rw-r--r--   0 doman      (501) staff       (20)     2717 2023-04-18 10:05:40.000000 fooder-0.0.2/fooder_cli/product.py
--rw-r--r--   0 doman      (501) staff       (20)      100 2023-04-18 10:08:23.731930 fooder-0.0.2/setup.cfg
--rw-r--r--   0 doman      (501) staff       (20)      973 2023-04-18 10:07:57.000000 fooder-0.0.2/setup.py
+drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-04-19 16:41:50.160477 fooder-0.0.3/
+-rw-r--r--   0 doman      (501) staff       (20)    35149 2023-04-17 21:36:03.000000 fooder-0.0.3/LICENSE
+-rw-r--r--   0 doman      (501) staff       (20)     2134 2023-04-19 16:41:50.160534 fooder-0.0.3/PKG-INFO
+drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-04-19 16:41:50.158634 fooder-0.0.3/fooder.egg-info/
+-rw-r--r--   0 doman      (501) staff       (20)     2134 2023-04-19 16:41:50.000000 fooder-0.0.3/fooder.egg-info/PKG-INFO
+-rw-r--r--   0 doman      (501) staff       (20)      375 2023-04-19 16:41:50.000000 fooder-0.0.3/fooder.egg-info/SOURCES.txt
+-rw-r--r--   0 doman      (501) staff       (20)        1 2023-04-19 16:41:50.000000 fooder-0.0.3/fooder.egg-info/dependency_links.txt
+-rw-r--r--   0 doman      (501) staff       (20)       49 2023-04-19 16:41:50.000000 fooder-0.0.3/fooder.egg-info/entry_points.txt
+-rw-r--r--   0 doman      (501) staff       (20)       40 2023-04-19 16:41:50.000000 fooder-0.0.3/fooder.egg-info/requires.txt
+-rw-r--r--   0 doman      (501) staff       (20)       11 2023-04-19 16:41:50.000000 fooder-0.0.3/fooder.egg-info/top_level.txt
+drwxr-xr-x   0 doman      (501) staff       (20)        0 2023-04-19 16:41:50.160290 fooder-0.0.3/fooder_cli/
+-rw-r--r--   0 doman      (501) staff       (20)        0 2023-04-17 21:36:03.000000 fooder-0.0.3/fooder_cli/__init__.py
+-rw-r--r--   0 doman      (501) staff       (20)       63 2023-04-17 21:36:03.000000 fooder-0.0.3/fooder_cli/__main__.py
+-rw-r--r--   0 doman      (501) staff       (20)     9704 2023-04-18 10:04:23.000000 fooder-0.0.3/fooder_cli/client.py
+-rw-r--r--   0 doman      (501) staff       (20)     1626 2023-04-18 10:06:34.000000 fooder-0.0.3/fooder_cli/diary.py
+-rw-r--r--   0 doman      (501) staff       (20)      675 2023-04-18 10:04:11.000000 fooder-0.0.3/fooder_cli/entry.py
+-rw-r--r--   0 doman      (501) staff       (20)     3785 2023-04-19 16:39:05.000000 fooder-0.0.3/fooder_cli/main.py
+-rw-r--r--   0 doman      (501) staff       (20)      719 2023-04-18 10:04:56.000000 fooder-0.0.3/fooder_cli/meal.py
+-rw-r--r--   0 doman      (501) staff       (20)     2717 2023-04-18 10:05:40.000000 fooder-0.0.3/fooder_cli/product.py
+-rw-r--r--   0 doman      (501) staff       (20)      100 2023-04-19 16:41:50.160833 fooder-0.0.3/setup.cfg
+-rw-r--r--   0 doman      (501) staff       (20)      973 2023-04-19 16:39:48.000000 fooder-0.0.3/setup.py
```

### Comparing `fooder-0.0.2/LICENSE` & `fooder-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fooder-0.0.2/PKG-INFO` & `fooder-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fooder
-Version: 0.0.2
+Version: 0.0.3
 Summary: Minimalistic cli diary for tracking calories
 Home-page: https://github.com/ickyicky/fooder-cli-client
 Author: Piotr Domanski
 Author-email: pi.domanski@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fooder-0.0.2/fooder.egg-info/PKG-INFO` & `fooder-0.0.3/fooder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fooder
-Version: 0.0.2
+Version: 0.0.3
 Summary: Minimalistic cli diary for tracking calories
 Home-page: https://github.com/ickyicky/fooder-cli-client
 Author: Piotr Domanski
 Author-email: pi.domanski@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fooder-0.0.2/fooder_cli/client.py` & `fooder-0.0.3/fooder_cli/client.py`

 * *Files identical despite different names*

### Comparing `fooder-0.0.2/fooder_cli/diary.py` & `fooder-0.0.3/fooder_cli/diary.py`

 * *Files identical despite different names*

### Comparing `fooder-0.0.2/fooder_cli/entry.py` & `fooder-0.0.3/fooder_cli/entry.py`

 * *Files identical despite different names*

### Comparing `fooder-0.0.2/fooder_cli/main.py` & `fooder-0.0.3/fooder_cli/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,23 +6,38 @@
 from getpass import getpass
 from datetime import date
 from rich.prompt import Prompt
 from rich.panel import Panel
 from rich.text import Text
 from rich import print
 from argparse import ArgumentParser
+from typing import Optional
 
 
-def login(client) -> None:
-    username = input("Username: ")
-    password = getpass("Password: ")
+def login(
+    client: FooderClient, username: Optional[str] = None, password: Optional[str] = None
+) -> None:
+    """
+    Login to fooder api
+
+    :param client: FooderClient instance
+    :param username: username
+    :param password: password
+    """
+    username = username or input("Username: ")
+    password = password or getpass("Password: ")
     client.login(username, password)
 
 
 def main_loop(client: FooderClient) -> None:
+    """
+    Main loop of fooder cli
+
+    :param client: FooderClient instance
+    """
     diary = None
     meal = None
 
     actions = [
         (1, "Show diary"),
         (2, "Add entry to diary"),
         (3, "Add meal to diary"),
@@ -94,14 +109,33 @@
 
 
 def main() -> None:
     parser = ArgumentParser()
     parser.add_argument("--access-token", default="~/.cache/fooder/.token")
     parser.add_argument("--refresh-token", default="~/.cache/fooder/.refresh_token")
     parser.add_argument("--url", default="https://fooderapi.domandoman.xyz/api")
+    parser.add_argument(
+        "--username",
+        type=str,
+        action="store",
+        required=False,
+        help="username for login",
+    )
+    parser.add_argument(
+        "--password",
+        type=str,
+        action="store",
+        required=False,
+        help="password for login, if not specified, you will be asked for it",
+    )
+
     args = parser.parse_args()
     client = FooderClient(
         args.access_token,
         args.refresh_token,
         args.url,
     )
+
+    if args.username:
+        login(client, args.username, args.password)
+
     main_loop(client)
```

### Comparing `fooder-0.0.2/fooder_cli/meal.py` & `fooder-0.0.3/fooder_cli/meal.py`

 * *Files identical despite different names*

### Comparing `fooder-0.0.2/fooder_cli/product.py` & `fooder-0.0.3/fooder_cli/product.py`

 * *Files identical despite different names*

### Comparing `fooder-0.0.2/setup.py` & `fooder-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read().splitlines()
 
 
 setup(
     name="fooder",
-    version="0.0.2",
+    version="0.0.3",
     author="Piotr Domanski",
     author_email="pi.domanski@gmail.com",
     description="Minimalistic cli diary for tracking calories",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ickyicky/fooder-cli-client",
     classifiers=[
```


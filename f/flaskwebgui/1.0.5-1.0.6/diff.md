# Comparing `tmp/flaskwebgui-1.0.5.tar.gz` & `tmp/flaskwebgui-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskwebgui-1.0.5.tar", last modified: Tue Apr 18 13:24:56 2023, max compression
+gzip compressed data, was "flaskwebgui-1.0.6.tar", last modified: Wed Apr 19 14:30:03 2023, max compression
```

## Comparing `flaskwebgui-1.0.5.tar` & `flaskwebgui-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 alin      (1000) alin      (1000)        0 2023-04-18 13:24:56.309650 flaskwebgui-1.0.5/
--rw-rw-r--   0 alin      (1000) alin      (1000)     1064 2023-03-11 07:58:47.000000 flaskwebgui-1.0.5/LICENSE
--rw-rw-r--   0 alin      (1000) alin      (1000)     7923 2023-04-18 13:24:56.309650 flaskwebgui-1.0.5/PKG-INFO
--rw-rw-r--   0 alin      (1000) alin      (1000)     7616 2023-03-11 09:28:14.000000 flaskwebgui-1.0.5/README.md
--rw-rw-r--   0 alin      (1000) alin      (1000)       38 2023-04-18 13:24:56.309650 flaskwebgui-1.0.5/setup.cfg
--rw-rw-r--   0 alin      (1000) alin      (1000)      824 2023-04-18 13:24:41.000000 flaskwebgui-1.0.5/setup.py
-drwxrwxr-x   0 alin      (1000) alin      (1000)        0 2023-04-18 13:24:56.305650 flaskwebgui-1.0.5/src/
-drwxrwxr-x   0 alin      (1000) alin      (1000)        0 2023-04-18 13:24:56.305650 flaskwebgui-1.0.5/src/flaskwebgui.egg-info/
--rw-rw-r--   0 alin      (1000) alin      (1000)     7923 2023-04-18 13:24:56.000000 flaskwebgui-1.0.5/src/flaskwebgui.egg-info/PKG-INFO
--rw-rw-r--   0 alin      (1000) alin      (1000)      239 2023-04-18 13:24:56.000000 flaskwebgui-1.0.5/src/flaskwebgui.egg-info/SOURCES.txt
--rw-rw-r--   0 alin      (1000) alin      (1000)        1 2023-04-18 13:24:56.000000 flaskwebgui-1.0.5/src/flaskwebgui.egg-info/dependency_links.txt
--rw-rw-r--   0 alin      (1000) alin      (1000)       12 2023-04-18 13:24:56.000000 flaskwebgui-1.0.5/src/flaskwebgui.egg-info/requires.txt
--rw-rw-r--   0 alin      (1000) alin      (1000)       12 2023-04-18 13:24:56.000000 flaskwebgui-1.0.5/src/flaskwebgui.egg-info/top_level.txt
--rw-rw-r--   0 alin      (1000) alin      (1000)     7509 2023-04-18 13:24:11.000000 flaskwebgui-1.0.5/src/flaskwebgui.py
+drwxrwxr-x   0 alin      (1000) alin      (1000)        0 2023-04-19 14:30:03.605465 flaskwebgui-1.0.6/
+-rw-rw-r--   0 alin      (1000) alin      (1000)     1064 2023-03-11 07:58:47.000000 flaskwebgui-1.0.6/LICENSE
+-rw-rw-r--   0 alin      (1000) alin      (1000)     8635 2023-04-19 14:30:03.605465 flaskwebgui-1.0.6/PKG-INFO
+-rw-rw-r--   0 alin      (1000) alin      (1000)     8328 2023-04-19 14:28:40.000000 flaskwebgui-1.0.6/README.md
+-rw-rw-r--   0 alin      (1000) alin      (1000)       38 2023-04-19 14:30:03.605465 flaskwebgui-1.0.6/setup.cfg
+-rw-rw-r--   0 alin      (1000) alin      (1000)      824 2023-04-19 14:29:11.000000 flaskwebgui-1.0.6/setup.py
+drwxrwxr-x   0 alin      (1000) alin      (1000)        0 2023-04-19 14:30:03.601465 flaskwebgui-1.0.6/src/
+drwxrwxr-x   0 alin      (1000) alin      (1000)        0 2023-04-19 14:30:03.601465 flaskwebgui-1.0.6/src/flaskwebgui.egg-info/
+-rw-rw-r--   0 alin      (1000) alin      (1000)     8635 2023-04-19 14:30:03.000000 flaskwebgui-1.0.6/src/flaskwebgui.egg-info/PKG-INFO
+-rw-rw-r--   0 alin      (1000) alin      (1000)      239 2023-04-19 14:30:03.000000 flaskwebgui-1.0.6/src/flaskwebgui.egg-info/SOURCES.txt
+-rw-rw-r--   0 alin      (1000) alin      (1000)        1 2023-04-19 14:30:03.000000 flaskwebgui-1.0.6/src/flaskwebgui.egg-info/dependency_links.txt
+-rw-rw-r--   0 alin      (1000) alin      (1000)       12 2023-04-19 14:30:03.000000 flaskwebgui-1.0.6/src/flaskwebgui.egg-info/requires.txt
+-rw-rw-r--   0 alin      (1000) alin      (1000)       12 2023-04-19 14:30:03.000000 flaskwebgui-1.0.6/src/flaskwebgui.egg-info/top_level.txt
+-rw-rw-r--   0 alin      (1000) alin      (1000)     7633 2023-04-19 14:18:49.000000 flaskwebgui-1.0.6/src/flaskwebgui.py
```

### Comparing `flaskwebgui-1.0.5/LICENSE` & `flaskwebgui-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flaskwebgui-1.0.5/PKG-INFO` & `flaskwebgui-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskwebgui
-Version: 1.0.5
+Version: 1.0.6
 Summary: Create desktop applications with Flask/Django/FastAPI!
 Home-page: https://github.com/ClimenteA/flaskwebgui
 Author: Climente Alin
 Author-email: climente.alin@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -165,14 +165,44 @@
 ```py
 python gui.py  
 ```
 
 Install `waitress` for more performance.
 
 
+## Close application using a route
+
+You can close the application using the `close_application` from flaskwebgui. Please note that this requires installing `pyautogui` package.
+
+
+```python
+
+from flaskwebgui import FlaskUI, close_application
+
+# Any python webframework routing here
+
+@app.route("/close", methods=["GET"])
+def close_window():
+    close_application()
+
+```
+
+And somewhere a link: 
+
+```html
+
+<a href="/close" class="exit" role="button">
+    CLOSE
+</a>
+
+```
+
+When `close_application` is called `ctrl+w` keystrokes are pressed to close the chrome window and the current python process is killed. This hacky implemantation does the job. Feel free to open a PR for a cleaner cross platform alternative.
+
+
 ## Configurations
 
 Default FlaskUI class parameters:
 
 - `server: Union[str, Callable[[Any], None]]`: function which receives `server_kwargs` to start server (see examples folder);
 - `server_kwargs: dict = None`: kwargs which will be passed down to `server` function;
 - `app: Any = None`: `wsgi` or `asgi` app;
```

### Comparing `flaskwebgui-1.0.5/README.md` & `flaskwebgui-1.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -154,14 +154,44 @@
 ```py
 python gui.py  
 ```
 
 Install `waitress` for more performance.
 
 
+## Close application using a route
+
+You can close the application using the `close_application` from flaskwebgui. Please note that this requires installing `pyautogui` package.
+
+
+```python
+
+from flaskwebgui import FlaskUI, close_application
+
+# Any python webframework routing here
+
+@app.route("/close", methods=["GET"])
+def close_window():
+    close_application()
+
+```
+
+And somewhere a link: 
+
+```html
+
+<a href="/close" class="exit" role="button">
+    CLOSE
+</a>
+
+```
+
+When `close_application` is called `ctrl+w` keystrokes are pressed to close the chrome window and the current python process is killed. This hacky implemantation does the job. Feel free to open a PR for a cleaner cross platform alternative.
+
+
 ## Configurations
 
 Default FlaskUI class parameters:
 
 - `server: Union[str, Callable[[Any], None]]`: function which receives `server_kwargs` to start server (see examples folder);
 - `server_kwargs: dict = None`: kwargs which will be passed down to `server` function;
 - `app: Any = None`: `wsgi` or `asgi` app;
```

### Comparing `flaskwebgui-1.0.5/setup.py` & `flaskwebgui-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open("requirements.txt", "r") as r:
     install_requires = r.readlines()
 
 
 setup(
     name="flaskwebgui",
-    version="1.0.5",
+    version="1.0.6",
     description="Create desktop applications with Flask/Django/FastAPI!",
     url="https://github.com/ClimenteA/flaskwebgui",
     author="Climente Alin",
     author_email="climente.alin@gmail.com",
     license="MIT",
     py_modules=["flaskwebgui"],
     install_requires=install_requires,
```

### Comparing `flaskwebgui-1.0.5/src/flaskwebgui.egg-info/PKG-INFO` & `flaskwebgui-1.0.6/src/flaskwebgui.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskwebgui
-Version: 1.0.5
+Version: 1.0.6
 Summary: Create desktop applications with Flask/Django/FastAPI!
 Home-page: https://github.com/ClimenteA/flaskwebgui
 Author: Climente Alin
 Author-email: climente.alin@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -165,14 +165,44 @@
 ```py
 python gui.py  
 ```
 
 Install `waitress` for more performance.
 
 
+## Close application using a route
+
+You can close the application using the `close_application` from flaskwebgui. Please note that this requires installing `pyautogui` package.
+
+
+```python
+
+from flaskwebgui import FlaskUI, close_application
+
+# Any python webframework routing here
+
+@app.route("/close", methods=["GET"])
+def close_window():
+    close_application()
+
+```
+
+And somewhere a link: 
+
+```html
+
+<a href="/close" class="exit" role="button">
+    CLOSE
+</a>
+
+```
+
+When `close_application` is called `ctrl+w` keystrokes are pressed to close the chrome window and the current python process is killed. This hacky implemantation does the job. Feel free to open a PR for a cleaner cross platform alternative.
+
+
 ## Configurations
 
 Default FlaskUI class parameters:
 
 - `server: Union[str, Callable[[Any], None]]`: function which receives `server_kwargs` to start server (see examples folder);
 - `server_kwargs: dict = None`: kwargs which will be passed down to `server` function;
 - `app: Any = None`: `wsgi` or `asgi` app;
```

### Comparing `flaskwebgui-1.0.5/src/flaskwebgui.py` & `flaskwebgui-1.0.6/src/flaskwebgui.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,21 @@
             for conns in proc.connections(kind="inet"):
                 if conns.laddr.port == port:
                     proc.send_signal(signal.SIGTERM)
         except psutil.AccessDenied:
             continue
 
 
+def close_application():
+    import pyautogui
+
+    pyautogui.hotkey("ctrl", "w")
+    os.kill(os.getpid(), signal.SIGKILL)
+
+
 def find_browser_on_linux():
     paths = [
         "/usr/bin/google-chrome",
         "/usr/bin/microsoft-edge-stable",
         "/usr/bin/microsoft-edge",
         "/usr/bin/brave-browser",
     ]
```


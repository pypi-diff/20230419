# Comparing `tmp/fps_auth-0.1.3.tar.gz` & `tmp/fps_auth-0.1.4.tar.gz`

## Comparing `fps_auth-0.1.3.tar` & `fps_auth-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth-0.1.3/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth-0.1.3/fps_auth/__init__.py
--rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 fps_auth-0.1.3/fps_auth/backends.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 fps_auth-0.1.3/fps_auth/config.py
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 fps_auth-0.1.3/fps_auth/db.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 fps_auth-0.1.3/fps_auth/main.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fps_auth-0.1.3/fps_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_auth-0.1.3/fps_auth/py.typed
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 fps_auth-0.1.3/fps_auth/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_auth-0.1.3/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth-0.1.3/COPYING.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_auth-0.1.3/README.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 fps_auth-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fps_auth-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth-0.1.4/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth-0.1.4/fps_auth/__init__.py
+-rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 fps_auth-0.1.4/fps_auth/backends.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fps_auth-0.1.4/fps_auth/config.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 fps_auth-0.1.4/fps_auth/db.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 fps_auth-0.1.4/fps_auth/main.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fps_auth-0.1.4/fps_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_auth-0.1.4/fps_auth/py.typed
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 fps_auth-0.1.4/fps_auth/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_auth-0.1.4/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth-0.1.4/COPYING.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_auth-0.1.4/README.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 fps_auth-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fps_auth-0.1.4/PKG-INFO
```

### Comparing `fps_auth-0.1.3/fps_auth/backends.py` & `fps_auth-0.1.4/fps_auth/backends.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.3/fps_auth/config.py` & `fps_auth-0.1.4/fps_auth/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,7 +12,8 @@
     mode: str = "token"
     token: str = uuid4().hex
     global_email: str = "guest@jupyter.com"
     cookie_secure: bool = False  # FIXME: should default to True, and set to False for tests
     clear_users: bool = False
     test: bool = False
     login_url: Optional[str] = None
+    directory: Optional[str] = None
```

### Comparing `fps_auth-0.1.3/fps_auth/db.py` & `fps_auth-0.1.4/fps_auth/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,19 @@
     create_db_and_tables: Any
     get_async_session: Any
     get_user_db: Any
     secret: Any
 
 
 def get_db(auth_config: _AuthConfig) -> Res:
-    jupyter_dir = Path.home() / ".local" / "share" / "jupyter"
+    jupyter_dir = (
+        Path.home() / ".local" / "share" / "jupyter"
+        if auth_config.directory is None
+        else Path(auth_config.directory)
+    )
     jupyter_dir.mkdir(parents=True, exist_ok=True)
     name = "jupyverse"
     if auth_config.test:
         name += "_test"
     secret_path = jupyter_dir / f"{name}_secret"
     userdb_path = jupyter_dir / f"{name}_users.db"
```

### Comparing `fps_auth-0.1.3/fps_auth/main.py` & `fps_auth-0.1.4/fps_auth/main.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.3/fps_auth/routes.py` & `fps_auth-0.1.4/fps_auth/routes.py`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.3/.gitignore` & `fps_auth-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.3/COPYING.md` & `fps_auth-0.1.4/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.3/pyproject.toml` & `fps_auth-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_auth-0.1.3/PKG-INFO` & `fps_auth-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_auth
-Version: 0.1.3
+Version: 0.1.4
 Summary: An FPS plugin for the authentication API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```


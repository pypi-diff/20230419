# Comparing `tmp/toui-1.1.0b0.tar.gz` & `tmp/toui-1.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-1.1.0b0.tar", last modified: Sat Apr 15 18:13:02 2023, max compression
+gzip compressed data, was "toui-1.2.0a1.tar", last modified: Wed Apr 19 04:22:56 2023, max compression
```

## Comparing `toui-1.1.0b0.tar` & `toui-1.2.0a1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 18:13:02.396935 toui-1.1.0b0/
--rw-rw-rw-   0        0        0     1094 2023-03-28 04:20:49.000000 toui-1.1.0b0/LICENSE
--rw-rw-rw-   0        0        0       16 2023-03-28 04:20:49.000000 toui-1.1.0b0/MANIFEST.in
--rw-rw-rw-   0        0        0     3056 2023-04-15 18:13:02.394935 toui-1.1.0b0/PKG-INFO
--rw-rw-rw-   0        0        0     2620 2023-04-13 08:05:30.000000 toui-1.1.0b0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 18:13:02.298381 toui-1.1.0b0/examples/
--rw-rw-rw-   0        0        0        0 2023-03-28 04:20:49.000000 toui-1.1.0b0/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-04-13 08:21:09.000000 toui-1.1.0b0/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0      556 2023-03-28 04:20:49.000000 toui-1.1.0b0/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-03-28 04:20:49.000000 toui-1.1.0b0/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-03-28 04:20:49.000000 toui-1.1.0b0/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-03-28 04:20:49.000000 toui-1.1.0b0/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-03-28 04:20:49.000000 toui-1.1.0b0/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-03-28 04:20:49.000000 toui-1.1.0b0/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-03-28 04:20:49.000000 toui-1.1.0b0/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:13:02.301004 toui-1.1.0b0/images/
--rw-rw-rw-   0        0        0    29049 2023-03-28 04:20:49.000000 toui-1.1.0b0/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-04-15 18:13:02.398404 toui-1.1.0b0/setup.cfg
--rw-rw-rw-   0        0        0     1225 2023-04-13 08:27:05.000000 toui-1.1.0b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:13:02.346802 toui-1.1.0b0/toui/
--rw-rw-rw-   0        0        0      213 2023-04-15 17:57:55.000000 toui-1.1.0b0/toui/__init__.py
--rw-rw-rw-   0        0        0      431 2023-04-15 14:31:15.000000 toui-1.1.0b0/toui/_defaults.py
--rw-rw-rw-   0        0        0     1093 2023-04-15 17:56:59.000000 toui-1.1.0b0/toui/_helpers.py
--rw-rw-rw-   0        0        0     7483 2023-04-15 17:49:55.000000 toui-1.1.0b0/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     3164 2023-04-15 17:30:00.000000 toui-1.1.0b0/toui/_signals.py
--rw-rw-rw-   0        0        0    20894 2023-04-15 18:09:47.000000 toui-1.1.0b0/toui/apps.py
--rw-rw-rw-   0        0        0    20399 2023-04-15 16:18:17.000000 toui-1.1.0b0/toui/elements.py
--rw-rw-rw-   0        0        0      168 2023-03-28 04:20:49.000000 toui-1.1.0b0/toui/exceptions.py
--rw-rw-rw-   0        0        0    15251 2023-04-15 16:14:35.000000 toui-1.1.0b0/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-03-28 04:20:49.000000 toui-1.1.0b0/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:13:02.391323 toui-1.1.0b0/toui.egg-info/
--rw-rw-rw-   0        0        0     3056 2023-04-15 18:13:02.000000 toui-1.1.0b0/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-04-15 18:13:02.000000 toui-1.1.0b0/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 18:13:02.000000 toui-1.1.0b0/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-04-15 18:13:02.000000 toui-1.1.0b0/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-15 18:13:02.000000 toui-1.1.0b0/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 04:22:56.746577 toui-1.2.0a1/
+-rw-rw-rw-   0        0        0     1094 2023-03-28 04:20:49.000000 toui-1.2.0a1/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-03-28 04:20:49.000000 toui-1.2.0a1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3056 2023-04-19 04:22:56.745573 toui-1.2.0a1/PKG-INFO
+-rw-rw-rw-   0        0        0     2620 2023-04-13 08:05:30.000000 toui-1.2.0a1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 04:22:56.679569 toui-1.2.0a1/examples/
+-rw-rw-rw-   0        0        0        0 2023-03-28 04:20:49.000000 toui-1.2.0a1/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-04-13 08:21:09.000000 toui-1.2.0a1/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0      556 2023-03-28 04:20:49.000000 toui-1.2.0a1/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-03-28 04:20:49.000000 toui-1.2.0a1/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-03-28 04:20:49.000000 toui-1.2.0a1/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-03-28 04:20:49.000000 toui-1.2.0a1/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-03-28 04:20:49.000000 toui-1.2.0a1/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-03-28 04:20:49.000000 toui-1.2.0a1/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-03-28 04:20:49.000000 toui-1.2.0a1/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-04-19 04:22:56.681812 toui-1.2.0a1/images/
+-rw-rw-rw-   0        0        0    29049 2023-03-28 04:20:49.000000 toui-1.2.0a1/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-04-19 04:22:56.747575 toui-1.2.0a1/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2023-04-13 08:27:05.000000 toui-1.2.0a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 04:22:56.709021 toui-1.2.0a1/toui/
+-rw-rw-rw-   0        0        0      216 2023-04-19 04:19:58.000000 toui-1.2.0a1/toui/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-04-15 14:31:15.000000 toui-1.2.0a1/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1093 2023-04-15 17:56:59.000000 toui-1.2.0a1/toui/_helpers.py
+-rw-rw-rw-   0        0        0     9783 2023-04-19 03:21:10.000000 toui-1.2.0a1/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     7391 2023-04-19 03:38:33.000000 toui-1.2.0a1/toui/_signals.py
+-rw-rw-rw-   0        0        0    24975 2023-04-19 04:15:22.000000 toui-1.2.0a1/toui/apps.py
+-rw-rw-rw-   0        0        0    20507 2023-04-19 03:34:58.000000 toui-1.2.0a1/toui/elements.py
+-rw-rw-rw-   0        0        0      168 2023-03-28 04:20:49.000000 toui-1.2.0a1/toui/exceptions.py
+-rw-rw-rw-   0        0        0    15251 2023-04-15 16:14:35.000000 toui-1.2.0a1/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-03-28 04:20:49.000000 toui-1.2.0a1/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-04-19 04:22:56.743572 toui-1.2.0a1/toui.egg-info/
+-rw-rw-rw-   0        0        0     3056 2023-04-19 04:22:56.000000 toui-1.2.0a1/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-04-19 04:22:56.000000 toui-1.2.0a1/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 04:22:56.000000 toui-1.2.0a1/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-04-19 04:22:56.000000 toui-1.2.0a1/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-19 04:22:56.000000 toui-1.2.0a1/toui.egg-info/top_level.txt
```

### Comparing `toui-1.1.0b0/LICENSE` & `toui-1.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-1.1.0b0/PKG-INFO` & `toui-1.2.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 1.1.0b0
+Version: 1.2.0a1
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Home-page: UNKNOWN
 Author: Mubarak Almehairbi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `toui-1.1.0b0/README.md` & `toui-1.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `toui-1.1.0b0/examples/advanced_example_1_toui_blueprint.py` & `toui-1.2.0a1/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-1.1.0b0/examples/example_1_simple_website.py` & `toui-1.2.0a1/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-1.1.0b0/examples/example_2_simple_desktop_app.py` & `toui-1.2.0a1/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-1.1.0b0/examples/example_3_updating_page.py` & `toui-1.2.0a1/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-1.1.0b0/examples/example_4_function_with_arg.py` & `toui-1.2.0a1/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-1.1.0b0/examples/example_5_user_variables.py` & `toui-1.2.0a1/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-1.1.0b0/images/logo.png` & `toui-1.2.0a1/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-1.1.0b0/setup.py` & `toui-1.2.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `toui-1.1.0b0/toui/_helpers.py` & `toui-1.2.0a1/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-1.1.0b0/toui/_javascript_templates.py` & `toui-1.2.0a1/toui/_javascript_templates.py`

 * *Files 22% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 function _send(jsonstring) {{
     return jsonstring
 }}
 """
 
 
 common_template = f"""
+_touiFiles = {{}}
+
 function _getDoc() {{
     var serializer = new XMLSerializer()
     const doc = serializer.serializeToString(document)
     return doc
     }}
 
 function _setDoc(kwargs) {{
@@ -86,26 +88,76 @@
     if (element.type == "file") {{
         for (var file of element.files) {{
             var selector = _getElementSelector(element)
             var fileJSON = {{name: file.name,
                              size: file.size,
                              type: file.type,
                              'last-modified': file.lastModified,
-                             'last-modified-date': file.lastModifiedDate,
                              selector: selector}}
             if (kwargs['with_content'] == true) {{
                 await file.text().then(function (text) {{
                     fileJSON['content'] = text
                 }})
             }}
+            var keys = Object.keys(_touiFiles)
+            var newKey = 0
+            if (keys.length != 0) {{
+                var lastKey = keys.sort().reverse()[0]
+                const newKey = parseInt(lastKey) + 1
+            }}
+            _touiFiles[newKey.toString()] = file
+            fileJSON['file-id'] = newKey.toString()
             files.push(fileJSON)
         }}
     }}
-    var jsonstring = JSON.stringify({{data: files, type: "files"}})
-    return _send(jsonstring)
+    var jsonString = JSON.stringify({{data: files, type: "files"}})
+    var dataSent = _send(jsonString)
+    return dataSent
+}}
+
+async function _saveFile(kwargs) {{
+    var fileId = kwargs['file-id']
+    var file = _touiFiles[fileId]
+    var reader = new FileReader()
+    if (kwargs['binary'] == true) {{
+        reader.onload = function () {{
+            const buffer = reader.result
+            const content = new Uint8Array(buffer)
+            const lengthPerPart = 16000
+            const charsLength = content.length
+            for (var i = 0; i < charsLength; i += lengthPerPart) {{
+                var smallerContent = [...content.slice(i, i + lengthPerPart)]
+                var jsonString = JSON.stringify({{type: "save files",
+                                                  data: smallerContent,
+                                                  end: false}})
+                var dataSent = _send(jsonString)
+            }}
+            var jsonString = JSON.stringify({{type: "save files", data: [],
+                                              end: true}})
+            var dataSent = _send(jsonString)
+        }}
+        reader.readAsArrayBuffer(file)
+    }} else {{
+        reader.onload = function () {{
+            const content = reader.result
+            const lengthPerPart = 16000
+            const charsLength = content.length
+            for (var i = 0; i < charsLength; i += lengthPerPart) {{
+                var smallerContent = content.substring(i, i + lengthPerPart)
+                var jsonString = JSON.stringify({{type: "save files",
+                                                  data: smallerContent,
+                                                  end: false}})
+                var dataSent = _send(jsonString)
+            }}
+            var jsonString = JSON.stringify({{type: "save files", data: "",
+                                              end: true}})
+            var dataSent = _send(jsonString)
+        }}
+        reader.readAsText(file)
+    }}
 }}
     
 function _getElement(kwargs) {{
     var number = 0
     if ('number' in kwargs) {{
         var number = parseInt(kwargs['number'])
     }}
@@ -237,14 +289,17 @@
     }}
     if (func == "_goTo") {{
         _goTo(kwargs)
     }}
     if (func == "_getFiles") {{
         _getFiles(kwargs)
     }}
+    if (func == "_saveFile") {{
+        _saveFile(kwargs)
+    }}
 }}"""
 
 def custom_func(name):
     text = f"""
     function {name}(...args) {{
         _toPy('{name}', ...args)
     }}
```

### Comparing `toui-1.1.0b0/toui/apps.py` & `toui-1.2.0a1/toui/apps.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 A module that creates web apps and desktop apps.
 """
 import __main__
-from flask import Flask, session
+from flask import Flask, session, request
 from flask_sock import Sock
+from flask_login import LoginManager, UserMixin, current_user, login_user, logout_user
+from flask_sqlalchemy import SQLAlchemy
 import webview
 import json
 import inspect
 import time
 import os
 from copy import copy
 from abc import ABCMeta, abstractmethod
@@ -123,17 +125,14 @@
 
     See Also
     --------
     :py:class:`toui.pages.Page`
     :py:class:`DesktopApp`
 
     """
-
-    _auth = None
-    _default_vars = {}
     
     def __init__(self, name=None, assets_folder=None, secret_key=None):
         """
 
         Parameters
         ----------
         name: str (optional)
@@ -158,17 +157,21 @@
         if secret_key is None:
             warn("No secret key was set. Generating a random secret key for Flask.")
             secret_key = os.urandom(50)
         self.flask_app.secret_key = secret_key
         self._socket = Sock(self.flask_app)
         self.pages = []
         self._socket.route("/toui-communicate")(self._communicate)
+
         self.forbidden_urls = ['/toui-communicate']
         self._validate_ws = validate_ws
         self._validate_data = validate_data
+        self._auth = None
+        self._default_vars = {}
+        self._user_cls = None
 
     def add_pages(self, *pages, do_copy=False, blueprint=None, endpoint=None):
         """
         Adds pages to the app.
 
         Parameters
         ----------
@@ -310,15 +313,128 @@
             session['user page'] = new_page
             if self._func_exists(func):
                 self._call_func(func, *args)
             del session['user page']
             e = time.time()
             debug(f"TIME: {e - s}s")
 
+    def create_user_database(self, database_uri):
+        """
+        Connects to a database that has data specific to each user.
+
+        The database is a table that contains the following columns: `username`, `password`, and `id`.
+
+        Parameters
+        ----------
+        database_uri
+
+        Returns
+        -------
+
+        """
+        self.flask_app.config['SQLALCHEMY_DATABASE_URI'] = database_uri
+        self._db = SQLAlchemy(self.flask_app)
+        self._login_manager = LoginManager(self.flask_app)
+        self._load_user = self._login_manager.user_loader(self._load_user)
+        class User(UserMixin, self._db.Model):
+            __tablename__ = "user"
+
+            id = self._db.Column(self._db.Integer, primary_key=True)
+            username = self._db.Column(self._db.String(80), unique=True, nullable=False)
+            password = self._db.Column(self._db.String(300), nullable=False, unique=True)
+
+            def __repr__(self):
+                return f'<User {self.username}>'
+        self._user_cls = User
+        with self.flask_app.app_context():
+            self._db.create_all()
+
+    def _load_user(self, user_id):
+        return self._user_cls.get(int(user_id))
+
     # Website-specific methods
+    def get_request(self):
+        """
+        Gets data sent from client using HTTP request.
+
+        This method returns the `request` object of `Flask`. The `request` object has some useful attributes such as
+        `request.files` which retrieves uploaded files.
+
+        Examples
+        --------
+        To use this method, first create the app and a page:
+
+        >>> app = Website(__name__, secret_key="some key")
+        >>> home_page = Page(html_str=\"\"\"<form method="post" enctype="multipart/form-data">
+        ...                              <input type="file" name="filename">
+        ...                              <input type="submit">
+        ...                              </form>\"\"\", url="/")
+
+        Then create a function that will be called when an HTTP request is made:
+
+        >>> def request_function():
+        ...     request = app.get_request()
+        ...     print(request.files)
+
+        Now add the function to `Page.on_url_request()` method:
+
+        >>> home_page.on_url_request(request_function)
+
+        Add the page to the app and run the app:
+
+        >>> app.add_pages(home_page)
+        >>> if __name__ == "__main__":
+        ...     app.run() # doctest: +SKIP
+
+        Returns
+        -------
+        flask.request
+
+        See Also
+        --------
+        flask.request
+            https://flask.palletsprojects.com/en/2.2.x/api/#flask.request
+
+        Page.on_url_request
+
+        """
+        return request
+
+    def signup_user(self, username, password):
+        if self._user_cls is None:
+            raise Exception("You have not created the user database yet.")
+        if self.username_exists(username):
+            return
+        new_user = self._user_cls(username=username, password=password)
+        self._db.session.add(new_user)
+        self._db.session.commit()
+        login_user(new_user)
+
+    def signin_user(self, username, password):
+        if self._user_cls is None:
+            raise Exception("You have not created the user database yet.")
+        user = self._user_cls.query.filter_by(username=username, password=password).first()
+        if user:
+            login_user(user)
+
+    def signout_user(self):
+        logout_user()
+
+    def username_exists(self, username):
+        if self._user_cls is None:
+            raise Exception("You have not created the user database yet.")
+        if self._user_cls.query.filter_by(username=username).first():
+            info("User exists")
+            return True
+        else:
+            return False
+
+    def get_current_user(self):
+        return current_user
+
     def set_restriction(self, username, password):
         """
         Makes the app private.
 
         Adds a username and password to the app.
 
         Parameters
@@ -353,15 +469,14 @@
         --------
         flask_sock
         simple_websockets
 
         """
         self._validate_ws = func
 
-
     def set_data_validation(self, func):
         """
         Validate data received from JavaScript before using it.
 
         ToUI receives data from JavaScript in the form of a JSON object. To validate this data
         before allowing ToUI to use it, input a function that checks the data. This function
         should have one argument `data` and should either return ``True`` or ``False``.
```

### Comparing `toui-1.1.0b0/toui/elements.py` & `toui-1.2.0a1/toui/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,28 +386,33 @@
         value
             The new value of the ``value`` attribute.
 
         """
         self.set_attr("value", value)
 
     @_ElementSignal(return_type="js")
-    def get_files(self, with_content=True):
+    def get_files(self, with_content=False):
         """
         Gets uploaded files from element.
 
         This method is useful when uploading files using ``<input type="file">`` element.
 
         Parameters
         ----------
-        with_content: bool, default=True
+        with_content: bool, default=False
             If ``True``, the contents of the files will be included in the output.
 
         Returns
         -------
-        list(dict)
+        list(File)
+            A list of `File` objects.
+
+        See Also
+        --------
+        ~toui._signals.File
 
         """
         return []
 
     def get_content(self):
         """
         Gets the inner HTML content of the element.
```

### Comparing `toui-1.1.0b0/toui/pages.py` & `toui-1.2.0a1/toui/pages.py`

 * *Files identical despite different names*

### Comparing `toui-1.1.0b0/toui/structure.py` & `toui-1.2.0a1/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-1.1.0b0/toui.egg-info/PKG-INFO` & `toui-1.2.0a1/toui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 1.1.0b0
+Version: 1.2.0a1
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Home-page: UNKNOWN
 Author: Mubarak Almehairbi
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `toui-1.1.0b0/toui.egg-info/SOURCES.txt` & `toui-1.2.0a1/toui.egg-info/SOURCES.txt`

 * *Files identical despite different names*


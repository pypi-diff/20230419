# Comparing `tmp/django_google_sso-2.5.0.tar.gz` & `tmp/django_google_sso-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_google_sso-2.5.0.tar", max compression
+gzip compressed data, was "django_google_sso-3.0.0.tar", max compression
```

## Comparing `django_google_sso-2.5.0.tar` & `django_google_sso-3.0.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
--rw-r--r--   0        0        0     1072 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/LICENSE
--rw-r--r--   0        0        0     2814 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/README.md
--rw-r--r--   0        0        0       22 2023-04-05 16:31:19.329924 django_google_sso-2.5.0/django_google_sso/__init__.py
--rw-r--r--   0        0        0      797 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/admin.py
--rw-r--r--   0        0        0      267 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/apps.py
--rw-r--r--   0        0        0     1463 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/conf.py
--rw-r--r--   0        0        0      242 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/hooks.py
--rw-r--r--   0        0        0     5747 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/main.py
--rw-r--r--   0        0        0     1325 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/migrations/0001_initial.py
--rw-r--r--   0        0        0      396 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/migrations/0002_alter_googlessouser_picture_url.py
--rw-r--r--   0        0        0        0 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/migrations/__init__.py
--rw-r--r--   0        0        0      597 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/models.py
--rw-r--r--   0        0        0     1835 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/templates/admin_sso/login.html
--rw-r--r--   0        0        0        0 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/tests/__init__.py
--rw-r--r--   0        0        0     2586 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/tests/conftest.py
--rw-r--r--   0        0        0      248 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/tests/test_conf.py
--rw-r--r--   0        0        0     2260 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/tests/test_google_auth.py
--rw-r--r--   0        0        0      839 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/tests/test_models.py
--rw-r--r--   0        0        0     2533 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/tests/test_user_helper.py
--rw-r--r--   0        0        0     5478 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/tests/test_views.py
--rw-r--r--   0        0        0      313 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/urls.py
--rw-r--r--   0        0        0     3817 2023-04-05 16:31:07.429905 django_google_sso-2.5.0/django_google_sso/views.py
--rw-r--r--   0        0        0     2183 2023-04-05 16:31:19.329924 django_google_sso-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     3903 1970-01-01 00:00:00.000000 django_google_sso-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2849 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/README.md
+-rw-r--r--   0        0        0       22 2023-04-19 01:06:22.224449 django_google_sso-3.0.0/django_google_sso/__init__.py
+-rw-r--r--   0        0        0     1915 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/admin.py
+-rw-r--r--   0        0        0      267 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/apps.py
+-rw-r--r--   0        0        0     1747 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/conf.py
+-rw-r--r--   0        0        0      242 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/hooks.py
+-rw-r--r--   0        0        0     5787 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/main.py
+-rw-r--r--   0        0        0     1325 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/migrations/0001_initial.py
+-rw-r--r--   0        0        0      396 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/migrations/0002_alter_googlessouser_picture_url.py
+-rw-r--r--   0        0        0        0 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/migrations/__init__.py
+-rw-r--r--   0        0        0      597 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/models.py
+-rw-r--r--   0        0        0      898 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/static/django_google_sso/google_button.css
+-rw-r--r--   0        0        0     2110 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/templates/google_sso/login.html
+-rw-r--r--   0        0        0        0 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/templatetags/__init__.py
+-rw-r--r--   0        0        0     1490 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/templatetags/sso_tags.py
+-rw-r--r--   0        0        0        0 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/tests/__init__.py
+-rw-r--r--   0        0        0     2586 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/tests/conftest.py
+-rw-r--r--   0        0        0      248 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/tests/test_conf.py
+-rw-r--r--   0        0        0     2260 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/tests/test_google_auth.py
+-rw-r--r--   0        0        0      839 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/tests/test_models.py
+-rw-r--r--   0        0        0     2533 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/tests/test_user_helper.py
+-rw-r--r--   0        0        0     5478 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/tests/test_views.py
+-rw-r--r--   0        0        0      313 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/urls.py
+-rw-r--r--   0        0        0     3817 2023-04-19 01:06:07.024413 django_google_sso-3.0.0/django_google_sso/views.py
+-rw-r--r--   0        0        0     2189 2023-04-19 01:06:22.228449 django_google_sso-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3952 1970-01-01 00:00:00.000000 django_google_sso-3.0.0/PKG-INFO
```

### Comparing `django_google_sso-2.5.0/LICENSE` & `django_google_sso-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_google_sso-2.5.0/README.md` & `django_google_sso-3.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -95,14 +95,16 @@
 ```shell
 $ python manage.py migrate
 ```
 
 That's it. Start django on port 8000 and open your browser in `http://localhost:8000/admin/login` and you should see the
 Google SSO button.
 
-![](docs/images/django_login_with_google_white.png)
+<p align="center">
+   <img src="docs/images/django_login_with_google_light.png"/>
+</p>
 
 ---
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

#### html2text {}

```diff
@@ -20,10 +20,10 @@
 auto create users for allowable domains: ```python # settings.py
 GOOGLE_SSO_ALLOWABLE_DOMAINS = ["example.com"] ``` 5. In `urls.py` please add
 the **Django-Google-SSO** views: ```python # urls.py from django.urls import
 include, path urlpatterns = [ # other urlpatterns... path( "google_sso/",
 include("django_google_sso.urls", namespace="django_google_sso") ), ] ``` 6.
 And run migrations: ```shell $ python manage.py migrate ``` That's it. Start
 django on port 8000 and open your browser in `http://localhost:8000/admin/
-login` and you should see the Google SSO button. ![](docs/images/
-django_login_with_google_white.png) --- ## License This project is licensed
-under the terms of the MIT license.
+login` and you should see the Google SSO button.
+               [docs/images/django_login_with_google_light.png]
+--- ## License This project is licensed under the terms of the MIT license.
```

### Comparing `django_google_sso-2.5.0/django_google_sso/conf.py` & `django_google_sso-3.0.0/django_google_sso/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,7 +31,16 @@
 )
 
 GOOGLE_SSO_PRE_LOGIN_CALLBACK = getattr(
     settings,
     "GOOGLE_SSO_PRE_LOGIN_CALLBACK",
     "django_google_sso.hooks.pre_login_user",
 )
+
+GOOGLE_SSO_LOGO_URL = getattr(
+    settings,
+    "GOOGLE_SSO_LOGO_URL",
+    "https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/"
+    "Google_%22G%22_Logo.svg/512px-Google_%22G%22_Logo.svg.png",
+)
+
+GOOGLE_SSO_TEXT = getattr(settings, "GOOGLE_SSO_TEXT", "Sign in with Google")
```

### Comparing `django_google_sso-2.5.0/django_google_sso/main.py` & `django_google_sso-3.0.0/django_google_sso/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,17 @@
     def get_client_config(self) -> Credentials:
         client_config = {
             "web": {
                 "client_id": conf.GOOGLE_SSO_CLIENT_ID,
                 "project_id": conf.GOOGLE_SSO_PROJECT_ID,
                 "client_secret": conf.GOOGLE_SSO_CLIENT_SECRET,
                 "auth_uri": "https://accounts.google.com/o/oauth2/auth",
-                "auth_provider_x509_cert_url": "https://www.googleapis.com/oauth2/v1/certs",
+                "auth_provider_x509_cert_url": (
+                    "https://www.googleapis.com/oauth2/v1/certs"
+                ),
                 "token_uri": "https://oauth2.googleapis.com/token",
                 "redirect_uris": [self.get_redirect_uri()],
             }
         }
         return client_config
 
     def get_netloc(self):
```

### Comparing `django_google_sso-2.5.0/django_google_sso/migrations/0001_initial.py` & `django_google_sso-3.0.0/django_google_sso/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-2.5.0/django_google_sso/models.py` & `django_google_sso-3.0.0/django_google_sso/models.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-2.5.0/django_google_sso/tests/conftest.py` & `django_google_sso-3.0.0/django_google_sso/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-2.5.0/django_google_sso/tests/test_google_auth.py` & `django_google_sso-3.0.0/django_google_sso/tests/test_google_auth.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-2.5.0/django_google_sso/tests/test_models.py` & `django_google_sso-3.0.0/django_google_sso/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-2.5.0/django_google_sso/tests/test_user_helper.py` & `django_google_sso-3.0.0/django_google_sso/tests/test_user_helper.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-2.5.0/django_google_sso/tests/test_views.py` & `django_google_sso-3.0.0/django_google_sso/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-2.5.0/django_google_sso/views.py` & `django_google_sso-3.0.0/django_google_sso/views.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-2.5.0/pyproject.toml` & `django_google_sso-3.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.black]
-target-version = ['py38', 'py39']
+target-version = ['py39']
 include = '\.pyi?$'
 exclude = '''
 (
   /(
       \.eggs         # exclude a few common directories in the
     | \.git          # root of the project
     | \.hg
@@ -37,26 +37,26 @@
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "python -m pip install -U twine poetry && poetry build"
 
 [tool.poetry]
 name = "django-google-sso"
-version = "2.5.0"
-description = "Easily add Google SSO login to Django Admin"
-authors = ["Chris Maillefaud <chrismaillefaud@gmail.com>"]
+version = "3.0.0"
+description = "Easily add Google Authentication to your Django Projects"
+authors = ["Chris Maillefaud <chrismaille@megalus.com.br>"]
 readme = "README.md"
 repository = "https://github.com/megalus/django-google-sso"
 keywords = ["google", "django", "sso"]
 license = "MIT"
 classifiers = [
     "Framework :: Django",
-    "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "Development Status :: 4 - Beta",
     "Environment :: Plugins"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <4.0"
```

### Comparing `django_google_sso-2.5.0/PKG-INFO` & `django_google_sso-3.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-google-sso
-Version: 2.5.0
-Summary: Easily add Google SSO login to Django Admin
+Version: 3.0.0
+Summary: Easily add Google Authentication to your Django Projects
 Home-page: https://github.com/megalus/django-google-sso
 License: MIT
 Keywords: google,django,sso
 Author: Chris Maillefaud
-Author-email: chrismaillefaud@gmail.com
+Author-email: chrismaille@megalus.com.br
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django (>=4.0)
@@ -125,15 +125,17 @@
 ```shell
 $ python manage.py migrate
 ```
 
 That's it. Start django on port 8000 and open your browser in `http://localhost:8000/admin/login` and you should see the
 Google SSO button.
 
-![](docs/images/django_login_with_google_white.png)
+<p align="center">
+   <img src="docs/images/django_login_with_google_light.png"/>
+</p>
 
 ---
 
 ## License
 
 This project is licensed under the terms of the MIT license.
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: django-google-sso Version: 2.5.0 Summary: Easily
-add Google SSO login to Django Admin Home-page: https://github.com/megalus/
-django-google-sso License: MIT Keywords: google,django,sso Author: Chris
-Maillefaud Author-email: chrismaillefaud@gmail.com Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 4 - Beta Classifier: Environment :: Plugins
-Classifier: Framework :: Django Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0 Classifier: Framework :: Django :: 4.1
-Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
-:: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: django (>=4.0) Requires-Dist: google-auth Requires-Dist: google-auth-
-httplib2 Requires-Dist: google-auth-oauthlib Requires-Dist: loguru Project-URL:
-Repository, https://github.com/megalus/django-google-sso Description-Content-
-Type: text/markdown
+Metadata-Version: 2.1 Name: django-google-sso Version: 3.0.0 Summary: Easily
+add Google Authentication to your Django Projects Home-page: https://
+github.com/megalus/django-google-sso License: MIT Keywords: google,django,sso
+Author: Chris Maillefaud Author-email: chrismaille@megalus.com.br Requires-
+Python: >=3.9,<4.0 Classifier: Development Status :: 4 - Beta Classifier:
+Environment :: Plugins Classifier: Framework :: Django Classifier: Framework ::
+Django :: 4.0 Classifier: Framework :: Django :: 4.1 Classifier: Framework ::
+Django :: 4.2 Classifier: Intended Audience :: Developers Classifier: License
+:: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: django (>=4.0) Requires-Dist: google-auth Requires-Dist: google-
+auth-httplib2 Requires-Dist: google-auth-oauthlib Requires-Dist: loguru
+Project-URL: Repository, https://github.com/megalus/django-google-sso
+Description-Content-Type: text/markdown
                               [Django Google SSO]
        Easily integrate Google Authentication into your Django projects
         [PyPI] [Build] [PyPI_-_Python_Version] [PyPI_-_Django_Version]
 ## Welcome to Django Google SSO This library aims to simplify the process of
 authenticating users with Google in Django Admin pages, inspired by libraries
 like [django_microsoft_auth](https://github.com/AngellusMortis/
 django_microsoft_auth) and [django-admin-sso](https://github.com/matthiask/
@@ -35,10 +35,10 @@
 auto create users for allowable domains: ```python # settings.py
 GOOGLE_SSO_ALLOWABLE_DOMAINS = ["example.com"] ``` 5. In `urls.py` please add
 the **Django-Google-SSO** views: ```python # urls.py from django.urls import
 include, path urlpatterns = [ # other urlpatterns... path( "google_sso/",
 include("django_google_sso.urls", namespace="django_google_sso") ), ] ``` 6.
 And run migrations: ```shell $ python manage.py migrate ``` That's it. Start
 django on port 8000 and open your browser in `http://localhost:8000/admin/
-login` and you should see the Google SSO button. ![](docs/images/
-django_login_with_google_white.png) --- ## License This project is licensed
-under the terms of the MIT license.
+login` and you should see the Google SSO button.
+               [docs/images/django_login_with_google_light.png]
+--- ## License This project is licensed under the terms of the MIT license.
```


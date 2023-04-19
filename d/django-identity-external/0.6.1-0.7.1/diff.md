# Comparing `tmp/django-identity-external-0.6.1.tar.gz` & `tmp/django-identity-external-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-identity-external-0.6.1.tar", last modified: Wed May  8 21:13:14 2019, max compression
+gzip compressed data, was "django-identity-external-0.7.1.tar", last modified: Wed Apr 19 19:27:09 2023, max compression
```

## Comparing `django-identity-external-0.6.1.tar` & `django-identity-external-0.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adelton   (1000) adelton   (1000)        0 2019-05-08 21:13:14.000000 django-identity-external-0.6.1/
--rw-rw-r--   0 adelton   (1000) adelton   (1000)    11358 2018-12-17 22:08:23.000000 django-identity-external-0.6.1/LICENSE
--rw-rw-r--   0 adelton   (1000) adelton   (1000)       59 2019-05-08 20:34:13.000000 django-identity-external-0.6.1/MANIFEST.in
--rw-rw-r--   0 adelton   (1000) adelton   (1000)     5002 2019-05-08 21:13:14.000000 django-identity-external-0.6.1/PKG-INFO
--rw-rw-r--   0 adelton   (1000) adelton   (1000)     3126 2019-05-08 21:11:40.000000 django-identity-external-0.6.1/README
--rw-rw-r--   0 adelton   (1000) adelton   (1000)     3367 2019-05-08 21:11:40.000000 django-identity-external-0.6.1/README.rst
-drwxrwxr-x   0 adelton   (1000) adelton   (1000)        0 2019-05-08 21:13:14.000000 django-identity-external-0.6.1/django_identity_external.egg-info/
--rw-rw-r--   0 adelton   (1000) adelton   (1000)     5002 2019-05-08 21:13:14.000000 django-identity-external-0.6.1/django_identity_external.egg-info/PKG-INFO
--rw-rw-r--   0 adelton   (1000) adelton   (1000)      327 2019-05-08 21:13:14.000000 django-identity-external-0.6.1/django_identity_external.egg-info/SOURCES.txt
--rw-rw-r--   0 adelton   (1000) adelton   (1000)        1 2019-05-08 21:13:14.000000 django-identity-external-0.6.1/django_identity_external.egg-info/dependency_links.txt
--rw-rw-r--   0 adelton   (1000) adelton   (1000)       12 2019-05-08 21:13:14.000000 django-identity-external-0.6.1/django_identity_external.egg-info/requires.txt
--rw-rw-r--   0 adelton   (1000) adelton   (1000)        9 2019-05-08 21:13:14.000000 django-identity-external-0.6.1/django_identity_external.egg-info/top_level.txt
-drwxrwxr-x   0 adelton   (1000) adelton   (1000)        0 2019-05-08 21:13:14.000000 django-identity-external-0.6.1/identity/
--rw-rw-r--   0 adelton   (1000) adelton   (1000)        0 2018-12-17 22:08:23.000000 django-identity-external-0.6.1/identity/__init__.py
--rw-rw-r--   0 adelton   (1000) adelton   (1000)     2847 2019-05-08 21:12:29.000000 django-identity-external-0.6.1/identity/external.py
--rw-rw-r--   0 adelton   (1000) adelton   (1000)       38 2019-05-08 21:13:14.000000 django-identity-external-0.6.1/setup.cfg
--rw-rw-r--   0 adelton   (1000) adelton   (1000)     1318 2019-05-08 21:12:41.000000 django-identity-external-0.6.1/setup.py
+drwxr-xr-x   0 adelton   (1000) adelton   (1000)        0 2023-04-19 19:27:09.877152 django-identity-external-0.7.1/
+-rw-rw-r--   0 adelton   (1000) adelton   (1000)    11358 2018-12-17 22:08:23.000000 django-identity-external-0.7.1/LICENSE
+-rw-rw-r--   0 adelton   (1000) adelton   (1000)       59 2019-05-08 20:34:13.000000 django-identity-external-0.7.1/MANIFEST.in
+-rw-r--r--   0 adelton   (1000) adelton   (1000)     4437 2023-04-19 19:27:09.876152 django-identity-external-0.7.1/PKG-INFO
+-rw-r--r--   0 adelton   (1000) adelton   (1000)     3325 2023-04-04 08:06:18.000000 django-identity-external-0.7.1/README
+-rw-r--r--   0 adelton   (1000) adelton   (1000)     3574 2023-04-04 08:06:18.000000 django-identity-external-0.7.1/README.rst
+drwxr-xr-x   0 adelton   (1000) adelton   (1000)        0 2023-04-19 19:27:09.876152 django-identity-external-0.7.1/django_identity_external.egg-info/
+-rw-rw-r--   0 adelton   (1000) adelton   (1000)     4437 2023-04-19 19:27:09.000000 django-identity-external-0.7.1/django_identity_external.egg-info/PKG-INFO
+-rw-rw-r--   0 adelton   (1000) adelton   (1000)      327 2023-04-19 19:27:09.000000 django-identity-external-0.7.1/django_identity_external.egg-info/SOURCES.txt
+-rw-rw-r--   0 adelton   (1000) adelton   (1000)        1 2023-04-19 19:27:09.000000 django-identity-external-0.7.1/django_identity_external.egg-info/dependency_links.txt
+-rw-rw-r--   0 adelton   (1000) adelton   (1000)       12 2023-04-19 19:27:09.000000 django-identity-external-0.7.1/django_identity_external.egg-info/requires.txt
+-rw-rw-r--   0 adelton   (1000) adelton   (1000)        9 2023-04-19 19:27:09.000000 django-identity-external-0.7.1/django_identity_external.egg-info/top_level.txt
+drwxr-xr-x   0 adelton   (1000) adelton   (1000)        0 2023-04-19 19:27:09.876152 django-identity-external-0.7.1/identity/
+-rw-rw-r--   0 adelton   (1000) adelton   (1000)        0 2018-12-17 22:08:23.000000 django-identity-external-0.7.1/identity/__init__.py
+-rw-r--r--   0 adelton   (1000) adelton   (1000)     3196 2023-04-19 19:24:15.000000 django-identity-external-0.7.1/identity/external.py
+-rw-r--r--   0 adelton   (1000) adelton   (1000)       38 2023-04-19 19:27:09.877152 django-identity-external-0.7.1/setup.cfg
+-rw-r--r--   0 adelton   (1000) adelton   (1000)     1221 2023-04-19 19:24:15.000000 django-identity-external-0.7.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-identity-external-0.6.1/LICENSE` & `django-identity-external-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-identity-external-0.6.1/PKG-INFO` & `django-identity-external-0.7.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,112 +1,115 @@
 Metadata-Version: 2.1
 Name: django-identity-external
-Version: 0.6.1
+Version: 0.7.1
 Summary: Django middleware for handling of external identities.
 Home-page: https://github.com/adelton/django-identity-external
 Author: Jan Pazdziora
 Author-email: jan.pazdziora@django.adelton.com
 License: Apache 2.0 License
-Description: 
-        ====================================================
-        	Django identity.external middlewares
-        ====================================================
-        
-        Set of middlewares to simplify consumption of external identity
-        information in Web projects set up with Django Web framework.
-        
-        ---------------------------------------------------
-        identity.external.PersistentRemoteUserMiddlewareVar
-        ---------------------------------------------------
-        
-        When non-standard (different than ``REMOTE_USER``) environment variable is
-        used to pass information about externally authenticated user, this
-        middleware can be used to customize the variable name without writing
-        Python code.
-        
-        For example, when consuming the information from some authentication
-        HTTP proxy, HTTP request header values are passed as ``HTTP_``-prefixed
-        environment variables. If the authenticated user name is in ``X-Remote-User``
-        HTTP request header, it is available in ``HTTP_X_REMOTE_USER``
-        environment variable. Setting variable ``REMOTE_USER_VAR`` to
-        ``HTTP_X_REMOTE_USER``, for example with Apache HTTP Server directive ::
-        
-        	SetEnv REMOTE_USER_VAR HTTP_X_REMOTE_USER
-        
-        and enabling ``identity.external.PersistentRemoteUserMiddlewareVar`` in
-        ``MIDDLEWARE`` list after
-        ``django.contrib.auth.middleware.AuthenticationMiddleware`` like ::
-        
-        	MIDDLEWARE = [
-        		...
-        		'django.contrib.auth.middleware.AuthenticationMiddleware',
-        		'identity.external.PersistentRemoteUserMiddlewareVar',
-        		...
-        	]
-        
-        will run ``django.contrib.auth.middleware.PersistentRemoteUserMiddleware``
-        with value from environment variable ``HTTP_X_REMOTE_USER``.
-        
-        ------------------------------------------
-        identity.external.RemoteUserAttrMiddleware
-        ------------------------------------------
-        
-        When user is externally authenticated, for example via
-        ``django.contrib.auth.middleware.RemoteUserMiddleware`` or
-        ``django.contrib.auth.middleware.PersistentRemoteUserMiddleware``, additional
-        user attributes can be provided by the external authentication source.
-        
-        This middleware will update user's email address, first and last name,
-        and group membership in groups prefixed with ext: with information coming
-        from environment variables
-        
-        - ``REMOTE_USER_EMAIL``
-        - ``REMOTE_USER_FIRSTNAME``
-        - ``REMOTE_USER_LASTNAME``
-        - ``REMOTE_USER_GROUP_N``
-        - ``REMOTE_USER_GROUP_1``, ``REMOTE_USER_GROUP_2``, ...
-        - ``REMOTE_USER_GROUPS``
-        
-        where the ``REMOTE_USER`` prefix of these variables can be changed with the
-        ``REMOTE_USER_VAR`` environment variable, just like with
-        ``identity.external.PersistentRemoteUserMiddlewareVar``.
-        
-        Users that are in external group ``admins`` (and thus get assigned to group
-        ``ext:admins`` in Django) will also get the ``is_staff`` flag set and thus
-        will be able to log in to the admin application.
-        
-        The ``ext:`` prefixed groups have to be already created in Django database for
-        the user membership to be updated in them.
-        
-        In the ``MIDDLEWARE`` list, this middleware has to be listed after the
-        authenticating middleware, for example ::
-        
-        	MIDDLEWARE = [
-        	    ...
-        	    'django.contrib.auth.middleware.AuthenticationMiddleware',
-        	    'django.contrib.auth.middleware.PersistentRemoteUserMiddleware',
-        	    'identity.external.RemoteUserAttrMiddleware',
-        	    ...
-        	]
-        
-        --------
-        See also
-        --------
-        
-        - *External authentication for Django projects*:
-          https://www.adelton.com/django/external-authentication-for-django-projects
-          Presentation at EuroPython 2015.
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.0
+Classifier: Framework :: Django :: 4
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+
+====================================================
+	Django identity.external middlewares
+====================================================
+
+Set of middlewares to simplify consumption of external identity
+information in Web projects set up with Django Web framework.
+
+---------------------------------------------------
+identity.external.PersistentRemoteUserMiddlewareVar
+---------------------------------------------------
+
+When non-standard (different than ``REMOTE_USER``) environment variable is
+used to pass information about externally authenticated user, this
+middleware can be used to customize the variable name without writing
+Python code.
+
+For example, when consuming the information from some authentication
+HTTP proxy, HTTP request header values are passed as ``HTTP_``-prefixed
+environment variables. If the authenticated user name is in ``X-Remote-User``
+HTTP request header, it is available in ``HTTP_X_REMOTE_USER``
+environment variable. Setting variable ``REMOTE_USER_VAR`` to
+``HTTP_X_REMOTE_USER``, for example with Apache HTTP Server directive ::
+
+	SetEnv REMOTE_USER_VAR HTTP_X_REMOTE_USER
+
+and enabling ``identity.external.PersistentRemoteUserMiddlewareVar`` in
+``MIDDLEWARE`` list after
+``django.contrib.auth.middleware.AuthenticationMiddleware`` like ::
+
+	MIDDLEWARE = [
+		...
+		'django.contrib.auth.middleware.AuthenticationMiddleware',
+		'identity.external.PersistentRemoteUserMiddlewareVar',
+		...
+	]
+
+will run ``django.contrib.auth.middleware.PersistentRemoteUserMiddleware``
+with value from environment variable ``HTTP_X_REMOTE_USER``.
+
+------------------------------------------
+identity.external.RemoteUserAttrMiddleware
+------------------------------------------
+
+When user is externally authenticated, for example via
+``django.contrib.auth.middleware.RemoteUserMiddleware`` or
+``django.contrib.auth.middleware.PersistentRemoteUserMiddleware``, additional
+user attributes can be provided by the external authentication source.
+
+This middleware will update user's email address, first and last name,
+and group membership in groups prefixed with ext: with information coming
+from environment variables
+
+- ``REMOTE_USER_EMAIL``
+- ``REMOTE_USER_FIRSTNAME``
+- ``REMOTE_USER_LASTNAME``
+- ``REMOTE_USER_GROUP_N``
+- ``REMOTE_USER_GROUP_1``, ``REMOTE_USER_GROUP_2``, ...
+- ``REMOTE_USER_GROUPS``
+
+where the ``REMOTE_USER`` prefix of these variables can be changed with the
+``REMOTE_USER_VAR`` environment variable, just like with
+``identity.external.PersistentRemoteUserMiddlewareVar``.
+
+The values are used verbating, as provided by Django. When
+``REMOTE_USER_VALUES_ENCODING`` environment variable is set to ``base64url``,
+the values are expected to be in this format and decoded to Unicode.
+
+Users that are in external group ``admins`` (and thus get assigned to group
+``ext:admins`` in Django) will also get the ``is_staff`` flag set and thus
+will be able to log in to the admin application.
+
+The ``ext:`` prefixed groups have to be already created in Django database for
+the user membership to be updated in them.
+
+In the ``MIDDLEWARE`` list, this middleware has to be listed after the
+authenticating middleware, for example ::
+
+	MIDDLEWARE = [
+	    ...
+	    'django.contrib.auth.middleware.AuthenticationMiddleware',
+	    'django.contrib.auth.middleware.PersistentRemoteUserMiddleware',
+	    'identity.external.RemoteUserAttrMiddleware',
+	    ...
+	]
+
+--------
+See also
+--------
+
+- *External authentication for Django projects*:
+  https://www.adelton.com/django/external-authentication-for-django-projects
+  Presentation at EuroPython 2015.
```

### Comparing `django-identity-external-0.6.1/README` & `django-identity-external-0.7.1/README`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,18 @@
 	REMOTE_USER_GROUP_1, REMOTE_USER_GROUP_2, ...
 	REMOTE_USER_GROUPS
 
 where the REMOTE_USER prefix of these variables can be changed with the
 REMOTE_USER_VAR environment variable, just like with
 identity.external.PersistentRemoteUserMiddlewareVar.
 
+The values are used verbating, as provided by Django. When
+REMOTE_USER_VALUES_ENCODING environment variable is set to base64url,
+the values are expected to be in this format and decoded to Unicode.
+
 Users that are in external group admins (and thus get assigned to group
 ext:admins in Django) will also get the is_staff flag set and thus will be
 able to log in to the admin application.
 
 The ext: prefixed groups have to be already created in Django database for
 the user membership to be updated in them.
```

### Comparing `django-identity-external-0.6.1/README.rst` & `django-identity-external-0.7.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,18 @@
 - ``REMOTE_USER_GROUP_1``, ``REMOTE_USER_GROUP_2``, ...
 - ``REMOTE_USER_GROUPS``
 
 where the ``REMOTE_USER`` prefix of these variables can be changed with the
 ``REMOTE_USER_VAR`` environment variable, just like with
 ``identity.external.PersistentRemoteUserMiddlewareVar``.
 
+The values are used verbating, as provided by Django. When
+``REMOTE_USER_VALUES_ENCODING`` environment variable is set to ``base64url``,
+the values are expected to be in this format and decoded to Unicode.
+
 Users that are in external group ``admins`` (and thus get assigned to group
 ``ext:admins`` in Django) will also get the ``is_staff`` flag set and thus
 will be able to log in to the admin application.
 
 The ``ext:`` prefixed groups have to be already created in Django database for
 the user membership to be updated in them.
```

### Comparing `django-identity-external-0.6.1/django_identity_external.egg-info/PKG-INFO` & `django-identity-external-0.7.1/django_identity_external.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,112 +1,115 @@
 Metadata-Version: 2.1
 Name: django-identity-external
-Version: 0.6.1
+Version: 0.7.1
 Summary: Django middleware for handling of external identities.
 Home-page: https://github.com/adelton/django-identity-external
 Author: Jan Pazdziora
 Author-email: jan.pazdziora@django.adelton.com
 License: Apache 2.0 License
-Description: 
-        ====================================================
-        	Django identity.external middlewares
-        ====================================================
-        
-        Set of middlewares to simplify consumption of external identity
-        information in Web projects set up with Django Web framework.
-        
-        ---------------------------------------------------
-        identity.external.PersistentRemoteUserMiddlewareVar
-        ---------------------------------------------------
-        
-        When non-standard (different than ``REMOTE_USER``) environment variable is
-        used to pass information about externally authenticated user, this
-        middleware can be used to customize the variable name without writing
-        Python code.
-        
-        For example, when consuming the information from some authentication
-        HTTP proxy, HTTP request header values are passed as ``HTTP_``-prefixed
-        environment variables. If the authenticated user name is in ``X-Remote-User``
-        HTTP request header, it is available in ``HTTP_X_REMOTE_USER``
-        environment variable. Setting variable ``REMOTE_USER_VAR`` to
-        ``HTTP_X_REMOTE_USER``, for example with Apache HTTP Server directive ::
-        
-        	SetEnv REMOTE_USER_VAR HTTP_X_REMOTE_USER
-        
-        and enabling ``identity.external.PersistentRemoteUserMiddlewareVar`` in
-        ``MIDDLEWARE`` list after
-        ``django.contrib.auth.middleware.AuthenticationMiddleware`` like ::
-        
-        	MIDDLEWARE = [
-        		...
-        		'django.contrib.auth.middleware.AuthenticationMiddleware',
-        		'identity.external.PersistentRemoteUserMiddlewareVar',
-        		...
-        	]
-        
-        will run ``django.contrib.auth.middleware.PersistentRemoteUserMiddleware``
-        with value from environment variable ``HTTP_X_REMOTE_USER``.
-        
-        ------------------------------------------
-        identity.external.RemoteUserAttrMiddleware
-        ------------------------------------------
-        
-        When user is externally authenticated, for example via
-        ``django.contrib.auth.middleware.RemoteUserMiddleware`` or
-        ``django.contrib.auth.middleware.PersistentRemoteUserMiddleware``, additional
-        user attributes can be provided by the external authentication source.
-        
-        This middleware will update user's email address, first and last name,
-        and group membership in groups prefixed with ext: with information coming
-        from environment variables
-        
-        - ``REMOTE_USER_EMAIL``
-        - ``REMOTE_USER_FIRSTNAME``
-        - ``REMOTE_USER_LASTNAME``
-        - ``REMOTE_USER_GROUP_N``
-        - ``REMOTE_USER_GROUP_1``, ``REMOTE_USER_GROUP_2``, ...
-        - ``REMOTE_USER_GROUPS``
-        
-        where the ``REMOTE_USER`` prefix of these variables can be changed with the
-        ``REMOTE_USER_VAR`` environment variable, just like with
-        ``identity.external.PersistentRemoteUserMiddlewareVar``.
-        
-        Users that are in external group ``admins`` (and thus get assigned to group
-        ``ext:admins`` in Django) will also get the ``is_staff`` flag set and thus
-        will be able to log in to the admin application.
-        
-        The ``ext:`` prefixed groups have to be already created in Django database for
-        the user membership to be updated in them.
-        
-        In the ``MIDDLEWARE`` list, this middleware has to be listed after the
-        authenticating middleware, for example ::
-        
-        	MIDDLEWARE = [
-        	    ...
-        	    'django.contrib.auth.middleware.AuthenticationMiddleware',
-        	    'django.contrib.auth.middleware.PersistentRemoteUserMiddleware',
-        	    'identity.external.RemoteUserAttrMiddleware',
-        	    ...
-        	]
-        
-        --------
-        See also
-        --------
-        
-        - *External authentication for Django projects*:
-          https://www.adelton.com/django/external-authentication-for-django-projects
-          Presentation at EuroPython 2015.
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.0
+Classifier: Framework :: Django :: 4
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+
+====================================================
+	Django identity.external middlewares
+====================================================
+
+Set of middlewares to simplify consumption of external identity
+information in Web projects set up with Django Web framework.
+
+---------------------------------------------------
+identity.external.PersistentRemoteUserMiddlewareVar
+---------------------------------------------------
+
+When non-standard (different than ``REMOTE_USER``) environment variable is
+used to pass information about externally authenticated user, this
+middleware can be used to customize the variable name without writing
+Python code.
+
+For example, when consuming the information from some authentication
+HTTP proxy, HTTP request header values are passed as ``HTTP_``-prefixed
+environment variables. If the authenticated user name is in ``X-Remote-User``
+HTTP request header, it is available in ``HTTP_X_REMOTE_USER``
+environment variable. Setting variable ``REMOTE_USER_VAR`` to
+``HTTP_X_REMOTE_USER``, for example with Apache HTTP Server directive ::
+
+	SetEnv REMOTE_USER_VAR HTTP_X_REMOTE_USER
+
+and enabling ``identity.external.PersistentRemoteUserMiddlewareVar`` in
+``MIDDLEWARE`` list after
+``django.contrib.auth.middleware.AuthenticationMiddleware`` like ::
+
+	MIDDLEWARE = [
+		...
+		'django.contrib.auth.middleware.AuthenticationMiddleware',
+		'identity.external.PersistentRemoteUserMiddlewareVar',
+		...
+	]
+
+will run ``django.contrib.auth.middleware.PersistentRemoteUserMiddleware``
+with value from environment variable ``HTTP_X_REMOTE_USER``.
+
+------------------------------------------
+identity.external.RemoteUserAttrMiddleware
+------------------------------------------
+
+When user is externally authenticated, for example via
+``django.contrib.auth.middleware.RemoteUserMiddleware`` or
+``django.contrib.auth.middleware.PersistentRemoteUserMiddleware``, additional
+user attributes can be provided by the external authentication source.
+
+This middleware will update user's email address, first and last name,
+and group membership in groups prefixed with ext: with information coming
+from environment variables
+
+- ``REMOTE_USER_EMAIL``
+- ``REMOTE_USER_FIRSTNAME``
+- ``REMOTE_USER_LASTNAME``
+- ``REMOTE_USER_GROUP_N``
+- ``REMOTE_USER_GROUP_1``, ``REMOTE_USER_GROUP_2``, ...
+- ``REMOTE_USER_GROUPS``
+
+where the ``REMOTE_USER`` prefix of these variables can be changed with the
+``REMOTE_USER_VAR`` environment variable, just like with
+``identity.external.PersistentRemoteUserMiddlewareVar``.
+
+The values are used verbating, as provided by Django. When
+``REMOTE_USER_VALUES_ENCODING`` environment variable is set to ``base64url``,
+the values are expected to be in this format and decoded to Unicode.
+
+Users that are in external group ``admins`` (and thus get assigned to group
+``ext:admins`` in Django) will also get the ``is_staff`` flag set and thus
+will be able to log in to the admin application.
+
+The ``ext:`` prefixed groups have to be already created in Django database for
+the user membership to be updated in them.
+
+In the ``MIDDLEWARE`` list, this middleware has to be listed after the
+authenticating middleware, for example ::
+
+	MIDDLEWARE = [
+	    ...
+	    'django.contrib.auth.middleware.AuthenticationMiddleware',
+	    'django.contrib.auth.middleware.PersistentRemoteUserMiddleware',
+	    'identity.external.RemoteUserAttrMiddleware',
+	    ...
+	]
+
+--------
+See also
+--------
+
+- *External authentication for Django projects*:
+  https://www.adelton.com/django/external-authentication-for-django-projects
+  Presentation at EuroPython 2015.
```

### Comparing `django-identity-external-0.6.1/identity/external.py` & `django-identity-external-0.7.1/identity/external.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 
-# Copyright 2016 Jan Pazdziora
+# Copyright 2016--2023 Jan Pazdziora
 #
 # Licensed under the Apache License, Version 2.0 (the "License").
 
 from django.contrib.auth import load_backend, BACKEND_SESSION_KEY
 from django.contrib.auth.models import Group
 from django.contrib.auth.backends import RemoteUserBackend
 from django.contrib.auth.middleware import RemoteUserMiddleware
 
 from django.contrib.auth.middleware import PersistentRemoteUserMiddleware
+import base64
 
 class PersistentRemoteUserMiddlewareVar(PersistentRemoteUserMiddleware):
 	def process_request(self, request):
 		self.header = request.META.get("REMOTE_USER_VAR", "REMOTE_USER")
 		return super(PersistentRemoteUserMiddleware, self).process_request(request)
 
+def _decode_value(request, value):
+	if value is not None \
+		and request.META.get("REMOTE_USER_VALUES_ENCODING", "none") == "base64url":
+		return base64.urlsafe_b64decode(value + "==").decode()
+	return value
+
 class RemoteUserAttrMiddleware(RemoteUserMiddleware):
 	group_prefix = 'ext:'
 	staff_group = 'ext:admins'
 
 	def update_user_groups(self, request):
 		user = request.user
 
 		ext_groups = []
 		ext_group_count = request.META.get(self.header + "_GROUP_N", None)
 		ext_groups_singlestring = request.META.get(self.header + "_GROUPS", None)
 		if ext_group_count is not None:
 			for i in range(1, int(ext_group_count) + 1):
 				g = request.META.get(self.header + "_GROUP_" + str(i), None)
 				if g is not None:
-					ext_groups.append(g)
+					ext_groups.append(_decode_value(request, g))
 		elif ext_groups_singlestring is not None:
-			ext_groups = ext_groups_singlestring.split(':')
+			ext_groups = _decode_value(request, ext_groups_singlestring).split(':')
 		else:
 			return
 
 		current_groups = {}
 		for g in user.groups.filter(name__startswith=self.group_prefix):
 			current_groups[g.name] = g
 
@@ -61,20 +68,20 @@
 		   request.user.get_username() == self.clean_username(request.META[self.header], request):
 			stored_backend = load_backend(request.session.get(BACKEND_SESSION_KEY, ''))
 			if isinstance(stored_backend, RemoteUserBackend):
 				user = request.user
 				need_save = False
 				email = request.META.get(self.header + "_EMAIL", None)
 				if email is not None:
-					user.email = email
+					user.email = _decode_value(request, email)
 					need_save = True
 				firstname = request.META.get(self.header + "_FIRSTNAME", None)
 				if firstname is not None:
-					user.first_name = firstname
+					user.first_name = _decode_value(request, firstname)
 					need_save = True
 				lastname = request.META.get(self.header + "_LASTNAME", None)
 				if lastname is not None:
-					user.last_name = lastname
+					user.last_name = _decode_value(request, lastname)
 					need_save = True
 				if need_save or request.META.get(self.header + "_GROUP_N", None) or request.META.get(self.header + "_GROUPS", None):
 					self.update_user_groups(request)
 					user.save()
```

### Comparing `django-identity-external-0.6.1/setup.py` & `django-identity-external-0.7.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 	README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
 	name = 'django-identity-external',
-	version = '0.6.1',
+	version = '0.7.1',
 	packages = find_packages(),
 	include_package_data = True,
 	license = 'Apache 2.0 License',
 	description = 'Django middleware for handling of external identities.',
 	long_description = README,
 	long_description_content_type = 'text/x-rst',
 	url = 'https://github.com/adelton/django-identity-external',
@@ -21,20 +21,18 @@
 	author_email = 'jan.pazdziora@django.adelton.com',
 	install_requires = [
 		'django>=2.0',
 	],
 	classifiers = [
 		'Environment :: Web Environment',
 		'Framework :: Django',
-		# New PersistentRemoteUserMiddleware in Django 1.9
-		'Framework :: Django :: 2.0',
+		'Framework :: Django :: 4',
 		'Intended Audience :: Developers',
 		'License :: OSI Approved :: Apache Software License',
 		'Operating System :: OS Independent',
 		'Programming Language :: Python',
 		'Programming Language :: Python :: 3',
-		'Programming Language :: Python :: 3.4',
-		'Programming Language :: Python :: 3.5',
+		'Programming Language :: Python :: 3.11',
 		'Topic :: Internet :: WWW/HTTP',
 		'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
 	],
 )
```


# Comparing `tmp/fractal-tokens-1.2.0.tar.gz` & `tmp/fractal-tokens-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal-tokens-1.2.0.tar", last modified: Mon Apr 17 12:32:25 2023, max compression
+gzip compressed data, was "fractal-tokens-1.2.1.tar", last modified: Wed Apr 19 15:28:30 2023, max compression
```

## Comparing `fractal-tokens-1.2.0.tar` & `fractal-tokens-1.2.1.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0      187 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/.coveragerc
--rw-r--r--   0        0        0      100 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/.flake8
--rw-r--r--   0        0        0      945 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/.gitignore
--rw-r--r--   0        0        0      161 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/.isort.cfg
--rw-r--r--   0        0        0     1708 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/LICENSE
--rw-r--r--   0        0        0     1470 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/Makefile
--rw-r--r--   0        0        0    22752 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/README.md
--rw-r--r--   0        0        0      780 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/align_version.py
--rw-r--r--   0        0        0        0 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/asymmetric/__init__.py
--rw-r--r--   0        0        0      460 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/asymmetric/app.py
--rw-r--r--   0        0        0      589 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/asymmetric/utils.py
--rw-r--r--   0        0        0        0 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/automatic/__init__.py
--rw-r--r--   0        0        0     2186 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/automatic/app.py
--rw-r--r--   0        0        0      578 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/automatic/utils.py
--rw-r--r--   0        0        0        0 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/dummy/__init__.py
--rw-r--r--   0        0        0      507 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/dummy/app.py
--rw-r--r--   0        0        0        0 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/fastapi_demo/__init__.py
--rw-r--r--   0        0        0     1145 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/fastapi_demo/app.py
--rw-r--r--   0        0        0       33 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/fastapi_demo/requirements.txt
--rw-r--r--   0        0        0     1042 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/fastapi_demo/utils.py
--rw-r--r--   0        0        0        0 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/fastapi_roles_demo/__init__.py
--rw-r--r--   0        0        0     1419 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/fastapi_roles_demo/app.py
--rw-r--r--   0        0        0       47 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/fastapi_roles_demo/requirements.txt
--rw-r--r--   0        0        0     1634 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/fastapi_roles_demo/utils.py
--rw-r--r--   0        0        0        0 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/symmetric/__init__.py
--rw-r--r--   0        0        0      406 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/examples/symmetric/app.py
--rw-r--r--   0        0        0      132 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/fractal_tokens/__init__.py
--rw-r--r--   0        0        0      707 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/fractal_tokens/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-17 12:32:10.567541 fractal-tokens-1.2.0/fractal_tokens/services/__init__.py
--rw-r--r--   0        0        0      898 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/fractal_tokens/services/dummy.py
--rw-r--r--   0        0        0     2907 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/fractal_tokens/services/generic.py
--rw-r--r--   0        0        0     1471 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/fractal_tokens/services/jwk.py
--rw-r--r--   0        0        0      782 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/fractal_tokens/services/jwt/__init__.py
--rw-r--r--   0        0        0     4033 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/fractal_tokens/services/jwt/asymmetric.py
--rw-r--r--   0        0        0     2582 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/fractal_tokens/services/jwt/automatic.py
--rw-r--r--   0        0        0     1008 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/fractal_tokens/services/jwt/symmetric.py
--rw-r--r--   0        0        0      113 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/fractal_tokens/settings.py
--rw-r--r--   0        0        0     1632 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       69 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/setup.py
--rw-r--r--   0        0        0        0 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/conftest.py
--rw-r--r--   0        0        0       89 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      152 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/services/__init__.py
--rw-r--r--   0        0        0      162 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/services/dummy.py
--rw-r--r--   0        0        0     1676 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/services/jwk.py
--rw-r--r--   0        0        0      181 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/services/jwt/__init__.py
--rw-r--r--   0        0        0     2269 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/services/jwt/asymmetric.py
--rw-r--r--   0        0        0      655 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/services/jwt/automatic.py
--rw-r--r--   0        0        0      253 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/services/jwt/symmetric.py
--rw-r--r--   0        0        0       92 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/fixtures/utils.py
--rw-r--r--   0        0        0        0 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/services/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/services/jwt/__init__.py
--rw-r--r--   0        0        0     2749 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/services/jwt/test_asymmetric.py
--rw-r--r--   0        0        0     2225 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/services/jwt/test_automatic.py
--rw-r--r--   0        0        0     1835 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/services/jwt/test_symmetric.py
--rw-r--r--   0        0        0      739 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/services/test_dummy.py
--rw-r--r--   0        0        0      719 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tests/services/test_jwk.py
--rw-r--r--   0        0        0      653 2023-04-17 12:32:10.571541 fractal-tokens-1.2.0/tox.ini
--rw-r--r--   0        0        0    23626 1970-01-01 00:00:00.000000 fractal-tokens-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/.coveragerc
+-rw-r--r--   0        0        0      100 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/.flake8
+-rw-r--r--   0        0        0      945 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/.gitignore
+-rw-r--r--   0        0        0      161 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/.isort.cfg
+-rw-r--r--   0        0        0     1708 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1470 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/Makefile
+-rw-r--r--   0        0        0    22752 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/README.md
+-rw-r--r--   0        0        0      780 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/align_version.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/examples/asymmetric/__init__.py
+-rw-r--r--   0        0        0      460 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/examples/asymmetric/app.py
+-rw-r--r--   0        0        0      589 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/examples/asymmetric/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/examples/automatic/__init__.py
+-rw-r--r--   0        0        0     2186 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/examples/automatic/app.py
+-rw-r--r--   0        0        0      578 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/examples/automatic/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/examples/dummy/__init__.py
+-rw-r--r--   0        0        0      507 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/examples/dummy/app.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:28:12.351519 fractal-tokens-1.2.1/examples/fastapi_demo/__init__.py
+-rw-r--r--   0        0        0     1145 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/examples/fastapi_demo/app.py
+-rw-r--r--   0        0        0       33 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/examples/fastapi_demo/requirements.txt
+-rw-r--r--   0        0        0     1042 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/examples/fastapi_demo/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/examples/fastapi_roles_demo/__init__.py
+-rw-r--r--   0        0        0     1419 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/examples/fastapi_roles_demo/app.py
+-rw-r--r--   0        0        0       47 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/examples/fastapi_roles_demo/requirements.txt
+-rw-r--r--   0        0        0     1602 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/examples/fastapi_roles_demo/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/examples/symmetric/__init__.py
+-rw-r--r--   0        0        0      406 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/examples/symmetric/app.py
+-rw-r--r--   0        0        0      132 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/fractal_tokens/__init__.py
+-rw-r--r--   0        0        0      707 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/fractal_tokens/exceptions.py
+-rw-r--r--   0        0        0       77 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/fractal_tokens/py.typed
+-rw-r--r--   0        0        0        0 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/fractal_tokens/services/__init__.py
+-rw-r--r--   0        0        0      898 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/fractal_tokens/services/dummy.py
+-rw-r--r--   0        0        0     2907 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/fractal_tokens/services/generic.py
+-rw-r--r--   0        0        0     1471 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/fractal_tokens/services/jwk.py
+-rw-r--r--   0        0        0      782 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/fractal_tokens/services/jwt/__init__.py
+-rw-r--r--   0        0        0     4033 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/fractal_tokens/services/jwt/asymmetric.py
+-rw-r--r--   0        0        0     2582 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/fractal_tokens/services/jwt/automatic.py
+-rw-r--r--   0        0        0     1008 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/fractal_tokens/services/jwt/symmetric.py
+-rw-r--r--   0        0        0      113 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/fractal_tokens/settings.py
+-rw-r--r--   0        0        0     1632 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/setup.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/conftest.py
+-rw-r--r--   0        0        0       89 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      152 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/fixtures/services/__init__.py
+-rw-r--r--   0        0        0      162 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/fixtures/services/dummy.py
+-rw-r--r--   0        0        0     1676 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/fixtures/services/jwk.py
+-rw-r--r--   0        0        0      181 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/fixtures/services/jwt/__init__.py
+-rw-r--r--   0        0        0     2269 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/fixtures/services/jwt/asymmetric.py
+-rw-r--r--   0        0        0      655 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/fixtures/services/jwt/automatic.py
+-rw-r--r--   0        0        0      253 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/fixtures/services/jwt/symmetric.py
+-rw-r--r--   0        0        0       92 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/fixtures/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/services/jwt/__init__.py
+-rw-r--r--   0        0        0     2749 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/services/jwt/test_asymmetric.py
+-rw-r--r--   0        0        0     2225 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/services/jwt/test_automatic.py
+-rw-r--r--   0        0        0     1835 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/services/jwt/test_symmetric.py
+-rw-r--r--   0        0        0      739 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/services/test_dummy.py
+-rw-r--r--   0        0        0      719 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tests/services/test_jwk.py
+-rw-r--r--   0        0        0      653 2023-04-19 15:28:12.355519 fractal-tokens-1.2.1/tox.ini
+-rw-r--r--   0        0        0    23626 1970-01-01 00:00:00.000000 fractal-tokens-1.2.1/PKG-INFO
```

### Comparing `fractal-tokens-1.2.0/.github/workflows/build.yml` & `fractal-tokens-1.2.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/.github/workflows/publish.yml` & `fractal-tokens-1.2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/.gitignore` & `fractal-tokens-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/.pre-commit-config.yaml` & `fractal-tokens-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/LICENSE` & `fractal-tokens-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/Makefile` & `fractal-tokens-1.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/README.md` & `fractal-tokens-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/align_version.py` & `fractal-tokens-1.2.1/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/examples/asymmetric/utils.py` & `fractal-tokens-1.2.1/examples/asymmetric/utils.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/examples/automatic/app.py` & `fractal-tokens-1.2.1/examples/automatic/app.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/examples/automatic/utils.py` & `fractal-tokens-1.2.1/examples/automatic/utils.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/examples/fastapi_demo/app.py` & `fractal-tokens-1.2.1/examples/fastapi_demo/app.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/examples/fastapi_demo/utils.py` & `fractal-tokens-1.2.1/examples/fastapi_demo/utils.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/examples/fastapi_roles_demo/app.py` & `fractal-tokens-1.2.1/examples/fastapi_roles_demo/app.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/examples/fastapi_roles_demo/utils.py` & `fractal-tokens-1.2.1/examples/fastapi_roles_demo/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 
 from fastapi import Depends
 from fastapi.security import OAuth2PasswordBearer
-from fractal_roles.models import Role, TokenPayloadRolesMixin  # type: ignore
-from fractal_roles.services import RolesService as BaseRolesService  # type: ignore
+from fractal_roles.models import Role, TokenPayloadRolesMixin
+from fractal_roles.services import RolesService as BaseRolesService
 
 from fractal_tokens.services.generic import TokenPayload, TokenService
 
 oauth2_scheme = OAuth2PasswordBearer(tokenUrl="login")
 
 
 @dataclass
```

### Comparing `fractal-tokens-1.2.0/fractal_tokens/exceptions.py` & `fractal-tokens-1.2.1/fractal_tokens/exceptions.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/fractal_tokens/services/dummy.py` & `fractal-tokens-1.2.1/fractal_tokens/services/dummy.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/fractal_tokens/services/generic.py` & `fractal-tokens-1.2.1/fractal_tokens/services/generic.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/fractal_tokens/services/jwk.py` & `fractal-tokens-1.2.1/fractal_tokens/services/jwk.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/fractal_tokens/services/jwt/__init__.py` & `fractal-tokens-1.2.1/fractal_tokens/services/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/fractal_tokens/services/jwt/asymmetric.py` & `fractal-tokens-1.2.1/fractal_tokens/services/jwt/asymmetric.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/fractal_tokens/services/jwt/automatic.py` & `fractal-tokens-1.2.1/fractal_tokens/services/jwt/automatic.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/fractal_tokens/services/jwt/symmetric.py` & `fractal-tokens-1.2.1/fractal_tokens/services/jwt/symmetric.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/pyproject.toml` & `fractal-tokens-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-tokens"
-version = "1.2.0"
+version = "1.2.1"
 description = "Fractal Tokens provides a flexible way to generate and verify JWT tokens for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
```

### Comparing `fractal-tokens-1.2.0/tests/fixtures/services/jwk.py` & `fractal-tokens-1.2.1/tests/fixtures/services/jwk.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/tests/fixtures/services/jwt/asymmetric.py` & `fractal-tokens-1.2.1/tests/fixtures/services/jwt/asymmetric.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/tests/fixtures/services/jwt/automatic.py` & `fractal-tokens-1.2.1/tests/fixtures/services/jwt/automatic.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/tests/services/jwt/test_asymmetric.py` & `fractal-tokens-1.2.1/tests/services/jwt/test_asymmetric.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/tests/services/jwt/test_automatic.py` & `fractal-tokens-1.2.1/tests/services/jwt/test_automatic.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/tests/services/jwt/test_symmetric.py` & `fractal-tokens-1.2.1/tests/services/jwt/test_symmetric.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/tests/services/test_dummy.py` & `fractal-tokens-1.2.1/tests/services/test_dummy.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/tests/services/test_jwk.py` & `fractal-tokens-1.2.1/tests/services/test_jwk.py`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/tox.ini` & `fractal-tokens-1.2.1/tox.ini`

 * *Files identical despite different names*

### Comparing `fractal-tokens-1.2.0/PKG-INFO` & `fractal-tokens-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-tokens
-Version: 1.2.0
+Version: 1.2.1
 Summary: Fractal Tokens provides a flexible way to generate and verify JWT tokens for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal-tokens
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```


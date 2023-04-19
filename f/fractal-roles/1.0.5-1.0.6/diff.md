# Comparing `tmp/fractal-roles-1.0.5.tar.gz` & `tmp/fractal-roles-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal-roles-1.0.5.tar", last modified: Sun Jan  8 15:50:26 2023, max compression
+gzip compressed data, was "fractal-roles-1.0.6.tar", last modified: Wed Apr 19 15:25:46 2023, max compression
```

## Comparing `fractal-roles-1.0.5.tar` & `fractal-roles-1.0.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0      187 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/.coveragerc
--rw-r--r--   0        0        0      100 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/.flake8
--rw-r--r--   0        0        0      945 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/.gitignore
--rw-r--r--   0        0        0      161 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/.isort.cfg
--rw-r--r--   0        0        0     1707 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/LICENSE
--rw-r--r--   0        0        0     1436 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/Makefile
--rw-r--r--   0        0        0     9356 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/README.md
--rw-r--r--   0        0        0      780 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/align_version.py
--rw-r--r--   0        0        0        0 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/examples/account/__init__.py
--rw-r--r--   0        0        0      553 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/examples/account/app.py
--rw-r--r--   0        0        0     1143 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/examples/account/roles.py
--rw-r--r--   0        0        0        0 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/examples/account_user/__init__.py
--rw-r--r--   0        0        0      597 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/examples/account_user/app.py
--rw-r--r--   0        0        0     1485 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/examples/account_user/roles.py
--rw-r--r--   0        0        0        0 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/examples/alternative/__init__.py
--rw-r--r--   0        0        0      998 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/examples/alternative/app.py
--rw-r--r--   0        0        0     1291 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/examples/alternative/roles.py
--rw-r--r--   0        0        0        0 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/examples/basic/__init__.py
--rw-r--r--   0        0        0      507 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/examples/basic/app.py
--rw-r--r--   0        0        0      357 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/examples/basic/roles.py
--rw-r--r--   0        0        0        0 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/examples/readme/__init__.py
--rw-r--r--   0        0        0      892 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/examples/readme/app.py
--rw-r--r--   0        0        0     1029 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/examples/readme/roles.py
--rw-r--r--   0        0        0      149 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/fractal_roles/__init__.py
--rw-r--r--   0        0        0       46 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/fractal_roles/exceptions.py
--rw-r--r--   0        0        0     1156 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/fractal_roles/models.py
--rw-r--r--   0        0        0     1503 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/fractal_roles/services.py
--rw-r--r--   0        0        0     1636 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/pyproject.toml
--rw-r--r--   0        0        0       69 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/setup.py
--rw-r--r--   0        0        0        0 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/tests/conftest.py
--rw-r--r--   0        0        0     2960 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/tests/fixtures.py
--rw-r--r--   0        0        0      878 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/tests/test_service.py
--rw-r--r--   0        0        0      603 2023-01-08 15:50:11.219346 fractal-roles-1.0.5/tox.ini
--rw-r--r--   0        0        0    10228 1970-01-01 00:00:00.000000 fractal-roles-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/.coveragerc
+-rw-r--r--   0        0        0      100 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/.flake8
+-rw-r--r--   0        0        0      945 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/.gitignore
+-rw-r--r--   0        0        0      161 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/.isort.cfg
+-rw-r--r--   0        0        0     1707 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1436 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/Makefile
+-rw-r--r--   0        0        0     9356 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/README.md
+-rw-r--r--   0        0        0      780 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/align_version.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/examples/account/__init__.py
+-rw-r--r--   0        0        0      553 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/examples/account/app.py
+-rw-r--r--   0        0        0     1111 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/examples/account/roles.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/examples/account_user/__init__.py
+-rw-r--r--   0        0        0      597 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/examples/account_user/app.py
+-rw-r--r--   0        0        0     1453 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/examples/account_user/roles.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/examples/alternative/__init__.py
+-rw-r--r--   0        0        0      998 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/examples/alternative/app.py
+-rw-r--r--   0        0        0     1259 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/examples/alternative/roles.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/examples/basic/__init__.py
+-rw-r--r--   0        0        0      507 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/examples/basic/app.py
+-rw-r--r--   0        0        0      357 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/examples/basic/roles.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/examples/readme/__init__.py
+-rw-r--r--   0        0        0      892 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/examples/readme/app.py
+-rw-r--r--   0        0        0      997 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/examples/readme/roles.py
+-rw-r--r--   0        0        0      149 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/fractal_roles/__init__.py
+-rw-r--r--   0        0        0       46 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/fractal_roles/exceptions.py
+-rw-r--r--   0        0        0     1140 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/fractal_roles/models.py
+-rw-r--r--   0        0        0       77 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/fractal_roles/py.typed
+-rw-r--r--   0        0        0     1503 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/fractal_roles/services.py
+-rw-r--r--   0        0        0     1636 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/setup.py
+-rw-r--r--   0        0        0        0 2023-04-19 15:25:32.335974 fractal-roles-1.0.6/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-19 15:25:32.339974 fractal-roles-1.0.6/tests/conftest.py
+-rw-r--r--   0        0        0     2928 2023-04-19 15:25:32.339974 fractal-roles-1.0.6/tests/fixtures.py
+-rw-r--r--   0        0        0      878 2023-04-19 15:25:32.339974 fractal-roles-1.0.6/tests/test_service.py
+-rw-r--r--   0        0        0      603 2023-04-19 15:25:32.339974 fractal-roles-1.0.6/tox.ini
+-rw-r--r--   0        0        0    10228 1970-01-01 00:00:00.000000 fractal-roles-1.0.6/PKG-INFO
```

### Comparing `fractal-roles-1.0.5/.github/workflows/build.yml` & `fractal-roles-1.0.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal-roles-1.0.5/.github/workflows/publish.yml` & `fractal-roles-1.0.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal-roles-1.0.5/.gitignore` & `fractal-roles-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal-roles-1.0.5/.pre-commit-config.yaml` & `fractal-roles-1.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal-roles-1.0.5/LICENSE` & `fractal-roles-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal-roles-1.0.5/Makefile` & `fractal-roles-1.0.6/Makefile`

 * *Files identical despite different names*

### Comparing `fractal-roles-1.0.5/README.md` & `fractal-roles-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fractal-roles-1.0.5/align_version.py` & `fractal-roles-1.0.6/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal-roles-1.0.5/examples/account/app.py` & `fractal-roles-1.0.6/examples/account/app.py`

 * *Files identical despite different names*

### Comparing `fractal-roles-1.0.5/examples/account/roles.py` & `fractal-roles-1.0.6/examples/account/roles.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Optional
 
-from fractal_specifications.generic.operators import EqualsSpecification  # type: ignore
-from fractal_specifications.generic.specification import Specification  # type: ignore
+from fractal_specifications.generic.operators import EqualsSpecification
+from fractal_specifications.generic.specification import Specification
 
 from fractal_roles.models import Method, Methods, Role, TokenPayloadRolesMixin
 from fractal_roles.services import RolesService as BaseRolesService
 
 
 @dataclass
 class TokenPayloadRoles(TokenPayloadRolesMixin):
```

### Comparing `fractal-roles-1.0.5/examples/account_user/app.py` & `fractal-roles-1.0.6/examples/account_user/app.py`

 * *Files identical despite different names*

### Comparing `fractal-roles-1.0.5/examples/account_user/roles.py` & `fractal-roles-1.0.6/examples/account_user/roles.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Optional
 
-from fractal_specifications.generic.operators import EqualsSpecification  # type: ignore
-from fractal_specifications.generic.specification import Specification  # type: ignore
+from fractal_specifications.generic.operators import EqualsSpecification
+from fractal_specifications.generic.specification import Specification
 
 from fractal_roles.models import Method, Methods, Role, TokenPayloadRolesMixin
 from fractal_roles.services import RolesService as BaseRolesService
 
 
 @dataclass
 class TokenPayloadRoles(TokenPayloadRolesMixin):
```

### Comparing `fractal-roles-1.0.5/examples/alternative/app.py` & `fractal-roles-1.0.6/examples/alternative/app.py`

 * *Files identical despite different names*

### Comparing `fractal-roles-1.0.5/examples/alternative/roles.py` & `fractal-roles-1.0.6/examples/alternative/roles.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Optional
 
-from fractal_specifications.generic.operators import EqualsSpecification  # type: ignore
-from fractal_specifications.generic.specification import Specification  # type: ignore
+from fractal_specifications.generic.operators import EqualsSpecification
+from fractal_specifications.generic.specification import Specification
 
 from fractal_roles.models import Method, Role, TokenPayloadRolesMixin
 from fractal_roles.services import RolesService as BaseRolesService
 
 
 @dataclass
 class TokenPayloadRoles(TokenPayloadRolesMixin):
```

### Comparing `fractal-roles-1.0.5/examples/readme/app.py` & `fractal-roles-1.0.6/examples/readme/app.py`

 * *Files identical despite different names*

### Comparing `fractal-roles-1.0.5/examples/readme/roles.py` & `fractal-roles-1.0.6/examples/readme/roles.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 
-from fractal_specifications.generic.operators import EqualsSpecification  # type: ignore
-from fractal_specifications.generic.specification import Specification  # type: ignore
+from fractal_specifications.generic.operators import EqualsSpecification
+from fractal_specifications.generic.specification import Specification
 
 from fractal_roles.models import Method, Methods, Role, TokenPayloadRolesMixin
 from fractal_roles.services import RolesService as BaseRolesService
 
 
 @dataclass
 class TokenPayloadRoles(TokenPayloadRolesMixin):
```

### Comparing `fractal-roles-1.0.5/fractal_roles/models.py` & `fractal-roles-1.0.6/fractal_roles/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from typing import Callable, Optional, Protocol
 
-from fractal_specifications.generic.specification import (  # type: ignore
+from fractal_specifications.generic.specification import (
     EmptySpecification,
     Specification,
 )
 
 
 class Role:
     def __getattr__(self, item):
```

### Comparing `fractal-roles-1.0.5/fractal_roles/services.py` & `fractal-roles-1.0.6/fractal_roles/services.py`

 * *Files identical despite different names*

### Comparing `fractal-roles-1.0.5/pyproject.toml` & `fractal-roles-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-roles"
-version = "1.0.5"
+version = "1.0.6"
 description = "Fractal Roles provides a flexible way to define fine-grained roles & permissions for users of your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
```

### Comparing `fractal-roles-1.0.5/tests/fixtures.py` & `fractal-roles-1.0.6/tests/fixtures.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 from typing import Optional
 
 import pytest
-from fractal_specifications.generic.operators import EqualsSpecification  # type: ignore
-from fractal_specifications.generic.specification import Specification  # type: ignore
+from fractal_specifications.generic.operators import EqualsSpecification
+from fractal_specifications.generic.specification import Specification
 
 from fractal_roles.models import Method, Methods, Role, TokenPayloadRolesMixin
 from fractal_roles.services import RolesService as BaseRolesService
 
 
 @dataclass
 class Task:
```

### Comparing `fractal-roles-1.0.5/tests/test_service.py` & `fractal-roles-1.0.6/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `fractal-roles-1.0.5/tox.ini` & `fractal-roles-1.0.6/tox.ini`

 * *Files identical despite different names*

### Comparing `fractal-roles-1.0.5/PKG-INFO` & `fractal-roles-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-roles
-Version: 1.0.5
+Version: 1.0.6
 Summary: Fractal Roles provides a flexible way to define fine-grained roles & permissions for users of your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal-roles
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```


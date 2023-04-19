# Comparing `tmp/flow360-0.2.0b3.tar.gz` & `tmp/flow360-0.2.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow360-0.2.0b3.tar", max compression
+gzip compressed data, was "flow360-0.2.0b4.tar", max compression
```

## Comparing `flow360-0.2.0b3.tar` & `flow360-0.2.0b4.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rw-r--r--   0        0        0    26526 2023-04-18 16:43:34.940230 flow360-0.2.0b3/LICENSE
--rw-r--r--   0        0        0     1427 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/__init__.py
--rw-r--r--   0        0        0       53 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/cli/__init__.py
--rw-r--r--   0        0        0     1126 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/cli/app.py
--rw-r--r--   0        0        0        0 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/cloud/__init__.py
--rw-r--r--   0        0        0     2897 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/cloud/http_util.py
--rw-r--r--   0        0        0     1466 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/cloud/rest_api.py
--rw-r--r--   0        0        0     8847 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/cloud/s3_utils.py
--rw-r--r--   0        0        0      687 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/cloud/security.py
--rw-r--r--   0        0        0        0 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/__init__.py
--rw-r--r--   0        0        0    23078 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/case.py
--rw-r--r--   0        0        0      142 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/constants.py
--rw-r--r--   0        0        0    25502 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/flow360_params/flow360_params.py
--rw-r--r--   0        0        0    18013 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/flow360_params/params_base.py
--rw-r--r--   0        0        0     7651 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/flow360_params/solvers.py
--rw-r--r--   0        0        0      220 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/meshing/__init__.py
--rw-r--r--   0        0        0     6160 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/meshing/params.py
--rw-r--r--   0        0        0     8159 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/resource_base.py
--rw-r--r--   0        0        0    10172 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/surface_mesh.py
--rw-r--r--   0        0        0     2327 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/types.py
--rw-r--r--   0        0        0     1019 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/utils.py
--rw-r--r--   0        0        0     2955 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/validator.py
--rw-r--r--   0        0        0    21592 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/component/volume_mesh.py
--rw-r--r--   0        0        0     2137 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/environment.py
--rw-r--r--   0        0        0      237 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/examples/__init__.py
--rw-r--r--   0        0        0     4024 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/examples/actuatorDisk/flow360.json
--rw-r--r--   0        0        0      447 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/examples/actuator_disk.py
--rw-r--r--   0        0        0    24017 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/examples/airplane/geometry.csm
--rw-r--r--   0        0        0      675 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/examples/airplane/surface_params.json
--rw-r--r--   0        0        0     3702 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/examples/airplane/volume_params.json
--rw-r--r--   0        0        0      292 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/examples/airplane.py
--rw-r--r--   0        0        0     5406 2023-04-18 16:43:34.940230 flow360-0.2.0b3/flow360/examples/base_test_case.py
--rw-r--r--   0        0        0  1157943 2023-04-18 16:43:34.948230 flow360-0.2.0b3/flow360/examples/betDisk/flow360.json
--rw-r--r--   0        0        0  1158028 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/betLine/flow360.json
--rw-r--r--   0        0        0  1158029 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      432 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/bet_disk.py
--rw-r--r--   0        0        0      432 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/bet_line.py
--rw-r--r--   0        0        0     1430 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/cylinder/flow360.json
--rw-r--r--   0        0        0     1492 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0      373 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/cylinder.py
--rw-r--r--   0        0        0       63 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/om6wing/Flow360Mesh.json
--rw-r--r--   0        0        0     1500 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/om6wing/case.yaml
--rw-r--r--   0        0        0     2509 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/om6wing/flow360.json
--rw-r--r--   0        0        0      427 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
--rw-r--r--   0        0        0     2305 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      391 2023-04-18 16:43:34.952231 flow360-0.2.0b3/flow360/examples/om6wing.py
--rw-r--r--   0        0        0     2744 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/rotatingSpheres/flow360.json
--rw-r--r--   0        0        0      913 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/rotatingSpheres/flow360mesh.json
--rw-r--r--   0        0        0     3379 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
--rw-r--r--   0        0        0     3376 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
--rw-r--r--   0        0        0      347 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/examples/rotating_spheres.py
--rw-r--r--   0        0        0     1354 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/exceptions.py
--rw-r--r--   0        0        0     5809 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/log.py
--rw-r--r--   0        0        0     1146 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/solver_version.py
--rw-r--r--   0        0        0       38 2023-04-18 16:43:34.956231 flow360-0.2.0b3/flow360/version.py
--rw-r--r--   0        0        0     1465 2023-04-18 16:43:57.257523 flow360-0.2.0b3/pyproject.toml
--rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 flow360-0.2.0b3/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-04-19 18:35:50.436583 flow360-0.2.0b4/LICENSE
+-rw-r--r--   0        0        0     1427 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/__init__.py
+-rw-r--r--   0        0        0       53 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/cli/__init__.py
+-rw-r--r--   0        0        0     2526 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/cli/app.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/cloud/__init__.py
+-rw-r--r--   0        0        0     2944 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/cloud/http_util.py
+-rw-r--r--   0        0        0     1466 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/cloud/rest_api.py
+-rw-r--r--   0        0        0     8847 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/cloud/s3_utils.py
+-rw-r--r--   0        0        0      222 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/cloud/security.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/__init__.py
+-rw-r--r--   0        0        0    23078 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/case.py
+-rw-r--r--   0        0        0      142 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/constants.py
+-rw-r--r--   0        0        0    25502 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/flow360_params/flow360_params.py
+-rw-r--r--   0        0        0    18013 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/flow360_params/params_base.py
+-rw-r--r--   0        0        0     7651 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/flow360_params/solvers.py
+-rw-r--r--   0        0        0      220 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/meshing/__init__.py
+-rw-r--r--   0        0        0     6160 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/meshing/params.py
+-rw-r--r--   0        0        0     8586 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/resource_base.py
+-rw-r--r--   0        0        0    10172 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/surface_mesh.py
+-rw-r--r--   0        0        0     2327 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/types.py
+-rw-r--r--   0        0        0     1019 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/utils.py
+-rw-r--r--   0        0        0     2955 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/validator.py
+-rw-r--r--   0        0        0    21592 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/component/volume_mesh.py
+-rw-r--r--   0        0        0     2228 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/environment.py
+-rw-r--r--   0        0        0      237 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/examples/__init__.py
+-rw-r--r--   0        0        0     4024 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/examples/actuatorDisk/flow360.json
+-rw-r--r--   0        0        0      447 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/examples/actuator_disk.py
+-rw-r--r--   0        0        0    24017 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/examples/airplane/geometry.csm
+-rw-r--r--   0        0        0      675 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/examples/airplane/surface_params.json
+-rw-r--r--   0        0        0     3702 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/examples/airplane/volume_params.json
+-rw-r--r--   0        0        0      292 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/examples/airplane.py
+-rw-r--r--   0        0        0     5406 2023-04-19 18:35:50.436583 flow360-0.2.0b4/flow360/examples/base_test_case.py
+-rw-r--r--   0        0        0  1157943 2023-04-19 18:35:50.440583 flow360-0.2.0b4/flow360/examples/betDisk/flow360.json
+-rw-r--r--   0        0        0  1158028 2023-04-19 18:35:50.444583 flow360-0.2.0b4/flow360/examples/betLine/flow360.json
+-rw-r--r--   0        0        0  1158029 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      432 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/bet_disk.py
+-rw-r--r--   0        0        0      432 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/bet_line.py
+-rw-r--r--   0        0        0     1430 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/cylinder/flow360.json
+-rw-r--r--   0        0        0     1492 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0      373 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/cylinder.py
+-rw-r--r--   0        0        0       63 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/om6wing/Flow360Mesh.json
+-rw-r--r--   0        0        0     1500 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/om6wing/case.yaml
+-rw-r--r--   0        0        0     2509 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/om6wing/flow360.json
+-rw-r--r--   0        0        0      427 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
+-rw-r--r--   0        0        0     2305 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      391 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/om6wing.py
+-rw-r--r--   0        0        0     2744 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/rotatingSpheres/flow360.json
+-rw-r--r--   0        0        0      913 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/rotatingSpheres/flow360mesh.json
+-rw-r--r--   0        0        0     3379 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
+-rw-r--r--   0        0        0     3376 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
+-rw-r--r--   0        0        0      347 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/examples/rotating_spheres.py
+-rw-r--r--   0        0        0     1354 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/exceptions.py
+-rw-r--r--   0        0        0     5809 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/log.py
+-rw-r--r--   0        0        0     1146 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/solver_version.py
+-rw-r--r--   0        0        0     2377 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/user_config.py
+-rw-r--r--   0        0        0       38 2023-04-19 18:35:50.448583 flow360-0.2.0b4/flow360/version.py
+-rw-r--r--   0        0        0     1465 2023-04-19 18:36:07.724608 flow360-0.2.0b4/pyproject.toml
+-rw-r--r--   0        0        0     1507 1970-01-01 00:00:00.000000 flow360-0.2.0b4/PKG-INFO
```

### Comparing `flow360-0.2.0b3/LICENSE` & `flow360-0.2.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/__init__.py` & `flow360-0.2.0b4/flow360/__init__.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/cloud/http_util.py` & `flow360-0.2.0b4/flow360/cloud/http_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 from functools import wraps
 
 import requests
 
 from ..environment import Env
 from ..exceptions import AuthorisationError, WebError, WebNotFoundError
 from ..log import log
+from ..user_config import user_config
 from ..version import __version__
 from .security import api_key
 
 
 def api_key_auth(request):
     """
     Set the authentication.
     :param request:
     :return:
     """
-    key = api_key(Env.current.apikey_profile)
+    key = api_key()
     if not key:
         raise AuthorisationError(
-            "API key not found, please set it by commandline: flow360 configure."
+            f"API key not found for profile={user_config.profile}, please set it by commandline: flow360 configure."
         )
     request.headers["simcloud-api-key"] = key
     request.headers["flow360-python-version"] = __version__
     return request
 
 
 def http_interceptor(func):
```

### Comparing `flow360-0.2.0b3/flow360/cloud/rest_api.py` & `flow360-0.2.0b4/flow360/cloud/rest_api.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/cloud/s3_utils.py` & `flow360-0.2.0b4/flow360/cloud/s3_utils.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/component/case.py` & `flow360-0.2.0b4/flow360/component/case.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/component/flow360_params/flow360_params.py` & `flow360-0.2.0b4/flow360/component/flow360_params/flow360_params.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/component/flow360_params/params_base.py` & `flow360-0.2.0b4/flow360/component/flow360_params/params_base.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/component/flow360_params/solvers.py` & `flow360-0.2.0b4/flow360/component/flow360_params/solvers.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/component/meshing/params.py` & `flow360-0.2.0b4/flow360/component/meshing/params.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/component/resource_base.py` & `flow360-0.2.0b4/flow360/component/resource_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from functools import wraps
 from typing import List, Optional, Union
 
 from pydantic import BaseModel, Extra, Field
 
 from ..cloud.rest_api import RestApi
 from ..log import log
+from ..user_config import user_config
 
 
 class Flow360Status(Enum):
     """
     Flow360Status component
     """
 
@@ -117,14 +118,24 @@
 
     def __init__(self):
         # remove from traceback:
         # 1. This line (self.traceback)
         # 2. Call of this init
         self.traceback = traceback.format_stack()[:-2]
 
+        if not user_config.suppress_submit_warning():
+            log.warning(
+                f"""\
+Remeber to submit your {self.__class__.__name__} to cloud to have it processed.
+Please run .submit() after .create()
+To suppress this message run: flow360 configure --suppress-submit-warning"""
+            )
+            for line in self.traceback:
+                print(line.strip())
+
     @property
     def id(self):
         """
         returns id of resource
         """
         return self._id
 
@@ -138,17 +149,17 @@
         """
         if self.id is None:
             return False
         return True
 
     def __del__(self):
         if self.is_cloud_resource() is False and self.traceback is not None:
-            log.warning(
+            print(
                 f"\
-You have not submitted your {self.__class__.__name__} to cloud. \
+WARNING: You have not submitted your {self.__class__.__name__} to cloud. \
 It will not be process. Please run .submit() after .create()"
             )
             for line in self.traceback:
                 print(line.strip())
 
 
 class Flow360Resource(RestApi):
```

### Comparing `flow360-0.2.0b3/flow360/component/surface_mesh.py` & `flow360-0.2.0b4/flow360/component/surface_mesh.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/component/types.py` & `flow360-0.2.0b4/flow360/component/types.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/component/utils.py` & `flow360-0.2.0b4/flow360/component/utils.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/component/validator.py` & `flow360-0.2.0b4/flow360/component/validator.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/component/volume_mesh.py` & `flow360-0.2.0b4/flow360/component/volume_mesh.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/environment.py` & `flow360-0.2.0b4/flow360/environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Environment Setup
 """
 
 from pydantic import BaseModel
 
+from .user_config import user_config
+
 
 class EnvironmentConfig(BaseModel):
     """
     Basic Configuration for definition environment.
     """
 
     name: str
@@ -17,14 +19,15 @@
 
     def active(self):
         """
         Activate the particular environment.
         :return:
         """
         Env.set_current(self)
+        user_config.set_profile(self.apikey_profile)
 
     def get_real_url(self, path: str):
         """
         Get the real url for the particular environment.
         :param path:
         :return:
         """
```

### Comparing `flow360-0.2.0b3/flow360/examples/actuatorDisk/flow360.json` & `flow360-0.2.0b4/flow360/examples/actuatorDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/airplane/geometry.csm` & `flow360-0.2.0b4/flow360/examples/airplane/geometry.csm`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/airplane/surface_params.json` & `flow360-0.2.0b4/flow360/examples/airplane/surface_params.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/airplane/volume_params.json` & `flow360-0.2.0b4/flow360/examples/airplane/volume_params.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/base_test_case.py` & `flow360-0.2.0b4/flow360/examples/base_test_case.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/betDisk/flow360.json` & `flow360-0.2.0b4/flow360/examples/betDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/betLine/flow360.json` & `flow360-0.2.0b4/flow360/examples/betLine/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/betLine/release-21.3.3.0ge/flow360.json` & `flow360-0.2.0b4/flow360/examples/betLine/release-21.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/cylinder/flow360.json` & `flow360-0.2.0b4/flow360/examples/cylinder/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json` & `flow360-0.2.0b4/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/om6wing/case.yaml` & `flow360-0.2.0b4/flow360/examples/om6wing/case.yaml`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/om6wing/flow360.json` & `flow360-0.2.0b4/flow360/examples/om6wing/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json` & `flow360-0.2.0b4/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/rotatingSpheres/flow360.json` & `flow360-0.2.0b4/flow360/examples/rotatingSpheres/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/rotatingSpheres/flow360mesh.json` & `flow360-0.2.0b4/flow360/examples/rotatingSpheres/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json` & `flow360-0.2.0b4/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json` & `flow360-0.2.0b4/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json` & `flow360-0.2.0b4/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json` & `flow360-0.2.0b4/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/exceptions.py` & `flow360-0.2.0b4/flow360/exceptions.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/log.py` & `flow360-0.2.0b4/flow360/log.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/flow360/solver_version.py` & `flow360-0.2.0b4/flow360/solver_version.py`

 * *Files identical despite different names*

### Comparing `flow360-0.2.0b3/pyproject.toml` & `flow360-0.2.0b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flow360"
-version = "v0.2.0b3"
+version = "v0.2.0b4"
 description = ""
 authors = ["Flexcompute <support@flexcompute.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.7.4"
 pydantic = "^1.9.2"
 pytest = "^7.1.2"
```

### Comparing `flow360-0.2.0b3/PKG-INFO` & `flow360-0.2.0b4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flow360
-Version: 0.2.0b3
+Version: 0.2.0b4
 Summary: 
 Author: Flexcompute
 Author-email: support@flexcompute.com
 Requires-Python: >=3.7.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


# Comparing `tmp/fps_auth_fief-0.1.3.tar.gz` & `tmp/fps_auth_fief-0.1.4.tar.gz`

## Comparing `fps_auth_fief-0.1.3.tar` & `fps_auth_fief-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.3/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.3/fps_auth_fief/__init__.py
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.3/fps_auth_fief/backend.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.3/fps_auth_fief/config.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.3/fps_auth_fief/main.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.3/fps_auth_fief/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.3/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.3/COPYING.md
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.3/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.4/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.4/fps_auth_fief/__init__.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.4/fps_auth_fief/backend.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.4/fps_auth_fief/config.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.4/fps_auth_fief/main.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.4/fps_auth_fief/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.4/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.4/COPYING.md
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.4/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 fps_auth_fief-0.1.4/PKG-INFO
```

### Comparing `fps_auth_fief-0.1.3/fps_auth_fief/backend.py` & `fps_auth_fief-0.1.4/fps_auth_fief/backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict, List, Optional, Tuple
 
 from fastapi import Depends, HTTPException, Request, Response, WebSocket, status
 from fastapi.security import APIKeyCookie
-from fief_client import FiefAccessTokenInfo, FiefAsync, FiefUserInfo  # type: ignore
-from fief_client.integrations.fastapi import FiefAuth  # type: ignore
+from fief_client import FiefAccessTokenInfo, FiefAsync, FiefUserInfo
+from fief_client.integrations.fastapi import FiefAuth
 from jupyverse_api.auth import User
 
 from .config import _AuthFiefConfig
 
 
 class Backend:
     def __init__(self, auth_fief_config: _AuthFiefConfig):
```

### Comparing `fps_auth_fief-0.1.3/fps_auth_fief/main.py` & `fps_auth_fief-0.1.4/fps_auth_fief/main.py`

 * *Files identical despite different names*

### Comparing `fps_auth_fief-0.1.3/fps_auth_fief/routes.py` & `fps_auth_fief-0.1.4/fps_auth_fief/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from typing import Dict, List
 
 from fastapi import APIRouter, Depends, Query, Request, Response
 from fastapi.responses import RedirectResponse
-from fief_client import FiefAccessTokenInfo  # type: ignore
+from fief_client import FiefAccessTokenInfo
 from jupyverse_api import Router
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 
 from .backend import Backend
 from .config import _AuthFiefConfig
```

### Comparing `fps_auth_fief-0.1.3/.gitignore` & `fps_auth_fief-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_auth_fief-0.1.3/COPYING.md` & `fps_auth_fief-0.1.4/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_auth_fief-0.1.3/pyproject.toml` & `fps_auth_fief-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_auth_fief-0.1.3/PKG-INFO` & `fps_auth_fief-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_auth_fief
-Version: 0.1.3
+Version: 0.1.4
 Summary: An FPS plugin for the authentication API, using Fief
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```


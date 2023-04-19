# Comparing `tmp/hspylib-firebase-0.9.95.tar.gz` & `tmp/hspylib-firebase-0.9.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-firebase-0.9.95.tar", last modified: Wed Mar 29 22:13:41 2023, max compression
+gzip compressed data, was "hspylib-firebase-0.9.96.tar", last modified: Wed Apr 19 19:04:54 2023, max compression
```

## Comparing `hspylib-firebase-0.9.95.tar` & `hspylib-firebase-0.9.96.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-03-29 22:13:41.264834 hspylib-firebase-0.9.95/
--rw-r--r--   0 hjunior    (504) staff       (20)       95 2022-06-17 15:16:57.000000 hspylib-firebase-0.9.95/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1580 2023-03-29 22:13:41.263853 hspylib-firebase-0.9.95/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      708 2023-03-29 22:13:40.000000 hspylib-firebase-0.9.95/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-03-29 22:13:41.233581 hspylib-firebase-0.9.95/firebase/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-03-29 22:13:40.000000 hspylib-firebase-0.9.95/firebase/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      722 2022-12-23 00:36:53.000000 hspylib-firebase-0.9.95/firebase/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      221 2023-03-29 22:13:40.000000 hspylib-firebase-0.9.95/firebase/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     4427 2023-01-12 17:14:59.000000 hspylib-firebase-0.9.95/firebase/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-03-29 22:13:41.243445 hspylib-firebase-0.9.95/firebase/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      226 2023-03-29 22:13:40.000000 hspylib-firebase-0.9.95/firebase/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6536 2023-03-06 16:46:30.000000 hspylib-firebase-0.9.95/firebase/core/agent_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5008 2023-03-06 16:46:30.000000 hspylib-firebase-0.9.95/firebase/core/file_processor.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2946 2023-01-23 19:15:41.000000 hspylib-firebase-0.9.95/firebase/core/firebase.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2608 2023-01-23 20:08:17.000000 hspylib-firebase-0.9.95/firebase/core/firebase_auth.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-03-29 22:13:41.247587 hspylib-firebase-0.9.95/firebase/domain/
--rw-r--r--   0 hjunior    (504) staff       (20)      172 2023-03-29 22:13:40.000000 hspylib-firebase-0.9.95/firebase/domain/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3339 2023-03-06 16:46:30.000000 hspylib-firebase-0.9.95/firebase/domain/firebase_dto.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-03-29 22:13:41.251680 hspylib-firebase-0.9.95/firebase/exception/
--rw-r--r--   0 hjunior    (504) staff       (20)      173 2023-03-29 22:13:40.000000 hspylib-firebase-0.9.95/firebase/exception/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      765 2022-12-22 23:12:20.000000 hspylib-firebase-0.9.95/firebase/exception/exceptions.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-03-29 22:13:41.253223 hspylib-firebase-0.9.95/firebase/resources/
--rw-r--r--   0 hjunior    (504) staff       (20)      130 2022-11-12 19:14:41.000000 hspylib-firebase-0.9.95/firebase/resources/application.properties
--rw-r--r--   0 hjunior    (504) staff       (20)      237 2022-02-18 20:00:37.000000 hspylib-firebase-0.9.95/firebase/welcome.txt
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-03-29 22:13:41.262274 hspylib-firebase-0.9.95/hspylib_firebase.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1580 2023-03-29 22:13:41.000000 hspylib-firebase-0.9.95/hspylib_firebase.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      647 2023-03-29 22:13:41.000000 hspylib-firebase-0.9.95/hspylib_firebase.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-03-29 22:13:41.000000 hspylib-firebase-0.9.95/hspylib_firebase.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       73 2023-03-29 22:13:41.000000 hspylib-firebase-0.9.95/hspylib_firebase.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        9 2023-03-29 22:13:41.000000 hspylib-firebase-0.9.95/hspylib_firebase.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-03-29 22:13:41.264985 hspylib-firebase-0.9.95/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     1864 2023-01-12 17:14:59.000000 hspylib-firebase-0.9.95/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:54.250276 hspylib-firebase-0.9.96/
+-rw-r--r--   0 hjunior    (504) staff       (20)       95 2022-06-17 15:16:57.000000 hspylib-firebase-0.9.96/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1580 2023-04-19 19:04:54.249626 hspylib-firebase-0.9.96/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      708 2023-04-19 19:04:53.000000 hspylib-firebase-0.9.96/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:54.222685 hspylib-firebase-0.9.96/firebase/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-04-19 19:04:53.000000 hspylib-firebase-0.9.96/firebase/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      722 2022-12-23 00:36:53.000000 hspylib-firebase-0.9.96/firebase/__classpath__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      221 2023-04-19 19:04:53.000000 hspylib-firebase-0.9.96/firebase/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4427 2023-04-18 23:04:54.000000 hspylib-firebase-0.9.96/firebase/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:54.232660 hspylib-firebase-0.9.96/firebase/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      226 2023-04-19 19:04:53.000000 hspylib-firebase-0.9.96/firebase/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6536 2023-04-18 23:04:54.000000 hspylib-firebase-0.9.96/firebase/core/agent_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     5008 2023-04-18 23:04:54.000000 hspylib-firebase-0.9.96/firebase/core/file_processor.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2946 2023-04-18 23:04:54.000000 hspylib-firebase-0.9.96/firebase/core/firebase.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2608 2023-04-18 23:04:54.000000 hspylib-firebase-0.9.96/firebase/core/firebase_auth.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:54.236900 hspylib-firebase-0.9.96/firebase/domain/
+-rw-r--r--   0 hjunior    (504) staff       (20)      172 2023-04-19 19:04:53.000000 hspylib-firebase-0.9.96/firebase/domain/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3338 2023-04-18 23:04:54.000000 hspylib-firebase-0.9.96/firebase/domain/firebase_dto.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:54.241230 hspylib-firebase-0.9.96/firebase/exception/
+-rw-r--r--   0 hjunior    (504) staff       (20)      173 2023-04-19 19:04:53.000000 hspylib-firebase-0.9.96/firebase/exception/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      765 2022-12-22 23:12:20.000000 hspylib-firebase-0.9.96/firebase/exception/exceptions.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:54.242463 hspylib-firebase-0.9.96/firebase/resources/
+-rw-r--r--   0 hjunior    (504) staff       (20)      130 2022-11-12 19:14:41.000000 hspylib-firebase-0.9.96/firebase/resources/application.properties
+-rw-r--r--   0 hjunior    (504) staff       (20)      237 2022-02-18 20:00:37.000000 hspylib-firebase-0.9.96/firebase/welcome.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:54.248703 hspylib-firebase-0.9.96/hspylib_firebase.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1580 2023-04-19 19:04:54.000000 hspylib-firebase-0.9.96/hspylib_firebase.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      647 2023-04-19 19:04:54.000000 hspylib-firebase-0.9.96/hspylib_firebase.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-04-19 19:04:54.000000 hspylib-firebase-0.9.96/hspylib_firebase.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       73 2023-04-19 19:04:54.000000 hspylib-firebase-0.9.96/hspylib_firebase.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        9 2023-04-19 19:04:54.000000 hspylib-firebase-0.9.96/hspylib_firebase.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-04-19 19:04:54.250390 hspylib-firebase-0.9.96/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     1865 2023-04-05 21:45:47.000000 hspylib-firebase-0.9.96/setup.py
```

### Comparing `hspylib-firebase-0.9.95/PKG-INFO` & `hspylib-firebase-0.9.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-firebase
-Version: 0.9.95
+Version: 0.9.96
 Summary: HSPyLib - Firebase integration
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-firebase/
@@ -24,12 +24,12 @@
 Description-Content-Type: text/markdown
 
 # HomeSetup - Firebase integration
 
 ## Upload and Download files to/from your firebase database
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.95/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.96/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-firebase)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-firebase-0.9.95/README.md` & `hspylib-firebase-0.9.96/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HomeSetup - Firebase integration
 
 ## Upload and Download files to/from your firebase database
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.95/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.96/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-firebase)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-firebase-0.9.95/firebase/__classpath__.py` & `hspylib-firebase-0.9.96/firebase/__classpath__.py`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.95/firebase/__main__.py` & `hspylib-firebase-0.9.96/firebase/__main__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,28 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
 """
 
+import logging as log
+import os
+import sys
+import urllib3
 from clitt.core.tui.tui_application import TUIApplication
-from firebase.__classpath__ import _Classpath
-from firebase.core.firebase import Firebase
 from hspylib.core.enums.charset import Charset
 from hspylib.core.tools.commons import syserr
 from hspylib.core.zoned_datetime import now
 from hspylib.modules.application.exit_status import ExitStatus
 from hspylib.modules.application.version import Version
 from textwrap import dedent
 
-import logging as log
-import os
-import sys
-import urllib3
+from firebase.__classpath__ import _Classpath
+from firebase.core.firebase import Firebase
 
 # Disable this warning because we are hitting our own database
 urllib3.disable_warnings()
 
 
 class Main(TUIApplication):
     """Firebase Agent - Manage your firebase integration"""
```

### Comparing `hspylib-firebase-0.9.95/firebase/core/agent_config.py` & `hspylib-firebase-0.9.96/firebase/core/agent_config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,31 +8,31 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
 """
+import logging as log
+import os
 from clitt.core.tui.minput.input_validator import InputValidator
 from clitt.core.tui.minput.minput import MenuInput, minput
 from datasource.firebase.firebase_configuration import FirebaseConfiguration
-from firebase.core.firebase_auth import FirebaseAuth
-from firebase.exception.exceptions import FirebaseAuthenticationError
 from hspylib.core.config.app_config import AppConfigs
 from hspylib.core.config.properties import Properties
 from hspylib.core.enums.charset import Charset
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.tools.commons import dirname, file_is_not_empty, sysout, touch_file
 from hspylib.core.tools.dict_tools import get_or_default_by_key
 from os.path import basename
 from requests.structures import CaseInsensitiveDict
 from typing import Any, Optional
 
-import logging as log
-import os
+from firebase.core.firebase_auth import FirebaseAuth
+from firebase.exception.exceptions import FirebaseAuthenticationError
 
 
 class AgentConfig(metaclass=Singleton):
     """Holds the firebase agent configurations.
     """
 
     def __init__(self, filename: str) -> None:
```

### Comparing `hspylib-firebase-0.9.95/firebase/core/file_processor.py` & `hspylib-firebase-0.9.96/firebase/core/file_processor.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,27 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
 """
+import json
+import logging as log
+import os
 from abc import ABC
-from firebase.domain.firebase_dto import FirebaseDto
 from fnmatch import fnmatch
 from hspylib.core.enums.http_code import HttpCode
 from hspylib.core.preconditions import check_argument, check_not_none
 from hspylib.core.tools.commons import syserr, sysout
 from hspylib.modules.fetch.fetch import get, put
 from requests.exceptions import HTTPError
 from typing import List
 
-import json
-import logging as log
-import os
+from firebase.domain.firebase_dto import FirebaseDto
 
 
 class FileProcessor(ABC):
     """Utility class to upload / download B64-encoded files.
     """
 
     @staticmethod
```

### Comparing `hspylib-firebase-0.9.95/firebase/core/firebase.py` & `hspylib-firebase-0.9.96/firebase/core/firebase.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -9,22 +9,22 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
 """
 
-from firebase.core.agent_config import AgentConfig
-from firebase.core.file_processor import FileProcessor
-from firebase.core.firebase_auth import FirebaseAuth
+import logging as log
+import os
 from hspylib.core.preconditions import check_argument
 from typing import List
 
-import logging as log
-import os
+from firebase.core.agent_config import AgentConfig
+from firebase.core.file_processor import FileProcessor
+from firebase.core.firebase_auth import FirebaseAuth
 
 
 class Firebase:
     """Provides the firebase application functionalities.
     """
 
     def __init__(self) -> None:
```

### Comparing `hspylib-firebase-0.9.95/firebase/core/firebase_auth.py` & `hspylib-firebase-0.9.96/firebase/core/firebase_auth.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -8,25 +8,25 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
 """
+import firebase_admin
+import os
 from abc import ABC
-from firebase.exception.exceptions import FirebaseAuthenticationError, FirebaseException, InvalidFirebaseCredentials
 from firebase_admin import auth, credentials
 from firebase_admin.auth import UserNotFoundError, UserRecord
 from firebase_admin.exceptions import FirebaseError
 from hspylib.core.preconditions import check_not_none
 from hspylib.core.tools.commons import sysout
 from typing import Optional
 
-import firebase_admin
-import os
+from firebase.exception.exceptions import FirebaseAuthenticationError, FirebaseException, InvalidFirebaseCredentials
 
 
 class FirebaseAuth(ABC):
     """Firebase authentication utils
     Ref: https://www.youtube.com/watch?v=esqNgnayVE8
     """
```

### Comparing `hspylib-firebase-0.9.95/firebase/domain/firebase_dto.py` & `hspylib-firebase-0.9.96/firebase/domain/firebase_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,23 +8,22 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
 """
+import json
+import logging as log
+import os
 from hspylib.core.enums.charset import Charset
 from hspylib.core.zoned_datetime import now
 from hspylib.modules.security.security import b64_decode, b64_encode
 from typing import List
 
-import json
-import logging as log
-import os
-
 
 class FirebaseDto:
     """Represents a Firebase DTO.
     """
 
     @staticmethod
     def from_file(filepath: str, contents: str | bytes, encoding: str = Charset.UTF_8.val) -> 'FirebaseDto':
```

### Comparing `hspylib-firebase-0.9.95/firebase/exception/exceptions.py` & `hspylib-firebase-0.9.96/firebase/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.95/hspylib_firebase.egg-info/PKG-INFO` & `hspylib-firebase-0.9.96/hspylib_firebase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-firebase
-Version: 0.9.95
+Version: 0.9.96
 Summary: HSPyLib - Firebase integration
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-firebase/
@@ -24,12 +24,12 @@
 Description-Content-Type: text/markdown
 
 # HomeSetup - Firebase integration
 
 ## Upload and Download files to/from your firebase database
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.95/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.96/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-firebase)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-firebase-0.9.95/hspylib_firebase.egg-info/SOURCES.txt` & `hspylib-firebase-0.9.96/hspylib_firebase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.95/setup.py` & `hspylib-firebase-0.9.96/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2022, HSPyLib team
 """
 
 import pathlib
+
 import setuptools
 
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
```


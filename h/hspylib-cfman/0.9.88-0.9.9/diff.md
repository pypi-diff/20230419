# Comparing `tmp/hspylib-cfman-0.9.88.tar.gz` & `tmp/hspylib-cfman-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-cfman-0.9.88.tar", last modified: Wed Apr 19 19:04:14 2023, max compression
+gzip compressed data, was "hspylib-cfman-0.9.9.tar", last modified: Tue Feb 22 22:53:31 2022, max compression
```

## Comparing `hspylib-cfman-0.9.88.tar` & `hspylib-cfman-0.9.9.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:14.804630 hspylib-cfman-0.9.88/
--rw-r--r--   0 hjunior    (504) staff       (20)       49 2022-02-23 03:43:53.000000 hspylib-cfman-0.9.88/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-04-19 19:04:14.803637 hspylib-cfman-0.9.88/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      677 2023-04-19 19:04:13.000000 hspylib-cfman-0.9.88/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:14.783353 hspylib-cfman-0.9.88/cfman/
--rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-04-19 19:04:13.000000 hspylib-cfman-0.9.88/cfman/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      716 2022-12-23 00:36:17.000000 hspylib-cfman-0.9.88/cfman/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      202 2023-04-19 19:04:13.000000 hspylib-cfman-0.9.88/cfman/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3627 2023-04-18 23:04:16.000000 hspylib-cfman-0.9.88/cfman/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:14.791992 hspylib-cfman-0.9.88/cfman/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      238 2023-04-19 19:04:13.000000 hspylib-cfman-0.9.88/cfman/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     7762 2023-04-18 23:04:17.000000 hspylib-cfman-0.9.88/cfman/core/cf.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3012 2023-04-18 23:04:17.000000 hspylib-cfman-0.9.88/cfman/core/cf_application.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5406 2023-04-18 23:04:17.000000 hspylib-cfman-0.9.88/cfman/core/cf_blue_green_checker.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1243 2023-04-05 17:17:35.000000 hspylib-cfman-0.9.88/cfman/core/cf_endpoint.py
--rw-r--r--   0 hjunior    (504) staff       (20)    15432 2023-04-18 23:04:17.000000 hspylib-cfman-0.9.88/cfman/core/cf_manager.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:14.795074 hspylib-cfman-0.9.88/cfman/exception/
--rw-r--r--   0 hjunior    (504) staff       (20)      167 2023-04-19 19:04:13.000000 hspylib-cfman-0.9.88/cfman/exception/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      845 2023-04-05 17:12:04.000000 hspylib-cfman-0.9.88/cfman/exception/exceptions.py
--rw-r--r--   0 hjunior    (504) staff       (20)      204 2022-02-17 02:35:48.000000 hspylib-cfman-0.9.88/cfman/welcome.txt
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:14.802546 hspylib-cfman-0.9.88/hspylib_cfman.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1548 2023-04-19 19:04:14.000000 hspylib-cfman-0.9.88/hspylib_cfman.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      520 2023-04-19 19:04:14.000000 hspylib-cfman-0.9.88/hspylib_cfman.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-04-19 19:04:14.000000 hspylib-cfman-0.9.88/hspylib_cfman.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       28 2023-04-19 19:04:14.000000 hspylib-cfman-0.9.88/hspylib_cfman.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-04-19 19:04:14.000000 hspylib-cfman-0.9.88/hspylib_cfman.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-04-19 19:04:14.804767 hspylib-cfman-0.9.88/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     1935 2023-04-05 21:45:25.000000 hspylib-cfman-0.9.88/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 22:53:31.889535 hspylib-cfman-0.9.9/
+-rw-r--r--   0 hjunior    (504) staff       (20)      125 2022-02-18 20:26:15.000000 hspylib-cfman-0.9.9/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)      692 2022-02-22 22:53:31.888630 hspylib-cfman-0.9.9/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)       56 2022-02-13 18:53:57.000000 hspylib-cfman-0.9.9/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 22:53:31.853447 hspylib-cfman-0.9.9/cfman/
+-rw-r--r--   0 hjunior    (504) staff       (20)        5 2022-02-22 22:53:29.000000 hspylib-cfman-0.9.9/cfman/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      180 2022-02-22 19:08:33.000000 hspylib-cfman-0.9.9/cfman/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2857 2022-02-22 01:53:41.000000 hspylib-cfman-0.9.9/cfman/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 22:53:31.861883 hspylib-cfman-0.9.9/cfman/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      208 2022-02-22 19:08:33.000000 hspylib-cfman-0.9.9/cfman/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3953 2022-02-15 20:32:21.000000 hspylib-cfman-0.9.9/cfman/core/cf.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2343 2022-02-22 02:28:30.000000 hspylib-cfman-0.9.9/cfman/core/cf_application.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      721 2022-02-15 20:32:22.000000 hspylib-cfman-0.9.9/cfman/core/cf_endpoint.py
+-rw-r--r--   0 hjunior    (504) staff       (20)    10821 2022-02-22 02:29:52.000000 hspylib-cfman-0.9.9/cfman/core/cf_manager.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 22:53:31.865348 hspylib-cfman-0.9.9/cfman/exception/
+-rw-r--r--   0 hjunior    (504) staff       (20)      165 2022-02-22 19:08:33.000000 hspylib-cfman-0.9.9/cfman/exception/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      771 2022-02-11 19:26:38.000000 hspylib-cfman-0.9.9/cfman/exception/exceptions.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 22:53:31.866996 hspylib-cfman-0.9.9/cfman/resources/
+-rw-r--r--   0 hjunior    (504) staff       (20)        0 2022-02-02 16:37:07.000000 hspylib-cfman-0.9.9/cfman/resources/application.properties
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 22:53:31.871837 hspylib-cfman-0.9.9/cfman/resources/log/
+-rw-r--r--   0 hjunior    (504) staff       (20)        0 2022-02-02 16:37:07.000000 hspylib-cfman-0.9.9/cfman/resources/log/.gitkeep
+-rw-r--r--   0 hjunior    (504) staff       (20)     1180 2022-02-22 06:29:07.000000 hspylib-cfman-0.9.9/cfman/resources/log/application.log
+-rw-r--r--   0 hjunior    (504) staff       (20)      204 2022-02-17 02:35:48.000000 hspylib-cfman-0.9.9/cfman/welcome.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2022-02-22 22:53:31.887321 hspylib-cfman-0.9.9/hspylib_cfman.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)      692 2022-02-22 22:53:31.000000 hspylib-cfman-0.9.9/hspylib_cfman.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      565 2022-02-22 22:53:31.000000 hspylib-cfman-0.9.9/hspylib_cfman.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2022-02-22 22:53:31.000000 hspylib-cfman-0.9.9/hspylib_cfman.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       36 2022-02-22 22:53:31.000000 hspylib-cfman-0.9.9/hspylib_cfman.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2022-02-22 22:53:31.000000 hspylib-cfman-0.9.9/hspylib_cfman.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2022-02-22 22:53:31.889698 hspylib-cfman-0.9.9/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     1572 2022-02-15 20:32:22.000000 hspylib-cfman-0.9.9/setup.py
```

### Comparing `hspylib-cfman-0.9.88/cfman/core/cf_manager.py` & `hspylib-cfman-0.9.9/cfman/core/cf_manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,392 +1,266 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib-CFMan
-   @package: cfman.core
+   TODO Purpose of the file
+   @project: HSPyLib
+   hspylib.app.cfman.core
       @file: cf_manager.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2021, HSPyLib team
 """
-import requests
 import sys
-from clitt.core.tui.mchoose import mchoose
-from clitt.core.tui.menu.tui_menu_utils import TUIMenuUtils
-from clitt.core.tui.minput.minput import MenuInput, minput
-from clitt.core.tui.mselect import mselect
-from functools import partial
+from time import sleep
+from typing import List, Optional
+
+from hspylib.core.config.app_config import AppConfigs
 from hspylib.core.enums.http_code import HttpCode
-from hspylib.core.preconditions import check_state
-from hspylib.core.tools.commons import syserr, sysout
-from hspylib.modules.cache.ttl_cache import TTLCache
-from hspylib.modules.cli.vt100.vt_utils import clear_screen
+from hspylib.core.tools.commons import file_is_not_empty, syserr, sysout
+from hspylib.modules.cli.tui.extra.mchoose import mchoose
+from hspylib.modules.cli.tui.extra.minput.minput import MenuInput, minput
+from hspylib.modules.cli.tui.extra.mselect import mselect
+from hspylib.modules.cli.tui.menu.menu_utils import MenuUtils
 from hspylib.modules.fetch.fetch import head
-from retry import retry
-from time import sleep
-from typing import List, Optional, Tuple
 
 from cfman.core.cf import CloudFoundry
 from cfman.core.cf_application import CFApplication
-from cfman.core.cf_blue_green_checker import CFBlueGreenChecker
 from cfman.core.cf_endpoint import CFEndpoint
 from cfman.exception.exceptions import CFAuthenticationError, CFConnectionError, CFExecutionError
 
 
 class CFManager:
-    """Responsible for the CloudFoundry application functionalities.
-    """
+    """Represents the cloud foundry manager application and it's functionalities"""
 
-    CFMAN_ACTIONS = [
-        "Information", "Target", "Logs",
-        "Start", "Stop", "Restart", "Restage",
-        "Status", "Blue-Green-Check"
+    CF_ACTIONS = [
+        'Logs',
+        'Restart',
+        'Restage',
+        'Status',
+        'Start',
+        'Stop',
+        'Target',
     ]
 
     @staticmethod
     def _abort():
-        """Abort the execution and exit.
-        """
         sys.exit(1)
 
     @staticmethod
     def _allow_multiple(action: str) -> bool:
-        """Whether the action allows multiple application selection or not.
-        :param action the action to check
-        """
-        return action.lower() in [
-            "start", "stop", "restart", "restage"
-        ]
+        """Checks whether the action allows multiple apps selection or not"""
+        return action.lower() not in ['logs', 'target']
 
     @staticmethod
     def _is_callable(action: str) -> bool:
-        """Whether the provided action is callable or not.
-        :param action the action to check
-        """
-        return action.lower() in [
-            "logs", "start", "stop", "restart", "restage"
-        ]
-
-    @staticmethod
-    def required_states(action: str) -> str | Tuple[str, str]:
-        """Return the required application statue of the provided action
-        :param action the action to check
-        """
-        match action:
-            case "start":
-                return "stopped"
-            case "logs" | "stop" | "restart":
-                return "started"
-            case _:
-                return "started", "stopped"
-
-    def __init__(
-        self,
-        api: str,
-        org: str,
-        space: str,
-        username: str,
-        password: str,
-        no_cache: str,
-        cf_endpoints: str):
+        """Checks whether the action is callable or not"""
+        return action.lower() not in ['status', 'target']
 
+    def __init__(self, api: str, org: str, space: str, username: str, password: str, cf_endpoints: str):
+        assert file_is_not_empty(cf_endpoints), \
+            f'CF Endpoints file {cf_endpoints} is empty or does not exist !'
+        self.configs = AppConfigs.INSTANCE
         self._cf = CloudFoundry()
-        self._cache = TTLCache()
         self._api = api
         self._org = org
         self._space = space
         self._username = username
         self._password = password
-        self._no_cache = no_cache or False
         self._cf_endpoints_file = cf_endpoints
         self._cf_apps = None
         self._done = False
 
-    def __str__(self) -> str:
-        return (
-            f"%EOL%%GREEN%"
-            f"{'-=' * 40} %EOL%"
-            f"{self._api} %EOL%"
-            f"{'--' * 40} %EOL%"
-            f"{'USER:':>6} {self._username}%EOL%"
-            f"{'ORG:':>6} {self._org}%EOL%"
-            f"{'SPACE:':>6} {self._space}%EOL%"
-            f"{'-=' * 40}")
-
-    def __repr__(self) -> str:
-        return str(self)
-
-    @property
-    def apps(self) -> List[CFApplication]:
-        return self._get_apps() or []
-
     def run(self) -> None:
-        """Run the main cf manager application flow.
-        """
-        sysout("%BLUE%Checking CloudFoundry authorization...")
-        if self._cf.is_logged():
-            self._api = self._cf.api()
-            target = self._cf.target()
-            self._username, self._org, self._space = target.user, target.org, target.space
-            sysout("%YELLOW%Already authorized to CloudFoundry!")
+        """Execute main cf manager routines"""
+        sysout('%GREEN%Checking CloudFoundry authorization...')
+        if self._cf.connect():
+            sysout('%GREEN%Already authorized to CloudFoundry!')
         else:
             authorized = False
-            sysout("%YELLOW%Unauthorized to CloudFoundry, login required...")
-            sleep(2)
+            sysout('%YELLOW%Not authorized to CloudFoundry, login required...')
             while not authorized:
                 if not self._api:
+                    sleep(1)
                     self._select_endpoint()
                 if not self._username or not self._password:
-                    self._prompt_credentials()
-                sysout(f"%BLUE%Authorizing {self._username}@{self._api}...")
+                    sleep(1)
+                    self._require_credentials()
+                sysout(f'%GREEN%Authorizing {self._username}@{self._api}...')
                 authorized = self._authorize()
                 if not authorized:
                     self._password = None
-                    syserr("Not authorized !")
-                    self._abort()
-            sysout("%GREEN%Successfully authorized!")
-        sysout(f"%HOM%%ED0%%WHITE%--- Target information ---%EOL%{self}")
-        TUIMenuUtils.wait_keystroke()
+                    sleep(1)
+            sysout('%GREEN%Successfully authorized!')
+
         self._loop_actions()
 
-    @retry(exceptions=CFConnectionError, tries=3, delay=2, backoff=3, max_delay=30)
+    def _get_apps(self, refresh: bool = False) -> List[CFApplication]:
+        """Retrieve all cf applications under the target/org"""
+        if refresh or not self._cf_apps:
+            sysout(f'%GREEN%Retrieving applications from space: "{self._space}"...')
+            apps = self._cf.apps()
+            apps = list(map(CFApplication.of, apps if apps else []))
+            if not apps:
+                if "OK" not in self._cf.last_result:
+                    raise CFExecutionError(f'Unable to retrieve applications: => {self._cf.last_result}')
+                sysout('%YELLOW%No apps found')
+            self._cf_apps = apps
+
+        return self._cf_apps
+
     def _select_endpoint(self) -> None:
-        """Select the PCF endpoint to connect to.
-        """
+        """Select the PCF endpoint to connect to"""
         try:
-            with open(self._cf_endpoints_file, "r", encoding="utf-8") as f_hosts:
-                endpoints = list(map(lambda l: CFEndpoint(*l.strip().split(",")), f_hosts.readlines()))
+            with open(self._cf_endpoints_file, 'r', encoding='utf-8') as f_hosts:
+                endpoints = list(map(lambda l: CFEndpoint(l.split(',')), f_hosts.readlines()))
                 if len(endpoints) > 0:
-                    selected = mselect(endpoints, title="Please select an endpoint")
+                    selected = mselect(endpoints, title='Please select an endpoint')
                     if not selected:
                         self._abort()
-                    sysout(f"%BLUE%Connecting to endpoint: {selected}...")
+                    sysout(f"%GREEN%Connecting to endpoint: {selected}...")
                     try:
                         response = head(selected.host)
                         if response.status_code and HttpCode.OK:
                             self._api = selected.host
                         else:
-                            syserr(
-                                CFConnectionError(
-                                    f"Failed to contact CF API %EOL%"
-                                    f"  Status: ({response.status_code}): {selected}"))
+                            syserr(f'Failed to connect to API ({response.status_code}): {selected}')
                             self._abort()
-                    except requests.exceptions.ConnectionError as err:
-                        syserr(
-                            CFConnectionError(
-                                f"Failed to connect to CloudFoundry API%EOL%"
-                                f"  Host: '{selected.host}'%EOL%"
-                                f"  => {err.__class__.__name__}"))
-                        self._abort()
+                    except Exception as err:
+                        raise CFConnectionError(f'Failed to connect to API => {selected.host}') from err
                 else:
-                    syserr(
-                        CFExecutionError(
-                            f"No endpoint yet configured. Please create the file \"{self._cf_endpoints_file}\" "
-                            f"with at least one endpoint and try again!"))
+                    syserr(f"No endpoint yet configured. Please create the file {self._cf_endpoints_file} "
+                           f"with at least one endpoint configured and try again.")
                     self._abort()
-        except (IndexError, FileNotFoundError) as err:
-            syserr(
-                CFExecutionError(
-                    f"Endpoint file \"{self._cf_endpoints_file}\" is invalid: %EOL%"
-                    f"  => {str(err)}! %EOL%"
-                    f"Make sure it exists contains the following: %EOL%"
-                    f"<alias>,<cf_api_url>,<protected [true|false]>%EOL%"))
+        except IndexError:
+            syserr(f'{self._cf_endpoints_file} '
+                   f'has invalid cf endpoints format. Please use: <alias>, <url>, <protected [true,false]>')
             self._abort()
 
-    def _prompt_credentials(self) -> None:
-        """Prompt the user for his PCF credentials.
-        """
-        # fmt: off
-        form_fields = (
-            MenuInput.builder()
-                .field()
-                    .label("Username")
-                    .value(self._username)
-                    .build()
-                .field()
-                    .label("Password")
-                    .itype("password")
-                    .value(self._password)
-                    .build()
+    def _require_credentials(self) -> None:
+        """Prompt the user for PCF credentials"""
+        form_fields = MenuInput.builder() \
+            .field().label('Username').value(self._username).build() \
+            .field().label('Password').itype('password').value(self._password).build() \
             .build()
-        )
-        # fmt: on
-        result = minput(form_fields, title="Please type your Cloud Foundry credentials")
+        result = minput(form_fields, title='Please type your Cloud Foundry credentials')
         if result:
             self._username = result.username
             self._password = result.password
         else:
             self._abort()
 
     def _authorize(self) -> bool:
-        """Send an authorization request to PCF.
-        """
+        """Send an authorization request to PCF"""
         if not self._cf.api(self._api):
-            raise CFExecutionError(f"Unable to set API: => {self._cf.last_output}")
+            raise CFExecutionError(f'Unable to set API: => {self._cf.last_result}')
         if not self._cf.auth(self._username, self._password):
-            raise CFAuthenticationError(f"Unable to authenticate to => {self._api}")
+            raise CFAuthenticationError(f'Unable to authenticate to => {self._api}')
 
         return True
 
     def _set_org(self) -> None:
-        """Set the active PCF organization.
-        """
+        """Set the active organization"""
         if not self._org:
-            sysout(f"%BLUE%Retrieving all organizations from api: \"{self._api}\"...")
-            if not (orgs := self._cf.orgs()):
-                raise CFExecutionError(f"Unable to retrieve organizations: => {self._cf.last_output}")
-            self._org = mselect(orgs, title="Please select the PCF organization")
+            sysout('%YELLOW%Checking organization...')
+            orgs = self._cf.orgs()
+            if not orgs:
+                raise CFExecutionError(f'Unable to retrieve organizations: => {self._cf.last_result}')
+            self._org = mselect(orgs, title='Please select the organization')
             if not self._org:
                 self._abort()
             else:
                 self._target()
 
     def _set_space(self) -> None:
-        """Set the active PCF space.
-        """
+        """Set the active space"""
         if not self._space:
-            if self._no_cache or not (spaces := self._cache.read(f"cf-spaces-{self._org}")):
-                sysout(f"%BLUE%Retrieving all spaces from org: \"{self._org}\"...")
-                spaces = self._cf.spaces()
-                self._cache.save(f"cf-spaces-{self._org}", spaces)
+            sysout('%YELLOW%Checking space...')
+            spaces = self._cf.spaces()
             if not spaces:
-                raise CFExecutionError(f"Unable to retrieve org={self._org} spaces: => {self._cf.last_output}")
-            self._space = mselect(spaces, title="Please select the PCF space")
+                raise CFExecutionError(f'Unable to retrieve spaces: => {self._cf.last_result}')
+            self._space = mselect(spaces, title='Please select a space')
             if not self._space:
                 self._abort()
             else:
                 self._target()
 
-    def _get_apps(self) -> List[CFApplication]:
-        """Retrieve all cf applications under the targeted org-space.
-        """
-        if self._no_cache or not (apps := self._cache.read(f"cf-apps-{self._space}")):
-            sysout(f"%BLUE%Retrieving applications from space: \"{self._space}\"...")
-            apps = self._cf.apps()
-            sysout(f"%GREEN%Found {len(apps)} apps in space: \"{self._space}\"")
-            self._cache.save(f"cf-apps-{self._space}", apps)
-        if not apps:
-            if "OK" not in self._cf.last_output:
-                raise CFExecutionError(f"Unable to retrieve applications: => {self._cf.last_output}")
-            syserr(f"%YELLOW%No applications found for space: \"{self._space}\"")
-        cf_apps = list(map(CFApplication.of, apps if apps else []))
-        self._cf_apps = cf_apps
-
-        return self._cf_apps
-
-    def _choose_apps(self, required_states: str | Tuple[str, str]) -> Optional[List[CFApplication]]:
-        """Choose multiple PCF apps from the available list.
-        :param required_states used to filter the apps to choose by the application state.
-        """
-        self._cf_apps = list(filter(lambda app: app.state.lower() in required_states, self.apps))
+    def _choose_apps(self) -> Optional[List[CFApplication]]:
+        """Choose multiple PCF apps from the available list"""
         if not self._cf_apps:
-            return None
-        return mchoose(self._cf_apps, checked=False, title="Please choose the applications you want to manage")
+            self._cf_apps = self._get_apps()
+        return mchoose(self._cf_apps, checked=False, title='Please choose the applications you want to manage')
 
-    def _select_app(self, required_states: str | Tuple[str, str]) -> Optional[CFApplication]:
-        """Select a single PCF app from the available list.
-        :param required_states used to filter the apps to choose by the application state.
-        """
-        self._cf_apps = list(filter(lambda app: app.state.lower() in required_states, self.apps))
+    def _select_app(self) -> Optional[CFApplication]:
+        """Select a single PCF app from the available list"""
         if not self._cf_apps:
-            return None
-        return mselect(self._cf_apps, title="Please select the application you want to manage")
+            self._cf_apps = self._get_apps()
+        return mselect(self._cf_apps, title='Please select the application you want to manage')
 
     def _target(self) -> None:
-        """Attempt to target to a PCF org-space.
-        """
-        if not self._cf.target(user=self._username, org=self._org, space=self._space):
-            raise CFExecutionError(f"Unable to target ORG: {self._org} => {self._cf.last_output}")
-        sleep(1)
+        """Send a target request to PCF"""
+        sysout(f"%GREEN%Targeting ORG={self._org} and SPACE={self._space}...")
+        if not self._cf.target(org=self._org, space=self._space):
+            raise CFExecutionError(f"Unable to target ORG: {self._org} => {self._cf.last_result}")
 
     def _loop_actions(self) -> None:
-        """Wait for the user interactions.
-        """
-        while self._assert_target():
-            if not (action := mselect(CFManager.CFMAN_ACTIONS, "Please select an action to perform")):
+        """Wait for the user interactions"""
+        while not self._done:
+            if self._org and self._space and not self._cf.is_targeted():
+                self._target()
+            else:
+                self._set_org()
+                self._set_space()
+
+            if not self._org or not self._space or not self._cf.is_targeted():
+                raise CFExecutionError(
+                    f"Unable to target ORG={self._org}  SPACE={self._space} => {self._cf.last_result}")
+
+            action = mselect(CFManager.CF_ACTIONS, 'Please select an action to perform')
+
+            if not action:
                 self._done = True
-                return
-            if self._is_callable(action):
-                self._perform_callable(action)
             else:
-                match action.lower():
-                    case "status":
+                if self._is_callable(action):
+                    self._perform_callable(action)
+                else:
+                    if action.lower() == 'status':
                         self._display_app_status()
-                    case "target":
+                    elif action.lower() == 'target':
                         self._space = self._org = self._cf_apps = None
-                        self._cf.clear_target()
+                        self._cf.targeted = {'org': None, 'space': None, 'targeted': False}
                         continue
-                    case "blue-green-check":
-                        self._blue_green_check()
-                    case "information":
-                        sysout(f"%HOM%%ED0%%WHITE%--- Target information ---%EOL%{self}")
 
-                TUIMenuUtils.wait_keystroke()
-
-    def _assert_target(self) -> bool:
-        if not self._org:
-            self._set_org()
-        if not self._space:
-            self._set_space()
-        if not self._cf.is_targeted():
-            self._target()
-        if not self._org or not self._space or not self._cf.is_targeted():
-            raise CFExecutionError(
-                f"Unable to target ORG={self._org}  SPACE={self._space} => {self._cf.last_output}"
-            )
-        return not self._done
-
-    def _display_app_status(self) -> None:
-        """Display all PCF space-application statuses.
-        """
-        apps = self.apps
+                    MenuUtils.wait_enter()
 
+    def _display_app_status(self):
+        """Display select apps status"""
+        apps = self._get_apps(refresh=True)
         if len(apps) > 0:
-            clear_screen()
-            # fmt: off
-            sysout(
-                f"%BLUE%Listing '{self._org}::{self._space}' applications ...%EOL%%WHITE%"
-                f"{'-=' * 60 + '%EOL%'}"
-                f"{'Name':{CFApplication.max_name_length + 2}}"
-                f"{'State':<9}{'Instances':<12}{'Mem':<6}{'Disk':<6}Routes%EOL%")
-            # fmt: on
-            list(map(CFApplication.print_status, apps))
-            sysout('-=' * 60 + '%EOL%')
-
-    def _blue_green_check(self) -> None:
-        """Display all PCF space-application blue/green check.
-        """
-        if len(self.apps) > 0:
-            clear_screen()
-            sysout(f"%BLUE%Checking blue/green deployments ...%EOL%")
-            CFBlueGreenChecker.check(self._org, self._space, self.apps)
-
-    def _perform_callable(self, action: str) -> None:
-        """Wrapper of the _perform method.
-        :param action the action to perform.
-        """
-        act = action.lower()
-        if self._allow_multiple(act):
-            apps = self._choose_apps(self.required_states(act))
+            # pylint: disable=consider-using-f-string
+            sysout("%WHITE%{}  {}  {}  {}  {}  {}".format(
+                'Name'.ljust(CFApplication.max_name_length),
+                'State'.ljust(7), 'Instances'.ljust(10), 'Mem'.ljust(4),
+                'Disk'.ljust(4), 'URLs',
+            ))
+            for app in apps:
+                app.print_status()
+
+    def _perform_callable(self, action):
+        """Perform the selected callable action"""
+        if self._allow_multiple(action.lower()):
+            apps = self._choose_apps()
         else:
-            app = self._select_app(self.required_states(act))
+            app = self._select_app()
             apps = [app] if app else None
         if apps:
-            perform = partial(self._perform, action=act, org=self._org, space=self._space)
-            list(map(lambda a: perform(app=a.name), apps))
+            for app in apps:
+                self._perform(action, app=app.name, org=self._org, space=self._space)
 
-    def _perform(self, action: str, **kwargs) -> None:
-        """Perform the selected PCF action.
-        Kwargs:
-              org (str): the PCF organization name.
-            space (str): the PCF space name.
-        :param kwargs arbitrary PCF action arguments.
-        :param action the action to perform.
-        """
-        sysout(f"%BLUE%Performing {action} {str(kwargs)}...")
-        action_method = getattr(self._cf, action)
-        check_state(callable(action_method))
-        sysout(action_method(**kwargs))
+    def _perform(self, action: str, **kwargs):
+        """Perform the selected PCF action"""
+        sysout(f'%GREEN%Performing {action.lower()} {str(kwargs)}...')
+        method_to_call = getattr(self._cf, action.lower())
+        sysout(method_to_call(**kwargs))
```

### Comparing `hspylib-cfman-0.9.88/hspylib_cfman.egg-info/SOURCES.txt` & `hspylib-cfman-0.9.9/hspylib_cfman.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 MANIFEST.in
 README.md
 setup.py
 cfman/.version
-cfman/__classpath__.py
 cfman/__init__.py
 cfman/__main__.py
 cfman/welcome.txt
 cfman/core/__init__.py
 cfman/core/cf.py
 cfman/core/cf_application.py
-cfman/core/cf_blue_green_checker.py
 cfman/core/cf_endpoint.py
 cfman/core/cf_manager.py
 cfman/exception/__init__.py
 cfman/exception/exceptions.py
+cfman/resources/application.properties
+cfman/resources/log/.gitkeep
+cfman/resources/log/application.log
 hspylib_cfman.egg-info/PKG-INFO
 hspylib_cfman.egg-info/SOURCES.txt
 hspylib_cfman.egg-info/dependency_links.txt
 hspylib_cfman.egg-info/requires.txt
 hspylib_cfman.egg-info/top_level.txt
```

### Comparing `hspylib-cfman-0.9.88/setup.py` & `hspylib-cfman-0.9.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,56 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib-CFMan
+   TODO Purpose of the file
+   @project: HSPyLib
       @file: setup.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
-
-   Reference: https://setuptools.pypa.io/en/latest/references/keywords.html
+   Copyright 2021, HSPyLib team
 """
 
 import pathlib
 
 import setuptools
 
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # The version of the package
-VERSION = (HERE / "cfman/.version").read_text().strip()
+VERSION = (HERE / "cfman/.version").read_text()
 
 # The package requirements
 REQUIREMENTS = list(filter(None, (HERE / "requirements.txt").read_text().splitlines()))
 
 # This call to setup() does all the work
 setuptools.setup(
-    name="hspylib-cfman",
+    name='hspylib-cfman',
     version=VERSION,
-    description="HSPyLib - CloudFoundry manager",
-    author="Hugo Saporetti Junior",
-    author_email="yorevs@hotmail.com",
+    description='HomeSetup CloudFoundry manager',
+    author='Hugo Saporetti Junior',
+    author_email='yorevs@hotmail.com',
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/yorevs/hspylib",
-    project_urls={"GitHub": "https://github.com/yorevs/hspylib", "PyPi": "https://pypi.org/project/hspylib-cfman/"},
-    license="MIT",
-    license_files="LICENSE.md",
-    packages=setuptools.find_namespace_packages(),
+    license='MIT',
+    packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
-        "Operating System :: Unix",
-        "Development Status :: 3 - Alpha",
-        "Environment :: Console",
-        "Natural Language :: English",
-        "Topic :: Terminals",
+        "Operating System :: Unix"
+
     ],
-    python_requires=">=3.10",
+    python_requires='>=3.7',
     install_requires=REQUIREMENTS,
-    keywords="pivotal,pcf,cloudfoundry,manager,application",
-    platforms="Darwin,Linux",
 )
```


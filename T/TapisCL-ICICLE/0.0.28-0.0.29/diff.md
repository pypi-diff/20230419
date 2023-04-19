# Comparing `tmp/TapisCL-ICICLE-0.0.28.tar.gz` & `tmp/TapisCL-ICICLE-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.28.tar", last modified: Tue Apr 18 23:40:11 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.29.tar", last modified: Wed Apr 19 04:52:39 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.28.tar` & `TapisCL-ICICLE-0.0.29.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 23:40:11.605894 TapisCL-ICICLE-0.0.28/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.28/LICENSE
--rw-rw-rw-   0        0        0    44210 2023-04-18 23:40:11.605391 TapisCL-ICICLE-0.0.28/PKG-INFO
--rw-rw-rw-   0        0        0     2300 2023-04-18 23:36:28.000000 TapisCL-ICICLE-0.0.28/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 23:40:11.596109 TapisCL-ICICLE-0.0.28/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/__main__.py
--rw-rw-rw-   0        0        0     1597 2023-04-18 02:12:46.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/args.py
--rw-rw-rw-   0        0        0    10894 2023-04-18 02:36:57.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/cli.py
--rw-rw-rw-   0        0        0     9161 2023-04-18 02:36:33.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/decorators.py
--rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/exceptions.py
--rw-rw-rw-   0        0        0     5754 2023-04-18 02:23:18.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/helpers.py
--rw-rw-rw-   0        0        0     2023 2023-04-18 02:17:20.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/schemas.py
--rw-rw-rw-   0        0        0    10260 2023-04-18 02:42:20.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/server.py
--rw-rw-rw-   0        0        0     1645 2023-04-18 02:26:10.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/socketOpts.py
--rw-rw-rw-   0        0        0    19155 2023-04-18 23:35:02.000000 TapisCL-ICICLE-0.0.28/TapisCLICICLE/tapisObjectWrappers.py
-drwxrwxrwx   0        0        0        0 2023-04-18 23:40:11.604447 TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    44210 2023-04-18 23:40:11.000000 TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-04-18 23:40:11.000000 TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 23:40:11.000000 TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-18 23:40:11.000000 TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-04-18 23:40:11.000000 TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-18 23:40:11.000000 TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-04-18 23:39:28.000000 TapisCL-ICICLE-0.0.28/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 23:40:11.605894 TapisCL-ICICLE-0.0.28/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 04:52:39.517221 TapisCL-ICICLE-0.0.29/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.29/LICENSE
+-rw-rw-rw-   0        0        0    44210 2023-04-19 04:52:39.516220 TapisCL-ICICLE-0.0.29/PKG-INFO
+-rw-rw-rw-   0        0        0     2300 2023-04-18 23:36:28.000000 TapisCL-ICICLE-0.0.29/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 04:52:39.509058 TapisCL-ICICLE-0.0.29/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/__main__.py
+-rw-rw-rw-   0        0        0     1474 2023-04-19 03:20:32.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/args.py
+-rw-rw-rw-   0        0        0    10959 2023-04-19 04:50:36.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/cli.py
+-rw-rw-rw-   0        0        0     9161 2023-04-19 04:39:15.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/decorators.py
+-rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/exceptions.py
+-rw-rw-rw-   0        0        0     5592 2023-04-19 04:46:55.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/helpers.py
+-rw-rw-rw-   0        0        0     2023 2023-04-18 02:17:20.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/schemas.py
+-rw-rw-rw-   0        0        0    10424 2023-04-19 04:49:26.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/server.py
+-rw-rw-rw-   0        0        0     1645 2023-04-18 02:26:10.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/socketOpts.py
+-rw-rw-rw-   0        0        0    19567 2023-04-19 04:33:11.000000 TapisCL-ICICLE-0.0.29/TapisCLICICLE/tapisObjectWrappers.py
+drwxrwxrwx   0        0        0        0 2023-04-19 04:52:39.515224 TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    44210 2023-04-19 04:52:39.000000 TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-04-19 04:52:39.000000 TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 04:52:39.000000 TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-19 04:52:39.000000 TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-04-19 04:52:39.000000 TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-19 04:52:39.000000 TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-04-19 04:51:53.000000 TapisCL-ICICLE-0.0.29/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 04:52:39.517221 TapisCL-ICICLE-0.0.29/setup.cfg
```

### Comparing `TapisCL-ICICLE-0.0.28/LICENSE` & `TapisCL-ICICLE-0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.28/PKG-INFO` & `TapisCL-ICICLE-0.0.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.28
+Version: 0.0.29
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.28/README.md` & `TapisCL-ICICLE-0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.28/TapisCLICICLE/args.py` & `TapisCL-ICICLE-0.0.29/TapisCLICICLE/args.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,18 +36,14 @@
             "args":["-n", "--name"],
             "kwargs":{"action":"store"}
         },
         "uuid":{
             "args":["-U", "--uuid"],
             "kwargs":{"action":"store"}
         },
-        "description":{
-            "args":["-d", "--description"],
-            "kwargs":{"action":"store"}
-        },
         "link":{
             "args":["-l", "--link"],
             "kwargs":{"action":"store"}
         },
         "verbose":{
             "args":["-v", "--verbose"],
             "kwargs":{"action":"store_true"}
```

### Comparing `TapisCL-ICICLE-0.0.28/TapisCLICICLE/cli.py` & `TapisCL-ICICLE-0.0.29/TapisCLICICLE/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,17 @@
 
     def fillout_form(self, form: list) -> dict:
         """
         fill out a form as requested by the server for more complicated functions
         """
         filled_form = dict()
         for field in form:
-            value = str(input(f"{field}: "))
+            value = str(input(f"{field}: ")).strip()
+            if not value:
+                value = None
             filled_form.update({field:value})
         return filled_form
 
     def command_operator(self, kwargs: dict | list, exit_: int=0): 
         """
         parse arguments, handling bash and CLI input
         """
```

### Comparing `TapisCL-ICICLE-0.0.28/TapisCLICICLE/decorators.py` & `TapisCL-ICICLE-0.0.29/TapisCLICICLE/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.28/TapisCLICICLE/exceptions.py` & `TapisCL-ICICLE-0.0.29/TapisCLICICLE/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.28/TapisCLICICLE/helpers.py` & `TapisCL-ICICLE-0.0.29/TapisCLICICLE/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,17 +27,16 @@
     """
     filters the kwargs received by the server to prevent an error from happening
     """
     def filter_kwargs(self, func: typing.Callable, kwargs: dict) -> dict:
         filtered = dict()
         variables = list(get_parameters(func))
         for arg in variables:
-            if arg != "password" and arg != "expression": filtered.update({arg:kwargs[arg]})
-            elif arg == "password": filtered.update({'password':None})
-            elif arg == "expression": filtered.update({'expression':None})
+            if arg in command_parameters: filtered.update({arg:kwargs[arg]})
+            else: filtered.update({arg:None})
         return filtered
 
     def print_dict(self, dict_):
         for key, value in dict_.items():
             print(f"{key}: {value}")
     
 
@@ -78,15 +77,15 @@
                 if map == self.command_map:
                     argument_help = f"{command_name}"
                     arguments = get_parameters(command)
                 else:
                     argument_help = f"{command_name} -c help"
             if arguments:
                 for argument in arguments:
-                    if argument != "password" and argument != "description" and argument != "expression":
+                    if argument in args.Args.argparser_args:
                         argument_help += f" {command_parameters[argument]['args'][1]} <{argument}>"
 
             command_help['syntax'] = argument_help
             help_menu[command_name] = command_help
         return help_menu
             
     def help_generation(self) -> dict:
```

### Comparing `TapisCL-ICICLE-0.0.28/TapisCLICICLE/schemas.py` & `TapisCL-ICICLE-0.0.29/TapisCLICICLE/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.28/TapisCLICICLE/server.py` & `TapisCL-ICICLE-0.0.29/TapisCLICICLE/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from getpass import getpass
 import time
 import re
 from tapipy.tapis import Tapis
 import socket
 import os
 import logging
-from tapisObjectWrappers import Files, Apps, Pods, Systems, Neo4jCLI
+from tapisObjectWrappers import Files, Apps, Pods, Systems, Neo4jCLI, PostgresCLI
 import typing
 
 try:
     from . import exceptions
     from . import socketOpts as SO
     from . import helpers
     from . import schemas
@@ -86,14 +86,15 @@
         }
         self.command_map = {
             'help':self.help,
             'whoami':self.pods.whoami,
             'exit':self.__exit,
             'shutdown':self.__shutdown,
             'neo4j':self.neo4j,
+            'postgres':self.postgres,
             'switch_service':self.tapis_init
         }
         help0, help1 = self.help_generation()
         self.help = dict(help0, **help1)
 
     @decorators.Auth
     def tapis_init(self, username: str, password: str, link: str) -> tuple[typing.Any, str, str] | None:  # link is the baseURL
@@ -131,14 +132,15 @@
             os.system(f"export JWT={access_token}")
 
         self.pods = Pods(t, username, password, connection=self.connection)
         self.systems = Systems(t, username, password, connection=self.connection)
         self.files = Files(t, username, password, connection=self.connection)
         self.apps = Apps(t, username, password, connection=self.connection)
         self.neo4j = Neo4jCLI(t, username, password, connection=self.connection)
+        self.postgres = PostgresCLI(t, username, password, connection=self.connection)
 
         self.t = t
         self.url = url
         self.access_token = access_token
 
         self.logger.info(f"initiated in {time.time()-start}")
 
@@ -253,14 +255,14 @@
                 error_response = schemas.ResponseData(response_message = str(e), exit_status=1)
                 self.json_send(error_response.dict())
                 self.connection.close()  # close the connection
                 self.accept()  # wait for CLI to reconnect
             except (exceptions.CommandNotFoundError, exceptions.NoConfirmationError, exceptions.InvalidCredentialsReceived, Exception) as e:
                 error_response = schemas.ResponseData(response_message = str(e))
                 self.json_send(error_response.dict())
-                self.logger.warning(str(e))
+                self.logger.warning(f"{str(e)}\n{e.__traceback__}")
 
 
 
 if __name__ == '__main__':
     server = Server(socket.gethostbyname(socket.gethostname()), 30000)
     server.main()
```

### Comparing `TapisCL-ICICLE-0.0.28/TapisCLICICLE/socketOpts.py` & `TapisCL-ICICLE-0.0.29/TapisCLICICLE/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.28/TapisCLICICLE/tapisObjectWrappers.py` & `TapisCL-ICICLE-0.0.29/TapisCLICICLE/tapisObjectWrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import pyperclip
 import tapipy
 from tapipy.tapis import TapisResult
 from py2neo import Graph
 import typing
 import os
+import psycopg2
 try:
     from . import helpers
     from . import decorators
 except:
     import helpers 
     import decorators
 
@@ -27,25 +28,20 @@
 
         self.command_map = command_map
         
         if self.command_map:
             self.help = self.help_generation()
 
     def __call__(self, **kwargs):
-        try:
-            command = self.command_map[kwargs['command']]
-            kwargs = self.filter_kwargs(command, kwargs)
-            result = command(**kwargs)
-            if type(result) == TapisResult:
-                return str(result)
-            return result
-        except (tapipy.errors.NotFoundError, tapipy.errors.BadRequestError, tapipy.errors.BaseTapyException) as e:
-            return str(e)
-        except KeyError:
-            return self.help
+        command = self.command_map[kwargs['command']]
+        kwargs = self.filter_kwargs(command, kwargs)
+        result = command(**kwargs)
+        if type(result) == TapisResult:
+            return str(result)
+        return result
     
     def help(self, name: typing.Optional[str]):
         """
         @help: get help information for the command group
         """
         if name:
             return self.help[name]
@@ -55,20 +51,21 @@
 class TapisQuery(tapisObject):
     def __init__(self, tapis_object, uname, pword, connection=None):
         super().__init__(tapis_object, uname, pword, connection=connection)
         self.t = tapis_object
         self.__code__ = self.query.__code__
 
     def __call__(self, **kwargs):
-        try:
-            kwargs = self.filter_kwargs(self.query, kwargs)
-            result = self.query(**kwargs)
-            return result
-        except (tapipy.errors.NotFoundError, tapipy.errors.BadRequestError, tapipy.errors.BaseTapyException) as e:
-            return str(e)
+        kwargs = self.filter_kwargs(self.query, kwargs)
+        result = self.query(**kwargs)
+        return result
+        
+    def get_credentials(self):
+        uname, pword = self.t.pods.get_pod_credentials(pod_id=id).user_username, self.t.pods.get_pod_credentials(pod_id=id).user_password
+        return uname, pword
 
 
 class Systems(tapisObject):
     """
     @help: Access Tapis systems through the connected service
     @doc: provides a CLI interface to the Tapis Systems service
     """
@@ -169,32 +166,47 @@
     @decorators.NeedsConfirmation
     def delete_system(self, id: str) -> str:
         """
         @help: delete the selected system
         """
         return_value = self.t.systems.deleteSystem(systemId=id)
         return return_value
+    
+
+class PostgresCLI(TapisQuery):
+    """
+    @help: integrated CLI to interface with Postgres pods
+    """
+    @decorators.RequiresExpression
+    def query(self, id: str, expression: str) -> str:
+        uname, pword = self.get_credentials()
+        with psycopg2.connect(f"postgresql://{uname}:{pword}@{id}.pods.{self.t.base_url.split('https://')[1]}:443") as conn:
+            conn.autocommit = True
+            with conn.cursor() as cur:
+                cur.execute(query=expression)
+                return_value = cur.fetchall()
+        return str(f'[+][{id}] {return_value}')
 
 
 class Neo4jCLI(TapisQuery):
     """
     @help: integrated CLI to interface with Neo4j pods
     """
     @decorators.RequiresExpression
     def query(self, id: str, expression: str) -> str: # function to submit queries to a Neo4j knowledge graph
-        uname, pword = self.t.pods.get_pod_credentials(pod_id=id).user_username, self.t.pods.get_pod_credentials(pod_id=id).user_password
-        graph = Graph(f"bolt+ssc://{id}.pods.icicle.tapis.io:443", auth=(uname, pword), secure=True, verify=True)
+        uname, pword = self.get_credentials()
+        graph = Graph(f"bolt+ssc://{id}.pods.{self.t.base_url.split('https://')[1]}:443", auth=(uname, pword), secure=True, verify=True)
 
         try:
             return_value = graph.run(expression)
             print(type(return_value))
             if str(return_value) == '(No data)' and 'create' in expression.lower(): # if no data is returned (mostly if something is created) then just say 'success'
-                return f'[+][{id}@pods.icicle.tapis.io:443] Success'
+                return f'[+][{id}@pods.{self.t.base_url.split("https://")[1]}:443] Success'
             elif str(return_value) == '(No data)':
-                return f'[-][{id}@pods.icicle.tapis.io:443] KG is empty'
+                return f'[-][{id}@pods.{self.t.base_url.split("https://")[1]}:443] KG is empty'
 
             print(return_value)
             print(type(return_value))
             return str(f'[+][{id}] {return_value}')
         except Exception as e:
             return str(e)
 
@@ -242,15 +254,15 @@
         """
         user_info = self.t.authenticator.get_userinfo()
         if verbose:
             return str(user_info)
         return user_info.username
 
     @decorators.RequiresForm
-    def create_pod(self, description: str, id: str, template: str, verbose: bool) -> str:
+    def create_pod(self, id: str, template: str, verbose: bool, description: str | None = None) -> str:
         """
         @help: create a new pod on the selected Tapis service
         """
         pod_information = self.t.pods.create_pod(pod_id=id, pod_template=template, description=description)
         if verbose:
             return str(pod_information)
         return pod_information
```

### Comparing `TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.28
+Version: 0.0.29
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.28/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.0.29/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.28/pyproject.toml` & `TapisCL-ICICLE-0.0.29/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.28"
+version = "0.0.29"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
@@ -18,15 +18,16 @@
 ]
 keywords = ["Tapis", "CLI", "Agave", "HPC", "Tapis Pods", "TACC"]
 dependencies = [
     "pydantic",
     "pyfiglet",
     "tapipy",
     "pyperclip",
-    "py2neo"
+    "py2neo",
+    "psycopg"
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = []
 
 [project.urls]
```


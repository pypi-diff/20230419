# Comparing `tmp/convex-0.2.0.tar.gz` & `tmp/convex-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convex-0.2.0.tar", max compression
+gzip compressed data, was "convex-0.3.0.tar", max compression
```

## Comparing `convex-0.2.0.tar` & `convex-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    11343 2023-02-25 00:40:22.088939 convex-0.2.0/LICENSE
--rw-r--r--   0        0        0     9635 2023-02-25 03:30:10.861708 convex-0.2.0/README.md
--rw-r--r--   0        0        0     3287 2023-02-25 03:30:10.861904 convex-0.2.0/convex/__init__.py
--rw-r--r--   0        0        0        0 2023-02-25 00:40:22.089306 convex-0.2.0/convex/py.typed
--rw-r--r--   0        0        0    21018 2023-02-25 00:40:22.089525 convex-0.2.0/convex/values.py
--rw-r--r--   0        0        0     1258 2023-02-25 03:30:10.862434 convex-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    10554 1970-01-01 00:00:00.000000 convex-0.2.0/setup.py
--rw-r--r--   0        0        0    10564 1970-01-01 00:00:00.000000 convex-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-04-11 18:46:13.543061 convex-0.3.0/LICENSE
+-rw-r--r--   0        0        0     9588 2023-04-18 23:43:48.499613 convex-0.3.0/README.md
+-rw-r--r--   0        0        0     3529 2023-04-18 23:43:48.499788 convex-0.3.0/convex/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 18:46:13.543422 convex-0.3.0/convex/py.typed
+-rw-r--r--   0        0        0    21018 2023-04-11 18:46:13.543566 convex-0.3.0/convex/values.py
+-rw-r--r--   0        0        0     1258 2023-04-18 23:43:48.499938 convex-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10517 1970-01-01 00:00:00.000000 convex-0.3.0/PKG-INFO
```

### Comparing `convex-0.2.0/LICENSE` & `convex-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `convex-0.2.0/README.md` & `convex-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # Convex
 
 The official Python client for [Convex](https://convex.dev/).
 
-Convex is the TypeScript-native programmable database for the web. No need for
-backend containers, caches, queues, and query languages. Convex replaces all of
-them with a few simple APIs.
-
-This Python client can write and read data from a Convex backend with queries,
-mutations, and actions. Get up and running at
-[docs.convex.dev](https://docs.convex.dev/introduction/).
+![PyPI](https://img.shields.io/pypi/v/convex?label=convex&logo=pypi)
+![GitHub](https://img.shields.io/github/license/get-convex/convex-py)
+
+Write and read data from a Convex backend with queries, mutations, and actions.
+Get up and running at [docs.convex.dev](https://docs.convex.dev/home).
 
 Installation:
 
     pip install convex
 
 Basic usage:
 
@@ -26,15 +24,15 @@
   '_id': Id(table_name='messages', id='c09S884lW4kTLdQMtu2ravf'),
   'author': 'Tom',
   'body': 'Have you tried Convex?'},
  {'_creationTime': 1668107497732.2295,
   '_id': Id(table_name='messages', id='G3m0cCQp65GQDfUjUDnTPEj'),
   'author': 'Sarah',
   'body': "Yeah, it's working pretty well for me."}]
->>> client.mutation("sendMessage")
+>>> client.mutation("sendMessage", dict(author="Me", body="Hello!"))
 ```
 
 To find the url of your convex backend, open the deployment you want to work
 with in the appropriate project in the
 [Convex dashboard](https://dashboard.convex.dev) and click "Settings" where the
 Deployment URL should be visible. To find out which queries, mutations, and
 actions are available check the Functions pane in the Dashboard
```

### Comparing `convex-0.2.0/convex/__init__.py` & `convex-0.3.0/convex/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,21 +24,24 @@
     "ConvexError",
     "ConvexClient",
     "ConvexSet",
     "ConvexMap",
 ]
 
 
-__version__ = "0.2.0"  # Also update in pyproject.toml
+__version__ = "0.3.0"  # Also update in pyproject.toml
 
 
 class ConvexExecutionError(Exception):
     """Convex execution error on server."""
 
 
+FunctionArgs = Optional[Dict[str, CoercibleToConvexValue]]
+
+
 class ConvexClient:
     """Client for communicating with convex."""
 
     def __init__(self, address: str) -> None:
         """Instantiate a `ConvexClient` that speaks to a deployment at `address`."""
         self.address: str = address
         self.auth: Optional[str] = None
@@ -57,20 +60,25 @@
         """Clear any auth previously set."""
         self.auth = None
 
     def set_debug(self, value: bool) -> None:
         """Set whether the result log lines should be printed on the console."""
         self.debug = value
 
-    def _request(
-        self, url: str, name: str, args: CoercibleToConvexValue
-    ) -> ConvexValue:
+    def _request(self, url: str, name: str, args: FunctionArgs) -> ConvexValue:
+        if args is None:
+            args = {}
+        if not type(args) is dict:
+            raise Exception(
+                f"Arguments to a Convex function must be a dictionary. Received: {args}"
+            )
+
         data: Dict[str, JsonValue] = {
             "path": name,
-            "args": convex_to_json(args),
+            "args": [convex_to_json(args)],
         }
         if self.debug:
             data["debug"] = self.debug
 
         headers = self.headers.copy()
         if self.auth is not None:
             headers["Authorization"] = self.auth
@@ -91,21 +99,21 @@
 
         if response["status"] == "success":
             return json_to_convex(response["value"])
         if response["status"] == "error":
             raise ConvexExecutionError(response["errorMessage"])
         raise Exception("Received unexpected response from Convex server.")
 
-    def query(self, name: str, *args: CoercibleToConvexValue) -> Any:
+    def query(self, name: str, args: FunctionArgs = None) -> Any:
         """Run a query on Convex."""
         url = f"{self.address}/api/query"
         return self._request(url, name, args)
 
-    def mutation(self, name: str, *args: CoercibleToConvexValue) -> Any:
+    def mutation(self, name: str, args: FunctionArgs = None) -> Any:
         """Run a mutation on Convex."""
         url = f"{self.address}/api/mutation"
         return self._request(url, name, args)
 
-    def action(self, name: str, *args: CoercibleToConvexValue) -> Any:
+    def action(self, name: str, args: FunctionArgs = None) -> Any:
         """Run an action on Convex."""
         url = f"{self.address}/api/action"
         return self._request(url, name, args)
```

### Comparing `convex-0.2.0/convex/values.py` & `convex-0.3.0/convex/values.py`

 * *Files identical despite different names*

### Comparing `convex-0.2.0/pyproject.toml` & `convex-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "convex"
-version = "0.2.0"  # Also update in __init__.py
+version = "0.3.0"  # Also update in __init__.py
 description = "Python client for the reactive backend-as-a-service Convex."
 authors = ["Convex, Inc. <support@convex.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://convex.dev"
 repository = "https://github.com/get-convex/convex-py"
 documentation = "https://docs.convex.dev"
```

### Comparing `convex-0.2.0/setup.py` & `convex-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,201 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: convex
+Version: 0.3.0
+Summary: Python client for the reactive backend-as-a-service Convex.
+Home-page: https://convex.dev
+License: Apache-2.0
+Author: Convex, Inc.
+Author-email: support@convex.dev
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Database :: Front-Ends
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Project-URL: Documentation, https://docs.convex.dev
+Project-URL: Repository, https://github.com/get-convex/convex-py
+Description-Content-Type: text/markdown
+
+# Convex
+
+The official Python client for [Convex](https://convex.dev/).
+
+![PyPI](https://img.shields.io/pypi/v/convex?label=convex&logo=pypi)
+![GitHub](https://img.shields.io/github/license/get-convex/convex-py)
+
+Write and read data from a Convex backend with queries, mutations, and actions.
+Get up and running at [docs.convex.dev](https://docs.convex.dev/home).
+
+Installation:
+
+    pip install convex
+
+Basic usage:
+
+```python
+>>> from convex import ConvexClient
+>>> client = ConvexClient('https://example-lion-123.convex.cloud')
+>>> messages = client.query("listMessages")
+>>> from pprint import pprint
+>>> pprint(messages)
+[{'_creationTime': 1668107495676.2854,
+  '_id': Id(table_name='messages', id='c09S884lW4kTLdQMtu2ravf'),
+  'author': 'Tom',
+  'body': 'Have you tried Convex?'},
+ {'_creationTime': 1668107497732.2295,
+  '_id': Id(table_name='messages', id='G3m0cCQp65GQDfUjUDnTPEj'),
+  'author': 'Sarah',
+  'body': "Yeah, it's working pretty well for me."}]
+>>> client.mutation("sendMessage", dict(author="Me", body="Hello!"))
+```
+
+To find the url of your convex backend, open the deployment you want to work
+with in the appropriate project in the
+[Convex dashboard](https://dashboard.convex.dev) and click "Settings" where the
+Deployment URL should be visible. To find out which queries, mutations, and
+actions are available check the Functions pane in the Dashboard
+
+To see logs emitted from Convex functions, set the debug mode to True.
+
+```python
+>>> client.set_debug(True)
+```
+
+To provide authentication for function execution, call `set_auth()`.
+
+```python
+>>> client.set_auth("token-from-authetication-flow")
+```
+
+[Join us on Discord](https://www.convex.dev/community) to get your questions
+answered or share what you're doing with Convex. If you're just getting started,
+see https://docs.convex.dev to see how to quickly spin up a backend that does
+everything you need in the Convex cloud.
+
+# Convex types
+
+Convex backend functions are written in JavaScript, so arguments passed to
+Convex RPC functions in Python are serialized, sent over the network, and
+deserialized into JavaScript objects. To learn about Convex's supported types
+see https://docs.convex.dev/using/types.
+
+In order to call a function that expects a JavaScript type, use the
+corresponding Python type or any other type that coerces to it. Values returned
+from Convex will be of the corresponding Python type.
+
+| JavaScript Type                                                                                             | Python Type                                                                                                                    | Example                           | Other Python Types that Convert     |
+| ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ | --------------------------------- | ----------------------------------- |
+| [Id](https://docs.convex.dev/api/classes/values.GenericId)                                                  | Id (see below)                                                                                                                 | `Id(tableName, id)`               |                                     |
+| [null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#null_type)                   | [None](https://docs.python.org/3/library/stdtypes.html#the-null-object)                                                        | `None`                            |                                     |
+| [bigint](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#bigint_type)               | ConvexBigInt (see below)                                                                                                       | `ConvexInt64(2**60)`              |                                     |
+| [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#number_type)               | [float](https://docs.python.org/3/library/functions.html#float) or [int](https://docs.python.org/3/library/functions.html#int) | `3.1`, `10`                       |                                     |
+| [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#boolean_type)             | [bool](https://docs.python.org/3/library/functions.html#bool)                                                                  | `True`, `False`                   |                                     |
+| [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#string_type)               | [str](https://docs.python.org/3/library/stdtypes.html#str)                                                                     | `'abc'`                           |                                     |
+| [ArrayBuffer](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/ArrayBuffer) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes)                                                                 | `b'abc'`                          | ArrayBuffer                         |
+| [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)             | [list](https://docs.python.org/3/library/stdtypes.html#list)                                                                   | `[1, 3.2, "abc"]`                 | tuple, collections.abc.Sequence     |
+| [Set](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set)                 | ConvexSet (see below)                                                                                                          | `ConvexSet([1,2])`                | set, frozenset, collections.abc.Set |
+| [Map](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Map)                 | ConvexMap (see below)                                                                                                          | `ConvexMap([('a', 1), ('b', 2)])` |                                     |
+| [object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#objects)                   | [dict](https://docs.python.org/3/library/stdtypes.html#dict)                                                                   | `{a: "abc"}`                      | collections.abc.Mapping             |
+
+### Id
+
+Id objects represent references to Convex documents. They contain a `table_name`
+string specifying a Convex table (tables can be viewed in
+[the dashboard](https://dashboard.convex.dev)) and a globably unique `id`
+string. If you'd like to learn more about the `id` string's format, see
+[our docs](https://docs.convex.dev/api/classes/values.GenericId).
+
+### Ints and Floats
+
+While
+[Convex supports storing Int64s and Float64s](https://docs.convex.dev/using/types#convex-types),
+idiomatic JavaScript pervasively uses the (floating point) `Number` type. In
+Python `float`s are often understood to contain the `int`s: the `float` type
+annotation is
+[generally understood as `Union[int, float]`](https://peps.python.org/pep-0484/#the-numeric-tower).
+
+Therefore, the Python Convex client converts Python's `float`s and `int`s to a
+`Float64` in Convex.
+
+To specify a JavaScript BigInt, use the ConvexInt64 class. Functions which
+return JavaScript BigInts will return ConvexBigInt64 instances.
+
+### ConvexSet
+
+Similar to a Python set, but any Convex values can be items.
+
+ConvexSets are returned from Convex cloud function calls that return JavaScript
+Sets.
+
+Generally when calling Convex functions from Python, a Python builtin set can be
+used instead of a ConvexSet. But for representing unusual types like sets
+containing objects, you'll have to use a ConvexSet:
+
+```python
+>>> set([{'a': 1}])
+Traceback (most recent call last):
+    ...
+TypeError: unhashable type: 'dict'
+>>> ConvexSet([{'a': 1}])
+ConvexSet([{'a': 1.0}])
+```
+
+ConvexSet instances are immutable so must be fully populated when being
+constructed. In order to store mutable items, ConvexSets store snapshots of data
+when it was added.
+
+```python
+>>> mutable_dict = {'a': 1}
+>>> s = ConvexSet([mutable_dict, 'hello', 1])
+>>> mutable_dict in s
+True
+>>> mutable_dict['b'] = 2
+>>> mutable_dict in s
+False
+>>> s
+ConvexSet([{'a': 1.0}, 'hello', 1.0])
+```
+
+ConvexSets perform a copy of each inserted item, so they require more memory
+than Python's builtin sets.
+
+### ConvexMap
+
+Similar to a Python map, but any Convex values can be keys.
+
+ConvexMaps are returned from Convex cloud function calls that return JavaScript
+Maps.
+
+ConvexMaps are useful when calling Convex functions that expect a Map because
+dictionaries correspond to JavaScript objects, not Maps.
+
+ConvexMap instances are immutable so must be fully populated when being
+constructed. In order to store mutable items, ConvexMaps store snapshots of data
+when it was added.
+
+```python
+>>> mutable_dict = {'a': 1}
+>>> s = ConvexMap([(mutable_dict, 123), ('b', 456)])
+>>> mutable_dict in s
+True
+>>> mutable_dict['b'] = 2
+>>> mutable_dict in s
+False
+>>> s
+ConvexMap([({'a': 1.0}, 123.0), ('b', 456.0)])
+```
+
+ConvexMaps perform a copy of each inserted key/value pair, so they require more
+memory than Python's builtin dictionaries.
+
+# Versioning
+
+While we are pre-1.0.0, we'll update the minor version for large changes, and
+the patch version for small bugfixes. We may make backwards incompatible changes
+to the python client's API, but we will limit those to minor version bumps.
 
-packages = \
-['convex']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['requests>=2.28.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'convex',
-    'version': '0.2.0',
-    'description': 'Python client for the reactive backend-as-a-service Convex.',
-    'long_description': '# Convex\n\nThe official Python client for [Convex](https://convex.dev/).\n\nConvex is the TypeScript-native programmable database for the web. No need for\nbackend containers, caches, queues, and query languages. Convex replaces all of\nthem with a few simple APIs.\n\nThis Python client can write and read data from a Convex backend with queries,\nmutations, and actions. Get up and running at\n[docs.convex.dev](https://docs.convex.dev/introduction/).\n\nInstallation:\n\n    pip install convex\n\nBasic usage:\n\n```python\n>>> from convex import ConvexClient\n>>> client = ConvexClient(\'https://example-lion-123.convex.cloud\')\n>>> messages = client.query("listMessages")\n>>> from pprint import pprint\n>>> pprint(messages)\n[{\'_creationTime\': 1668107495676.2854,\n  \'_id\': Id(table_name=\'messages\', id=\'c09S884lW4kTLdQMtu2ravf\'),\n  \'author\': \'Tom\',\n  \'body\': \'Have you tried Convex?\'},\n {\'_creationTime\': 1668107497732.2295,\n  \'_id\': Id(table_name=\'messages\', id=\'G3m0cCQp65GQDfUjUDnTPEj\'),\n  \'author\': \'Sarah\',\n  \'body\': "Yeah, it\'s working pretty well for me."}]\n>>> client.mutation("sendMessage")\n```\n\nTo find the url of your convex backend, open the deployment you want to work\nwith in the appropriate project in the\n[Convex dashboard](https://dashboard.convex.dev) and click "Settings" where the\nDeployment URL should be visible. To find out which queries, mutations, and\nactions are available check the Functions pane in the Dashboard\n\nTo see logs emitted from Convex functions, set the debug mode to True.\n\n```python\n>>> client.set_debug(True)\n```\n\nTo provide authentication for function execution, call `set_auth()`.\n\n```python\n>>> client.set_auth("token-from-authetication-flow")\n```\n\n[Join us on Discord](https://www.convex.dev/community) to get your questions\nanswered or share what you\'re doing with Convex. If you\'re just getting started,\nsee https://docs.convex.dev to see how to quickly spin up a backend that does\neverything you need in the Convex cloud.\n\n# Convex types\n\nConvex backend functions are written in JavaScript, so arguments passed to\nConvex RPC functions in Python are serialized, sent over the network, and\ndeserialized into JavaScript objects. To learn about Convex\'s supported types\nsee https://docs.convex.dev/using/types.\n\nIn order to call a function that expects a JavaScript type, use the\ncorresponding Python type or any other type that coerces to it. Values returned\nfrom Convex will be of the corresponding Python type.\n\n| JavaScript Type                                                                                             | Python Type                                                                                                                    | Example                           | Other Python Types that Convert     |\n| ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ | --------------------------------- | ----------------------------------- |\n| [Id](https://docs.convex.dev/api/classes/values.GenericId)                                                  | Id (see below)                                                                                                                 | `Id(tableName, id)`               |                                     |\n| [null](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#null_type)                   | [None](https://docs.python.org/3/library/stdtypes.html#the-null-object)                                                        | `None`                            |                                     |\n| [bigint](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#bigint_type)               | ConvexBigInt (see below)                                                                                                       | `ConvexInt64(2**60)`              |                                     |\n| [number](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#number_type)               | [float](https://docs.python.org/3/library/functions.html#float) or [int](https://docs.python.org/3/library/functions.html#int) | `3.1`, `10`                       |                                     |\n| [boolean](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#boolean_type)             | [bool](https://docs.python.org/3/library/functions.html#bool)                                                                  | `True`, `False`                   |                                     |\n| [string](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#string_type)               | [str](https://docs.python.org/3/library/stdtypes.html#str)                                                                     | `\'abc\'`                           |                                     |\n| [ArrayBuffer](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/ArrayBuffer) | [bytes](https://docs.python.org/3/library/stdtypes.html#bytes)                                                                 | `b\'abc\'`                          | ArrayBuffer                         |\n| [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)             | [list](https://docs.python.org/3/library/stdtypes.html#list)                                                                   | `[1, 3.2, "abc"]`                 | tuple, collections.abc.Sequence     |\n| [Set](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Set)                 | ConvexSet (see below)                                                                                                          | `ConvexSet([1,2])`                | set, frozenset, collections.abc.Set |\n| [Map](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Map)                 | ConvexMap (see below)                                                                                                          | `ConvexMap([(\'a\', 1), (\'b\', 2)])` |                                     |\n| [object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures#objects)                   | [dict](https://docs.python.org/3/library/stdtypes.html#dict)                                                                   | `{a: "abc"}`                      | collections.abc.Mapping             |\n\n### Id\n\nId objects represent references to Convex documents. They contain a `table_name`\nstring specifying a Convex table (tables can be viewed in\n[the dashboard](https://dashboard.convex.dev)) and a globably unique `id`\nstring. If you\'d like to learn more about the `id` string\'s format, see\n[our docs](https://docs.convex.dev/api/classes/values.GenericId).\n\n### Ints and Floats\n\nWhile\n[Convex supports storing Int64s and Float64s](https://docs.convex.dev/using/types#convex-types),\nidiomatic JavaScript pervasively uses the (floating point) `Number` type. In\nPython `float`s are often understood to contain the `int`s: the `float` type\nannotation is\n[generally understood as `Union[int, float]`](https://peps.python.org/pep-0484/#the-numeric-tower).\n\nTherefore, the Python Convex client converts Python\'s `float`s and `int`s to a\n`Float64` in Convex.\n\nTo specify a JavaScript BigInt, use the ConvexInt64 class. Functions which\nreturn JavaScript BigInts will return ConvexBigInt64 instances.\n\n### ConvexSet\n\nSimilar to a Python set, but any Convex values can be items.\n\nConvexSets are returned from Convex cloud function calls that return JavaScript\nSets.\n\nGenerally when calling Convex functions from Python, a Python builtin set can be\nused instead of a ConvexSet. But for representing unusual types like sets\ncontaining objects, you\'ll have to use a ConvexSet:\n\n```python\n>>> set([{\'a\': 1}])\nTraceback (most recent call last):\n    ...\nTypeError: unhashable type: \'dict\'\n>>> ConvexSet([{\'a\': 1}])\nConvexSet([{\'a\': 1.0}])\n```\n\nConvexSet instances are immutable so must be fully populated when being\nconstructed. In order to store mutable items, ConvexSets store snapshots of data\nwhen it was added.\n\n```python\n>>> mutable_dict = {\'a\': 1}\n>>> s = ConvexSet([mutable_dict, \'hello\', 1])\n>>> mutable_dict in s\nTrue\n>>> mutable_dict[\'b\'] = 2\n>>> mutable_dict in s\nFalse\n>>> s\nConvexSet([{\'a\': 1.0}, \'hello\', 1.0])\n```\n\nConvexSets perform a copy of each inserted item, so they require more memory\nthan Python\'s builtin sets.\n\n### ConvexMap\n\nSimilar to a Python map, but any Convex values can be keys.\n\nConvexMaps are returned from Convex cloud function calls that return JavaScript\nMaps.\n\nConvexMaps are useful when calling Convex functions that expect a Map because\ndictionaries correspond to JavaScript objects, not Maps.\n\nConvexMap instances are immutable so must be fully populated when being\nconstructed. In order to store mutable items, ConvexMaps store snapshots of data\nwhen it was added.\n\n```python\n>>> mutable_dict = {\'a\': 1}\n>>> s = ConvexMap([(mutable_dict, 123), (\'b\', 456)])\n>>> mutable_dict in s\nTrue\n>>> mutable_dict[\'b\'] = 2\n>>> mutable_dict in s\nFalse\n>>> s\nConvexMap([({\'a\': 1.0}, 123.0), (\'b\', 456.0)])\n```\n\nConvexMaps perform a copy of each inserted key/value pair, so they require more\nmemory than Python\'s builtin dictionaries.\n\n# Versioning\n\nWhile we are pre-1.0.0, we\'ll update the minor version for large changes, and\nthe patch version for small bugfixes. We may make backwards incompatible changes\nto the python client\'s API, but we will limit those to minor version bumps.\n',
-    'author': 'Convex, Inc.',
-    'author_email': 'support@convex.dev',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://convex.dev',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```


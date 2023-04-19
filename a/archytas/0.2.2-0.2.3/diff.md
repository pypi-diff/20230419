# Comparing `tmp/archytas-0.2.2.tar.gz` & `tmp/archytas-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archytas-0.2.2.tar", max compression
+gzip compressed data, was "archytas-0.2.3.tar", max compression
```

## Comparing `archytas-0.2.2.tar` & `archytas-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    32472 2023-04-18 20:18:52.896203 archytas-0.2.2/LICENSE
--rw-r--r--   0        0        0     2577 2023-04-18 20:18:52.896203 archytas-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/__init__.py
--rw-r--r--   0        0        0     3214 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/agent.py
--rw-r--r--   0        0        0      513 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/auth.py
--rw-r--r--   0        0        0     6701 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/demo_tools.py
--rw-r--r--   0        0        0     3229 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/prompt.py
--rw-r--r--   0        0        0     5548 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/react.py
--rw-r--r--   0        0        0     1005 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/repl.py
--rw-r--r--   0        0        0    17317 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/tool_utils.py
--rw-r--r--   0        0        0     1521 2023-04-18 20:18:52.896203 archytas-0.2.2/archytas/tools.py
--rw-r--r--   0        0        0      758 2023-04-18 20:18:52.900203 archytas-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3369 1970-01-01 00:00:00.000000 archytas-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    32472 2023-04-19 16:53:36.933413 archytas-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2577 2023-04-19 16:53:36.933413 archytas-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/__init__.py
+-rw-r--r--   0        0        0     3214 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/agent.py
+-rw-r--r--   0        0        0      513 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/auth.py
+-rw-r--r--   0        0        0     8468 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/demo_tools.py
+-rw-r--r--   0        0        0     3583 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/prompt.py
+-rw-r--r--   0        0        0     5866 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/react.py
+-rw-r--r--   0        0        0     1055 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/repl.py
+-rw-r--r--   0        0        0    17591 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/tool_utils.py
+-rw-r--r--   0        0        0     1778 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/tools.py
+-rw-r--r--   0        0        0      758 2023-04-19 16:53:36.937413 archytas-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3369 1970-01-01 00:00:00.000000 archytas-0.2.3/PKG-INFO
```

### Comparing `archytas-0.2.2/LICENSE` & `archytas-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `archytas-0.2.2/README.md` & `archytas-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `archytas-0.2.2/archytas/agent.py` & `archytas-0.2.3/archytas/agent.py`

 * *Files identical despite different names*

### Comparing `archytas-0.2.2/archytas/auth.py` & `archytas-0.2.3/archytas/auth.py`

 * *Files identical despite different names*

### Comparing `archytas-0.2.2/archytas/prompt.py` & `archytas-0.2.3/archytas/prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,18 +58,30 @@
     Args:
         tools (list): A list of tools to use. Each tool should have the @tool decorator. applied.
     
     Returns:
         str: The prompt for the ReAct agent
     """
     # collect all the tool names (including class.method names)
-    tool_names = [name for tool in tools for name in get_tool_names(tool)]
+    tool_names = build_all_tool_names(tools)
     
     chunks = [prelude, tool_intro]
     for tool in tools:
         chunks.append(get_tool_prompt_description(tool))
     chunks.append(system_tools+'\n')
     chunks.append(formatting(tool_names)+'\n')
     chunks.append(notes)
     return '\n\n'.join(chunks)
 
         
+def build_all_tool_names(tools: list[Callable]) -> list[str]:
+    """
+    Build a list of tool names from a list of tools
+
+    Args:
+        tools (list): A list of tools to use. Each tool should have the @tool decorator. applied.
+
+    Returns:
+        list: A list of tool names
+    """
+    tool_names = [name for tool in tools for name in get_tool_names(tool)]
+    return tool_names
```

### Comparing `archytas-0.2.2/archytas/react.py` & `archytas-0.2.3/archytas/react.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from archytas.agent import Agent
-from archytas.prompt import build_prompt
+from archytas.prompt import build_prompt, build_all_tool_names
 from archytas.tools import ask_user
 from archytas.tool_utils import make_tool_dict
 import json
 from rich import print
 
 
 class FailedTaskError(Exception): ...
@@ -21,14 +21,18 @@
 
         # create a dictionary for looking up tools by name
         tools = tools or []
         if allow_ask_user: 
             tools.append(ask_user)
         self.tools = make_tool_dict(tools)
 
+        #check that the tools dict keys match the list of generated tool names
+        names, keys = sorted(build_all_tool_names(tools)), sorted([*self.tools.keys()])
+        assert names == keys, f'Internal Error: tools dict keys does not match list of generated tool names. {names} != {keys}'
+
         # create the prompt with the tools
         self.prompt = build_prompt(tools)
         self._agent = Agent(model=model, prompt=self.prompt)
 
         # react settings
         self.max_errors = max_errors or float('inf')
         self.max_react_steps = max_react_steps or float('inf')
```

### Comparing `archytas-0.2.2/archytas/tool_utils.py` & `archytas-0.2.3/archytas/tool_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,26 +107,22 @@
         #get the list of @tool methods in the class
         methods = inspect.getmembers(cls, predicate=inspect.isfunction)
         methods = [method for name, method in methods if is_tool(method)]
 
         # get the class docstring description
         docstring = inspect.getdoc(cls)
 
-        @functools.wraps(cls)
-        def wrapper(*args, **kwargs):
-            # create an instance of the class
-            c = cls(*args, **kwargs)
-
-            # attach the metadata to the instance
-            c._name = name if name else cls.__name__
-            c._is_class_tool_instance = True
-            c._docstring = docstring
-            c._tool_methods = methods
+        class wrapper:
+            def __init__(self, *args, **kwargs):
+                # create an instance of the class
+                self._instance = cls(*args, **kwargs)
+
+                # mark this as a class tool instance
+                self._is_class_tool_instance = True
 
-            return c
 
         # attach the metadata to the class
         wrapper._name = name if name else cls.__name__
         wrapper._is_class_tool = True
         wrapper._docstring = docstring
         wrapper._tool_methods = methods
         
@@ -136,14 +132,16 @@
 
 
 
 def make_func_tool_wrapper(func:Callable, name:str|None=None):
     def wrapper(args:dict|list|str|int|float|bool|None):
         """Output from LLM will be dumped into a json object. Depending on object type, call func accordingly."""
         
+        #TODO: make this look at _call_type rather than isinstance to determine what to do
+        #      single argument functions that take a dict vs mutli-argument functions will both have a dict, but they need to be called differently func(args) vs func(**args)
         if isinstance(args, dict):
             result = func(**args)
         elif isinstance(args, list):
             result = func(*args)
         elif isinstance(args, (str, int, float, bool)):
             result = func(args)
         elif args is None:
@@ -233,20 +231,18 @@
     
     #otherwise, just return the name of the tool
     return [get_tool_name(obj)]
 
 
 
 def get_tool_prompt_description(obj:Callable|type|Any):
-    if hasattr(obj, '_is_class_tool'):
+    if hasattr(obj, '_is_class_tool') or hasattr(obj, '_is_class_tool_instance'):
         return get_tool_class_prompt_description(obj)
     if hasattr(obj, '_is_function_tool') or hasattr(obj, '_is_method_tool'):
         return get_tool_func_prompt_description(obj)
-    if hasattr(obj, '_is_class_tool_instance'):
-        return get_tool_class_prompt_description(obj)
 
     raise TypeError(f"get_tool_prompt_description can only be used on @tools. Got {obj}")
 
 def get_tool_func_prompt_description(func:Callable):
     assert is_tool(func), f"Function {func.__name__} does not have the @tool decorator attached"
     assert inspect.isfunction(func), f"get_tool_func_prompt_description can only be used on functions. Got {func}"
 
@@ -269,15 +265,16 @@
     
     #################### INPUT ####################
     chunks.append('    _input_: ')
     
     if len(args_list) == 0:
         chunks.append("None")
     
-    elif len(args_list) == 1:
+
+    elif len(args_list) == 1 and args_list[0][1] is not dict:
         arg_name, arg_type, arg_desc, arg_default = args_list[0]
         chunks.append(f"({arg_type.__name__}")
         if arg_default:
             chunks.append(f", optional")
         chunks.append(f") {arg_desc}")
     
     else:
@@ -439,22 +436,24 @@
         
         if hasattr(tool, '_is_method_tool'):
             #TODO: not sure if methods should be allowed since they need usually need a class instance...
             raise NotImplementedError("Free-floating tool methods are not yet supported")
             pdb.set_trace()
         
 
-        # handle if instance of class or class itself
-        if hasattr(tool, '_is_class_tool'):
-            instance = tool()
-        else:
-            assert hasattr(tool, '_is_class_tool_instance'), f"Tool {tool} is not a function, method, or class tool"
+        # collect methods from @toolset. handle if instance of class or class itself
+        assert hasattr(tool, '_is_class_tool'), f"Tool {tool} is not a function, method, or class tool"
+        if hasattr(tool, '_is_class_tool_instance'):
             instance = tool
+        else:
+            instance = tool()
 
-        for _, method in inspect.getmembers(instance, predicate=inspect.ismethod):
+        # add each method to the tool dictionary under the name 'class_name.method_name'
+        methods = inspect.getmembers(instance._instance, predicate=inspect.ismethod)
+        for _, method in methods:
             if not hasattr(method, '_name'):
                 continue
             method_name = f'{name}.{method._name}'
             if method_name in tool_dict:
                 raise ValueError(f"Tool name '{method_name}' is already in use")
             tool_dict[method_name] = method
 
@@ -463,15 +462,15 @@
 
 
 
 
 def test():
     from archytas.tools import ask_user, datetime_tool, timestamp
     from archytas.demo_tools import fib_n, example_tool, calculator, Jackpot
-    
+
     for t in [ask_user, datetime_tool, timestamp, fib_n, example_tool, calculator, Jackpot]:
         print(get_tool_prompt_description(t))
         print()
 
 
 
 if __name__ == '__main__':
```

### Comparing `archytas-0.2.2/archytas/tools.py` & `archytas-0.2.3/archytas/tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     
     Args:
         query (str): The question to ask the user
 
     Returns:
         str: The user's response
     """
-    return input(query)
+    return input(f'{query} $ ')
 
 
 
 from datetime import datetime
 import pytz
 @tool(name='datetime')
 def datetime_tool(format:str='%Y-%m-%d %H:%M:%S %Z', timezone:str='UTC') -> str:
@@ -48,7 +48,16 @@
         float: The current unix timestamp in seconds 
 
     Examples:
         >>> timestamp()
         1681445698.726113
     """
     return datetime.now().timestamp()
+
+
+
+"""
+python repl tool
+- have a oneshot and multishot version
+- should be able to import the functions to be included, and create the tool instance with the list of functions/modules/etc.
+- maybe a list of recommended modules the llm can import
+"""
```

### Comparing `archytas-0.2.2/pyproject.toml` & `archytas-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archytas"
-version = "0.2.2"
+version = "0.2.3"
 description = "A library for pairing LLM agents with tools so they perform open ended tasks"
 authors = ["David Andrew Samson <david.andrew.engineer@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [project.urls]
 "Homepage" = "https://github.com/jataware/archytas"
```

### Comparing `archytas-0.2.2/PKG-INFO` & `archytas-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archytas
-Version: 0.2.2
+Version: 0.2.3
 Summary: A library for pairing LLM agents with tools so they perform open ended tasks
 License: GPL-3.0-or-later
 Author: David Andrew Samson
 Author-email: david.andrew.engineer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```


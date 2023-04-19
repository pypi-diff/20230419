# Comparing `tmp/pyterranetes-0.8.0.tar.gz` & `tmp/pyterranetes-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyterranetes-0.8.0.tar", last modified: Wed Sep 11 15:04:13 2019, max compression
+gzip compressed data, was "dist/pyterranetes-0.9.0.tar", last modified: Wed Sep 11 16:17:28 2019, max compression
```

## Comparing `pyterranetes-0.8.0.tar` & `pyterranetes-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-11 15:04:13.000000 pyterranetes-0.8.0/
--rw-r--r--   0 root         (0) root         (0)      687 2019-09-11 15:04:13.000000 pyterranetes-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      168 2019-09-11 15:03:59.000000 pyterranetes-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-11 15:04:13.000000 pyterranetes-0.8.0/bin/
--rwxrwxrwx   0 root         (0) root         (0)     1917 2019-09-11 15:03:59.000000 pyterranetes-0.8.0/bin/p10s
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-11 15:04:13.000000 pyterranetes-0.8.0/p10s/
--rw-rw-rw-   0 root         (0) root         (0)      740 2019-09-11 15:03:59.000000 pyterranetes-0.8.0/p10s/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2019-09-11 15:03:59.000000 pyterranetes-0.8.0/p10s/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2019-09-11 15:03:59.000000 pyterranetes-0.8.0/p10s/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3275 2019-09-11 15:03:59.000000 pyterranetes-0.8.0/p10s/generator.py
--rw-rw-rw-   0 root         (0) root         (0)     6205 2019-09-11 15:03:59.000000 pyterranetes-0.8.0/p10s/kubernetes.py
--rw-rw-rw-   0 root         (0) root         (0)     3369 2019-09-11 15:03:59.000000 pyterranetes-0.8.0/p10s/loads.py
--rw-rw-rw-   0 root         (0) root         (0)    14868 2019-09-11 15:03:59.000000 pyterranetes-0.8.0/p10s/terraform.py
--rw-rw-rw-   0 root         (0) root         (0)      911 2019-09-11 15:03:59.000000 pyterranetes-0.8.0/p10s/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4334 2019-09-11 15:03:59.000000 pyterranetes-0.8.0/p10s/values.py
--rw-rw-rw-   0 root         (0) root         (0)     2481 2019-09-11 15:03:59.000000 pyterranetes-0.8.0/p10s/watcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-11 15:04:13.000000 pyterranetes-0.8.0/pyterranetes.egg-info/
--rw-r--r--   0 root         (0) root         (0)      687 2019-09-11 15:04:13.000000 pyterranetes-0.8.0/pyterranetes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      380 2019-09-11 15:04:13.000000 pyterranetes-0.8.0/pyterranetes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-09-11 15:04:13.000000 pyterranetes-0.8.0/pyterranetes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2019-09-11 15:04:13.000000 pyterranetes-0.8.0/pyterranetes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2019-09-11 15:04:13.000000 pyterranetes-0.8.0/pyterranetes.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      217 2019-09-11 15:04:13.000000 pyterranetes-0.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2984 2019-09-11 15:03:59.000000 pyterranetes-0.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-11 16:17:28.000000 pyterranetes-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)      687 2019-09-11 16:17:28.000000 pyterranetes-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      168 2019-09-11 16:17:16.000000 pyterranetes-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-11 16:17:28.000000 pyterranetes-0.9.0/bin/
+-rwxrwxrwx   0 root         (0) root         (0)     1917 2019-09-11 16:17:16.000000 pyterranetes-0.9.0/bin/p10s
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-11 16:17:28.000000 pyterranetes-0.9.0/p10s/
+-rw-rw-rw-   0 root         (0) root         (0)      740 2019-09-11 16:17:16.000000 pyterranetes-0.9.0/p10s/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2019-09-11 16:17:16.000000 pyterranetes-0.9.0/p10s/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2019-09-11 16:17:16.000000 pyterranetes-0.9.0/p10s/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3275 2019-09-11 16:17:16.000000 pyterranetes-0.9.0/p10s/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     6205 2019-09-11 16:17:16.000000 pyterranetes-0.9.0/p10s/kubernetes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3369 2019-09-11 16:17:16.000000 pyterranetes-0.9.0/p10s/loads.py
+-rw-rw-rw-   0 root         (0) root         (0)    17267 2019-09-11 16:17:16.000000 pyterranetes-0.9.0/p10s/terraform.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2019-09-11 16:17:16.000000 pyterranetes-0.9.0/p10s/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4334 2019-09-11 16:17:16.000000 pyterranetes-0.9.0/p10s/values.py
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2019-09-11 16:17:16.000000 pyterranetes-0.9.0/p10s/watcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-09-11 16:17:28.000000 pyterranetes-0.9.0/pyterranetes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      687 2019-09-11 16:17:28.000000 pyterranetes-0.9.0/pyterranetes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      380 2019-09-11 16:17:28.000000 pyterranetes-0.9.0/pyterranetes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-09-11 16:17:28.000000 pyterranetes-0.9.0/pyterranetes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2019-09-11 16:17:28.000000 pyterranetes-0.9.0/pyterranetes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2019-09-11 16:17:28.000000 pyterranetes-0.9.0/pyterranetes.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      217 2019-09-11 16:17:28.000000 pyterranetes-0.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2019-09-11 16:17:16.000000 pyterranetes-0.9.0/setup.py
```

### Comparing `pyterranetes-0.8.0/PKG-INFO` & `pyterranetes-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyterranetes
-Version: 0.8.0
+Version: 0.9.0
 Summary: A toolkit for reducing duplication in terraform and k8s code.
 Home-page: https://sig11.gitlab.io/pyterranetes/
 Author: Marco Baringer
 Author-email: mb@bese.it
 License: MIT
 Description: A toolkit for reducing duplication in terraform and k8s code.
 Platform: UNKNOWN
```

### Comparing `pyterranetes-0.8.0/bin/p10s` & `pyterranetes-0.9.0/bin/p10s`

 * *Files identical despite different names*

### Comparing `pyterranetes-0.8.0/p10s/__init__.py` & `pyterranetes-0.9.0/p10s/__init__.py`

 * *Files identical despite different names*

### Comparing `pyterranetes-0.8.0/p10s/base.py` & `pyterranetes-0.9.0/p10s/base.py`

 * *Files identical despite different names*

### Comparing `pyterranetes-0.8.0/p10s/generator.py` & `pyterranetes-0.9.0/p10s/generator.py`

 * *Files identical despite different names*

### Comparing `pyterranetes-0.8.0/p10s/kubernetes.py` & `pyterranetes-0.9.0/p10s/kubernetes.py`

 * *Files identical despite different names*

### Comparing `pyterranetes-0.8.0/p10s/loads.py` & `pyterranetes-0.9.0/p10s/loads.py`

 * *Files identical despite different names*

### Comparing `pyterranetes-0.8.0/p10s/terraform.py` & `pyterranetes-0.9.0/p10s/terraform.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,46 @@
-"""
-Generating terraform with pyterranetes is, as with kubernetes, just a
+"""Generating terraform with pyterranetes is, as with kubernetes, just a
 question of writing a p10s script which creates a
 ``terraform.Context`` object and adds terraform blocks to it:
 
 .. code-block:: python
 
     from p10s import tf
 
     c = tf.Context()
 
+    # Fully explicit style
     c += tf.Variable("foo", dict(
         default=0
     ))
 
-    c += tf.variables(key="${data.terraform_remote_state.key}"})
-
     c += tf.Resource("type", "name", dict(
         var = 'value'
     ))
 
+    # Helper function
+    c += tf.variables(key="${data.terraform_remote_state.key}"})
+    c += tf.outputs(key="${module.m.key}"})
+
+    # HCL syntax if a large amount of code needs to be converted to
+    # pyterranetes quickly
     c += tf.from_hcl(""\"
         module "m" {
           source = "../m/"
         }
     ""\")
 
-    c += tf.outputs(key="${module.m.key}"})
-
-    ...
+    # property/attribute syntax for a more pythonic feeling
+    c.resource.type.name = {
+        'key': 'value',
+    }
 
+    c.module.name = {
+        'source': './modules/my-module/',
+    }
 
 For each terraform configuration block there is a corresponding python
 class. Depending on the block type and how it's used some of the
 classes provid convenience methods and constructors. All of the
 classes have a ``.body`` property representing the data inside the
 block.
 
@@ -78,14 +86,36 @@
     }
 
 When parsing hcl pyterranetes will convert both of these to a single
 entry with key ``key`` and value a dict with the values of the
 corresponsding block. As pyterranetes only actually generates
 ``.tf.json`` and not ``.tf`` (hcl) files, there is also no ambiguity
 in the output.
+
+Alternatively there's another way to add blocks to a context using the
+properties ``resource``, ``module`` and ``variable`` (there is
+currently no equivalent auto syntax for provider, local or output
+blocks).
+
+.. code-block:: python
+
+    from p10s import tf
+
+    c = tf.Context()
+
+    c.resource.random_id.project_name = {
+        'byte_length': 8
+    }
+
+    c.module.mod = {
+        'source': './modules/module'
+    }
+
+    c.variable.name = 'default-value'
+
 """
 
 import collections.abc
 import json
 from copy import deepcopy
 from pprint import pformat
 
@@ -164,14 +194,26 @@
     def _render_data(self):
         return self.data
 
     def render(self):
         with self._output_stream() as tf_json:
             tf_json.write(json.dumps(self._render_data(), indent=4, sort_keys=True))
 
+    @property
+    def resource(self):
+        return AutoResource(self)
+
+    @property
+    def module(self):
+        return AutoModule(self)
+
+    @property
+    def variable(self):
+        return AutoVariable(self)
+
 
 class DuplicateBlockError(ValueError):
     def __init__(self, existing, new_block):
         self.existing = existing
         self.new_block = new_block
 
 
@@ -219,30 +261,31 @@
             return self.__dict__ == other.__dict__
         else:
             return super().__eq__(other)
 
 
 class NoArgsBlock(TerraformBlock):
     def __init__(self, body):
-        super().__init__({self.KIND: body or {}})
+        super().__init__({self.KIND: body})
 
     def _body(self):
         return self.data[self.KIND]
 
     def _key(self):
         return [self.KIND]
 
     def __repr__(self):
         return "#<%s %s>" % (self.KIND, len(self.body))
 
 
 class NameBlock(TerraformBlock):
     def __init__(self, name, body=None):
         self._name = name
-        super().__init__({self.KIND: {name: body or {}}})
+        body = body if body is not None else {}
+        super().__init__({self.KIND: {name: body}})
 
     def _body(self):
         return self.data[self.KIND][self.name]
 
     @property
     def name(self):
         return self._name
@@ -261,15 +304,16 @@
         return "#<%s %s %s>" % (self.KIND, self.name, len(self.body))
 
 
 class TypeNameBlock(TerraformBlock):
     def __init__(self, type, name, body=None):
         self._type = type
         self._name = name
-        super().__init__({self.KIND: {type: {name: body or {}}}})
+        body = body if body is not None else {}
+        super().__init__({self.KIND: {type: {name: body}}})
 
     def _body(self):
         return self.data[self.KIND][self._type][self._name]
 
     @property
     def type(self):
         return self._type
@@ -282,18 +326,17 @@
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, name):
-        self.data[self.KIND][self._type][name] = self.data[self.KIND][self._type][
-            self.name
-        ]
-        del self.data[self.KIND][self._type][self._name]
+        type_block = self.data[self.KIND][self._type]
+        type_block[name] = type_block[self._name]
+        del type_block[self._name]
         self._name = name
 
     def _key(self):
         return [self.KIND, self.type, self.name]
 
     def __repr__(self):
         return "#<%s %s %s %s>" % (self.KIND, self.type, self.name, len(self.body))
@@ -553,7 +596,56 @@
     if len(blocks) == 1:
         return blocks[0]
     else:
         raise Exception(
             "Expected exactly one block when using `from_hcl` but got %s blocks from %s"
             % (len(blocks), hcl_string)
         )
+
+
+class AutoResource:
+    def __init__(self, context):
+        self._context_ = context
+        self._type_ = None
+
+    def __getattr__(self, name):
+        if name in ["_type_", "_context_"]:
+            super().__getattribute__(name)
+        else:
+            self._type_ = name
+            return self
+
+    def __setattr__(self, name, body):
+        if name in ["_type_", "_context_"]:
+            super().__setattr__(name, body)
+        else:
+            if self._type_ is None:
+                raise Exception("Can't set name before _type_ is set.")
+            self._context_ += Resource(self._type_, name, body)
+
+
+class AutoModule:
+    def __init__(self, context):
+        self._context_ = context
+
+    def __setattr__(self, name, body):
+        if name in ["_context_"]:
+            super().__setattr__(name, body)
+        else:
+            self._context_ += Module(name, body)
+
+    def __setitem__(self, name, body):
+        self._context_ += Module(name, body)
+
+
+class AutoVariable:
+    def __init__(self, context):
+        self._context_ = context
+
+    def __setattr__(self, key, value):
+        if key in ["_context_"]:
+            super().__setattr__(key, value)
+        else:
+            self._context_ += Variable(key, {"default": value})
+
+    def __setitem__(self, name, value):
+        self._context_ += Variable(name, {"default": value})
```

### Comparing `pyterranetes-0.8.0/p10s/utils.py` & `pyterranetes-0.9.0/p10s/utils.py`

 * *Files identical despite different names*

### Comparing `pyterranetes-0.8.0/p10s/values.py` & `pyterranetes-0.9.0/p10s/values.py`

 * *Files identical despite different names*

### Comparing `pyterranetes-0.8.0/p10s/watcher.py` & `pyterranetes-0.9.0/p10s/watcher.py`

 * *Files identical despite different names*

### Comparing `pyterranetes-0.8.0/pyterranetes.egg-info/PKG-INFO` & `pyterranetes-0.9.0/pyterranetes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyterranetes
-Version: 0.8.0
+Version: 0.9.0
 Summary: A toolkit for reducing duplication in terraform and k8s code.
 Home-page: https://sig11.gitlab.io/pyterranetes/
 Author: Marco Baringer
 Author-email: mb@bese.it
 License: MIT
 Description: A toolkit for reducing duplication in terraform and k8s code.
 Platform: UNKNOWN
```

### Comparing `pyterranetes-0.8.0/setup.py` & `pyterranetes-0.9.0/setup.py`

 * *Files identical despite different names*


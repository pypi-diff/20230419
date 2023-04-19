# Comparing `tmp/visual_blocks-0.0.1.tar.gz` & `tmp/visual_blocks-0.0.2.tar.gz`

## Comparing `visual_blocks-0.0.1.tar` & `visual_blocks-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 visual_blocks-0.0.1/.editorconfig
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 visual_blocks-0.0.1/src/visual_blocks/__init__.py
--rw-r--r--   0        0        0    10961 2020-02-02 00:00:00.000000 visual_blocks-0.0.1/src/visual_blocks/server.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 visual_blocks-0.0.1/.gitignore
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 visual_blocks-0.0.1/README.pypi.md
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 visual_blocks-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 visual_blocks-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 visual_blocks-0.0.2/.editorconfig
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 visual_blocks-0.0.2/src/visual_blocks/__init__.py
+-rw-r--r--   0        0        0    12437 2020-02-02 00:00:00.000000 visual_blocks-0.0.2/src/visual_blocks/server.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 visual_blocks-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 visual_blocks-0.0.2/README.pypi.md
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 visual_blocks-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 visual_blocks-0.0.2/PKG-INFO
```

### Comparing `visual_blocks-0.0.1/src/visual_blocks/server.py` & `visual_blocks-0.0.2/src/visual_blocks/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import shutil
 import sys
 import threading
 import traceback
 import urllib.parse
 import zipfile
 
-_VISUAL_BLOCKS_BUNDLE_VERSION = '1681851289'
+_VISUAL_BLOCKS_BUNDLE_VERSION = '1681885544'
 
 # Disable logging from werkzeug.
 #
 # Without this, flask will show a warning about using dev server (which is OK
 # in our usecase).
 logging.getLogger('werkzeug').disabled = True
 
@@ -73,15 +73,15 @@
 def _find_fn(name:str, functions):
   """Find a function in a list of functions by its string name."""
   names = [fn.__name__ for fn in functions]
   i = names.index(name)
   return functions[i]
 
 
-def Server(generic=None, text_to_text=None, height=900, tmp_dir='/tmp'):
+def Server(generic=None, text_to_text=None, text_to_tensors=None, height=900, tmp_dir='/tmp', read_saved_pipeline=True):
   """Creates a server that serves visual blocks web app in an iFrame.
 
   Other than serving the web app, it will also listen to requests sent from the
   web app at various API end points. Once a request is received, it will use the
   data in the request body to call the corresponding functions passed in.
 
   Args:
@@ -96,23 +96,35 @@
     text_to_text:
       A function or iterable of functions, defined in the same Colab notebook,
       that Visual Blocks can call to implement a text-to-text model runner
       block.
 
       A text_to_text function must take a string and return a string.
 
+    text_to_tensors:
+      A function or iterable of functions, defined in the same Colab notebook,
+      that Visual Blocks can call to implement a text-to-tensors model runner
+      block.
+
+      A text_to_tensors function must take a string and return the output
+      tensors, as an iterable of numpy.ndarrays.
+
     height:
       The height of the embedded iFrame.
 
     tmp_dir:
       The tmp dir where the server stores the web app's static resources.
+
+    read_saved_pipeline:
+      Whether to read the saved pipeline in the notebook or not.
   """
 
   generic = _ensure_iterable(generic)
   text_to_text = _ensure_iterable(text_to_text)
+  text_to_tensors = _ensure_iterable(text_to_tensors)
 
   app = Flask(__name__)
 
   # Disable startup messages.
   cli = sys.modules['flask.cli']
   cli.show_server_banner = lambda *x: None
 
@@ -147,14 +159,16 @@
   @app.route('/api/list_inference_functions')
   def list_inference_functions():
     result = {}
     if generic:
       result['generic'] = [fn.__name__ for fn in generic]
     if text_to_text:
       result['text_to_text'] = [fn.__name__ for fn in text_to_text]
+    if text_to_tensors:
+      result['text_to_tensors'] = [fn.__name__ for fn in text_to_tensors]
     return _make_json_response(result)
 
   # Note: using "/api/..." for POST requests is not allowed.
   @app.route('/apipost/inference', methods=['POST'])
   def inference_generic():
     """Handler for the generic api endpoint."""
     result = {}
@@ -188,14 +202,34 @@
       result['text'] = inference_fn(text)
     except Exception as e:
       msg = ''.join(traceback.format_exception(type(e), e, e.__traceback__))
       result = {'error': msg}
     finally:
       return _make_json_response(result)
 
+  # Note: using "/api/..." for POST requests is not allowed.
+  @app.route('/apipost/inference_text_to_tensors', methods=['POST'])
+  def inference_text_to_tensors():
+    """Handler for the text_to_tensors api endpoint."""
+    result = {}
+    try:
+      try:
+        inference_fn = _find_fn(request.json['function'], text_to_tensors)
+      except KeyError:
+        # TODO: remove this fallback try-block after .js implments function key
+        inference_fn = text_to_tensors[0]
+      text = request.json['text']
+      output_tensors = inference_fn(text)
+      result['tensors'] = [_ndarray_to_json(x) for x in output_tensors]
+    except Exception as e:
+      msg = ''.join(traceback.format_exception(type(e), e, e.__traceback__))
+      result = {'error': msg}
+    finally:
+      return _make_json_response(result)
+
   @app.route('/<path:path>')
   def get_static(path):
     """Handler for serving static resources."""
     return send_from_directory(site_root_path, path)
 
   def embed(port, height):
     """Embeds iFrame."""
@@ -244,27 +278,28 @@
         shell = shell.replace(k, v)
 
     js(shell)
 
   def read_pipeline_json_from_notebook():
     # Read the current notebook and find the pipeline json.
     cur_pipeline_json = ''
-    notebook_json_string = _message.blocking_request('get_ipynb', request='', timeout_sec=60)
-    for cell in notebook_json_string['ipynb']['cells']:
-      if 'outputs' not in cell:
-        continue
-      for cur_output in cell['outputs']:
-        if 'data' not in cur_output:
-          continue
-        if 'text/html' not in cur_output['data']:
+    if read_saved_pipeline:
+      notebook_json_string = _message.blocking_request('get_ipynb', request='', timeout_sec=300)
+      for cell in notebook_json_string['ipynb']['cells']:
+        if 'outputs' not in cell:
           continue
-        if cur_output['data']['text/html'] is not None:
-          cur_text = cur_output['data']['text/html']
-          if cur_text[0].startswith('{"project":'):
-            cur_pipeline_json = cur_text[0]
+        for cur_output in cell['outputs']:
+          if 'data' not in cur_output:
+            continue
+          if 'text/html' not in cur_output['data']:
+            continue
+          if cur_output['data']['text/html'] is not None:
+            cur_text = cur_output['data']['text/html']
+            if cur_text[0].startswith('{"project":'):
+              cur_pipeline_json = cur_text[0]
     return cur_pipeline_json
 
   def save_project(data):
     """Puts the given project json data into the given div.
 
     The content of the div will be persisted in notebook.
     """
```

### Comparing `visual_blocks-0.0.1/README.pypi.md` & `visual_blocks-0.0.2/README.pypi.md`

 * *Files identical despite different names*

### Comparing `visual_blocks-0.0.1/pyproject.toml` & `visual_blocks-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "visual_blocks"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Google LLC", email="opensource@google.com" },
 ]
 description = "Visual Blocks for Google Colaboratory"
 readme = "README.pypi.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `visual_blocks-0.0.1/PKG-INFO` & `visual_blocks-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visual_blocks
-Version: 0.0.1
+Version: 0.0.2
 Summary: Visual Blocks for Google Colaboratory
 Project-URL: Homepage, https://github.com/google/visual-blocks
 Project-URL: Bug Tracker, https://github.com/google/visual-blocks/issues
 Author-email: Google LLC <opensource@google.com>
 Classifier: Environment :: Other Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


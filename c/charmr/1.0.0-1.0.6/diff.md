# Comparing `tmp/charmr-1.0.0.tar.gz` & `tmp/charmr-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charmr-1.0.0.tar", last modified: Sat Apr 15 03:15:02 2023, max compression
+gzip compressed data, was "charmr-1.0.6.tar", last modified: Wed Apr 19 03:10:30 2023, max compression
```

## Comparing `charmr-1.0.0.tar` & `charmr-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-15 03:15:02.088199 charmr-1.0.0/
--rw-r--r--   0 ronharlev   (501) staff       (20)     2831 2023-04-15 03:15:02.087659 charmr-1.0.0/PKG-INFO
--rw-r--r--   0 ronharlev   (501) staff       (20)     2575 2023-04-15 03:09:55.000000 charmr-1.0.0/README.md
-drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-15 03:15:02.084411 charmr-1.0.0/charmr/
--rw-r--r--   0 ronharlev   (501) staff       (20)        0 2023-04-14 03:06:02.000000 charmr-1.0.0/charmr/__init__.py
--rw-r--r--   0 ronharlev   (501) staff       (20)     1145 2023-04-15 03:01:03.000000 charmr-1.0.0/charmr/ai.py
--rw-r--r--   0 ronharlev   (501) staff       (20)     1096 2023-03-14 23:17:20.000000 charmr-1.0.0/charmr/alias_manager.py
--rw-r--r--   0 ronharlev   (501) staff       (20)      548 2023-03-14 22:59:53.000000 charmr-1.0.0/charmr/load_code.py
--rw-r--r--   0 ronharlev   (501) staff       (20)     1838 2023-04-14 03:14:39.000000 charmr-1.0.0/charmr/main.py
-drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-15 03:15:02.087090 charmr-1.0.0/charmr.egg-info/
--rw-r--r--   0 ronharlev   (501) staff       (20)     2831 2023-04-15 03:15:02.000000 charmr-1.0.0/charmr.egg-info/PKG-INFO
--rw-r--r--   0 ronharlev   (501) staff       (20)      291 2023-04-15 03:15:02.000000 charmr-1.0.0/charmr.egg-info/SOURCES.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)        1 2023-04-15 03:15:02.000000 charmr-1.0.0/charmr.egg-info/dependency_links.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)       44 2023-04-15 03:15:02.000000 charmr-1.0.0/charmr.egg-info/entry_points.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)       21 2023-04-15 03:15:02.000000 charmr-1.0.0/charmr.egg-info/requires.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)        7 2023-04-15 03:15:02.000000 charmr-1.0.0/charmr.egg-info/top_level.txt
--rw-r--r--   0 ronharlev   (501) staff       (20)       38 2023-04-15 03:15:02.088324 charmr-1.0.0/setup.cfg
--rw-r--r--   0 ronharlev   (501) staff       (20)      655 2023-04-15 03:14:43.000000 charmr-1.0.0/setup.py
+drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-19 03:10:30.479851 charmr-1.0.6/
+-rw-r--r--   0 ronharlev   (501) staff       (20)     3952 2023-04-19 03:10:30.479510 charmr-1.0.6/PKG-INFO
+-rw-r--r--   0 ronharlev   (501) staff       (20)     3694 2023-04-19 02:57:00.000000 charmr-1.0.6/README.md
+drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-19 03:10:30.476264 charmr-1.0.6/charmr/
+-rw-r--r--   0 ronharlev   (501) staff       (20)        0 2023-04-14 03:06:02.000000 charmr-1.0.6/charmr/__init__.py
+-rw-r--r--   0 ronharlev   (501) staff       (20)     1455 2023-04-19 02:21:55.000000 charmr-1.0.6/charmr/ai.py
+-rw-r--r--   0 ronharlev   (501) staff       (20)     1096 2023-03-14 23:17:20.000000 charmr-1.0.6/charmr/alias_manager.py
+-rw-r--r--   0 ronharlev   (501) staff       (20)      572 2023-04-19 02:31:54.000000 charmr-1.0.6/charmr/load_code.py
+-rw-r--r--   0 ronharlev   (501) staff       (20)     2786 2023-04-19 03:07:10.000000 charmr-1.0.6/charmr/main.py
+drwxr-xr-x   0 ronharlev   (501) staff       (20)        0 2023-04-19 03:10:30.479053 charmr-1.0.6/charmr.egg-info/
+-rw-r--r--   0 ronharlev   (501) staff       (20)     3952 2023-04-19 03:10:30.000000 charmr-1.0.6/charmr.egg-info/PKG-INFO
+-rw-r--r--   0 ronharlev   (501) staff       (20)      291 2023-04-19 03:10:30.000000 charmr-1.0.6/charmr.egg-info/SOURCES.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)        1 2023-04-19 03:10:30.000000 charmr-1.0.6/charmr.egg-info/dependency_links.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)       44 2023-04-19 03:10:30.000000 charmr-1.0.6/charmr.egg-info/entry_points.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)       21 2023-04-19 03:10:30.000000 charmr-1.0.6/charmr.egg-info/requires.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)        7 2023-04-19 03:10:30.000000 charmr-1.0.6/charmr.egg-info/top_level.txt
+-rw-r--r--   0 ronharlev   (501) staff       (20)       38 2023-04-19 03:10:30.479943 charmr-1.0.6/setup.cfg
+-rw-r--r--   0 ronharlev   (501) staff       (20)      658 2023-04-19 03:10:25.000000 charmr-1.0.6/setup.py
```

### Comparing `charmr-1.0.0/charmr/ai.py` & `charmr-1.0.6/charmr/ai.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 import openai
 import os
 
 SYSTEM = """you are a file converter code generator. 
 You will get a description of the source and target files format, and any conversion, manipulation, 
 filtering or transformation to apply on the source to generate the target. 
-You will output a python function that accepts the text of the source file as a string and returns the target file content as string.
+You will output a python function.
+The source input is a stream.
+The target output is a stream as well.
 The function name will be "file_convert". 
+function signature is "file_convert(input_stream, output_stream)"
 Generate only the code, with no comments. 
 Don't generate any wrapper to the code. 
 The output should be compilable as python code, version 3.8.
 prefer string manipulation over using external packages where possible. 
 Do not output any explanation."""
 
 
-def get_code(prompt: str):
+prompt_with_rows = """
+{prompt}. 
+here are the first rows of the input file, use them to understand the file structure: 
+{header_rows}
+"""
+
+
+def get_code(prompt: str, model="gpt-3.5-turbo", header_rows=None):
     openai.api_key = os.getenv("OPENAI_API_KEY")
 
+    if header_rows:
+        prompt = prompt_with_rows.format(prompt=prompt, header_rows=header_rows)
+
     response = openai.ChatCompletion.create(
-        model="gpt-3.5-turbo",
+        model=model,
         messages=[
             {"role": "system", "content": f"{SYSTEM}"},
             {"role": "user", "content": f"{prompt}"},
         ],
         temperature=0.0,
         max_tokens=2048
         )
```

### Comparing `charmr-1.0.0/charmr/alias_manager.py` & `charmr-1.0.6/charmr/alias_manager.py`

 * *Files identical despite different names*

### Comparing `charmr-1.0.0/charmr/load_code.py` & `charmr-1.0.6/charmr/load_code.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-def run_function(code_string, parameter):
+def run_function(code_string, in_stream, out_stream):
     # Compile the code string
     compiled_code = compile(code_string, '<string>', 'exec')
 
     # Create a dictionary to hold the function namespace
     function_namespace = {}
 
     # Execute the compiled code in the function namespace
     exec(compiled_code, function_namespace)
 
     # Get the function from the namespace
     function = function_namespace.get('file_convert')
 
     # Call the function with the given parameter
-    result = function(parameter)
+    result = function(in_stream, out_stream)
 
     # Return the result
     return result
```

### Comparing `charmr-1.0.0/charmr/main.py` & `charmr-1.0.6/charmr/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,93 @@
+import sys
 from dotenv import load_dotenv
 from charmr import ai
 import argparse
 from charmr.load_code import run_function
 from charmr import alias_manager
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description='Charmr - Magical File Converter')
-    parser.add_argument('--input_file', '-i', type=str, help='Input file', required=True)
-    parser.add_argument('--output_file', '-o', type=str, help='Output file', required=True)
+    parser.add_argument('--input_file', '-i', type=str, help='Input file', required=False)
+    parser.add_argument('--output_file', '-o', type=str, help='Output file', required=False)
     parser.add_argument('--conversion', '-c', type=str, help='Conversion description', required=False)
     parser.add_argument('--alias', '-a', type=str, help='Conversion alias, for reuse', required=False)
     parser.add_argument('--view_code_only', '-v', help='View code without running', action='store_true')
-    #TODO add "inspect only" option`
+    parser.add_argument('--gpt_4', '-4', help='Use GPT-4', action='store_true')
+    parser.add_argument('--include_input_rows', '-r', type=int, help='Include N input rows in prompt', required=False)
     args = parser.parse_args()
     return args
 
 
 def read_input_file(file_path):
     with open(file_path, 'r') as f:
         file_content = f.read()
     return file_content
 
 
-def write_output_file(file_path, file_content):
-    with open(file_path, 'w') as f:
-        f.write(file_content)
+def read_first_n_lines(file_path, n):
+    with open(file_path, 'r') as f:
+        lines = []
+        for i in range(n):
+            line = f.readline()
+            if line:
+                lines.append(line)
+            else:
+                break
+    return lines
+
+
+def send_stream_to_stdout(stream):
+    for line in stream:
+        sys.stdout.write(line)
 
 
 def main():
     load_dotenv()
     args = parse_arguments()
 
-    input_file_content = read_input_file(args.input_file)
+    if args.include_input_rows:
+        first_lines = read_first_n_lines(args.input_file, args.include_input_rows)
+    else:
+        first_lines = None
+
+    if args.gpt_4:
+        model_name = "gpt-4"
+    else:
+        model_name = "gpt-3.5-turbo"
 
     if args.conversion:
-        conversion_code = ai.get_code(args.conversion)
+        conversion_code = ai.get_code(args.conversion, model=model_name, header_rows=first_lines)
+
         if args.alias:
             alias_manager.save_code(conversion_code, args.alias)
     else:
         if not args.alias:
             raise Exception("Alias must be provided when no conversion defined")
         else:
             conversion_code = alias_manager.load_code(args.alias)
 
     if not args.view_code_only:
-        output_file_content = run_function(conversion_code, input_file_content)
-        write_output_file(args.output_file, output_file_content)
+        if args.input_file:
+            in_stream = open(args.input_file, "r")
+        else:
+            in_stream = sys.stdin
+
+        if args.output_file:
+            out_stream = open(args.output_file, "w")
+        else:
+            out_stream = sys.stdout
+
+        run_function(conversion_code, in_stream, out_stream)
+        if args.input_file:
+            in_stream.close()
+        if args.output_file:
+            out_stream.close()
+
     else:
         print(conversion_code)
 
     # print(result)
 
 
 if __name__ == "__main__":
```

### Comparing `charmr-1.0.0/setup.py` & `charmr-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='charmr',
-    version='1.0.0',
-    description='A Magical File Converter',
+    version='1.0.6',
+    description='A Magical AI File Converter',
     url='https://github.com/harlev/charmr',
     author='Ron Harlev',
     author_email='harlev@gmail.com',
     packages=find_packages(),
     install_requires=[
         'openai',
         'python-dotenv'
```


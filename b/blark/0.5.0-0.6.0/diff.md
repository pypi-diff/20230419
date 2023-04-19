# Comparing `tmp/blark-0.5.0.tar.gz` & `tmp/blark-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blark-0.5.0.tar", last modified: Sat May 28 00:12:54 2022, max compression
+gzip compressed data, was "blark-0.6.0.tar", last modified: Wed Apr 19 20:47:59 2023, max compression
```

## Comparing `blark-0.5.0.tar` & `blark-0.6.0.tar`

### file list

```diff
@@ -1,49 +1,54 @@
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-05-28 00:12:54.430553 blark-0.5.0/
--rw-r--r--   0 klauer   (1318172782) 1704612529    17987 2022-05-28 00:12:43.000000 blark-0.5.0/LICENSE
--rw-r--r--   0 klauer   (1318172782) 1704612529      196 2022-05-28 00:12:43.000000 blark-0.5.0/MANIFEST.in
--rw-r--r--   0 klauer   (1318172782) 1704612529     4034 2022-05-28 00:12:54.430692 blark-0.5.0/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529     3769 2022-05-28 00:12:43.000000 blark-0.5.0/README.md
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-05-28 00:12:54.431814 blark-0.5.0/blark/
--rw-r--r--   0 klauer   (1318172782) 1704612529      426 2022-05-28 00:12:43.000000 blark-0.5.0/blark/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529       31 2022-05-28 00:12:43.000000 blark-0.5.0/blark/__main__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529      497 2022-05-28 00:12:54.431900 blark-0.5.0/blark/_version.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     5500 2022-05-28 00:12:43.000000 blark-0.5.0/blark/apischema_compat.py
--rw-r--r--   0 klauer   (1318172782) 1704612529       74 2022-05-28 00:12:43.000000 blark-0.5.0/blark/config.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    11719 2022-05-28 00:12:43.000000 blark-0.5.0/blark/dependency_store.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3019 2022-05-28 00:12:43.000000 blark-0.5.0/blark/format.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    24694 2022-05-28 00:12:43.000000 blark-0.5.0/blark/iec.lark
--rw-r--r--   0 klauer   (1318172782) 1704612529     2244 2022-05-28 00:12:43.000000 blark-0.5.0/blark/main.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    10408 2022-05-28 00:12:43.000000 blark-0.5.0/blark/parse.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    20684 2022-05-28 00:12:43.000000 blark-0.5.0/blark/sphinxdomain.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    29725 2022-05-28 00:12:43.000000 blark-0.5.0/blark/summary.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-05-28 00:12:54.427241 blark-0.5.0/blark/tests/
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-05-28 00:12:54.427792 blark-0.5.0/blark/tests/POUs/
--rw-r--r--   0 klauer   (1318172782) 1704612529      925 2022-05-28 00:12:43.000000 blark-0.5.0/blark/tests/POUs/F_SetStateParams.TcPOU
--rw-r--r--   0 klauer   (1318172782) 1704612529      578 2022-05-28 00:12:43.000000 blark-0.5.0/blark/tests/POUs/global_version.TcPOU
--rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-05-28 00:12:43.000000 blark-0.5.0/blark/tests/__init__.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2606 2022-05-28 00:12:43.000000 blark-0.5.0/blark/tests/conftest.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-05-28 00:12:54.430250 blark-0.5.0/blark/tests/source/
--rw-r--r--   0 klauer   (1318172782) 1704612529      653 2022-05-28 00:12:43.000000 blark-0.5.0/blark/tests/source/and_then_or_else.st
--rw-r--r--   0 klauer   (1318172782) 1704612529      183 2022-05-28 00:12:43.000000 blark-0.5.0/blark/tests/source/array_of_objects.st
--rw-r--r--   0 klauer   (1318172782) 1704612529      639 2022-05-28 00:12:43.000000 blark-0.5.0/blark/tests/source/commas_in_case.st
--rw-r--r--   0 klauer   (1318172782) 1704612529      134 2022-05-28 00:12:43.000000 blark-0.5.0/blark/tests/source/fb_w_public_access.st
--rw-r--r--   0 klauer   (1318172782) 1704612529      174 2022-05-28 00:12:43.000000 blark-0.5.0/blark/tests/source/pointer_to_pointer_to.st
--rw-r--r--   0 klauer   (1318172782) 1704612529      352 2022-05-28 00:12:43.000000 blark-0.5.0/blark/tests/source/stray_comment.st
--rw-r--r--   0 klauer   (1318172782) 1704612529      260 2022-05-28 00:12:43.000000 blark-0.5.0/blark/tests/source/type_and_fb.st
--rw-r--r--   0 klauer   (1318172782) 1704612529     2740 2022-05-28 00:12:43.000000 blark-0.5.0/blark/tests/test_cli.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     2998 2022-05-28 00:12:43.000000 blark-0.5.0/blark/tests/test_parsing.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    48214 2022-05-28 00:12:43.000000 blark-0.5.0/blark/tests/test_transformer.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     3737 2022-05-28 00:12:43.000000 blark-0.5.0/blark/tests/test_util.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    87054 2022-05-28 00:12:43.000000 blark-0.5.0/blark/transform.py
--rw-r--r--   0 klauer   (1318172782) 1704612529     9904 2022-05-28 00:12:43.000000 blark-0.5.0/blark/util.py
-drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2022-05-28 00:12:54.425553 blark-0.5.0/blark.egg-info/
--rw-r--r--   0 klauer   (1318172782) 1704612529     4034 2022-05-28 00:12:54.000000 blark-0.5.0/blark.egg-info/PKG-INFO
--rw-r--r--   0 klauer   (1318172782) 1704612529     1014 2022-05-28 00:12:54.000000 blark-0.5.0/blark.egg-info/SOURCES.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        1 2022-05-28 00:12:54.000000 blark-0.5.0/blark.egg-info/dependency_links.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       46 2022-05-28 00:12:54.000000 blark-0.5.0/blark.egg-info/entry_points.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       15 2022-05-28 00:12:54.000000 blark-0.5.0/blark.egg-info/requires.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529        6 2022-05-28 00:12:54.000000 blark-0.5.0/blark.egg-info/top_level.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529       15 2022-05-28 00:12:43.000000 blark-0.5.0/requirements.txt
--rw-r--r--   0 klauer   (1318172782) 1704612529      169 2022-05-28 00:12:54.431175 blark-0.5.0/setup.cfg
--rw-r--r--   0 klauer   (1318172782) 1704612529     1369 2022-05-28 00:12:43.000000 blark-0.5.0/setup.py
--rw-r--r--   0 klauer   (1318172782) 1704612529    78254 2022-05-28 00:12:43.000000 blark-0.5.0/versioneer.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-04-19 20:47:59.643683 blark-0.6.0/
+-rw-r--r--   0 klauer   (1318172782) 1704612529    17987 2022-05-28 00:12:43.000000 blark-0.6.0/LICENSE
+-rw-r--r--   0 klauer   (1318172782) 1704612529      196 2022-05-28 00:12:43.000000 blark-0.6.0/MANIFEST.in
+-rw-r--r--   0 klauer   (1318172782) 1704612529     8310 2023-04-19 20:47:59.644019 blark-0.6.0/PKG-INFO
+-rw-r--r--   0 klauer   (1318172782) 1704612529     8065 2023-04-19 20:46:40.000000 blark-0.6.0/README.md
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-04-19 20:47:59.649329 blark-0.6.0/blark/
+-rw-r--r--   0 klauer   (1318172782) 1704612529      426 2022-05-28 00:12:43.000000 blark-0.6.0/blark/__init__.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529       31 2022-05-28 00:12:43.000000 blark-0.6.0/blark/__main__.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529      497 2023-04-19 20:47:59.649780 blark-0.6.0/blark/_version.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     5500 2022-05-28 00:12:43.000000 blark-0.6.0/blark/apischema_compat.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529       74 2022-05-28 00:12:43.000000 blark-0.6.0/blark/config.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    11719 2022-05-28 00:12:43.000000 blark-0.6.0/blark/dependency_store.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     3019 2022-05-28 00:12:43.000000 blark-0.6.0/blark/format.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    24996 2023-04-19 20:46:40.000000 blark-0.6.0/blark/iec.lark
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2244 2022-05-28 00:12:43.000000 blark-0.6.0/blark/main.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    10408 2022-05-28 00:12:43.000000 blark-0.6.0/blark/parse.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    20684 2022-05-28 00:12:43.000000 blark-0.6.0/blark/sphinxdomain.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    29725 2022-05-28 00:12:43.000000 blark-0.6.0/blark/summary.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-04-19 20:47:59.630313 blark-0.6.0/blark/tests/
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-04-19 20:47:59.632447 blark-0.6.0/blark/tests/POUs/
+-rw-r--r--   0 klauer   (1318172782) 1704612529      925 2022-05-28 00:12:43.000000 blark-0.6.0/blark/tests/POUs/F_SetStateParams.TcPOU
+-rw-r--r--   0 klauer   (1318172782) 1704612529      578 2022-05-28 00:12:43.000000 blark-0.6.0/blark/tests/POUs/global_version.TcPOU
+-rw-r--r--   0 klauer   (1318172782) 1704612529        0 2022-05-28 00:12:43.000000 blark-0.6.0/blark/tests/__init__.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2606 2022-05-28 00:12:43.000000 blark-0.6.0/blark/tests/conftest.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-04-19 20:47:59.642950 blark-0.6.0/blark/tests/source/
+-rw-r--r--   0 klauer   (1318172782) 1704612529      653 2022-05-28 00:12:43.000000 blark-0.6.0/blark/tests/source/and_then_or_else.st
+-rw-r--r--   0 klauer   (1318172782) 1704612529      991 2023-04-19 20:46:40.000000 blark-0.6.0/blark/tests/source/array_initializer.st
+-rw-r--r--   0 klauer   (1318172782) 1704612529      183 2022-05-28 00:12:43.000000 blark-0.6.0/blark/tests/source/array_of_objects.st
+-rw-r--r--   0 klauer   (1318172782) 1704612529      149 2023-04-19 20:46:40.000000 blark-0.6.0/blark/tests/source/array_with_integer_initializer.st
+-rw-r--r--   0 klauer   (1318172782) 1704612529      639 2022-05-28 00:12:43.000000 blark-0.6.0/blark/tests/source/commas_in_case.st
+-rw-r--r--   0 klauer   (1318172782) 1704612529      187 2023-04-19 20:46:40.000000 blark-0.6.0/blark/tests/source/dereference_method.st
+-rw-r--r--   0 klauer   (1318172782) 1704612529      195 2023-04-19 20:46:40.000000 blark-0.6.0/blark/tests/source/fb_initializer.st
+-rw-r--r--   0 klauer   (1318172782) 1704612529      134 2022-05-28 00:12:43.000000 blark-0.6.0/blark/tests/source/fb_w_public_access.st
+-rw-r--r--   0 klauer   (1318172782) 1704612529      575 2023-04-19 20:46:40.000000 blark-0.6.0/blark/tests/source/object_oriented_dotaccess.st
+-rw-r--r--   0 klauer   (1318172782) 1704612529      174 2022-05-28 00:12:43.000000 blark-0.6.0/blark/tests/source/pointer_to_pointer_to.st
+-rw-r--r--   0 klauer   (1318172782) 1704612529      352 2022-05-28 00:12:43.000000 blark-0.6.0/blark/tests/source/stray_comment.st
+-rw-r--r--   0 klauer   (1318172782) 1704612529      260 2022-05-28 00:12:43.000000 blark-0.6.0/blark/tests/source/type_and_fb.st
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2740 2022-05-28 00:12:43.000000 blark-0.6.0/blark/tests/test_cli.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     2998 2022-05-28 00:12:43.000000 blark-0.6.0/blark/tests/test_parsing.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    49696 2023-04-19 20:46:40.000000 blark-0.6.0/blark/tests/test_transformer.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     3737 2022-05-28 00:12:43.000000 blark-0.6.0/blark/tests/test_util.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    89465 2023-04-19 20:46:40.000000 blark-0.6.0/blark/transform.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529     9904 2022-05-28 00:12:43.000000 blark-0.6.0/blark/util.py
+drwxr-xr-x   0 klauer   (1318172782) 1704612529        0 2023-04-19 20:47:59.621778 blark-0.6.0/blark.egg-info/
+-rw-r--r--   0 klauer   (1318172782) 1704612529     8310 2023-04-19 20:47:59.000000 blark-0.6.0/blark.egg-info/PKG-INFO
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1233 2023-04-19 20:47:59.000000 blark-0.6.0/blark.egg-info/SOURCES.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529        1 2023-04-19 20:47:59.000000 blark-0.6.0/blark.egg-info/dependency_links.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529       46 2023-04-19 20:47:59.000000 blark-0.6.0/blark.egg-info/entry_points.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529       15 2023-04-19 20:47:59.000000 blark-0.6.0/blark.egg-info/requires.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529        6 2023-04-19 20:47:59.000000 blark-0.6.0/blark.egg-info/top_level.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529       15 2022-05-28 00:12:43.000000 blark-0.6.0/requirements.txt
+-rw-r--r--   0 klauer   (1318172782) 1704612529      169 2023-04-19 20:47:59.646430 blark-0.6.0/setup.cfg
+-rw-r--r--   0 klauer   (1318172782) 1704612529     1369 2022-05-28 00:12:43.000000 blark-0.6.0/setup.py
+-rw-r--r--   0 klauer   (1318172782) 1704612529    78254 2022-05-28 00:12:43.000000 blark-0.6.0/versioneer.py
```

### Comparing `blark-0.5.0/LICENSE` & `blark-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark/apischema_compat.py` & `blark-0.6.0/blark/apischema_compat.py`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark/dependency_store.py` & `blark-0.6.0/blark/dependency_store.py`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark/format.py` & `blark-0.6.0/blark/format.py`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark/iec.lark` & `blark-0.6.0/blark/iec.lark`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 ?any_integer: "2#" BIT_STRING             -> binary_integer
             | "8#" OCTAL_STRING           -> octal_integer
             | "16#" HEX_STRING            -> hex_integer
             | SIGNED_INTEGER              -> signed_integer
             | integer
 
-integer: INTEGER
+integer: [ "10#" ] INTEGER
 
 real_literal: [ REAL_TYPE_NAME "#" ] /((\+|\-)?[0-9](_?[0-9])*)\.([0-9](_?[0-9])*)((e|E)(\+|\-)?([0-9](_?[0-9])*))?/
             | [ REAL_TYPE_NAME "#" ] /((\+|\-)?[0-9](_?[0-9])*)((e|E)(\+|\-)?([0-9](_?[0-9])*))/
 
 bit_string_literal: [ BIT_STRING_TYPE_NAME "#" ] "2#" BIT_STRING    -> binary_bit_string_literal
                   | [ BIT_STRING_TYPE_NAME "#" ] "8#" OCTAL_STRING  -> octal_bit_string_literal
                   | [ BIT_STRING_TYPE_NAME "#" ] "16#" HEX_STRING   -> hex_bit_string_literal
@@ -326,17 +326,20 @@
 array_spec_init: [ indirection_type ] array_specification [ ":=" array_initialization ]
 
 array_specification: "ARRAY"i "[" subrange ( "," subrange )* "]" "OF"i _array_spec_type
 
 _array_spec_type: STRING_TYPE
                 | function_call
                 | non_generic_type_name
+                | object_initializer_array
 
-array_initialization: "[" array_initial_element ( "," array_initial_element )* "]"
-                    | array_initial_element ( "," array_initial_element )*
+object_initializer_array: function_block_type_name "[" structure_initialization ( "," structure_initialization )* "]"
+
+array_initialization: "[" array_initial_element ( "," array_initial_element )* "]" -> bracketed_array_initialization
+                    | array_initial_element ( "," array_initial_element )*         -> bare_array_initialization
 
 array_initial_element: ( integer | enumerated_value ) "(" [ _array_initial_element ] ")" -> array_initial_element_count
                      | _array_initial_element
 
 _array_initial_element: constant
                       | structure_initialization
                       | enumerated_value
@@ -432,15 +435,15 @@
 
 array_var_init_decl: var1_list ":" array_spec_init
 
 structured_var_init_decl: var1_list ":" initialized_structure
 
 // Function blocks
 fb_decl: fb_decl_name_list ":" function_block_type_name [ ":=" structure_initialization ] -> fb_name_decl
-       | fb_decl_name_list ":" function_call                                              -> fb_invocation_decl
+       | fb_decl_name_list ":" function_call [ ":=" structure_initialization ]            -> fb_invocation_decl
 
 fb_decl_name_list: fb_name ( "," fb_name )*
 
 var_body: ( var_init_decl ";"+ )*
 
 array_var_declaration: var1_list ":" array_specification
 
@@ -700,61 +703,61 @@
 
 unary_expression: [ UNARY_OPERATOR ] primary_expression
 
 UNARY_OPERATOR: LOGICAL_NOT
               | MINUS
               | PLUS
 
-function_call: symbolic_variable "(" [ param_assignment ( "," param_assignment )* ","? ] ")"
+function_call: symbolic_variable "(" [ param_assignment ( "," param_assignment )* ","? ] ")" DEREFERENCED?
 
 ?primary_expression: "(" expression ")"      -> parenthesized_expression
                    | function_call
                    | _variable
                    | constant
 
 // B.3.2
 statement_list: _statement+
 
 _statement: ";"
-          | method_statement
           | assignment_statement
           | no_op_statement
           | set_statement
           | reset_statement
           | reference_assignment_statement
           | return_statement
+          | chained_function_call_statement
           | function_call_statement
           | if_statement
           | case_statement
           | for_statement
           | while_statement
           | repeat_statement
           | exit_statement
+          | continue_statement
 
 
 // B.3.2.1
 no_op_statement: _variable ";"+
 
 assignment_statement: _variable ":=" ( _variable ":=" )* expression ";"+
 
 set_statement: _variable "S="i expression ";"+
 
 reset_statement: _variable "R="i expression ";"+
 
 reference_assignment_statement: _variable "REF="i expression ";"+
 
-// method ::= expression [DEREFERENCED] '.' _identifier '(' ')';
-method_statement: symbolic_variable "(" ")" ";"+
-
 // B.3.2.2
 return_statement.1: "RETURN"i ";"*
 // return_statement: priority > 0 so that it doesn't clash with no_op_statement
 
 function_call_statement: function_call ";"+
 
+chained_function_call_statement: function_call ("." function_call)+ ";"+
+
 param_assignment: [ LOGICAL_NOT ] variable_name "=>" [ expression ] -> output_parameter_assignment
                 | variable_name ":=" [ expression ]
                 | expression
 
 // B.3.2.3
 if_statement: "IF"i expression "THEN"i [ statement_list ] ( else_if_clause )* [ else_clause ] "END_IF"i ";"*
 else_if_clause: "ELSIF"i expression "THEN"i [ statement_list ]
@@ -783,7 +786,9 @@
 _for_list: expression "TO"i expression [ "BY"i expression ]
 
 while_statement: "WHILE"i expression "DO"i statement_list "END_WHILE"i ";"*
 
 repeat_statement: "REPEAT"i statement_list "UNTIL"i expression "END_REPEAT"i ";"*
 
 exit_statement.1: "EXIT"i ";"*
+
+continue_statement.1: "CONTINUE"i ";"*
```

### Comparing `blark-0.5.0/blark/main.py` & `blark-0.6.0/blark/main.py`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark/parse.py` & `blark-0.6.0/blark/parse.py`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark/sphinxdomain.py` & `blark-0.6.0/blark/sphinxdomain.py`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark/summary.py` & `blark-0.6.0/blark/summary.py`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark/tests/POUs/F_SetStateParams.TcPOU` & `blark-0.6.0/blark/tests/POUs/F_SetStateParams.TcPOU`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark/tests/POUs/global_version.TcPOU` & `blark-0.6.0/blark/tests/POUs/global_version.TcPOU`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark/tests/conftest.py` & `blark-0.6.0/blark/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark/tests/source/and_then_or_else.st` & `blark-0.6.0/blark/tests/source/and_then_or_else.st`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark/tests/source/commas_in_case.st` & `blark-0.6.0/blark/tests/source/commas_in_case.st`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark/tests/test_cli.py` & `blark-0.6.0/blark/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark/tests/test_parsing.py` & `blark-0.6.0/blark/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark/tests/test_transformer.py` & `blark-0.6.0/blark/tests/test_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,24 @@
     transformed = parse_source_code(value, parser=parser)
     print("\n\nTransformed:")
     print(repr(transformed))
     print("\n\nOr:")
     print(transformed)
     if expected is None:
         expected = value
-    assert str(transformed) == expected, \
-        "Transformed object does not produce identical source code"
+    try:
+        assert str(transformed) == expected, \
+            "Transformed object does not produce identical source code"
+    except Exception:
+        tree = parse_source_code(value, parser=parser, transform=False)
+        print("\n\nTransformation failure. The original source code was:")
+        print(value)
+        print("\n\nThe parse tree is:")
+        print(tree.pretty())
+        raise
 
     conftest.check_serialization(
         transformed, deserialize=True, require_same_source=True
     )
     return transformed
 
 
@@ -59,14 +67,17 @@
         "microseconds",
         "nanoseconds",
         "minutes",
 
         # handled as aliases
         "case_list",
 
+        # handled as special cases
+        "array_initialization",
+
         # handled as tree
         "global_var_list",
         "var_body",
     }
 
     todo_rules = set()
 
@@ -79,14 +90,15 @@
 
 
 @pytest.mark.parametrize(
     "name, value, expected",
     [
         param("integer_literal", "-12", tf.Integer(value="-12")),
         param("integer_literal", "12", tf.Integer(value="12")),
+        param("integer_literal", "10#12", tf.Integer(value="12")),
         param("integer_literal", "INT#12", tf.Integer(value="12", type_name="INT")),
         param("integer_literal", "2#10010", tf.BinaryInteger(value="10010")),
         param("integer_literal", "8#22", tf.OctalInteger(value="22")),
         param("integer_literal", "16#12", tf.HexInteger(value="12")),
         param("integer_literal", "UDINT#12", tf.Integer(value="12", type_name="UDINT")),
         param("integer_literal", "UDINT#2#010", tf.BinaryInteger(value="010", type_name="UDINT")),  # noqa: E501
         param("integer_literal", "UDINT#2#1001_0011", tf.BinaryInteger(value="1001_0011", type_name="UDINT")),  # noqa: E501
@@ -350,18 +362,14 @@
         param("input_declarations", tf.multiline_code_block(
             """
             VAR_INPUT RETAIN
                 fbTest : FB_Test := (A := 1, B := 2, C := 3);
             END_VAR
             """,
             ),
-            marks=pytest.mark.xfail(reason="TODO; this is valid grammar, I think"),
-            # Identical paths:
-            #   fb_name_decl -> structure_initialization
-            #   array_initialization -> array_initial_element -> structure_initialization
         ),
     ],
 )
 def test_input_roundtrip(rule_name, value):
     roundtrip_rule(rule_name, value)
 
 
@@ -405,16 +413,14 @@
         param("output_declarations", tf.multiline_code_block(
             """
             VAR_OUTPUT RETAIN
                 fbTest : FB_Test := (A := 1, B := 2, C := 3);
             END_VAR
             """,
             ),
-            marks=pytest.mark.xfail(reason="TODO; this is valid grammar, I think"),
-            # Appears to collide with enum rule; need to fix
         ),
     ],
 )
 def test_output_roundtrip(rule_name, value):
     roundtrip_rule(rule_name, value)
 
 
@@ -441,27 +447,33 @@
             VAR_IN_OUT
                 iValue : INT;
                 sValue : STRING := 'abc';
                 wsValue : WSTRING := "abc";
                 fbTest : FB_Test(1, 2, 3);
                 fbTest : FB_Test(A := 1, B := 2, C => 3);
                 fbTest : FB_Test(1, 2, A := 1, B := 2, C => 3);
+                fbTest : FB_Test(initializer := 5) := (A := 1, B := 2, C := 3);
                 fbTest : FB_Test := (1, 2, 3);
             END_VAR
             """
         )),
         param("input_output_declarations", tf.multiline_code_block(
             """
             VAR_IN_OUT
+                fbProblematic1 : FB_Test(initializer := 5) := (A := 1, B := 2, C := 3);
+            END_VAR
+            """
+        )),
+        param("input_output_declarations", tf.multiline_code_block(
+            """
+            VAR_IN_OUT
                 fbTest : FB_Test := (A := 1, B := 2, C := 3);
             END_VAR
             """,
             ),
-            marks=pytest.mark.xfail(reason="TODO; this is valid grammar, I think"),
-            # Appears to collide with enum rule; need to fix
         ),
     ],
 )
 def test_input_output_roundtrip(rule_name, value):
     roundtrip_rule(rule_name, value)
 
 
@@ -765,14 +777,24 @@
                 Method();
                 IF 1 THEN
                     EXIT;
                 END_IF
             END_FUNCTION_BLOCK
             """
         )),
+        param("function_block_type_declaration", tf.multiline_code_block(
+            """
+            FUNCTION_BLOCK fbName
+                Method();
+                IF 1 THEN
+                    CONTINUE;
+                END_IF
+            END_FUNCTION_BLOCK
+            """
+        )),
         param("function_block_method_declaration", tf.multiline_code_block(
             """
             METHOD PRIVATE MethodName : RETURNTYPE
             END_METHOD
             """
         )),
         param("function_block_method_declaration", tf.multiline_code_block(
@@ -1059,14 +1081,29 @@
             """
             FOR iIndex[1] := 0 TO 10
             DO
                 iValue := iIndex * 2;
             END_FOR
             """
         )),
+        param("chained_function_call_statement", tf.multiline_code_block(
+            """
+            uut.call1().call2().call3().call4().done();
+            """
+        )),
+        param("chained_function_call_statement", tf.multiline_code_block(
+            """
+            uut.call1()^.call2().call3()^.call4().done();
+            """
+        )),
+        param("chained_function_call_statement", tf.multiline_code_block(
+            """
+            uut.call1()^.call2(A := 1).call3(B := 2)^.call4().done();
+            """
+        )),
     ],
 )
 def test_statement_roundtrip(rule_name, value):
     roundtrip_rule(rule_name, value)
 
 
 @pytest.mark.parametrize(
@@ -1494,7 +1531,22 @@
 )
 def test_meta(code: str, comments: List[str], pragmas: List[str]):
     transformed = parse_source_code(code)
     meta = transformed.items[0].meta
     found_comments, found_pragmas = meta.get_comments_and_pragmas()
     assert [str(comment) for comment in found_comments] == comments
     assert [str(pragma) for pragma in found_pragmas] == pragmas
+
+
+@pytest.mark.parametrize(
+    "statement, cls",
+    [
+        ("CONTINUE;", tf.ContinueStatement),
+        ("EXIT;", tf.ExitStatement),
+        ("RETURN;", tf.ReturnStatement),
+    ]
+)
+def test_statement_priority(statement: str, cls: type):
+    transformed = roundtrip_rule("statement_list", statement)
+    assert isinstance(transformed, tf.StatementList)
+    transformed_statement, = transformed.statements
+    assert isinstance(transformed_statement, cls)
```

### Comparing `blark-0.5.0/blark/tests/test_util.py` & `blark-0.6.0/blark/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark/transform.py` & `blark-0.6.0/blark/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,16 +162,16 @@
         -------
         comments : List[lark.Token]
         pragmas : List[lark.Token]
         """
         if not self.comments:
             return [], []
 
-        pragmas = []
-        comments = []
+        pragmas: List[lark.Token] = []
+        comments: List[lark.Token] = []
         by_type = {
             "SINGLE_LINE_COMMENT": comments,
             "MULTI_LINE_COMMENT": comments,
             "PRAGMA": pragmas,
         }
 
         for comment in self.comments:
@@ -500,15 +500,15 @@
 
 @dataclass
 @_rule_handler("ltime_of_day")
 class LtimeOfDay(Literal):
     """Long time of day literal value."""
     hour: lark.Token
     minute: lark.Token
-    second: lark.Token
+    second: Optional[lark.Token] = None
     meta: Optional[Meta] = meta_field()
 
     @property
     def value(self) -> str:
         """The long time of day value."""
         return f"{self.hour}:{self.minute}:{self.second}"
 
@@ -519,15 +519,15 @@
 @dataclass
 @_rule_handler("date")
 class Date(Literal):
     """Date literal value."""
 
     year: lark.Token
     month: lark.Token
-    day: lark.Token
+    day: Optional[lark.Token]
     meta: Optional[Meta] = meta_field()
 
     @property
     def value(self) -> str:
         """The time of day value."""
         return f"{self.year}-{self.month}-{self.day}"
 
@@ -566,15 +566,15 @@
     @staticmethod
     def from_lark(
         year: lark.Token,
         month: lark.Token,
         day: lark.Token,
         hour: lark.Token,
         minute: lark.Token,
-        second: lark.Token,
+        second: Optional[lark.Token],
     ) -> DateTime:
         return DateTime(
             date=Date(year=year, month=month, day=day),
             time=TimeOfDay(hour=hour, minute=minute, second=second),
         )
 
     @property
@@ -598,15 +598,15 @@
     @staticmethod
     def from_lark(
         year: lark.Token,
         month: lark.Token,
         day: lark.Token,
         hour: lark.Token,
         minute: lark.Token,
-        second: lark.Token,
+        second: Optional[lark.Token],
     ) -> LdateTime:
         return LdateTime(
             ldate=Ldate(year=year, month=month, day=day),
             ltime=LtimeOfDay(hour=hour, minute=minute, second=second),
         )
 
     @property
@@ -693,36 +693,42 @@
 
 
 class VariableLocationPrefix(str, Enum):
     input = "I"
     output = "Q"
     memory = "M"
 
+    def __str__(self) -> str:
+        return self.value
+
 
 class VariableSizePrefix(str, Enum):
     bit = "X"
     byte = "B"
     word_16 = "W"
     dword_32 = "D"
     lword_64 = "L"
 
+    def __str__(self) -> str:
+        return self.value
+
 
 @dataclass
 @_rule_handler("direct_variable")
 class DirectVariable(Variable):
     location_prefix: VariableLocationPrefix
     location: lark.Token
     size_prefix: VariableSizePrefix
     bits: Optional[List[lark.Token]] = None
     meta: Optional[Meta] = meta_field()
 
     @staticmethod
     def from_lark(
         location_prefix: lark.Token,
-        size_prefix: Optional[VariableSizePrefix],
+        size_prefix: Optional[lark.Token],
         location: lark.Token,
         *bits: lark.Token,
     ):
         return DirectVariable(
             location_prefix=VariableLocationPrefix(location_prefix),
             size_prefix=(
                 VariableSizePrefix(size_prefix)
@@ -793,40 +799,40 @@
         parts = ", ".join(str(subscript) for subscript in self.subscripts)
         return f"[{parts}]^" if self.dereferenced else f"[{parts}]"
 
 
 @dataclass
 @_rule_handler("field_selector")
 class FieldSelector:
-    field: SymbolicVariable
+    field: SimpleVariable
     dereferenced: bool
     meta: Optional[Meta] = meta_field()
 
     @staticmethod
-    def from_lark(dereferenced: Optional[lark.Token], field: SymbolicVariable):
+    def from_lark(dereferenced: Optional[lark.Token], field: SimpleVariable):
         return FieldSelector(
             field=field,
             dereferenced=dereferenced is not None
         )
 
     def __str__(self) -> str:
         return f"^.{self.field}" if self.dereferenced else f".{self.field}"
 
 
 @dataclass
 @_rule_handler("multi_element_variable")
 class MultiElementVariable(Variable):
-    name: SymbolicVariable
+    name: SimpleVariable
     dereferenced: bool
     elements: List[Union[SubscriptList, FieldSelector]]
     meta: Optional[Meta] = meta_field()
 
     @staticmethod
     def from_lark(
-        variable_name: SymbolicVariable,
+        variable_name: SimpleVariable,
         *subscript_or_field: Union[SubscriptList, FieldSelector]
     ) -> MultiElementVariable:
         return MultiElementVariable(
             name=variable_name,
             elements=list(subscript_or_field),
             dereferenced=False,
         )
@@ -942,17 +948,18 @@
     @property
     def full_type_name(self) -> str:
         """The full type name."""
         return self.spec.full_type_name
 
     @staticmethod
     def from_lark(
-        *args: lark.Token,
+        string_type: lark.Token,
+        length: Optional[lark.Token],
+        *value_parts: Optional[lark.Token],
     ) -> StringTypeInitialization:
-        string_type, length, *value_parts = args
         spec = StringTypeSpecification(string_type, length)
         _, value = value_parts or [None, None]
         return StringTypeInitialization(spec=spec, value=value)
 
     def __str__(self) -> str:
         return join_if(self.spec, " := ", self.value)
 
@@ -1155,22 +1162,24 @@
     def __str__(self) -> str:
         return join_if(self.indirection, " ", self.type)
 
 
 @dataclass
 @_rule_handler("array_specification")
 class ArraySpecification:
-    type: Union[DataType, FunctionCall]
+    type: Union[DataType, FunctionCall, ObjectInitializerArray]
     subranges: List[Subrange]
     meta: Optional[Meta] = meta_field()
 
     @property
-    def base_type_name(self) -> lark.Token:
+    def base_type_name(self) -> Union[str, lark.Token]:
         """The base type name."""
-        return self.type.type_name
+        if isinstance(self.type, DataType):
+            return self.type.type_name
+        return str(self.type.name)
 
     @property
     def full_type_name(self) -> str:
         """The full type name."""
         return str(self)
 
     @staticmethod
@@ -1213,39 +1222,74 @@
         return ArrayInitialElement(
             element=element,
             count=count,
         )
 
 
 @dataclass
-@_rule_handler("array_initialization")
+@_rule_handler("bracketed_array_initialization")
+class _BracketedArrayInitialization:
+    @staticmethod
+    def from_lark(*elements: ArrayInitialElement) -> ArrayInitialization:
+        return ArrayInitialization(list(elements), brackets=True)
+
+
+@dataclass
+@_rule_handler("bare_array_initialization")
+class _BareArrayInitialization:
+    @staticmethod
+    def from_lark(*elements: ArrayInitialElement) -> ArrayInitialization:
+        return ArrayInitialization(list(elements), brackets=False)
+
+
+@dataclass
 class ArrayInitialization:
     elements: List[ArrayInitialElement]
-    count: Optional[Union[EnumeratedValue, Integer]] = None
+    brackets: bool = False
+    meta: Optional[Meta] = meta_field()
+
+    def __str__(self) -> str:
+        elements = ", ".join(str(element) for element in self.elements)
+        if self.brackets:
+            return f"[{elements}]"
+        return elements
+
+
+@dataclass
+@_rule_handler("object_initializer_array")
+class ObjectInitializerArray:
+    name: SymbolicVariable
+    initializers: List[StructureInitialization]
     meta: Optional[Meta] = meta_field()
 
     @staticmethod
-    def from_lark(*elements: ArrayInitialElement):
-        return ArrayInitialization(list(elements))
+    def from_lark(
+        function_block_type_name: SymbolicVariable,
+        *initializers: List[StructureInitialization]
+    ) -> ObjectInitializerArray:
+        return ObjectInitializerArray(
+            name=function_block_type_name,
+            initializers=list(initializers)
+        )
 
     def __str__(self) -> str:
-        elements = ", ".join(str(element) for element in self.elements)
-        return f"[{elements}]"
+        initializers = ", ".join([f"({init})" for init in self.initializers])
+        return f"{self.name}[{initializers}]"
 
 
 @dataclass
 @_rule_handler("array_spec_init")
 class ArrayTypeInitialization:
     indirection: Optional[IndirectionType]
     spec: ArraySpecification
     value: Optional[ArrayInitialization]
     meta: Optional[Meta] = meta_field()
 
     @property
-    def base_type_name(self) -> lark.Token:
+    def base_type_name(self) -> Union[str, lark.Token]:
         """The base type name."""
         return self.spec.base_type_name
 
     @property
     def full_type_name(self) -> str:
         """The full type name."""
         return self.spec.full_type_name
@@ -1552,14 +1596,15 @@
 
 
 @dataclass
 @_rule_handler("function_call")
 class FunctionCall(Expression):
     name: SymbolicVariable
     parameters: List[ParameterAssignment]
+    dereferenced: bool
     meta: Optional[Meta] = meta_field()
 
     @property
     def base_type_name(self) -> str:
         """
         The base type name.
 
@@ -1583,34 +1628,42 @@
         This is used as part of the summary tool.
         """
         return str(self)
 
     @staticmethod
     def from_lark(
         name: SymbolicVariable,
-        *parameters: ParameterAssignment,
+        *params: Union[ParameterAssignment, lark.Token, None],
     ) -> FunctionCall:
         # Condition parameters (which may be `None`) to represent empty tuple
-        if parameters == (None, ):
-            parameters = []
+        if params and params[0] is None:
+            params = params[1:]
+        dereferenced = bool(params and params[-1] == "^")
+        if dereferenced:
+            params = params[:-1]
+
         return FunctionCall(
             name=name,
-            parameters=list(parameters)
+            parameters=typing.cast(List[ParameterAssignment], list(params)),
+            dereferenced=dereferenced,
         )
 
     def __str__(self) -> str:
+        dereference = ""
         parameters = ", ".join(str(param) for param in self.parameters)
-        return f"{self.name}({parameters})"
+        if self.dereferenced:
+            dereference = "^"
+        return f"{self.name}({parameters}){dereference}"
 
 
 @dataclass
 @_rule_handler("var1")
 class DeclaredVariable:
     # Alternate name: VariableWithLocation? MaybeLocatedVariable?
-    variable: SymbolicVariable
+    variable: SimpleVariable
     location: Optional[Union[IncompleteLocation, Location]]
     meta: Optional[Meta] = meta_field()
 
     @property
     def name(self) -> lark.Token:
         """The variable name."""
         return self.variable.name
@@ -1750,19 +1803,21 @@
 
 
 @dataclass
 @_rule_handler("fb_invocation_decl", comments=True)
 class FunctionBlockInvocationDeclaration(FunctionBlockDeclaration):
     variables: List[lark.Token]
     init: FunctionCall
+    defaults: Optional[StructureInitialization] = None
     meta: Optional[Meta] = meta_field()
 
     def __str__(self) -> str:
         variables = ", ".join(self.variables)
-        return f"{variables} : {self.init}"
+        name_and_type = f"{variables} : {self.init}"
+        return join_if(name_and_type, " := ", self.defaults)
 
 
 @as_tagged_union
 class ParameterAssignment:
     ...
 
 
@@ -2579,23 +2634,41 @@
     @staticmethod
     def from_lark(
         invocation: FunctionCall,
     ) -> FunctionCallStatement:
         return FunctionCallStatement(
             name=invocation.name,
             parameters=invocation.parameters,
+            dereferenced=invocation.dereferenced,
             meta=invocation.meta,
         )
 
     def __str__(self):
         invoc = super().__str__()
         return f"{invoc};"
 
 
 @dataclass
+@_rule_handler("chained_function_call_statement", comments=True)
+class ChainedFunctionCallStatement(Statement):
+    invocations: List[FunctionCall]
+    meta: Optional[Meta] = meta_field()
+
+    @staticmethod
+    def from_lark(*invocations: FunctionCall) -> ChainedFunctionCallStatement:
+        return ChainedFunctionCallStatement(
+            invocations=list(invocations)
+        )
+
+    def __str__(self) -> str:
+        invoc = ".".join(str(invocation) for invocation in self.invocations)
+        return f"{invoc};"
+
+
+@dataclass
 @_rule_handler("else_if_clause", comments=True)
 class ElseIfClause:
     if_expression: Expression
     statements: Optional[StatementList]
     meta: Optional[Meta] = meta_field()
 
     def __str__(self):
@@ -2633,15 +2706,15 @@
     else_clause: Optional[ElseClause]
     meta: Optional[Meta] = meta_field()
 
     @staticmethod
     def from_lark(
         if_expr: Expression,
         then: Optional[StatementList],
-        *args: Union[ElseIfClause, ElseClause]
+        *args: Optional[Union[ElseIfClause, ElseClause]]
     ) -> IfStatement:
         else_clause: Optional[ElseClause] = None
         if args and isinstance(args[-1], ElseClause) or args[-1] is None:
             else_clause = args[-1]
             args = args[:-1]
 
         else_ifs = typing.cast(List[ElseIfClause], list(args))
@@ -2783,14 +2856,23 @@
     meta: Optional[Meta] = meta_field()
 
     def __str__(self):
         return "EXIT;"
 
 
 @dataclass
+@_rule_handler("continue_statement", comments=True)
+class ContinueStatement(Statement):
+    meta: Optional[Meta] = meta_field()
+
+    def __str__(self):
+        return "CONTINUE;"
+
+
+@dataclass
 @_rule_handler("return_statement", comments=True)
 class ReturnStatement(Statement):
     meta: Optional[Meta] = meta_field()
 
     def __str__(self):
         return "RETURN;"
 
@@ -2812,24 +2894,14 @@
 
     def __str__(self):
         variables = " := ".join(str(var) for var in self.variables)
         return f"{variables} := {self.expression};"
 
 
 @dataclass
-@_rule_handler("method_statement", comments=True)
-class MethodStatement(Statement):
-    method: SymbolicVariable
-    meta: Optional[Meta] = meta_field()
-
-    def __str__(self):
-        return f"{self.method}();"
-
-
-@dataclass
 @_rule_handler("while_statement", comments=True)
 class WhileStatement(Statement):
     expression: Expression
     statements: StatementList
     meta: Optional[Meta] = meta_field()
 
     def __str__(self):
```

### Comparing `blark-0.5.0/blark/util.py` & `blark-0.6.0/blark/util.py`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/blark.egg-info/SOURCES.txt` & `blark-0.6.0/blark.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -30,13 +30,18 @@
 blark/tests/test_cli.py
 blark/tests/test_parsing.py
 blark/tests/test_transformer.py
 blark/tests/test_util.py
 blark/tests/POUs/F_SetStateParams.TcPOU
 blark/tests/POUs/global_version.TcPOU
 blark/tests/source/and_then_or_else.st
+blark/tests/source/array_initializer.st
 blark/tests/source/array_of_objects.st
+blark/tests/source/array_with_integer_initializer.st
 blark/tests/source/commas_in_case.st
+blark/tests/source/dereference_method.st
+blark/tests/source/fb_initializer.st
 blark/tests/source/fb_w_public_access.st
+blark/tests/source/object_oriented_dotaccess.st
 blark/tests/source/pointer_to_pointer_to.st
 blark/tests/source/stray_comment.st
 blark/tests/source/type_and_fb.st
```

### Comparing `blark-0.5.0/setup.py` & `blark-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `blark-0.5.0/versioneer.py` & `blark-0.6.0/versioneer.py`

 * *Files identical despite different names*


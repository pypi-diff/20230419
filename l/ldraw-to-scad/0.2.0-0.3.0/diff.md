# Comparing `tmp/ldraw-to-scad-0.2.0.tar.gz` & `tmp/ldraw-to-scad-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldraw-to-scad-0.2.0.tar", last modified: Sat Mar 18 02:03:22 2023, max compression
+gzip compressed data, was "ldraw-to-scad-0.3.0.tar", last modified: Wed Apr 19 11:20:07 2023, max compression
```

## Comparing `ldraw-to-scad-0.2.0.tar` & `ldraw-to-scad-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 02:03:22.903412 ldraw-to-scad-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-18 02:02:58.000000 ldraw-to-scad-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-03-18 02:03:22.903412 ldraw-to-scad-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-03-18 02:02:58.000000 ldraw-to-scad-0.2.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     3605 2023-03-18 02:02:58.000000 ldraw-to-scad-0.2.0/ldraw2scad
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-18 02:02:58.000000 ldraw-to-scad-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-18 02:03:22.903412 ldraw-to-scad-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 02:03:22.899412 ldraw-to-scad-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 02:03:22.899412 ldraw-to-scad-0.2.0/src/ldraw_to_scad/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-18 02:02:58.000000 ldraw-to-scad-0.2.0/src/ldraw_to_scad/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12652 2023-03-18 02:02:58.000000 ldraw-to-scad-0.2.0/src/ldraw_to_scad/ldrawconverter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-03-18 02:02:58.000000 ldraw-to-scad-0.2.0/src/ldraw_to_scad/lib.scad
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 02:03:22.903412 ldraw-to-scad-0.2.0/src/ldraw_to_scad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-03-18 02:03:22.000000 ldraw-to-scad-0.2.0/src/ldraw_to_scad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-18 02:03:22.000000 ldraw-to-scad-0.2.0/src/ldraw_to_scad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 02:03:22.000000 ldraw-to-scad-0.2.0/src/ldraw_to_scad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-18 02:03:22.000000 ldraw-to-scad-0.2.0/src/ldraw_to_scad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 02:03:22.903412 ldraw-to-scad-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-03-18 02:02:58.000000 ldraw-to-scad-0.2.0/tests/test_ldraw_to_scad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:20:07.661911 ldraw-to-scad-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 11:19:49.000000 ldraw-to-scad-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-19 11:20:07.661911 ldraw-to-scad-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-19 11:19:49.000000 ldraw-to-scad-0.3.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3605 2023-04-19 11:19:49.000000 ldraw-to-scad-0.3.0/ldraw2scad
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-19 11:19:49.000000 ldraw-to-scad-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-19 11:20:07.661911 ldraw-to-scad-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:20:07.657911 ldraw-to-scad-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:20:07.661911 ldraw-to-scad-0.3.0/src/ldraw_to_scad/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 11:19:49.000000 ldraw-to-scad-0.3.0/src/ldraw_to_scad/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13225 2023-04-19 11:19:49.000000 ldraw-to-scad-0.3.0/src/ldraw_to_scad/ldrawconverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-19 11:19:49.000000 ldraw-to-scad-0.3.0/src/ldraw_to_scad/lib.scad
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:20:07.661911 ldraw-to-scad-0.3.0/src/ldraw_to_scad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-19 11:20:07.000000 ldraw-to-scad-0.3.0/src/ldraw_to_scad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-19 11:20:07.000000 ldraw-to-scad-0.3.0/src/ldraw_to_scad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:20:07.000000 ldraw-to-scad-0.3.0/src/ldraw_to_scad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 11:20:07.000000 ldraw-to-scad-0.3.0/src/ldraw_to_scad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:20:07.661911 ldraw-to-scad-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-04-19 11:19:49.000000 ldraw-to-scad-0.3.0/tests/test_ldraw_to_scad.py
```

### Comparing `ldraw-to-scad-0.2.0/LICENSE` & `ldraw-to-scad-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ldraw-to-scad-0.2.0/PKG-INFO` & `ldraw-to-scad-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldraw-to-scad
-Version: 0.2.0
+Version: 0.3.0
 Summary: The LDraw to OpenSCAD converter library
 Home-page: https://github.com/orionrobots/ldraw-to-scad
 Author: Danny Staple
 Author-email: danny@orionrobots.co.uk
 Maintainer: Robert Schiele
 Maintainer-email: rschiele@gmail.com
 Project-URL: Bug Tracker, https://github.com/orionrobots/ldraw-to-scad/issues
```

### Comparing `ldraw-to-scad-0.2.0/README.md` & `ldraw-to-scad-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ldraw-to-scad-0.2.0/ldraw2scad` & `ldraw-to-scad-0.3.0/ldraw2scad`

 * *Files identical despite different names*

### Comparing `ldraw-to-scad-0.2.0/src/ldraw_to_scad/ldrawconverter.py` & `ldraw-to-scad-0.3.0/src/ldraw_to_scad/ldrawconverter.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,21 +63,19 @@
                             data[opt] = True
                         else:
                             print(f'Unknown !COLOUR option {opt}!')
                     alpha = int(data["ALPHA"]) if "ALPHA" in data else 255
                     colors.append(
                         f'(id=={data["CODE"]}) ? ["{data["VALUE"]}{alpha:02X}'
                         f'","{data["EDGE"]}"] : (')
-            colors.append('(id>=2*16^6) ? [str("#"')
-            for i in reversed(range(6)):
-                colors.append(f',"0123456789ABCDEF"[id/(16^{i})%16]')
-            colors.append('),str("#"')
-            for i in reversed(range(6)):
-                colors.append(f',"FEDCBA9876543210"[id/(16^{i})%16]')
-            colors.append(')] : ("UNKNOWN"'+')'*(len(colors)-13)+';')
+            colors.append('(id>=2*16^6) ? [chr(35, [for (i=[5:-1:0])'
+                          'let(n=floor(id/16^i)%16) n+(n<10?48:55)]),'
+                          'chr(35, [for (i=[5:-1:0])'
+                          'let(n=15-floor(id/16^i)%16) n+(n<10?48:55)])] :'
+                          '"UNKNOWN"'+')'*len(colors)+';')
             coltxt += '\n'.join(colors) + '\n'
         return coltxt
 
     def index_library(self):
         """ Index the whole library. """
         index = {}
         for sub_path in ['models', 'parts', 'p']:
@@ -134,16 +132,16 @@
         return self.filedep[0]
 
     @staticmethod
     def make_function_name(name):
         """ Calculate OpenSCAD name from LDraw name. """
         function_name = name.lower().split('.', 1)[0]
         function_name = function_name.replace('\\', '__').replace('-', '_').\
-            replace(' ', '_')
-        return 'ldraw_lib__' + function_name + '()'
+            replace('+', '_').replace(' ', '_')
+        return 'ldraw_lib__' + function_name
 
     def convert_line_0(self, result, params, stripped):
         """ Translate a '0' line. """
         if len(params) >= 2 and params[1] == 'BFC':
             for bfc in params[2:]:
                 result.append(f'  [0,"BFC","{bfc}"],')
         if len(params) >= 2 and params[1] == 'STEP':
@@ -151,37 +149,38 @@
         if len(params) >= 2 and params[1] == 'FILE':
             intfile = stripped.split(maxsplit=2)[2]
             if self.implement_function(intfile):
                 self.mpd_main = intfile
             else:
                 result.append("];")
                 intfile_name = LDrawConverter.make_function_name(intfile)
-                result.append(f"function {intfile_name} = [")
+                result.append(f"function {intfile_name}() = [")
         if len(params) >= 2 and params[1] == 'NOFILE':
             intfile = self.get_dummy()
             result.append("];")
             intfile_name = LDrawConverter.make_function_name(intfile)
-            result.append(f"function {intfile_name} = [")
+            result.append(f"function {intfile_name}() = [")
 
     def convert_line(self, part_line):
         """ Translate a single line. """
         stripped = part_line.rstrip()
         result = [f"// {stripped}"] if self.settings['commented'] else []
         params = stripped.split(maxsplit=14)
         if not params:
             return result
         if params[0] == "0":
             self.convert_line_0(result, params, stripped)
         elif params[0] == "1":
-            self.add_dep(params[14])
+            keyname = params[14].replace('/', '\\')
+            self.add_dep(keyname)
             if params[1][0:3] == '0x2':
                 params[1] = str(int(params[1], 0))
             result.append(
                 f"  [{','.join(params[:14])}, "
-                f"{LDrawConverter.make_function_name(params[14])}],")
+                f"{LDrawConverter.make_function_name(keyname)}()],")
         elif params[0] in ["2", "3", "4", "5"]:
             if params[1][0:3] == '0x2':
                 params[1] = str(int(params[1], 0))
             outparams = params[:{'2': 8, '3': 11, '4': 14, '5': 14}[params[0]]]
             result.append(f"  [{','.join(outparams)}],")
         return result
 
@@ -199,25 +198,32 @@
         result = []
         for line in lines:
             result.extend(self.convert_line(line))
         function_name = LDrawConverter.make_function_name(name)
         if self.settings['selfcontained']:
             for file in self.get_deps():
                 self.enqueue(file, path)
-            result = [f"function {function_name} = ["] + result + ["];"]
+            result = [f"function {function_name}() = ["] + result + ["];"]
         else:
             result = [self.include(['lib'], path)] + \
                      [self.include(self.find_part(name), path)
                       for name in sorted(self.get_deps())] + \
-                     [f"function {function_name} = ["] + result + ["];"] + \
-                     [f"makepoly({function_name}, "
-                      f"line={self.settings['line']});"]
+                     [f"function {function_name}() = ["] + result + ["];"] + \
+                     [f"module {function_name}(step=0, col=false, unit=2/5, "
+                      f"alt=false, line=0.2, solid=!$preview)"] + \
+                     [f"    makepoly({function_name}(), step=step, col=col, "
+                      f"unit=unit, alt=alt, line=line, solid=solid);"] + \
+                     [f"{function_name}(line={self.settings['line']});"]
         if self.mpd_main and self.mpd_main != name:
             main_function = LDrawConverter.make_function_name(self.mpd_main)
-            result.append(f"function {main_function} = {function_name};\n")
+            result.append(f"function {main_function}() = {function_name}();")
+            result.append(f"module {main_function}(step=0, col=false, "
+                          f"unit=2/5, alt=false, line=0.2, solid=!$preview)")
+            result.append(f"    {function_name}(step=step, col=col, "
+                          f"unit=unit, alt=alt, line=line, solid=solid);")
         return result
 
     def enqueue(self, name, path=None, ldrfile=None, scadfile=None):
         """ enqueue a file to be processed """
         if name not in self.queue[1]:
             if not ldrfile:
                 lpath, base = self.find_part(name)
```

### Comparing `ldraw-to-scad-0.2.0/src/ldraw_to_scad/lib.scad` & `ldraw-to-scad-0.3.0/src/ldraw_to_scad/lib.scad`

 * *Files identical despite different names*

### Comparing `ldraw-to-scad-0.2.0/src/ldraw_to_scad.egg-info/PKG-INFO` & `ldraw-to-scad-0.3.0/src/ldraw_to_scad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldraw-to-scad
-Version: 0.2.0
+Version: 0.3.0
 Summary: The LDraw to OpenSCAD converter library
 Home-page: https://github.com/orionrobots/ldraw-to-scad
 Author: Danny Staple
 Author-email: danny@orionrobots.co.uk
 Maintainer: Robert Schiele
 Maintainer-email: rschiele@gmail.com
 Project-URL: Bug Tracker, https://github.com/orionrobots/ldraw-to-scad/issues
```

### Comparing `ldraw-to-scad-0.2.0/tests/test_ldraw_to_scad.py` & `ldraw-to-scad-0.3.0/tests/test_ldraw_to_scad.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 class TestModule(TestCase):
     """ tests for generation of function names """
     def test_it_should_make_sensible_function_names(self):
         """ Module names must be valid c identifiers """
         # setup
         function_names_to_convert = [
-            ["stud.dat", "ldraw_lib__stud()"],
-            ["s\\stuff.dat", "ldraw_lib__s__stuff()"],
-            ["4744.dat", "ldraw_lib__4744()"],
-            ["2-4cyli.dat", "ldraw_lib__2_4cyli()"]
+            ["stud.dat", "ldraw_lib__stud"],
+            ["s\\stuff.dat", "ldraw_lib__s__stuff"],
+            ["4744.dat", "ldraw_lib__4744"],
+            ["2-4cyli.dat", "ldraw_lib__2_4cyli"]
         ]
         # test
         # assert
         for item, expected in function_names_to_convert:
             self.assertEqual(LDrawConverter.make_function_name(item), expected)
 
 
@@ -194,15 +194,19 @@
             "// 5 24 0.9239 0 0.3827 0.9239 1 0.3827 0.7071 0 0.7071 1 0 0",
             "  [5,24,0.9239,0,0.3827,0.9239,1,0.3827,0.7071,0,0.7071,1,0,0],",
             ("// 4 16 0.7071 1 0.7071 0.3827 1 0.9239 "
              "0.3827 0 0.9239 0.7071 0 0.7071"),
             ("  [4,16,0.7071,1,0.7071,0.3827,1,0.9239,"
              "0.3827,0,0.9239,0.7071,0,0.7071],"),
             "];",
-            "makepoly(ldraw_lib____main__(), line=0.2);"
+            ("module ldraw_lib____main__(step=0, col=false, unit=2/5, "
+             "alt=false, line=0.2, solid=!$preview)"),
+            ("    makepoly(ldraw_lib____main__(), step=step, col=col, "
+             "unit=unit, alt=alt, line=line, solid=solid);"),
+            "ldraw_lib____main__(line=0.2);"
         ])
 
     def test_reading_file(self):
         """ test conversion of file content """
         # Setup
         test_file = os.path.join(THIS_DIR, "simple_test.dat")
         # test
@@ -219,15 +223,19 @@
             "// 0 BFC CW",
             '  [0,"BFC","CW"],',
             "// ",
             "// 4 16  1 1  1  1 1 -1 -1 1 -1 -1 1  1",
             "  [4,16,1,1,1,1,1,-1,-1,1,-1,-1,1,1],",
             "// ",
             "];",
-            "makepoly(ldraw_lib____main__(), line=0.2);"
+            ("module ldraw_lib____main__(step=0, col=false, unit=2/5, "
+             "alt=false, line=0.2, solid=!$preview)"),
+            ("    makepoly(ldraw_lib____main__(), step=step, col=col, "
+             "unit=unit, alt=alt, line=line, solid=solid);"),
+            "ldraw_lib____main__(line=0.2);"
         ])
 
     def test_it_process_type_1_line_into_function(self):
         """ test whole function creation from type 1 line """
         # setup
         part_lines = [
             "1 16 25 24 23 22 21 20 19 18 17 16 15 14 simple_test.dat"]
@@ -241,15 +249,19 @@
             [
                 "use <LDraw/lib.scad>",
                 "use <LDraw/./simple_test.scad>",
                 "function ldraw_lib____main__() = [",
                 ("  [1,16,25,24,23,22,21,20,19,18,17,16,15,14, "
                  "ldraw_lib__simple_test()],"),
                 "];",
-                "makepoly(ldraw_lib____main__(), line=0.2);"
+                ("module ldraw_lib____main__(step=0, col=false, unit=2/5, "
+                 "alt=false, line=0.2, solid=!$preview)"),
+                ("    makepoly(ldraw_lib____main__(), step=step, col=col, "
+                 "unit=unit, alt=alt, line=line, solid=solid);"),
+                "ldraw_lib____main__(line=0.2);"
             ]
         )
 
     def test_multiple_type_1_lines_should_only_reference_functions_once(self):
         """ test that single function is only referenced/included once """
         # setup
         lines = [
@@ -267,15 +279,19 @@
             "use <LDraw/./simple_test.scad>",
             "function ldraw_lib____main__() = [",
             ("  [1,16,25,24,23,22,21,20,19,18,17,16,15,14, "
              "ldraw_lib__simple_test()],"),
             ("  [1,16,2.5,2.4,2.3,2.2,2.1,2.0,1.9,1.8,1.7,1.6,1.5,1.4, "
              "ldraw_lib__simple_test()],"),
             "];",
-            "makepoly(ldraw_lib____main__(), line=0.2);"
+            ("module ldraw_lib____main__(step=0, col=false, unit=2/5, "
+             "alt=false, line=0.2, solid=!$preview)"),
+            ("    makepoly(ldraw_lib____main__(), step=step, col=col, "
+             "unit=unit, alt=alt, line=line, solid=solid);"),
+            "ldraw_lib____main__(line=0.2);"
         ])
 
     def test_try_simplest_mpd(self):
         """ test MPD functionality """
         # setup
         lines = [
             # 1 - ref the mpd
@@ -304,15 +320,19 @@
             "];",
             "function ldraw_lib__mdr_inner() = [",
             '  [0,"BFC","CW"],',
             "  [4,16,1,1,0,0.9239,1,0.3827,0.9239,0,0.3827,1,0,0],",
             "];",
             "function ldraw_lib__dummy_2() = [",
             "];",
-            "makepoly(ldraw_lib____main__(), line=0.2);"
+            ("module ldraw_lib____main__(step=0, col=false, unit=2/5, "
+             "alt=false, line=0.2, solid=!$preview)"),
+            ("    makepoly(ldraw_lib____main__(), step=step, col=col, "
+             "unit=unit, alt=alt, line=line, solid=solid);"),
+            "ldraw_lib____main__(line=0.2);"
         ])
 
     def test_loading_an_mpd(self):
         """ test a complete MPD file """
         # Setup
         mpd_filename = os.path.join(THIS_DIR, "mpd_test.dat")
         # Test
@@ -347,10 +367,18 @@
             "// 1 16 25 24 23 22 21 20 19 18 17 16 15 14 simple_test.dat",
             ("  [1,16,25,24,23,22,21,20,19,18,17,16,15,14, "
              "ldraw_lib__simple_test()],"),
             "// 0 NOFILE",
             "];",
             "function ldraw_lib__dummy_2() = [",
             "];",
-            "makepoly(ldraw_lib____main__(), line=0.2);",
-            "function ldraw_lib__mdp_test() = ldraw_lib____main__();\n"
+            ("module ldraw_lib____main__(step=0, col=false, unit=2/5, "
+             "alt=false, line=0.2, solid=!$preview)"),
+            ("    makepoly(ldraw_lib____main__(), step=step, col=col, "
+             "unit=unit, alt=alt, line=line, solid=solid);"),
+            "ldraw_lib____main__(line=0.2);",
+            "function ldraw_lib__mdp_test() = ldraw_lib____main__();",
+            ("module ldraw_lib__mdp_test(step=0, col=false, unit=2/5, "
+             "alt=false, line=0.2, solid=!$preview)"),
+            ("    ldraw_lib____main__(step=step, col=col, unit=unit, "
+             "alt=alt, line=line, solid=solid);")
         ])
```


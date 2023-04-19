# Comparing `tmp/RepRepBuild-0.7.0.tar.gz` & `tmp/RepRepBuild-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RepRepBuild-0.7.0.tar", last modified: Mon Apr 17 08:03:13 2023, max compression
+gzip compressed data, was "RepRepBuild-0.7.1.tar", last modified: Wed Apr 19 14:05:26 2023, max compression
```

## Comparing `RepRepBuild-0.7.0.tar` & `RepRepBuild-0.7.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-17 08:03:13.857958 RepRepBuild-0.7.0/
--rw-r--r--   0 toon      (1000) toon      (1000)    35149 2017-09-30 07:16:26.000000 RepRepBuild-0.7.0/COPYING
--rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-17 08:03:13.857958 RepRepBuild-0.7.0/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)     1392 2023-03-21 07:41:05.000000 RepRepBuild-0.7.0/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1612 2023-04-17 08:02:34.000000 RepRepBuild-0.7.0/pyproject.toml
--rw-r--r--   0 toon      (1000) toon      (1000)       38 2023-04-17 08:03:13.857958 RepRepBuild-0.7.0/setup.cfg
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-17 08:03:13.844958 RepRepBuild-0.7.0/src/
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-17 08:03:13.845958 RepRepBuild-0.7.0/src/RepRepBuild.egg-info/
--rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-17 08:03:13.000000 RepRepBuild-0.7.0/src/RepRepBuild.egg-info/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)      571 2023-04-17 08:03:13.000000 RepRepBuild-0.7.0/src/RepRepBuild.egg-info/SOURCES.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        1 2023-04-17 08:03:13.000000 RepRepBuild-0.7.0/src/RepRepBuild.egg-info/dependency_links.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      362 2023-04-17 08:03:13.000000 RepRepBuild-0.7.0/src/RepRepBuild.egg-info/entry_points.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       36 2023-04-17 08:03:13.000000 RepRepBuild-0.7.0/src/RepRepBuild.egg-info/requires.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       12 2023-04-17 08:03:13.000000 RepRepBuild-0.7.0/src/RepRepBuild.egg-info/top_level.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-17 08:03:13.857958 RepRepBuild-0.7.0/src/reprepbuild/
--rw-r--r--   0 toon      (1000) toon      (1000)      775 2023-03-14 11:47:22.000000 RepRepBuild-0.7.0/src/reprepbuild/__init__.py
--rw-r--r--   0 toon      (1000) toon      (1000)    10101 2023-04-17 08:00:00.000000 RepRepBuild-0.7.0/src/reprepbuild/__main__.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1803 2023-03-25 09:41:44.000000 RepRepBuild-0.7.0/src/reprepbuild/articlezip.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3517 2023-04-12 08:19:13.000000 RepRepBuild-0.7.0/src/reprepbuild/bibtex.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3910 2023-03-25 09:41:50.000000 RepRepBuild-0.7.0/src/reprepbuild/latex.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4434 2023-03-25 09:51:45.000000 RepRepBuild-0.7.0/src/reprepbuild/latexdep.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1792 2023-03-25 09:42:18.000000 RepRepBuild-0.7.0/src/reprepbuild/normalizepdf.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4087 2023-03-25 09:44:04.000000 RepRepBuild-0.7.0/src/reprepbuild/pythonscript.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2856 2023-03-16 20:21:01.000000 RepRepBuild-0.7.0/src/reprepbuild/repeat.py
--rw-r--r--   0 toon      (1000) toon      (1000)     5006 2023-03-25 09:15:24.000000 RepRepBuild-0.7.0/src/reprepbuild/utils.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2340 2023-03-28 14:48:56.000000 RepRepBuild-0.7.0/src/reprepbuild/zip.py
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-19 14:05:26.330329 RepRepBuild-0.7.1/
+-rw-r--r--   0 toon      (1000) toon      (1000)    35149 2017-09-30 07:16:26.000000 RepRepBuild-0.7.1/COPYING
+-rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-19 14:05:26.330329 RepRepBuild-0.7.1/PKG-INFO
+-rw-r--r--   0 toon      (1000) toon      (1000)     1392 2023-03-21 07:41:05.000000 RepRepBuild-0.7.1/README.md
+-rw-r--r--   0 toon      (1000) toon      (1000)     1612 2023-04-19 14:04:50.000000 RepRepBuild-0.7.1/pyproject.toml
+-rw-r--r--   0 toon      (1000) toon      (1000)       38 2023-04-19 14:05:26.330329 RepRepBuild-0.7.1/setup.cfg
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-19 14:05:26.318328 RepRepBuild-0.7.1/src/
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-19 14:05:26.319328 RepRepBuild-0.7.1/src/RepRepBuild.egg-info/
+-rw-r--r--   0 toon      (1000) toon      (1000)    43045 2023-04-19 14:05:26.000000 RepRepBuild-0.7.1/src/RepRepBuild.egg-info/PKG-INFO
+-rw-r--r--   0 toon      (1000) toon      (1000)      571 2023-04-19 14:05:26.000000 RepRepBuild-0.7.1/src/RepRepBuild.egg-info/SOURCES.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)        1 2023-04-19 14:05:26.000000 RepRepBuild-0.7.1/src/RepRepBuild.egg-info/dependency_links.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)      362 2023-04-19 14:05:26.000000 RepRepBuild-0.7.1/src/RepRepBuild.egg-info/entry_points.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)       36 2023-04-19 14:05:26.000000 RepRepBuild-0.7.1/src/RepRepBuild.egg-info/requires.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)       12 2023-04-19 14:05:26.000000 RepRepBuild-0.7.1/src/RepRepBuild.egg-info/top_level.txt
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-04-19 14:05:26.329328 RepRepBuild-0.7.1/src/reprepbuild/
+-rw-r--r--   0 toon      (1000) toon      (1000)      775 2023-03-14 11:47:22.000000 RepRepBuild-0.7.1/src/reprepbuild/__init__.py
+-rw-r--r--   0 toon      (1000) toon      (1000)    11114 2023-04-19 14:01:26.000000 RepRepBuild-0.7.1/src/reprepbuild/__main__.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1803 2023-03-25 09:41:44.000000 RepRepBuild-0.7.1/src/reprepbuild/articlezip.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     3517 2023-04-12 08:19:13.000000 RepRepBuild-0.7.1/src/reprepbuild/bibtex.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     3910 2023-03-25 09:41:50.000000 RepRepBuild-0.7.1/src/reprepbuild/latex.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     4530 2023-04-19 14:02:59.000000 RepRepBuild-0.7.1/src/reprepbuild/latexdep.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1792 2023-03-25 09:42:18.000000 RepRepBuild-0.7.1/src/reprepbuild/normalizepdf.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     4119 2023-04-19 09:59:27.000000 RepRepBuild-0.7.1/src/reprepbuild/pythonscript.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     2856 2023-03-16 20:21:01.000000 RepRepBuild-0.7.1/src/reprepbuild/repeat.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     5006 2023-03-25 09:15:24.000000 RepRepBuild-0.7.1/src/reprepbuild/utils.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     2340 2023-03-28 14:48:56.000000 RepRepBuild-0.7.1/src/reprepbuild/zip.py
```

### Comparing `RepRepBuild-0.7.0/COPYING` & `RepRepBuild-0.7.1/COPYING`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.0/PKG-INFO` & `RepRepBuild-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.7.0
+Version: 0.7.1
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `RepRepBuild-0.7.0/README.md` & `RepRepBuild-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.0/pyproject.toml` & `RepRepBuild-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "RepRepBuild"
-version = "0.7.0"
+version = "0.7.1"
 authors = [
   { name="Toon Verstraelen", email="toon.verstraelen@ugent.be" },
 ]
 description = "Build tool for Reproducible Reporting"
 readme = "README.md"
 license = {file = "COPYING"}
 requires-python = ">=3.6"
```

### Comparing `RepRepBuild-0.7.0/src/RepRepBuild.egg-info/PKG-INFO` & `RepRepBuild-0.7.1/src/RepRepBuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RepRepBuild
-Version: 0.7.0
+Version: 0.7.1
 Summary: Build tool for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `RepRepBuild-0.7.0/src/RepRepBuild.egg-info/SOURCES.txt` & `RepRepBuild-0.7.1/src/RepRepBuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.0/src/reprepbuild/__init__.py` & `RepRepBuild-0.7.1/src/reprepbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.0/src/reprepbuild/__main__.py` & `RepRepBuild-0.7.1/src/reprepbuild/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     "copy": {"command": "cp $in $out"},
     "latexdiff": {"command": f"latexdiff --append-context2cmd={LATEXDIFF_CONTEXT2CMD} $in > $out"},
     "reprozip": {"command": "rr-zip $out $in"},
     "reproarticlezip": {"command": "rr-article-zip $out $in"},
     "svgtopdf": {
         "command": "inkscape $in --export-filename=$out --export-type=pdf; rr-normalize-pdf $out"
     },
-    "pythonscript": {"command": "rr-python-script $in -- $args > $out", "depfile": "$in.d"},
+    "pythonscript": {"command": "rr-python-script $in -- $args > $out", "depfile": "$noext.d"},
 }
 
 
 def latex_pattern(path):
     """Make ninja build commands to compile latex with pdflatex."""
     result = re.match(r"latex-(?P<prefix>[a-z0-9-]+)/(?P=prefix).tex$", path)
     if not result:
@@ -224,42 +224,65 @@
             return os.path.normpath(os.path.join(workdir, fn_local))
 
         # Loop over all cases to make build records
         for script_args in build_cases:
             build_info = reprepbuild_info(*script_args)
             strargs = check_script_args(script_args)
             fn_log = fixpath(f"{prefix}{strargs}.log")
+            implicit_inputs = [fixpath(ipath) for ipath in build_info.get("inputs", [])]
+            implicit_outputs = [fixpath(opath) for opath in build_info.get("outputs", [])]
             yield {
                 "inputs": path,
-                "implicit": [fixpath(ipath) for ipath in build_info.get("inputs", [])],
+                "implicit": implicit_inputs,
                 "rule": "pythonscript",
-                "implicit_outputs": [fixpath(opath) for opath in build_info.get("outputs", [])],
+                "implicit_outputs": implicit_outputs,
                 "outputs": fn_log,
                 "variables": {
                     "args": " ".join(str(arg) for arg in script_args),
-                    "strargs": strargs,
+                    "noext": fixpath(f"{prefix}{strargs}"),
                 },
                 "default": True,
             }
     finally:
         os.chdir(orig_workdir)
 
 
+def check_tex_outputs(outputs: list[str] | str | None):
+    """Raise an error when something produces a file with extension ``.tex``
+
+    When this is the case, the function raises an error recommends ``.itex`` instead for
+    autogenerated LaTeX sources.
+    """
+    if outputs is None:
+        return
+    if isinstance(outputs, str):
+        outputs = [outputs]
+    for path_out in outputs:
+        if path_out.endswith(".tex"):
+            raise ValueError(
+                "Programatically generated LaTeX files cannot end with '.tex' because this "
+                "would not allow for a distinction with static tex files in the build process. "
+                r"For example, use '.itex' instead and update the \input commands accordingly."
+            )
+
+
 def write_ninja(patterns, rules):
     """Search through the source for patterns that can be translated into ninja build commands."""
     # Loop over all files and create rules and builds for them
     rule_names = set()
     builds = []
     defaults = []
     for path in glob("**", recursive=True):
         for pattern in patterns:
             for build in pattern(path):
                 if build.get("default", False):
                     defaults.append(build["outputs"])
                     del build["default"]
+                check_tex_outputs(build.get("outputs", None))
+                check_tex_outputs(build.get("implicit_outputs", None))
                 rule_names.add(build["rule"])
                 builds.append(build)
 
     # Sanity check
     if len(builds) == 0:
         print("Nothing to build. Wrong current directory?")
         sys.exit(-1)
```

### Comparing `RepRepBuild-0.7.0/src/reprepbuild/articlezip.py` & `RepRepBuild-0.7.1/src/reprepbuild/articlezip.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.0/src/reprepbuild/bibtex.py` & `RepRepBuild-0.7.1/src/reprepbuild/bibtex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.0/src/reprepbuild/latex.py` & `RepRepBuild-0.7.1/src/reprepbuild/latex.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.0/src/reprepbuild/latexdep.py` & `RepRepBuild-0.7.1/src/reprepbuild/latexdep.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         cwd=workdir,
         check=False,
         stdin=subprocess.DEVNULL,
         stdout=subprocess.DEVNULL,
         stderr=subprocess.DEVNULL,
     )
 
-    # Extract relevant files for log, fls and bbl files.
+    # Extract relevant files from log and fls.
     inputs = parse_inputs_fls(os.path.join(workdir, prefix + ".fls"))
     # The encoding is unpredictable, so read log as binary.
     path_log = os.path.join(workdir, prefix + ".log")
     if os.path.isfile(path_log):
         with open(path_log, "rb") as f:
             for line in f:
                 fn_missing = None
@@ -109,15 +109,16 @@
                     inputs.append(os.path.join(workdir, fn_missing.decode("utf8")))
 
     # Write the dyndep, which is the most complete
     path_pdf = os.path.join(workdir, f"{prefix}.pdf")
     path_dyndep = path_tex + ".dd"
     write_dyndep(path_dyndep, path_pdf, [], inputs)
 
-    # Write a depfile for all tex sources, in which changes may affect dependencies.
+    # Write a depfile for all static tex sources, in which changes may affect dependencies.
+    # This filter is the reason for enforcing `.itex` or other extensions for autogenerated LaTeX.
     path_dep = path_tex + ".d"
     write_dep(path_dep, [path_dyndep], [path for path in inputs if path.endswith(".tex")])
 
     # Make a copy of the aux file for bibtex.
     # This copy circumvents one of the annoying LaTeX circular dependencies.
     # Without this trick, LaTeX is incompatible with build systems,
     # because the same files serve as input and output in one build step.
```

### Comparing `RepRepBuild-0.7.0/src/reprepbuild/normalizepdf.py` & `RepRepBuild-0.7.1/src/reprepbuild/normalizepdf.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.0/src/reprepbuild/pythonscript.py` & `RepRepBuild-0.7.1/src/reprepbuild/pythonscript.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,18 +105,19 @@
             continue
         imported_paths.add(module_path)
 
     # Write the depfile.
     def fixpath(fn_local):
         return os.path.normpath(os.path.join(workdir, fn_local))
 
-    outputs = [fixpath(opath) for opath in build_info.get("outputs", [])]
+    # Note: only explicit outputs must be added to the depfile, not the implicit ones.
     strargs = check_script_args(script_args)
-    outputs.append(fixpath(f"{prefix}{strargs}.log"))
-    path_dep = path_py + ".d"
+    noext = fixpath(f"{prefix}{strargs}")
+    outputs = [(f"{noext}.log")]
+    path_dep = f"{noext}.d"
     write_dep(path_dep, outputs, imported_paths)
 
     return result
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `RepRepBuild-0.7.0/src/reprepbuild/repeat.py` & `RepRepBuild-0.7.1/src/reprepbuild/repeat.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.0/src/reprepbuild/utils.py` & `RepRepBuild-0.7.1/src/reprepbuild/utils.py`

 * *Files identical despite different names*

### Comparing `RepRepBuild-0.7.0/src/reprepbuild/zip.py` & `RepRepBuild-0.7.1/src/reprepbuild/zip.py`

 * *Files identical despite different names*


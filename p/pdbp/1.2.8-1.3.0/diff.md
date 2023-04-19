# Comparing `tmp/pdbp-1.2.8.tar.gz` & `tmp/pdbp-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbp-1.2.8.tar", last modified: Thu Jan 19 21:04:46 2023, max compression
+gzip compressed data, was "pdbp-1.3.0.tar", last modified: Wed Apr 19 04:39:09 2023, max compression
```

## Comparing `pdbp-1.2.8.tar` & `pdbp-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-01-19 21:04:46.359911 pdbp-1.2.8/
--rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 pdbp-1.2.8/.gitignore
--rwxr-xr-x   0 michael    (501) staff       (20)     1536 2022-11-28 00:30:19.000000 pdbp-1.2.8/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 michael    (501) staff       (20)     1664 2022-11-28 00:28:34.000000 pdbp-1.2.8/CONTRIBUTING.md
--rw-r--r--   0 michael    (501) staff       (20)     1066 2022-11-28 00:19:16.000000 pdbp-1.2.8/LICENSE
--rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 pdbp-1.2.8/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     6210 2023-01-19 21:04:46.359959 pdbp-1.2.8/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     4090 2022-12-16 16:48:06.000000 pdbp-1.2.8/README.md
--rwxr-xr-x   0 michael    (501) staff       (20)      303 2022-11-28 07:12:13.000000 pdbp-1.2.8/SECURITY.md
--rwxr-xr-x   0 michael    (501) staff       (20)      117 2023-01-19 21:04:46.360123 pdbp-1.2.8/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     5309 2023-01-19 21:04:02.000000 pdbp-1.2.8/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-01-19 21:04:46.359231 pdbp-1.2.8/src/
--rwxr-xr-x   0 michael    (501) staff       (20)       39 2022-11-28 05:30:45.000000 pdbp-1.2.8/src/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-01-19 21:04:46.359820 pdbp-1.2.8/src/pdbp.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     6210 2023-01-19 21:04:46.000000 pdbp-1.2.8/src/pdbp.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      293 2023-01-19 21:04:46.000000 pdbp-1.2.8/src/pdbp.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-01-19 21:04:46.000000 pdbp-1.2.8/src/pdbp.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)      120 2023-01-19 21:04:46.000000 pdbp-1.2.8/src/pdbp.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        5 2023-01-19 21:04:46.000000 pdbp-1.2.8/src/pdbp.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)    45825 2023-01-19 21:04:02.000000 pdbp-1.2.8/src/pdbp.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 04:39:09.717706 pdbp-1.3.0/
+-rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 pdbp-1.3.0/.gitignore
+-rwxr-xr-x   0 michael    (501) staff       (20)     1536 2022-11-28 00:30:19.000000 pdbp-1.3.0/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 michael    (501) staff       (20)     1664 2022-11-28 00:28:34.000000 pdbp-1.3.0/CONTRIBUTING.md
+-rw-r--r--   0 michael    (501) staff       (20)     1066 2022-11-28 00:19:16.000000 pdbp-1.3.0/LICENSE
+-rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 pdbp-1.3.0/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)     6454 2023-04-19 04:39:09.717765 pdbp-1.3.0/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     4438 2023-04-19 04:33:33.000000 pdbp-1.3.0/README.md
+-rwxr-xr-x   0 michael    (501) staff       (20)      303 2022-11-28 07:12:13.000000 pdbp-1.3.0/SECURITY.md
+-rwxr-xr-x   0 michael    (501) staff       (20)       88 2023-04-19 04:39:09.717948 pdbp-1.3.0/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     5324 2023-04-19 04:33:33.000000 pdbp-1.3.0/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 04:39:09.716884 pdbp-1.3.0/src/
+-rwxr-xr-x   0 michael    (501) staff       (20)       39 2022-11-28 05:30:45.000000 pdbp-1.3.0/src/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 04:39:09.717606 pdbp-1.3.0/src/pdbp.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     6454 2023-04-19 04:39:09.000000 pdbp-1.3.0/src/pdbp.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      293 2023-04-19 04:39:09.000000 pdbp-1.3.0/src/pdbp.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-19 04:39:09.000000 pdbp-1.3.0/src/pdbp.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)      121 2023-04-19 04:39:09.000000 pdbp-1.3.0/src/pdbp.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        5 2023-04-19 04:39:09.000000 pdbp-1.3.0/src/pdbp.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)    52503 2023-04-19 04:33:33.000000 pdbp-1.3.0/src/pdbp.py
```

### Comparing `pdbp-1.2.8/.gitignore` & `pdbp-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pdbp-1.2.8/CODE_OF_CONDUCT.md` & `pdbp-1.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pdbp-1.2.8/CONTRIBUTING.md` & `pdbp-1.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pdbp-1.2.8/LICENSE` & `pdbp-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdbp-1.2.8/PKG-INFO` & `pdbp-1.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbp
-Version: 1.2.8
+Version: 1.3.0
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -23,15 +23,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -39,31 +38,31 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207774790-fb63af65-5f98-4d92-afe3-12c2733d4db6.png">
+<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207774790-fb63af65-5f98-4d92-afe3-12c2733d4db6.png">
 
 --------
 
 **[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
 --------
 
-<img width="600" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/204408641-9c221bb6-578b-4b0f-807b-8454844e42e8.png">
+<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/232536483-9236c513-c5ba-4444-8faa-e8ea64eb5ce2.png">
 
 
 ## Installation & Usage:
 
 ```bash
 pip install pdbp
 ```
@@ -80,14 +79,16 @@
 import pdbp  # noqa
 ```
 
 To trigger a breakpoint in your code with ``pytest``, add ``--trace`` (to start tests with a breakpoint) or ``--pdb`` (to trigger a breakpoint if a test fails).
 
 Basic **``Pdb+``** console commands: ``n``, ``c``, ``s`` => ``next``, ``continue``, ``step``.
 
+Use the ``u`` and ``d`` keys to travel ``up`` and ``down`` the stack!
+
 (To learn more **Pdb+** console commands, type ``help`` in the **Pdb+** console and press ``Enter/Return``.)
 
 --------
 
 **``pdbp`` (Pdb+)** makes improvements to ``pdbpp`` so that it works in all environments. It also includes other bug-fixes. "Sticky" mode is the default option, which shows multiple lines of code while letting you see where you're going (while typing ``n`` + ``Enter``).
 
 If you somehow reset ``pdb`` to Python's built-in version, you can always replace ``pdb`` with **``pdbp``** again as the default debugger by running this:
@@ -119,41 +120,47 @@
 import pdbp
 pdbp.set_trace()
 ```
 
 
 ### pdbp (Pdb+) commands:
 
-<img width="550" alt="Pdb+ Commands" src="https://user-images.githubusercontent.com/6788579/204386211-5fc44f73-e29f-4e87-b0ca-bb8ea69217af.png">
+<img width="760" alt="Pdb+ commands" src="https://user-images.githubusercontent.com/6788579/232948402-8700033f-a1b2-45f6-82e5-6b1a83d3d6c4.png">
+
+
+### Post Mortem Debug Mode:
+
+<img width="640" alt="Pdb+ Post Mortem Debug Mode" src="https://user-images.githubusercontent.com/6788579/232537816-0b9e9048-724f-48cb-81e3-5cc403109de9.png">
+
+
+### The ``where`` / ``w`` command, which displays the current stack:
+
+<img width="870" alt="Example of the 'where' command" src="https://user-images.githubusercontent.com/6788579/232962807-2d469603-a1d0-4891-8d0e-f03a4e1d0d00.png">
 
 
 ### Sticky Mode vs Non-Sticky Mode:
 
 The default mode (``sticky``) lets you see a lot more lines of code from the debugger when active. In Non-Sticky mode, only one line of code is shown at a time. You can switch between the two modes by typing ``sticky`` in the **Pdb+** console prompt and pressing ``Enter/Return``.
 
 > **Sticky Mode:**
 
-<img width="550" alt="Pdb+ Stick Mode" src="https://user-images.githubusercontent.com/6788579/204890148-53d2567b-9a56-4243-a7d7-66100a284312.png">
+<img width="600" alt="Pdb+ Stick Mode" src="https://user-images.githubusercontent.com/6788579/204890148-53d2567b-9a56-4243-a7d7-66100a284312.png">
 
 > **Non-Sticky Mode:**
 
-<img width="550" alt="Pdb+ Non-Sticky Mode" src="https://user-images.githubusercontent.com/6788579/204890164-8465bc22-0f20-43f1-8ab7-b4316718a4c6.png">
+<img width="600" alt="Pdb+ Non-Sticky Mode" src="https://user-images.githubusercontent.com/6788579/204890164-8465bc22-0f20-43f1-8ab7-b4316718a4c6.png">
 
 
 ### More examples:
 
 **``Pdb+``** is used by packages such as **``seleniumbase``**:
 
 * https://pypi.org/project/seleniumbase/
 * https://github.com/seleniumbase/SeleniumBase
 
 --------
 
-<img width="550" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/204896775-38d8551b-1d3c-4e95-9f5c-0e03c9de13da.png">
-
---------
-
-<img width="550" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/204359676-137cf541-12ef-469a-9d29-99709608ede0.png">
+<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/204896775-38d8551b-1d3c-4e95-9f5c-0e03c9de13da.png">
 
 --------
 
 (**Pdb+** is maintained by the [SeleniumBase Dev Team](https://github.com/seleniumbase/SeleniumBase))
```

### Comparing `pdbp-1.2.8/README.md` & `pdbp-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207774790-fb63af65-5f98-4d92-afe3-12c2733d4db6.png">
+<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207774790-fb63af65-5f98-4d92-afe3-12c2733d4db6.png">
 
 --------
 
 **[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
 --------
 
-<img width="600" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/204408641-9c221bb6-578b-4b0f-807b-8454844e42e8.png">
+<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/232536483-9236c513-c5ba-4444-8faa-e8ea64eb5ce2.png">
 
 
 ## Installation & Usage:
 
 ```bash
 pip install pdbp
 ```
@@ -31,14 +31,16 @@
 import pdbp  # noqa
 ```
 
 To trigger a breakpoint in your code with ``pytest``, add ``--trace`` (to start tests with a breakpoint) or ``--pdb`` (to trigger a breakpoint if a test fails).
 
 Basic **``Pdb+``** console commands: ``n``, ``c``, ``s`` => ``next``, ``continue``, ``step``.
 
+Use the ``u`` and ``d`` keys to travel ``up`` and ``down`` the stack!
+
 (To learn more **Pdb+** console commands, type ``help`` in the **Pdb+** console and press ``Enter/Return``.)
 
 --------
 
 **``pdbp`` (Pdb+)** makes improvements to ``pdbpp`` so that it works in all environments. It also includes other bug-fixes. "Sticky" mode is the default option, which shows multiple lines of code while letting you see where you're going (while typing ``n`` + ``Enter``).
 
 If you somehow reset ``pdb`` to Python's built-in version, you can always replace ``pdb`` with **``pdbp``** again as the default debugger by running this:
@@ -70,41 +72,47 @@
 import pdbp
 pdbp.set_trace()
 ```
 
 
 ### pdbp (Pdb+) commands:
 
-<img width="550" alt="Pdb+ Commands" src="https://user-images.githubusercontent.com/6788579/204386211-5fc44f73-e29f-4e87-b0ca-bb8ea69217af.png">
+<img width="760" alt="Pdb+ commands" src="https://user-images.githubusercontent.com/6788579/232948402-8700033f-a1b2-45f6-82e5-6b1a83d3d6c4.png">
+
+
+### Post Mortem Debug Mode:
+
+<img width="640" alt="Pdb+ Post Mortem Debug Mode" src="https://user-images.githubusercontent.com/6788579/232537816-0b9e9048-724f-48cb-81e3-5cc403109de9.png">
+
+
+### The ``where`` / ``w`` command, which displays the current stack:
+
+<img width="870" alt="Example of the 'where' command" src="https://user-images.githubusercontent.com/6788579/232962807-2d469603-a1d0-4891-8d0e-f03a4e1d0d00.png">
 
 
 ### Sticky Mode vs Non-Sticky Mode:
 
 The default mode (``sticky``) lets you see a lot more lines of code from the debugger when active. In Non-Sticky mode, only one line of code is shown at a time. You can switch between the two modes by typing ``sticky`` in the **Pdb+** console prompt and pressing ``Enter/Return``.
 
 > **Sticky Mode:**
 
-<img width="550" alt="Pdb+ Stick Mode" src="https://user-images.githubusercontent.com/6788579/204890148-53d2567b-9a56-4243-a7d7-66100a284312.png">
+<img width="600" alt="Pdb+ Stick Mode" src="https://user-images.githubusercontent.com/6788579/204890148-53d2567b-9a56-4243-a7d7-66100a284312.png">
 
 > **Non-Sticky Mode:**
 
-<img width="550" alt="Pdb+ Non-Sticky Mode" src="https://user-images.githubusercontent.com/6788579/204890164-8465bc22-0f20-43f1-8ab7-b4316718a4c6.png">
+<img width="600" alt="Pdb+ Non-Sticky Mode" src="https://user-images.githubusercontent.com/6788579/204890164-8465bc22-0f20-43f1-8ab7-b4316718a4c6.png">
 
 
 ### More examples:
 
 **``Pdb+``** is used by packages such as **``seleniumbase``**:
 
 * https://pypi.org/project/seleniumbase/
 * https://github.com/seleniumbase/SeleniumBase
 
 --------
 
-<img width="550" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/204896775-38d8551b-1d3c-4e95-9f5c-0e03c9de13da.png">
-
---------
-
-<img width="550" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/204359676-137cf541-12ef-469a-9d29-99709608ede0.png">
+<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/204896775-38d8551b-1d3c-4e95-9f5c-0e03c9de13da.png">
 
 --------
 
 (**Pdb+** is maintained by the [SeleniumBase Dev Team](https://github.com/seleniumbase/SeleniumBase))
```

### Comparing `pdbp-1.2.8/setup.py` & `pdbp-1.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """*** pdbp (Pdb+) ***
 An advanced console debugger for Python.
 Can be used as a drop-in replacement for pdb and pdbpp.
-(Python 2.7+ and Python 3.6+)"""
+(Python 3.6+)"""
 from setuptools import setup, find_packages  # noqa
 import os
 import sys
 
 
 this_dir = os.path.abspath(os.path.dirname(__file__))
 long_description = None
@@ -42,14 +42,16 @@
         else:
             print("*** No flake8 issues detected. Continuing...")
         print("\n*** Removing existing distribution packages: ***\n")
         os.system("rm -f dist/*.egg; rm -f dist/*.tar.gz; rm -f dist/*.whl")
         os.system("rm -rf build/bdist.*; rm -rf build/lib")
         print("\n*** Installing build: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade 'build>=0.10.0'")
+        print("\n*** Installing pkginfo: *** (Required for PyPI uploads)\n")
+        os.system("python -m pip install --upgrade 'pkginfo>=1.9.6'")
         print("\n*** Installing twine: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade 'twine>=4.0.2'")
         print("\n*** Installing tqdm: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade tqdm")
         print("\n*** Rebuilding distribution packages: ***\n")
         os.system("python -m build")  # Create new tar/wheel
         print("\n*** Publishing The Release to PyPI: ***\n")
@@ -57,15 +59,15 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name="pdbp",
-    version="1.2.8",
+    version="1.3.0",
     description="pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="pdb debugger tab color completion",
     url="https://github.com/mdmintz/pdbp",
     project_urls={
         "Changelog": "https://github.com/mdmintz/pdbp/releases",
@@ -89,15 +91,14 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
@@ -106,19 +107,19 @@
         "Topic :: Software Development",
         "Topic :: Software Development :: Debuggers",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Quality Assurance",
         "Topic :: Software Development :: Testing",
         "Topic :: Utilities",
     ],
-    python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*",  # noqa: E501
+    python_requires=">=3.6",
     install_requires=[
-        'pygments>=2.5.2;python_version<"3.6"',
-        'pygments>=2.14.0;python_version>="3.6"',
-        "tabcompleter>=1.1.0",
+        'pygments>=2.14.0;python_version<"3.7"',
+        'pygments>=2.15.1;python_version>="3.7"',
+        "tabcompleter>=1.2.0",
         "six>=1.16.0",
     ],
     setup_requires=[],
     include_package_data=True,
 )
 
 print("\n*** pdbp (Pdb+) Installation Complete! ***\n")
```

### Comparing `pdbp-1.2.8/src/pdbp.egg-info/PKG-INFO` & `pdbp-1.3.0/src/pdbp.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbp
-Version: 1.2.8
+Version: 1.3.0
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -23,15 +23,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -39,31 +38,31 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207774790-fb63af65-5f98-4d92-afe3-12c2733d4db6.png">
+<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207774790-fb63af65-5f98-4d92-afe3-12c2733d4db6.png">
 
 --------
 
 **[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
 --------
 
-<img width="600" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/204408641-9c221bb6-578b-4b0f-807b-8454844e42e8.png">
+<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/232536483-9236c513-c5ba-4444-8faa-e8ea64eb5ce2.png">
 
 
 ## Installation & Usage:
 
 ```bash
 pip install pdbp
 ```
@@ -80,14 +79,16 @@
 import pdbp  # noqa
 ```
 
 To trigger a breakpoint in your code with ``pytest``, add ``--trace`` (to start tests with a breakpoint) or ``--pdb`` (to trigger a breakpoint if a test fails).
 
 Basic **``Pdb+``** console commands: ``n``, ``c``, ``s`` => ``next``, ``continue``, ``step``.
 
+Use the ``u`` and ``d`` keys to travel ``up`` and ``down`` the stack!
+
 (To learn more **Pdb+** console commands, type ``help`` in the **Pdb+** console and press ``Enter/Return``.)
 
 --------
 
 **``pdbp`` (Pdb+)** makes improvements to ``pdbpp`` so that it works in all environments. It also includes other bug-fixes. "Sticky" mode is the default option, which shows multiple lines of code while letting you see where you're going (while typing ``n`` + ``Enter``).
 
 If you somehow reset ``pdb`` to Python's built-in version, you can always replace ``pdb`` with **``pdbp``** again as the default debugger by running this:
@@ -119,41 +120,47 @@
 import pdbp
 pdbp.set_trace()
 ```
 
 
 ### pdbp (Pdb+) commands:
 
-<img width="550" alt="Pdb+ Commands" src="https://user-images.githubusercontent.com/6788579/204386211-5fc44f73-e29f-4e87-b0ca-bb8ea69217af.png">
+<img width="760" alt="Pdb+ commands" src="https://user-images.githubusercontent.com/6788579/232948402-8700033f-a1b2-45f6-82e5-6b1a83d3d6c4.png">
+
+
+### Post Mortem Debug Mode:
+
+<img width="640" alt="Pdb+ Post Mortem Debug Mode" src="https://user-images.githubusercontent.com/6788579/232537816-0b9e9048-724f-48cb-81e3-5cc403109de9.png">
+
+
+### The ``where`` / ``w`` command, which displays the current stack:
+
+<img width="870" alt="Example of the 'where' command" src="https://user-images.githubusercontent.com/6788579/232962807-2d469603-a1d0-4891-8d0e-f03a4e1d0d00.png">
 
 
 ### Sticky Mode vs Non-Sticky Mode:
 
 The default mode (``sticky``) lets you see a lot more lines of code from the debugger when active. In Non-Sticky mode, only one line of code is shown at a time. You can switch between the two modes by typing ``sticky`` in the **Pdb+** console prompt and pressing ``Enter/Return``.
 
 > **Sticky Mode:**
 
-<img width="550" alt="Pdb+ Stick Mode" src="https://user-images.githubusercontent.com/6788579/204890148-53d2567b-9a56-4243-a7d7-66100a284312.png">
+<img width="600" alt="Pdb+ Stick Mode" src="https://user-images.githubusercontent.com/6788579/204890148-53d2567b-9a56-4243-a7d7-66100a284312.png">
 
 > **Non-Sticky Mode:**
 
-<img width="550" alt="Pdb+ Non-Sticky Mode" src="https://user-images.githubusercontent.com/6788579/204890164-8465bc22-0f20-43f1-8ab7-b4316718a4c6.png">
+<img width="600" alt="Pdb+ Non-Sticky Mode" src="https://user-images.githubusercontent.com/6788579/204890164-8465bc22-0f20-43f1-8ab7-b4316718a4c6.png">
 
 
 ### More examples:
 
 **``Pdb+``** is used by packages such as **``seleniumbase``**:
 
 * https://pypi.org/project/seleniumbase/
 * https://github.com/seleniumbase/SeleniumBase
 
 --------
 
-<img width="550" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/204896775-38d8551b-1d3c-4e95-9f5c-0e03c9de13da.png">
-
---------
-
-<img width="550" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/204359676-137cf541-12ef-469a-9d29-99709608ede0.png">
+<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/204896775-38d8551b-1d3c-4e95-9f5c-0e03c9de13da.png">
 
 --------
 
 (**Pdb+** is maintained by the [SeleniumBase Dev Team](https://github.com/seleniumbase/SeleniumBase))
```

### Comparing `pdbp-1.2.8/src/pdbp.py` & `pdbp-1.3.0/src/pdbp.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,42 +6,30 @@
 import code
 import codecs
 import inspect
 import os.path
 import pprint
 import re
 import signal
-import subprocess
 import sys
 import traceback
 import types
 from collections import OrderedDict
+from inspect import signature
+from io import StringIO
 from tabcompleter import Completer, ConfigurableClass, Color
 import tabcompleter
 
 __url__ = "https://github.com/mdmintz/pdbp"
 __version__ = tabcompleter.LazyVersion("pdbp")
-
-try:
-    from inspect import signature  # Python >= 3.3
-except ImportError:
-    try:
-        from funcsigs import signature
-    except ImportError:
-        def signature(obj):
-            return " [pip install funcsigs to show the signature]"
+run_from_main = False
 
 # Digits, Letters, [], or Dots
 side_effects_free = re.compile(r"^ *[_0-9a-zA-Z\[\].]* *$")
 
-if sys.version_info < (3, ):
-    from io import BytesIO as StringIO
-else:
-    from io import StringIO
-
 
 def import_from_stdlib(name):
     result = types.ModuleType(name)
     stdlibdir, _ = os.path.split(code.__file__)
     pyfile = os.path.join(stdlibdir, name + ".py")
     with open(pyfile) as f:
         src = f.read()
@@ -57,16 +45,14 @@
     newfunc = types.FunctionType(func.__code__, newglobals, func.__name__,
                                  func.__defaults__, func.__closure__)
     return newfunc
 
 
 def is_char_wide(char):
     # Returns True if the char is Chinese, Japanese, Korean, or another double.
-    if sys.version_info < (3, ):
-        return False  # Python 2.7 can't handle that
     special_c_r = [
         {"from": ord("\u4e00"), "to": ord("\u9FFF")},
         {"from": ord("\u3040"), "to": ord("\u30ff")},
         {"from": ord("\uac00"), "to": ord("\ud7a3")},
         {"from": ord("\uff01"), "to": ord("\uff60")},
     ]
     sc = any(
@@ -173,14 +159,18 @@
     linestarts.reverse()
     for i, lineno in linestarts:
         if lasti >= i:
             return lineno
     return 0
 
 
+class Restart(Exception):
+    pass
+
+
 class Undefined:
     def __repr__(self):
         return "<undefined>"
 
 
 undefined = Undefined()
 
@@ -195,27 +185,69 @@
         self.start_filename = kwds.pop("start_filename", None)
         self.config = self.get_config(self.ConfigFactory)
         self.config.setup(self)
         if self.config.disable_pytest_capturing:
             self._disable_pytest_capture_maybe()
         kwargs = self.config.default_pdb_kwargs.copy()
         kwargs.update(**kwds)
-        super(Pdb, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.prompt = self.config.prompt
         self.display_list = {}  # frame --> (name --> last seen value)
         self.sticky = self.config.sticky_by_default
         self.first_time_sticky = self.sticky
         self.ok_to_clear = False
         self.has_traceback = False
         self.sticky_ranges = {}  # frame --> (start, end)
         self.tb_lineno = {}  # frame --> lineno where the exception was raised
         self.history = []
         self.show_hidden_frames = False
         self._hidden_frames = []
         self.stdout = self.ensure_file_can_write_unicode(self.stdout)
+        self.saved_curframe = None
+        self.last_cmd = None
+
+    def _runmodule(self, module_name):
+        import __main__
+        import runpy
+        self._wait_for_mainpyfile = True
+        self._user_requested_quit = False
+        mod_name, mod_spec, code = runpy._get_module_details(module_name)
+        self.mainpyfile = self.canonic(code.co_filename)
+        __main__.__dict__.clear()
+        __main__.__dict__.update(
+            {
+                "__name__": "__main__",
+                "__file__": self.mainpyfile,
+                "__package__": mod_spec.parent,
+                "__loader__": mod_spec.loader,
+                "__spec__": mod_spec,
+                "__builtins__": __builtins__,
+            }
+        )
+        self.run(code)
+
+    def _runscript(self, filename):
+        import __main__
+        import io
+        __main__.__dict__.clear()
+        __main__.__dict__.update(
+            {
+                "__name__": "__main__",
+                "__file__": filename,
+                "__builtins__": __builtins__,
+            }
+        )
+        self._wait_for_mainpyfile = True
+        self.mainpyfile = self.canonic(filename)
+        self._user_requested_quit = False
+        with io.open_code(filename) as fp:
+            statement = (
+                "exec(compile(%r, %r, 'exec'))" % (fp.read(), self.mainpyfile)
+            )
+        self.run(statement)
 
     def ensure_file_can_write_unicode(self, f):
         # Wrap with an encoder, but only if not already wrapped.
         if (not hasattr(f, "stream")
                 and getattr(f, "encoding", False)
                 and f.encoding.lower() != "utf-8"):
             f = codecs.getwriter("utf-8")(getattr(f, "buffer", f))
@@ -293,15 +325,15 @@
             print(
                 '   %d frame%s hidden (Use "u" and "d" to travel)'
                 % (n, plural),
                 file=self.stdout,
             )
 
     def setup(self, frame, tb):
-        ret = super(Pdb, self).setup(frame, tb)
+        ret = super().setup(frame, tb)
         if not ret:
             while tb:
                 lineno = lasti2lineno(tb.tb_frame.f_code, tb.tb_lasti)
                 self.tb_lineno[tb.tb_frame] = lineno
                 tb = tb.tb_next
         return ret
 
@@ -321,15 +353,15 @@
             frame.f_locals.get("__tracebackhide__")
             or frame.f_globals.get("__tracebackhide__")
         ):
             return True
 
     def get_stack(self, f, t):
         # Show all the frames except ones that should be hidden.
-        fullstack, idx = super(Pdb, self).get_stack(f, t)
+        fullstack, idx = super().get_stack(f, t)
         self.fullstack = fullstack
         return self.compute_stack(fullstack, idx)
 
     def compute_stack(self, fullstack, idx=None):
         if idx is None:
             idx = len(fullstack) - 1
         if self.show_hidden_frames:
@@ -355,15 +387,15 @@
             self.curindex = len(self.stack) - 1
             self.curframe = self.stack[-1][0]
             self.print_current_stack_entry()
 
     def forget(self):
         if not hasattr(self, "lineno"):
             # Only forget if not used with recursive set_trace.
-            super(Pdb, self).forget()
+            super().forget()
         self.raise_lineno = {}
 
     @classmethod
     def _get_all_completions(cls, complete, text):
         r = []
         i = 0
         while True:
@@ -381,15 +413,15 @@
                 GLOBAL_PDB._pdbp_completing = True
             mydict = self.curframe.f_globals.copy()
             mydict.update(self.curframe.f_locals)
             completer = Completer(mydict)
             self._completions = self._get_all_completions(
                 completer.complete, text
             )
-            real_pdb = super(Pdb, self)
+            real_pdb = super()
             for x in self._get_all_completions(real_pdb.complete, text):
                 if x not in self._completions:
                     self._completions.append(x)
             if GLOBAL_PDB:
                 del GLOBAL_PDB._pdbp_completing
             # Remove "\t" from tabcompleter if there are pdb completions.
             if len(self._completions) > 1 and self._completions[0] == "\t":
@@ -423,15 +455,15 @@
                                   colorscheme=self.config.colorscheme)
         self._lexer = PythonLexer()
         return True
 
     stack_entry_regexp = re.compile(r"(.*?)\(([0-9]+?)\)(.*)", re.DOTALL)
 
     def format_stack_entry(self, frame_lineno, lprefix=": "):
-        entry = super(Pdb, self).format_stack_entry(frame_lineno, lprefix)
+        entry = super().format_stack_entry(frame_lineno, lprefix)
         entry = self.try_to_decode(entry)
         if self.config.highlight:
             match = self.stack_entry_regexp.match(entry)
             if match:
                 filename, lineno, other = match.groups()
                 filename = Color.set(self.config.filename_color, filename)
                 lineno = Color.set(self.config.line_number_color, lineno)
@@ -465,16 +497,16 @@
             if self.config.exc_line_color:
                 line = setbgcolor(line, self.config.exc_line_color)
         return line
 
     def parseline(self, line):
         if line.startswith("!!"):
             line = line[2:]
-            return super(Pdb, self).parseline(line)
-        cmd, arg, newline = super(Pdb, self).parseline(line)
+            return super().parseline(line)
+        cmd, arg, newline = super().parseline(line)
         if arg and arg.endswith("?"):
             if hasattr(self, "do_" + cmd):
                 cmd, arg = ("help", cmd)
             elif arg.endswith("??"):
                 arg = cmd + arg.split("?")[0]
                 cmd = "source"
                 self.do_inspect(arg)
@@ -484,49 +516,65 @@
                 cmd = "inspect"
                 return cmd, arg, newline
         if (
             cmd == "f"
             and len(newline) > 1
             and (newline[1] == "'" or newline[1] == '"')
         ):
-            return super(Pdb, self).parseline("!" + line)
+            return super().parseline("!" + line)
 
         if (
             cmd
             and hasattr(self, "do_" + cmd)
             and (
                 cmd in self.curframe.f_globals
                 or cmd in self.curframe.f_locals
                 or arg.startswith("=")
             )
         ):
-            return super(Pdb, self).parseline("!" + line)
+            return super().parseline("!" + line)
 
         if cmd == "list" and arg.startswith("("):
             line = "!" + line
-            return super(Pdb, self).parseline(line)
+            return super().parseline(line)
 
         return cmd, arg, newline
 
     def do_inspect(self, arg):
-        obj = self._getval(arg)
+        if not arg:
+            print('Inspect Usage: "inspect <VAR>"', file=self.stdout)
+            print(
+                "Local variables: %r" % self.curframe_locals.keys(),
+                file=self.stdout,
+            )
+            return
+        try:
+            obj = self._getval(arg)
+        except Exception:
+            print(
+                'See "locals()" or "globals()" for available args!',
+                file=self.stdout,
+            )
+            return
         data = OrderedDict()
         data["Type"] = type(obj).__name__
         data["String Form"] = str(obj).strip()
         try:
             data["Length"] = len(obj)
         except TypeError:
             pass
         try:
             data["File"] = inspect.getabsfile(obj)
         except TypeError:
             pass
-        if (isinstance(obj, type)
-                and hasattr(obj, "__init__")
-                and getattr(obj, "__module__") != "__builtin__"):
+        if (
+            isinstance(obj, type)
+            and hasattr(obj, "__init__")
+            and getattr(obj, "__module__") != "__builtin__"
+        ):
             data["Docstring"] = obj.__doc__
             data["Constructor information"] = ""
             try:
                 data[" Definition"] = "%s%s" % (arg, signature(obj))
             except ValueError:
                 pass
             data[" Docstring"] = obj.__init__.__doc__
@@ -538,43 +586,49 @@
             data["Docstring"] = obj.__doc__
         for key, value in data.items():
             formatted_key = Color.set(Color.red, key + ":")
             self.stdout.write("%-28s %s\n" % (formatted_key, value))
 
     def default(self, line):
         self.history.append(line)
-        return super(Pdb, self).default(line)
+        return super().default(line)
 
     def do_help(self, arg):
         try:
-            return super(Pdb, self).do_help(arg)
+            return super().do_help(arg)
         except AttributeError:
             print("*** No help for '{command}'".format(command=arg),
                   file=self.stdout)
     do_help.__doc__ = pdb.Pdb.do_help.__doc__
 
     def help_hidden_frames(self):
-        print('Use "u" and "d" to travel through the stack.', file=self.stdout)
-
-    def do_hf_unhide(self, arg):
-        self.show_hidden_frames = True
-        self.refresh_stack()
-
-    def do_hf_hide(self, arg):
-        self.show_hidden_frames = False
-        self.refresh_stack()
-
-    def do_hf_list(self, arg):
-        for frame_lineno in self._hidden_frames:
-            print(self.format_stack_entry(frame_lineno, pdb.line_prefix),
-                  file=self.stdout)
+        print('Use "u" and "d" to travel up/down the stack.', file=self.stdout)
 
     def do_longlist(self, arg):
-        self.lastcmd = "longlist"
-        self._printlonglist()
+        self.last_cmd = self.lastcmd = "longlist"
+        self.sticky = True
+        self._print_if_sticky()
+    do_ll = do_longlist
+
+    def do_jump(self, arg):
+        self.last_cmd = self.lastcmd = "jump"
+        if self.curindex + 1 != len(self.stack):
+            self.error("You can only jump within the bottom frame!")
+            return
+        try:
+            arg = int(arg)
+        except ValueError:
+            self.error("The 'jump' command requires a line number!")
+        else:
+            try:
+                self.curframe.f_lineno = arg
+                self.stack[self.curindex] = self.stack[self.curindex][0], arg
+                self.print_current_stack_entry()
+            except ValueError as e:
+                self.error('Jump failed: %s' % e)
 
     def _printlonglist(self, linerange=None, fnln=None):
         try:
             if self.curframe.f_code.co_name == "<module>":
                 lines, _ = inspect.findsource(self.curframe)
                 lineno = 1
             else:
@@ -584,16 +638,23 @@
                     print(file=self.stdout)
                     self.sticky = False
                     self.print_stack_entry(self.stack[self.curindex])
                     self.sticky = True
                     print(file=self.stdout, end="\n\033[F")
                     return
         except IOError as e:
-            print("** Error: %s **" % e, file=self.stdout)
-            return
+            try:
+                self.sticky = False
+                self.print_stack_entry(self.stack[self.curindex])
+                self.sticky = True
+                return
+            except Exception:
+                self.sticky = True
+                print("** (%s) **" % e, file=self.stdout)
+                return
         if linerange:
             start, end = linerange
             start = max(start, lineno)
             end = min(end, lineno + len(lines))
             lines = lines[start - lineno:end - lineno]
             lineno = start
         self._print_lines_pdbp(lines, lineno, fnln=fnln)
@@ -670,77 +731,162 @@
             if int(lineno) > 1:
                 num_color = self.config.line_number_color
                 print(Color.set(num_color, dots), file=self.stdout)
             else:
                 print(file=self.stdout)
         print("\n".join(lines), file=self.stdout, end="\n\n\033[F")
 
-    do_ll = do_longlist
-
     def do_list(self, arg):
+        try:
+            import linecache
+            y = 0
+            if run_from_main:
+                y = 6
+            filename = self.curframe.f_code.co_filename
+            lines = linecache.getlines(filename, self.curframe.f_globals)
+            if (
+                not arg
+                and (
+                    (self.last_cmd == "list" and self.lineno >= len(lines) + y)
+                    or self.last_cmd != "list"
+                    or (
+                        self.saved_curframe != self.curframe
+                        or self.lineno < self.curframe.f_lineno
+                    )
+                )
+            ):
+                arg = "."  # Go back to the active cursor point
+        except Exception:
+            pass
+        self.last_cmd = self.lastcmd = "list"
+        self.saved_curframe = self.curframe
         oldstdout = self.stdout
         self.stdout = StringIO()
-        super(Pdb, self).do_list(arg)
+        super().do_list(arg)
         src = self.format_source(self.stdout.getvalue())
         self.stdout = oldstdout
-        print(src, file=self.stdout, end="")
+        print(src, file=self.stdout, end="\n\033[F")
 
     do_list.__doc__ = pdb.Pdb.do_list.__doc__
     do_l = do_list
 
     def do_continue(self, arg):
+        self.last_cmd = self.lastcmd = "continue"
         if arg != "":
             self.do_tbreak(arg)
-        return super(Pdb, self).do_continue("")
+        return super().do_continue(arg)
     do_continue.__doc__ = pdb.Pdb.do_continue.__doc__
     do_c = do_cont = do_continue
 
+    def do_next(self, arg):
+        self.last_cmd = self.lastcmd = "next"
+        return super().do_next(arg)
+    do_next.__doc__ = pdb.Pdb.do_next.__doc__
+    do_n = do_next
+
+    def do_step(self, arg):
+        self.last_cmd = self.lastcmd = "step"
+        return super().do_step(arg)
+    do_step.__doc__ = pdb.Pdb.do_step.__doc__
+    do_s = do_step
+
+    def do_until(self, arg):
+        self.last_cmd = self.lastcmd = "until"
+        return super().do_until(arg)
+    do_until.__doc__ = pdb.Pdb.do_until.__doc__
+    do_unt = do_until
+
+    def do_p(self, arg):
+        try:
+            self.message(repr(self._getval(arg)))
+        except Exception:
+            if not arg:
+                print('Print usage: "p <VAR>"', file=self.stdout)
+                print(
+                    "Local variables: %r" % self.curframe_locals.keys(),
+                    file=self.stdout,
+                )
+                return
+            else:
+                print(
+                    'See "locals()" or "globals()" for available args!',
+                    file=self.stdout,
+                )
+                return
+    do_p.__doc__ = pdb.Pdb.do_p.__doc__
+
     def do_pp(self, arg):
-        width, height = self.get_terminal_size()
+        width, _ = self.get_terminal_size()
         try:
             pprint.pprint(self._getval(arg), self.stdout, width=width)
         except Exception:
-            pass
+            if not arg:
+                print('PrettyPrint usage: "pp <VAR>"', file=self.stdout)
+                print(
+                    "Local variables: %r" % self.curframe_locals.keys(),
+                    file=self.stdout,
+                )
+                return
+            else:
+                print(
+                    'See "locals()" or "globals()" for available args!',
+                    file=self.stdout,
+                )
+                return
     do_pp.__doc__ = pdb.Pdb.do_pp.__doc__
 
     def do_debug(self, arg):
+        self.last_cmd = self.lastcmd = "debug"
         Config = self.ConfigFactory
 
         class PdbpWithConfig(self.__class__):
             def __init__(self_withcfg, *args, **kwargs):
                 kwargs.setdefault("Config", Config)
                 super(PdbpWithConfig, self_withcfg).__init__(*args, **kwargs)
                 self_withcfg.use_rawinput = self.use_rawinput
-        if sys.version_info < (3, ):
-            do_debug_func = pdb.Pdb.do_debug.im_func
-        else:
-            do_debug_func = pdb.Pdb.do_debug
+        do_debug_func = pdb.Pdb.do_debug
         newglobals = do_debug_func.__globals__.copy()
         newglobals["Pdb"] = PdbpWithConfig
         orig_do_debug = rebind_globals(do_debug_func, newglobals)
         try:
             return orig_do_debug(self, arg)
         except Exception:
             exc_info = sys.exc_info()[:2]
             msg = traceback.format_exception_only(*exc_info)[-1].strip()
             self.error(msg)
-
     do_debug.__doc__ = pdb.Pdb.do_debug.__doc__
 
+    def do_run(self, arg):
+        """Restart/Rerun during ``python -m pdbp <script.py>`` mode."""
+        self.last_cmd = self.lastcmd = "run"
+        if arg:
+            import shlex
+            argv0 = sys.argv[0:1]
+            sys.argv = shlex.split(arg)
+            sys.argv[:0] = argv0
+        raise Restart
+    do_restart = do_run
+
     def do_interact(self, arg):
         ns = self.curframe.f_globals.copy()
         ns.update(self.curframe.f_locals)
         code.interact("*interactive*", local=ns)
 
     def do_track(self, arg):
         try:
             from rpython.translator.tool.reftracker import track
         except ImportError:
-            print("** cannot import pypy.translator.tool.reftracker **",
-                  file=self.stdout)
+            print(
+                "** cannot import pypy.translator.tool.reftracker **",
+                file=self.stdout,
+            )
+            print(
+                "This command requires pypy to be in the current PYTHONPATH.",
+                file=self.stdout,
+            )
             return
         try:
             val = self._getval(arg)
         except Exception:
             pass
         else:
             track(val)
@@ -884,14 +1030,21 @@
         if self.sticky:
             self._print_if_sticky()
         else:
             print(file=self.stdout)
             self.print_stack_entry(self.stack[self.curindex])
             print(file=self.stdout, end="\n\033[F")
 
+    def do_truncate(self, arg):
+        # Toggle line truncation. Usage: "truncate".
+        # (The changes only appear in "sticky" mode.)
+        self.config.truncate_long_lines = not self.config.truncate_long_lines
+        self.print_current_stack_entry()
+    do_trun = do_truncate
+
     def print_stack_trace(self):
         try:
             for frame_index, frame_lineno in enumerate(self.stack):
                 self.print_stack_entry(frame_lineno, frame_index=frame_index)
         except KeyboardInterrupt:
             pass
 
@@ -971,14 +1124,15 @@
             self.curframe = self.stack[self.curindex][0]
             self.curframe_locals = self.curframe.f_locals
             self.print_current_stack_entry()
             self.lineno = None
     do_f = do_frame
 
     def do_up(self, arg="1"):
+        self.last_cmd = self.lastcmd = "up"
         arg = "1" if arg == "" else arg
         try:
             arg = int(arg)
         except (ValueError, TypeError):
             print(
                 '*** Expected a number, got "{0}"'.format(arg),
                 file=self.stdout
@@ -992,14 +1146,15 @@
             self.curframe_locals = self.curframe.f_locals
             self.print_current_stack_entry()
             self.lineno = None
     do_up.__doc__ = pdb.Pdb.do_up.__doc__
     do_u = do_up
 
     def do_down(self, arg="1"):
+        self.last_cmd = self.lastcmd = "down"
         arg = "1" if arg == "" else arg
         try:
             arg = int(arg)
         except (ValueError, TypeError):
             print(
                 '*** Expected a number, got "{0}"'.format(arg),
                 file=self.stdout
@@ -1012,14 +1167,22 @@
             self.curframe = self.stack[self.curindex][0]
             self.curframe_locals = self.curframe.f_locals
             self.print_current_stack_entry()
             self.lineno = None
     do_down.__doc__ = pdb.Pdb.do_down.__doc__
     do_d = do_down
 
+    def do_where(self, arg):
+        self.last_cmd = self.lastcmd = "where"
+        self.sticky = False
+        print(file=self.stdout)
+        self.print_stack_trace()
+    do_w = do_where
+    do_bt = do_where
+
     @staticmethod
     def get_terminal_size():
         fallback = (80, 24)
         try:
             from shutil import get_terminal_size
         except ImportError:
             try:
@@ -1038,15 +1201,15 @@
             return width, height
         else:
             width, height = get_terminal_size(fallback)  # shutil
             return width, height
 
     def _open_editor(self, editor, lineno, filename):
         filename = filename.replace('"', '\\"')
-        os.system('%s +%d "%s"' % (editor, lineno, filename))
+        os.system('%s "%s"' % (editor, filename))
 
     def _get_current_position(self):
         frame = self.curframe
         lineno = frame.f_lineno
         filename = os.path.abspath(frame.f_code.co_filename)
         return filename, lineno
 
@@ -1061,67 +1224,36 @@
         match = re.match(r".*<\d+-codegen (.*):(\d+)>", filename)
         if match:
             filename = match.group(1)
             lineno = int(match.group(2))
         editor = self.config.editor
         self._open_editor(editor, lineno, filename)
 
-    do_ed = do_edit
-
     def _get_history(self):
         return [s for s in self.history if not side_effects_free.match(s)]
 
     def _get_history_text(self):
         import linecache
         line = linecache.getline(self.start_filename, self.start_lineno)
         nspaces = len(line) - len(line.lstrip())
         indent = " " * nspaces
         history = [indent + s for s in self._get_history()]
         return "\n".join(history) + "\n"
 
-    def _open_stdin_paste(self, stdin_paste, lineno, filename, text):
-        proc = subprocess.Popen([stdin_paste, "+%d" % lineno, filename],
-                                stdin=subprocess.PIPE)
-        proc.stdin.write(text)
-        proc.stdin.close()
-
-    def _put(self, text):
-        stdin_paste = self.config.stdin_paste
-        if stdin_paste is None:
-            print('** Error: the "stdin_paste" option is not configured **',
-                  file=self.stdout)
-        filename = self.start_filename
-        lineno = self.start_lineno
-        self._open_stdin_paste(stdin_paste, lineno, filename, text)
-
-    def do_put(self, arg):
-        text = self._get_history_text()
-        self._put(text)
-
-    def do_paste(self, arg):
-        arg = arg.strip()
-        old_stdout = self.stdout
-        self.stdout = StringIO()
-        self.onecmd(arg)
-        text = self.stdout.getvalue()
-        self.stdout = old_stdout
-        sys.stdout.write(text)
-        self._put(text)
-
     def set_trace(self, frame=None):
         """Remember starting frame. Used with pytest."""
         if frame is None:
             frame = sys._getframe().f_back
         self._via_set_trace_frame = frame
-        return super(Pdb, self).set_trace(frame)
+        return super().set_trace(frame)
 
     def is_skipped_module(self, module_name):
         if module_name is None:
             return False
-        return super(Pdb, self).is_skipped_module(module_name)
+        return super().is_skipped_module(module_name)
 
     if not hasattr(pdb.Pdb, "message"):  # For py27.
 
         def message(self, msg):
             print(msg, file=self.stdout)
 
     def error(self, msg):
@@ -1157,17 +1289,14 @@
                 and ctx.__traceback__.tb_frame.f_code.co_name == "onecmd"
             ):
                 removed_bdb_context.__context__ = None
                 break
             removed_bdb_context = removed_bdb_context.__context__
 
 
-if hasattr(pdb, "Restart"):
-    Restart = pdb.Restart
-
 if hasattr(pdb, "_usage"):
     _usage = pdb._usage
 
 # Copy some functions from pdb.py, but rebind the global dictionary.
 for name in "run runeval runctx runcall pm main".split():
     func = getattr(pdb, name)
     globals()[name] = rebind_globals(func, globals())
@@ -1246,30 +1375,23 @@
 
 
 def hideframe(func):
     c = func.__code__
     new_co_consts = c.co_consts + (_HIDE_FRAME,)
     if hasattr(c, "replace"):
         c = c.replace(co_consts=new_co_consts)
-    elif sys.version_info < (3, ):
-        c = types.CodeType(
-            c.co_argcount, c.co_nlocals, c.co_stacksize,
-            c.co_flags, c.co_code,
-            new_co_consts,
-            c.co_names, c.co_varnames, c.co_filename,
-            c.co_name, c.co_firstlineno, c.co_lnotab,
-            c.co_freevars, c.co_cellvars)
     else:
         c = types.CodeType(
             c.co_argcount, c.co_kwonlyargcount, c.co_nlocals, c.co_stacksize,
             c.co_flags, c.co_code,
             c.co_consts + (_HIDE_FRAME,),
             c.co_names, c.co_varnames, c.co_filename,
             c.co_name, c.co_firstlineno, c.co_lnotab,
-            c.co_freevars, c.co_cellvars)
+            c.co_freevars, c.co_cellvars,
+        )
     func.__code__ = c
     return func
 
 
 def always(obj, value):
     return True
 
@@ -1312,10 +1434,95 @@
     pdb.setbgcolor = setbgcolor
     pdb.set_trace = set_trace
     pdb.signature = signature
     pdb.Undefined = Undefined
     pdb.cleanup = cleanup
     pdb.xpm = xpm
 
+
+def print_pdb_continue_line():
+    from pdb import Pdb
+    width, height = Pdb.get_terminal_size()
+    pdb_continue = " PDB continue "
+    border_line = ">>>>>>>>%s>>>>>>>>" % pdb_continue
+    try:
+        terminal_size = width
+        if terminal_size < 30:
+            terminal_size = 30
+        border_len = terminal_size - len(pdb_continue)
+        border_left_len = int(border_len / 2)
+        border_right_len = int(border_len - border_left_len)
+        border_left = ">" * border_left_len
+        border_right = ">" * border_right_len
+        border_line = (border_left + pdb_continue + border_right)
+    except Exception:
+        pass
+    print("\n" + border_line + "\n")
+
+
+def main():
+    import getopt
+    opts, args = getopt.getopt(sys.argv[1:], "mhc:", ["help", "command="])
+    if not args:
+        print(_usage)
+        sys.exit(2)
+    commands = []
+    run_as_module = False
+    for opt, optarg in opts:
+        if opt in ["-h", "--help"]:
+            print(_usage)
+            sys.exit()
+        elif opt in ["-c", "--command"]:
+            commands.append(optarg)
+        elif opt in ["-m"]:
+            run_as_module = True
+    mainpyfile = args[0]
+    if not run_as_module and not os.path.exists(mainpyfile):
+        print("Error: %s does not exist!" % mainpyfile)
+        sys.exit(1)
+    sys.argv[:] = args
+    if not run_as_module:
+        mainpyfile = os.path.realpath(mainpyfile)
+        sys.path[0] = os.path.dirname(mainpyfile)
+    pdb = Pdb()
+    pdb.rcLines.extend(commands)
+    stay_in_pdb = True
+    while stay_in_pdb:
+        try:
+            if run_as_module:
+                pdb._runmodule(mainpyfile)
+            else:
+                pdb._runscript(mainpyfile)
+            if pdb._user_requested_quit:
+                break
+            print_pdb_continue_line()
+            stay_in_pdb = False
+        except Restart:
+            print("Restarting", mainpyfile, "with arguments:")
+            print("\t" + " ".join(sys.argv[1:]))
+            stay_in_pdb = True
+        except SystemExit:
+            print("The program exited via sys.exit(). Exit status:", end=" ")
+            print(sys.exc_info()[1])
+            stay_in_pdb = False
+        except SyntaxError:
+            try:
+                traceback.print_exc()
+            except Exception:
+                pass
+            sys.exit(1)
+            stay_in_pdb = False
+        except Exception:
+            try:
+                traceback.print_exc()
+            except Exception:
+                pass
+            t = sys.exc_info()[2]
+            pdb.interaction(None, t)
+            print_pdb_continue_line()
+            stay_in_pdb = False
+
+
 if __name__ == "__main__":
-    import pdb
-    pdb.main()
+    run_from_main = True
+    import pdbp
+    pdbp.main()
```


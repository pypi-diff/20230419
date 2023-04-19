# Comparing `tmp/pdbplus-1.2.8.tar.gz` & `tmp/pdbplus-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbplus-1.2.8.tar", last modified: Thu Jan 19 21:10:10 2023, max compression
+gzip compressed data, was "pdbplus-1.3.0.tar", last modified: Wed Apr 19 05:36:42 2023, max compression
```

## Comparing `pdbplus-1.2.8.tar` & `pdbplus-1.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-01-19 21:10:10.471109 pdbplus-1.2.8/
--rw-r--r--   0 michael    (501) staff       (20)     6261 2023-01-19 21:10:10.471009 pdbplus-1.2.8/PKG-INFO
--rwxr-xr-x   0 michael    (501) staff       (20)     4204 2022-11-30 22:56:23.000000 pdbplus-1.2.8/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-01-19 21:10:10.470860 pdbplus-1.2.8/pdbplus.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     6261 2023-01-19 21:10:10.000000 pdbplus-1.2.8/pdbplus.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      172 2023-01-19 21:10:10.000000 pdbplus-1.2.8/pdbplus.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-01-19 21:10:10.000000 pdbplus-1.2.8/pdbplus.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       12 2023-01-19 21:10:10.000000 pdbplus-1.2.8/pdbplus.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-01-19 21:10:10.000000 pdbplus-1.2.8/pdbplus.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2023-01-19 21:10:10.471136 pdbplus-1.2.8/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     4918 2023-01-19 21:06:17.000000 pdbplus-1.2.8/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 05:36:42.337043 pdbplus-1.3.0/
+-rw-r--r--   0 michael    (501) staff       (20)    10595 2023-04-19 05:36:42.336835 pdbplus-1.3.0/PKG-INFO
+-rwxr-xr-x   0 michael    (501) staff       (20)     8642 2023-04-19 05:28:37.000000 pdbplus-1.3.0/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 05:36:42.336683 pdbplus-1.3.0/pdbplus.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)    10595 2023-04-19 05:36:42.000000 pdbplus-1.3.0/pdbplus.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      172 2023-04-19 05:36:42.000000 pdbplus-1.3.0/pdbplus.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-19 05:36:42.000000 pdbplus-1.3.0/pdbplus.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       12 2023-04-19 05:36:42.000000 pdbplus-1.3.0/pdbplus.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-19 05:36:42.000000 pdbplus-1.3.0/pdbplus.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2023-04-19 05:36:42.337071 pdbplus-1.3.0/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     4948 2023-04-19 05:33:36.000000 pdbplus-1.3.0/setup.py
```

### Comparing `pdbplus-1.2.8/PKG-INFO` & `pdbplus-1.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,7 @@
-Metadata-Version: 2.1
-Name: pdbplus
-Version: 1.2.8
-Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
-Home-page: https://github.com/mdmintz/pdbp
-Author: Michael Mintz
-Author-email: mdmintz@gmail.com
-Maintainer: Michael Mintz
-License: MIT
-Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
-Project-URL: Download, https://pypi.org/project/pdbp/#files
-Project-URL: Bug Tracker, https://github.com/mdmintz/pdbp/issues
-Project-URL: PyPI, https://pypi.org/project/pdbp/
-Project-URL: Source, https://github.com/mdmintz/pdbp
-Platform: Windows
-Platform: Linux
-Platform: Mac OS-X
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: MacOS X
-Classifier: Environment :: Win32 (MS Windows)
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Debuggers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Utilities
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
-Description-Content-Type: text/markdown
-
 **[<img src="https://img.shields.io/badge/pypi-pdbplus-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbplus) is a proxy for installing [<img src="https://img.shields.io/badge/pypi-pdbp-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbp) (Pdb+).**
 ****
 
 <!-- Pdb+ Docs -->
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
@@ -152,7 +105,125 @@
 --------
 
 <img width="550" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/204359676-137cf541-12ef-469a-9d29-99709608ede0.png">
 
 --------
 
 (**Pdb+** is maintained by the [SeleniumBase Dev Team](https://github.com/seleniumbase/SeleniumBase))
+# pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
+
+<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207774790-fb63af65-5f98-4d92-afe3-12c2733d4db6.png">
+
+--------
+
+**[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
+
+<p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
+
+--------
+
+<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/232536483-9236c513-c5ba-4444-8faa-e8ea64eb5ce2.png">
+
+
+## Installation & Usage:
+
+```bash
+pip install pdbp
+```
+
+Then add ``import pdbp`` to an ``__init__.py`` of your project, which will automatically make **``Pdb+``** the default debugger at breakpoints:
+
+```python
+import pdbp
+```
+
+(If using ``flake8`` for code-linting, you may want to add ``# noqa`` to that line):
+
+```python
+import pdbp  # noqa
+```
+
+To trigger a breakpoint in your code with ``pytest``, add ``--trace`` (to start tests with a breakpoint) or ``--pdb`` (to trigger a breakpoint if a test fails).
+
+Basic **``Pdb+``** console commands: ``n``, ``c``, ``s`` => ``next``, ``continue``, ``step``.
+
+Use the ``u`` and ``d`` keys to travel ``up`` and ``down`` the stack!
+
+(To learn more **Pdb+** console commands, type ``help`` in the **Pdb+** console and press ``Enter/Return``.)
+
+--------
+
+**``pdbp`` (Pdb+)** makes improvements to ``pdbpp`` so that it works in all environments. It also includes other bug-fixes. "Sticky" mode is the default option, which shows multiple lines of code while letting you see where you're going (while typing ``n`` + ``Enter``).
+
+If you somehow reset ``pdb`` to Python's built-in version, you can always replace ``pdb`` with **``pdbp``** again as the default debugger by running this:
+
+```python
+import pdb
+import pdbp
+for key in pdbp.__dict__.keys():
+    pdb.__dict__[key] = pdbp.__dict__[key]
+```
+
+Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
+
+```python
+import pdb
+if hasattr(pdb, "DefaultConfig"):
+    pdb.DefaultConfig.filename_color = pdb.Color.blue
+    pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
+    pdb.DefaultConfig.show_hidden_frames_count = False
+    pdb.DefaultConfig.disable_pytest_capturing = True
+    pdb.DefaultConfig.enable_hidden_frames = False
+    pdb.DefaultConfig.truncate_long_lines = True
+    pdb.DefaultConfig.sticky_by_default = True
+```
+
+You can also trigger **``Pdb+``** activation like this:
+
+```python
+import pdbp
+pdbp.set_trace()
+```
+
+
+### pdbp (Pdb+) commands:
+
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
+
+
+### Sticky Mode vs Non-Sticky Mode:
+
+The default mode (``sticky``) lets you see a lot more lines of code from the debugger when active. In Non-Sticky mode, only one line of code is shown at a time. You can switch between the two modes by typing ``sticky`` in the **Pdb+** console prompt and pressing ``Enter/Return``.
+
+> **Sticky Mode:**
+
+<img width="600" alt="Pdb+ Stick Mode" src="https://user-images.githubusercontent.com/6788579/204890148-53d2567b-9a56-4243-a7d7-66100a284312.png">
+
+> **Non-Sticky Mode:**
+
+<img width="600" alt="Pdb+ Non-Sticky Mode" src="https://user-images.githubusercontent.com/6788579/204890164-8465bc22-0f20-43f1-8ab7-b4316718a4c6.png">
+
+
+### More examples:
+
+**``Pdb+``** is used by packages such as **``seleniumbase``**:
+
+* https://pypi.org/project/seleniumbase/
+* https://github.com/seleniumbase/SeleniumBase
+
+--------
+
+<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/204896775-38d8551b-1d3c-4e95-9f5c-0e03c9de13da.png">
+
+--------
+
+(**Pdb+** is maintained by the [SeleniumBase Dev Team](https://github.com/seleniumbase/SeleniumBase))
```

### Comparing `pdbplus-1.2.8/pdbplus.egg-info/PKG-INFO` & `pdbplus-1.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbplus
-Version: 1.2.8
+Version: 1.3.0
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -22,15 +22,14 @@
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
@@ -38,15 +37,15 @@
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
 
 **[<img src="https://img.shields.io/badge/pypi-pdbplus-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbplus) is a proxy for installing [<img src="https://img.shields.io/badge/pypi-pdbp-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/pdbp) (Pdb+).**
 ****
 
 <!-- Pdb+ Docs -->
 
@@ -152,7 +151,125 @@
 --------
 
 <img width="550" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/204359676-137cf541-12ef-469a-9d29-99709608ede0.png">
 
 --------
 
 (**Pdb+** is maintained by the [SeleniumBase Dev Team](https://github.com/seleniumbase/SeleniumBase))
+# pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
+
+<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207774790-fb63af65-5f98-4d92-afe3-12c2733d4db6.png">
+
+--------
+
+**[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
+
+<p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
+
+--------
+
+<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/232536483-9236c513-c5ba-4444-8faa-e8ea64eb5ce2.png">
+
+
+## Installation & Usage:
+
+```bash
+pip install pdbp
+```
+
+Then add ``import pdbp`` to an ``__init__.py`` of your project, which will automatically make **``Pdb+``** the default debugger at breakpoints:
+
+```python
+import pdbp
+```
+
+(If using ``flake8`` for code-linting, you may want to add ``# noqa`` to that line):
+
+```python
+import pdbp  # noqa
+```
+
+To trigger a breakpoint in your code with ``pytest``, add ``--trace`` (to start tests with a breakpoint) or ``--pdb`` (to trigger a breakpoint if a test fails).
+
+Basic **``Pdb+``** console commands: ``n``, ``c``, ``s`` => ``next``, ``continue``, ``step``.
+
+Use the ``u`` and ``d`` keys to travel ``up`` and ``down`` the stack!
+
+(To learn more **Pdb+** console commands, type ``help`` in the **Pdb+** console and press ``Enter/Return``.)
+
+--------
+
+**``pdbp`` (Pdb+)** makes improvements to ``pdbpp`` so that it works in all environments. It also includes other bug-fixes. "Sticky" mode is the default option, which shows multiple lines of code while letting you see where you're going (while typing ``n`` + ``Enter``).
+
+If you somehow reset ``pdb`` to Python's built-in version, you can always replace ``pdb`` with **``pdbp``** again as the default debugger by running this:
+
+```python
+import pdb
+import pdbp
+for key in pdbp.__dict__.keys():
+    pdb.__dict__[key] = pdbp.__dict__[key]
+```
+
+Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
+
+```python
+import pdb
+if hasattr(pdb, "DefaultConfig"):
+    pdb.DefaultConfig.filename_color = pdb.Color.blue
+    pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
+    pdb.DefaultConfig.show_hidden_frames_count = False
+    pdb.DefaultConfig.disable_pytest_capturing = True
+    pdb.DefaultConfig.enable_hidden_frames = False
+    pdb.DefaultConfig.truncate_long_lines = True
+    pdb.DefaultConfig.sticky_by_default = True
+```
+
+You can also trigger **``Pdb+``** activation like this:
+
+```python
+import pdbp
+pdbp.set_trace()
+```
+
+
+### pdbp (Pdb+) commands:
+
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
+
+
+### Sticky Mode vs Non-Sticky Mode:
+
+The default mode (``sticky``) lets you see a lot more lines of code from the debugger when active. In Non-Sticky mode, only one line of code is shown at a time. You can switch between the two modes by typing ``sticky`` in the **Pdb+** console prompt and pressing ``Enter/Return``.
+
+> **Sticky Mode:**
+
+<img width="600" alt="Pdb+ Stick Mode" src="https://user-images.githubusercontent.com/6788579/204890148-53d2567b-9a56-4243-a7d7-66100a284312.png">
+
+> **Non-Sticky Mode:**
+
+<img width="600" alt="Pdb+ Non-Sticky Mode" src="https://user-images.githubusercontent.com/6788579/204890164-8465bc22-0f20-43f1-8ab7-b4316718a4c6.png">
+
+
+### More examples:
+
+**``Pdb+``** is used by packages such as **``seleniumbase``**:
+
+* https://pypi.org/project/seleniumbase/
+* https://github.com/seleniumbase/SeleniumBase
+
+--------
+
+<img width="600" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/204896775-38d8551b-1d3c-4e95-9f5c-0e03c9de13da.png">
+
+--------
+
+(**Pdb+** is maintained by the [SeleniumBase Dev Team](https://github.com/seleniumbase/SeleniumBase))
```

### Comparing `pdbplus-1.2.8/setup.py` & `pdbplus-1.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,14 +39,16 @@
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
@@ -54,15 +56,15 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name='pdbplus',
-    version='1.2.8',
+    version='1.3.0',
     description="pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/mdmintz/pdbp",
     project_urls={
         "Changelog": "https://github.com/mdmintz/pdbp/releases",
         "Download": "https://pypi.org/project/pdbp/#files",
@@ -83,15 +85,14 @@
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
@@ -100,16 +101,16 @@
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
-        'pdbp>=1.2.8',
+        'pdbp>=1.3.0',
     ],
     setup_requires=[],
     packages=[],
 )
 
 print("\n*** pdbplus Installation Complete! ***\n")
```


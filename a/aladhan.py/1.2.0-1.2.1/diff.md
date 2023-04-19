# Comparing `tmp/aladhan.py-1.2.0.tar.gz` & `tmp/aladhan.py-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aladhan.py-1.2.0.tar", last modified: Sat Aug 27 16:51:35 2022, max compression
+gzip compressed data, was "aladhan.py-1.2.1.tar", last modified: Wed Apr 19 04:20:41 2023, max compression
```

## Comparing `aladhan.py-1.2.0.tar` & `aladhan.py-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 16:51:35.628530 aladhan.py-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-08-27 16:51:26.000000 aladhan.py-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3171 2022-08-27 16:51:35.628530 aladhan.py-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-08-27 16:51:26.000000 aladhan.py-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 16:51:35.628530 aladhan.py-1.2.0/aladhan/
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-08-27 16:51:26.000000 aladhan.py-1.2.0/aladhan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5780 2022-08-27 16:51:26.000000 aladhan.py-1.2.0/aladhan/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26206 2022-08-27 16:51:26.000000 aladhan.py-1.2.0/aladhan/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    31390 2022-08-27 16:51:26.000000 aladhan.py-1.2.0/aladhan/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-08-27 16:51:26.000000 aladhan.py-1.2.0/aladhan/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-08-27 16:51:26.000000 aladhan.py-1.2.0/aladhan/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     2955 2022-08-27 16:51:26.000000 aladhan.py-1.2.0/aladhan/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     8775 2022-08-27 16:51:26.000000 aladhan.py-1.2.0/aladhan/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     4184 2022-08-27 16:51:26.000000 aladhan.py-1.2.0/aladhan/methods.py
--rw-r--r--   0 runner    (1001) docker     (121)     3364 2022-08-27 16:51:26.000000 aladhan.py-1.2.0/aladhan/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 16:51:35.628530 aladhan.py-1.2.0/aladhan.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3171 2022-08-27 16:51:35.000000 aladhan.py-1.2.0/aladhan.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-08-27 16:51:35.000000 aladhan.py-1.2.0/aladhan.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 16:51:35.000000 aladhan.py-1.2.0/aladhan.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-08-27 16:51:35.000000 aladhan.py-1.2.0/aladhan.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-27 16:51:35.000000 aladhan.py-1.2.0/aladhan.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-08-27 16:51:35.628530 aladhan.py-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-08-27 16:51:26.000000 aladhan.py-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:20:41.261658 aladhan.py-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-19 04:20:30.000000 aladhan.py-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-19 04:20:41.261658 aladhan.py-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-19 04:20:30.000000 aladhan.py-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:20:41.261658 aladhan.py-1.2.1/aladhan/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-19 04:20:30.000000 aladhan.py-1.2.1/aladhan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-04-19 04:20:30.000000 aladhan.py-1.2.1/aladhan/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26208 2023-04-19 04:20:30.000000 aladhan.py-1.2.1/aladhan/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31138 2023-04-19 04:20:30.000000 aladhan.py-1.2.1/aladhan/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-19 04:20:30.000000 aladhan.py-1.2.1/aladhan/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-19 04:20:30.000000 aladhan.py-1.2.1/aladhan/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-19 04:20:30.000000 aladhan.py-1.2.1/aladhan/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-04-19 04:20:30.000000 aladhan.py-1.2.1/aladhan/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-19 04:20:30.000000 aladhan.py-1.2.1/aladhan/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-19 04:20:30.000000 aladhan.py-1.2.1/aladhan/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:20:41.261658 aladhan.py-1.2.1/aladhan.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-19 04:20:41.000000 aladhan.py-1.2.1/aladhan.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-19 04:20:41.000000 aladhan.py-1.2.1/aladhan.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 04:20:41.000000 aladhan.py-1.2.1/aladhan.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-19 04:20:41.000000 aladhan.py-1.2.1/aladhan.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 04:20:41.000000 aladhan.py-1.2.1/aladhan.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-19 04:20:41.265658 aladhan.py-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-19 04:20:30.000000 aladhan.py-1.2.1/setup.py
```

### Comparing `aladhan.py-1.2.0/LICENSE` & `aladhan.py-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aladhan.py-1.2.0/PKG-INFO` & `aladhan.py-1.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aladhan.py
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python wrapper for the Aladhan prayer times API
 Home-page: https://github.com/HETHAT/aladhan.py
 Author: HETHAT
 Author-email: zhethat@gmail.com
 License: MIT
 Project-URL: Documentation, https://aladhanpy.rtfd.org 
 Project-URL: Issue tracker, https://github.com/HETHAT/aladhan.py/issues
@@ -21,16 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: async
-Provides-Extra: sync
+Provides-Extra: dev
 License-File: LICENSE
 
 ``aladhan.py`` is a pythonic wrapper for the `Aladhan prayer times <https://aladhan.com/prayer-times-api>`_ API.
 
 .. image:: https://img.shields.io/pypi/v/aladhan.py?color=blue
     :target: https://pypi.python.org/pypi/aladhan.py
     :alt: PyPI version info
@@ -51,26 +50,14 @@
 
 To Install ``aladhan.py`` with pip:
 
 .. code:: sh
 
     pip install aladhan.py
 
-To install only with synchronous requirements
-
-.. code:: sh
-
-    pip install aladhan.py[sync]
-
-To install only with asynchronous requirements
-
-.. code:: sh
-
-    pip install aladhan.py[async]
-
 Quick Example
 -------------
 
 .. code:: py
 
     import aladhan
```

### Comparing `aladhan.py-1.2.0/README.rst` & `aladhan.py-1.2.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -52,73 +52,61 @@
 00000330: 7468 6f6e 2033 2e37 206f 7220 6869 6768  thon 3.7 or high
 00000340: 6572 2069 7320 7265 7175 6972 6564 2e2a  er is required.*
 00000350: 2a0a 0a54 6f20 496e 7374 616c 6c20 6060  *..To Install ``
 00000360: 616c 6164 6861 6e2e 7079 6060 2077 6974  aladhan.py`` wit
 00000370: 6820 7069 703a 0a0a 2e2e 2063 6f64 653a  h pip:.... code:
 00000380: 3a20 7368 0a0a 2020 2020 7069 7020 696e  : sh..    pip in
 00000390: 7374 616c 6c20 616c 6164 6861 6e2e 7079  stall aladhan.py
-000003a0: 0a0a 546f 2069 6e73 7461 6c6c 206f 6e6c  ..To install onl
-000003b0: 7920 7769 7468 2073 796e 6368 726f 6e6f  y with synchrono
-000003c0: 7573 2072 6571 7569 7265 6d65 6e74 730a  us requirements.
-000003d0: 0a2e 2e20 636f 6465 3a3a 2073 680a 0a20  ... code:: sh.. 
-000003e0: 2020 2070 6970 2069 6e73 7461 6c6c 2061     pip install a
-000003f0: 6c61 6468 616e 2e70 795b 7379 6e63 5d0a  ladhan.py[sync].
-00000400: 0a54 6f20 696e 7374 616c 6c20 6f6e 6c79  .To install only
-00000410: 2077 6974 6820 6173 796e 6368 726f 6e6f   with asynchrono
-00000420: 7573 2072 6571 7569 7265 6d65 6e74 730a  us requirements.
-00000430: 0a2e 2e20 636f 6465 3a3a 2073 680a 0a20  ... code:: sh.. 
-00000440: 2020 2070 6970 2069 6e73 7461 6c6c 2061     pip install a
-00000450: 6c61 6468 616e 2e70 795b 6173 796e 635d  ladhan.py[async]
-00000460: 0a0a 5175 6963 6b20 4578 616d 706c 650a  ..Quick Example.
-00000470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a2e  -------------...
-00000480: 2e20 636f 6465 3a3a 2070 790a 0a20 2020  . code:: py..   
-00000490: 2069 6d70 6f72 7420 616c 6164 6861 6e0a   import aladhan.
-000004a0: 0a20 2020 2063 6c69 656e 7420 3d20 616c  .    client = al
-000004b0: 6164 6861 6e2e 436c 6965 6e74 2829 0a20  adhan.Client(). 
-000004c0: 2020 2070 7261 7965 725f 7469 6d65 7320     prayer_times 
-000004d0: 3d20 636c 6965 6e74 2e67 6574 5f74 696d  = client.get_tim
-000004e0: 696e 6773 5f62 795f 6164 6472 6573 7328  ings_by_address(
-000004f0: 224c 6f6e 646f 6e22 290a 2020 2020 666f  "London").    fo
-00000500: 7220 7072 6179 6572 5f74 696d 6520 696e  r prayer_time in
-00000510: 2070 7261 7965 725f 7469 6d65 733a 0a20   prayer_times:. 
-00000520: 2020 2020 2020 2070 7269 6e74 2870 7261         print(pra
-00000530: 7965 725f 7469 6d65 290a 0a2a 596f 7520  yer_time)..*You 
-00000540: 6361 6e20 6c6f 6f6b 2069 6e74 6f20 6d6f  can look into mo
-00000550: 7265 2065 7861 6d70 6c65 732a 2060 6865  re examples* `he
-00000560: 7265 203c 6874 7470 733a 2f2f 6769 7468  re <https://gith
-00000570: 7562 2e63 6f6d 2f48 4554 4841 542f 616c  ub.com/HETHAT/al
-00000580: 6164 6861 6e2e 7079 2f74 7265 652f 6d61  adhan.py/tree/ma
-00000590: 696e 2f65 7861 6d70 6c65 733e 605f 0a0a  in/examples>`_..
-000005a0: 436f 6e74 7269 6275 7465 0a2d 2d2d 2d2d  Contribute.-----
-000005b0: 2d2d 2d2d 2d0a 0a2d 2060 536f 7572 6365  -----..- `Source
-000005c0: 2043 6f64 6520 3c68 7474 7073 3a2f 2f67   Code <https://g
-000005d0: 6974 6875 622e 636f 6d2f 4845 5448 4154  ithub.com/HETHAT
-000005e0: 2f61 6c61 6468 616e 2e70 793e 605f 0a2d  /aladhan.py>`_.-
-000005f0: 2060 4973 7375 6520 5472 6163 6b65 7220   `Issue Tracker 
-00000600: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-00000610: 636f 6d2f 4845 5448 4154 2f61 6c61 6468  com/HETHAT/aladh
-00000620: 616e 2e70 792f 6973 7375 6573 3e60 5f0a  an.py/issues>`_.
-00000630: 0a0a 5375 7070 6f72 740a 2d2d 2d2d 2d2d  ..Support.------
-00000640: 2d0a 0a49 6620 796f 7520 6172 6520 6861  -..If you are ha
-00000650: 7669 6e67 2069 7373 7565 732c 2070 6c65  ving issues, ple
-00000660: 6173 6520 6c65 7420 6d65 206b 6e6f 7720  ase let me know 
-00000670: 6279 206a 6f69 6e69 6e67 2074 6865 2060  by joining the `
-00000680: 6469 7363 6f72 6420 7375 7070 6f72 7420  discord support 
+000003a0: 0a0a 5175 6963 6b20 4578 616d 706c 650a  ..Quick Example.
+000003b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a2e  -------------...
+000003c0: 2e20 636f 6465 3a3a 2070 790a 0a20 2020  . code:: py..   
+000003d0: 2069 6d70 6f72 7420 616c 6164 6861 6e0a   import aladhan.
+000003e0: 0a20 2020 2063 6c69 656e 7420 3d20 616c  .    client = al
+000003f0: 6164 6861 6e2e 436c 6965 6e74 2829 0a20  adhan.Client(). 
+00000400: 2020 2070 7261 7965 725f 7469 6d65 7320     prayer_times 
+00000410: 3d20 636c 6965 6e74 2e67 6574 5f74 696d  = client.get_tim
+00000420: 696e 6773 5f62 795f 6164 6472 6573 7328  ings_by_address(
+00000430: 224c 6f6e 646f 6e22 290a 2020 2020 666f  "London").    fo
+00000440: 7220 7072 6179 6572 5f74 696d 6520 696e  r prayer_time in
+00000450: 2070 7261 7965 725f 7469 6d65 733a 0a20   prayer_times:. 
+00000460: 2020 2020 2020 2070 7269 6e74 2870 7261         print(pra
+00000470: 7965 725f 7469 6d65 290a 0a2a 596f 7520  yer_time)..*You 
+00000480: 6361 6e20 6c6f 6f6b 2069 6e74 6f20 6d6f  can look into mo
+00000490: 7265 2065 7861 6d70 6c65 732a 2060 6865  re examples* `he
+000004a0: 7265 203c 6874 7470 733a 2f2f 6769 7468  re <https://gith
+000004b0: 7562 2e63 6f6d 2f48 4554 4841 542f 616c  ub.com/HETHAT/al
+000004c0: 6164 6861 6e2e 7079 2f74 7265 652f 6d61  adhan.py/tree/ma
+000004d0: 696e 2f65 7861 6d70 6c65 733e 605f 0a0a  in/examples>`_..
+000004e0: 436f 6e74 7269 6275 7465 0a2d 2d2d 2d2d  Contribute.-----
+000004f0: 2d2d 2d2d 2d0a 0a2d 2060 536f 7572 6365  -----..- `Source
+00000500: 2043 6f64 6520 3c68 7474 7073 3a2f 2f67   Code <https://g
+00000510: 6974 6875 622e 636f 6d2f 4845 5448 4154  ithub.com/HETHAT
+00000520: 2f61 6c61 6468 616e 2e70 793e 605f 0a2d  /aladhan.py>`_.-
+00000530: 2060 4973 7375 6520 5472 6163 6b65 7220   `Issue Tracker 
+00000540: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
+00000550: 636f 6d2f 4845 5448 4154 2f61 6c61 6468  com/HETHAT/aladh
+00000560: 616e 2e70 792f 6973 7375 6573 3e60 5f0a  an.py/issues>`_.
+00000570: 0a0a 5375 7070 6f72 740a 2d2d 2d2d 2d2d  ..Support.------
+00000580: 2d0a 0a49 6620 796f 7520 6172 6520 6861  -..If you are ha
+00000590: 7669 6e67 2069 7373 7565 732c 2070 6c65  ving issues, ple
+000005a0: 6173 6520 6c65 7420 6d65 206b 6e6f 7720  ase let me know 
+000005b0: 6279 206a 6f69 6e69 6e67 2074 6865 2060  by joining the `
+000005c0: 6469 7363 6f72 6420 7375 7070 6f72 7420  discord support 
+000005d0: 7365 7276 6572 203c 6874 7470 733a 2f2f  server <https://
+000005e0: 6469 7363 6f72 642e 6767 2f6a 6542 4746  discord.gg/jeBGF
+000005f0: 3856 6575 643e 605f 0a0a 4c69 6365 6e73  8Veud>`_..Licens
+00000600: 650a 2d2d 2d2d 2d2d 2d0a 0a54 6865 2070  e.-------..The p
+00000610: 726f 6a65 6374 2069 7320 6c69 6365 6e73  roject is licens
+00000620: 6564 2075 6e64 6572 2074 6865 204d 4954  ed under the MIT
+00000630: 206c 6963 656e 7365 2e0a 0a4c 696e 6b73   license...Links
+00000640: 0a2d 2d2d 2d2d 2d0a 0a2d 2060 5079 5069  .------..- `PyPi
+00000650: 203c 6874 7470 733a 2f2f 7079 7069 2e70   <https://pypi.p
+00000660: 7974 686f 6e2e 6f72 672f 7079 7069 2f61  ython.org/pypi/a
+00000670: 6c61 6468 616e 2e70 793e 605f 0a2d 2060  ladhan.py>`_.- `
+00000680: 4469 7363 6f72 6420 7375 7070 6f72 7420  Discord support 
 00000690: 7365 7276 6572 203c 6874 7470 733a 2f2f  server <https://
 000006a0: 6469 7363 6f72 642e 6767 2f6a 6542 4746  discord.gg/jeBGF
-000006b0: 3856 6575 643e 605f 0a0a 4c69 6365 6e73  8Veud>`_..Licens
-000006c0: 650a 2d2d 2d2d 2d2d 2d0a 0a54 6865 2070  e.-------..The p
-000006d0: 726f 6a65 6374 2069 7320 6c69 6365 6e73  roject is licens
-000006e0: 6564 2075 6e64 6572 2074 6865 204d 4954  ed under the MIT
-000006f0: 206c 6963 656e 7365 2e0a 0a4c 696e 6b73   license...Links
-00000700: 0a2d 2d2d 2d2d 2d0a 0a2d 2060 5079 5069  .------..- `PyPi
-00000710: 203c 6874 7470 733a 2f2f 7079 7069 2e70   <https://pypi.p
-00000720: 7974 686f 6e2e 6f72 672f 7079 7069 2f61  ython.org/pypi/a
-00000730: 6c61 6468 616e 2e70 793e 605f 0a2d 2060  ladhan.py>`_.- `
-00000740: 4469 7363 6f72 6420 7375 7070 6f72 7420  Discord support 
-00000750: 7365 7276 6572 203c 6874 7470 733a 2f2f  server <https://
-00000760: 6469 7363 6f72 642e 6767 2f6a 6542 4746  discord.gg/jeBGF
-00000770: 3856 6575 643e 605f 0a2d 2060 446f 6375  8Veud>`_.- `Docu
-00000780: 6d65 6e74 6174 696f 6e20 3c68 7474 7073  mentation <https
-00000790: 3a2f 2f61 6c61 6468 616e 7079 2e72 6561  ://aladhanpy.rea
-000007a0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-000007b0: 6174 6573 743e 605f                      atest>`_
+000006b0: 3856 6575 643e 605f 0a2d 2060 446f 6375  8Veud>`_.- `Docu
+000006c0: 6d65 6e74 6174 696f 6e20 3c68 7474 7073  mentation <https
+000006d0: 3a2f 2f61 6c61 6468 616e 7079 2e72 6561  ://aladhanpy.rea
+000006e0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+000006f0: 6174 6573 743e 605f 0a                   atest>`_.
```

### Comparing `aladhan.py-1.2.0/aladhan/__init__.py` & `aladhan.py-1.2.1/aladhan/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 """
 
 from collections import namedtuple
 
 VersionInfo = namedtuple("VersionInfo", "major minor micro releaselevel serial")
 
 version_info = VersionInfo(
-    major=1, minor=2, micro=0, releaselevel="final", serial=0
+    major=1, minor=2, micro=1, releaselevel="final", serial=0
 )
 
 __title__ = "aladhan.py"
 __author__ = "HETHAT"
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 
 from . import methods
 from .client import Client
 from .data_classes import *
 from .enums import *
 from .methods import Method
```

### Comparing `aladhan.py-1.2.0/aladhan/__main__.py` & `aladhan.py-1.2.1/aladhan/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 import argparse
 import json
 import platform
 import sys
 import time
 
 import pkg_resources
-from pygments import highlight
-from pygments.formatters.terminal256 import Terminal256Formatter
-from pygments.lexers.web import JsonLexer
 
 import aladhan
 
 try:
     import aiohttp
 except ModuleNotFoundError:
     aiohttp = None
@@ -51,20 +48,16 @@
 
 
 def core(_, args):
     if args.version:
         show_version()
 
 
-def print_json(res, sh, indent):
+def print_json(res, indent):
     res = json.dumps(res, indent=indent)
-    if sh:
-        res = highlight(
-            res, lexer=JsonLexer(), formatter=Terminal256Formatter()
-        )
     print(res)
 
 
 def save_json(path, res, indent):
     with open(path, "w") as f:
         json.dump(res, f, indent=indent)
     print(f"saved response to {path}")
@@ -123,15 +116,15 @@
             res = func(**params)
         except aladhan.exceptions.HTTPException as e:
             res = e.response
     else:
         res = func()
     ts_end = time.perf_counter() - ts_start
     if args.file is None:
-        print_json(res, args.syntax_highlight, args.indent)
+        print_json(res, args.indent)
     else:
         save_json(args.file, res, args.indent)
     print(f"Taken time: {ts_end * 1000:.2f}ms")
 
 
 def add_request_args(subparser):
     parser = subparser.add_parser(
@@ -153,23 +146,14 @@
         "--file",
         action="store",
         help="Where to store the json response. "
         "If it wasn't given it will print to console.",
         default=None,
     )
     parser.add_argument(
-        "-s",
-        "--syntax_highlight",
-        action="store",
-        help="whither to highlight json syntax "
-        "when outputting to console or not. (default=True)",
-        type=lambda kv: "0" != kv.lower() != "false",
-        default=True,
-    )
-    parser.add_argument(
         "-i",
         "--indent",
         action="store",
         help="Indent format value, passing none -> no indents. (default=4)",
         type=lambda kv: int(kv) if kv.isnumeric() else None,
         default=4,
     )
```

### Comparing `aladhan.py-1.2.0/aladhan/client.py` & `aladhan.py-1.2.1/aladhan/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -841,15 +841,15 @@
 
         Raises
         ------
             :exc:`~aladhan.exceptions.BadRequest`
                Something went wrong.
         """
         return self.converter.to_list_of_obj(
-            self.http.get_hijri_holidays(year, adjustment), Date
+            self.http.get_islamic_holidays(year, adjustment), Date
         )
 
     def get_status(self) -> StatusR:
         """
         Returns
         -------
             :class:`dict`
```

### Comparing `aladhan.py-1.2.0/aladhan/data_classes.py` & `aladhan.py-1.2.1/aladhan/data_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,38 +220,30 @@
 
     *New in v0.1.2: timings, time_utc*
     *Changed in v1.2.0*: timings is removed and replaced with data.
     """
 
     __slots__ = ("data", "name", "time", "time_utc", "str_time")
 
-    def __init__(self, name: str, time: str, timestamp: int, data):
-        d = datetime.utcfromtimestamp(timestamp)
+    def __init__(self, name: str, time: str, data):
+        d = datetime.strptime(data.date.readable, "%d %b %Y")
         time = time.split()[0]
         self.data = data
         self.name = name
         self.time = datetime.strptime(time, "%H:%M").replace(
             d.year, d.month, d.day
         )
         try:
-            self.time_utc = self.time + data.meta.timezone.utcoffset(self.time)
+            self.time_utc = self.time - data.meta.timezone.utcoffset(self.time)
         except pytz.exceptions.NonExistentTimeError:  # pragma: no cover
             self.time_utc = None
         self.str_time = self.time.strftime("%H:%M %d-%m-%Y")
 
     @property
     def remaining(self):
-        """:class:`datetime.timedelta`: remaining time for prayer.
-
-        *New in v0.1.2*
-        """
-        return self.time - datetime.utcnow()
-
-    @property
-    def remaining_utc(self):
         """Optional[:class:`datetime.timedelta`]:
          remaining time for prayer for utc.
 
         *New in v0.1.2*
         """
         return self.time_utc and self.time_utc - datetime.utcnow()
 
@@ -983,15 +975,15 @@
         Sunset: str,
         Isha: str,
         Midnight: str,
         Firstthird: str,
         Lastthird: str,
     ):
         self.data = data
-        _Prayer = partial(Prayer, data=data, timestamp=data.date.timestamp)
+        _Prayer = partial(Prayer, data=data)
         self.imsak: Prayer = _Prayer("Imsak", Imsak)
         self.fajr: Prayer = _Prayer("Fajr", Fajr)
         self.sunrise: Prayer = _Prayer("Sunrise", Sunrise)
         self.dhuhr: Prayer = _Prayer("Dhuhr", Dhuhr)
         self.asr: Prayer = _Prayer("Asr", Asr)
         self.sunset: Prayer = _Prayer("Sunset", Sunset)
         self.maghrib: Prayer = _Prayer("Maghrib", Maghrib)
@@ -1128,16 +1120,16 @@
 
     *New in v1.2.0*
     """
 
     def __init__(self, meta, date, timings, client):
         ((prayer, time),) = timings.items()
         self.meta = Meta(data=self, **meta)
-        self.date = BaseDate(**date)
-        self.prayer = Prayer(prayer, time, self.date.timestamp, data=self)
+        self.date = Date(**date)
+        self.prayer = Prayer(prayer, time, data=self)
         self.client = client
 
     def __repr__(self):
         return f"<NextPrayerData | {self.prayer.name} {self.date.readable}>"
 
     def __hash__(self):
         return hash((self.meta, self.date))
```

### Comparing `aladhan.py-1.2.0/aladhan/endpoints.py` & `aladhan.py-1.2.1/aladhan/endpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # Hijri Calendar
 HIJRI_CALENDAR = BASE + "hijriCalendar"
 HIJRI_CALENDAR_BY_ADDRESS = HIJRI_CALENDAR + "ByAddress"
 HIJRI_CALENDAR_BY_CITY = HIJRI_CALENDAR + "ByCity"
 
 # Info
-STATUS = BASE + "status"
+STATUS = "https://api.aladhan.com/status"
 METHODS = BASE + "methods"  # won't be covered (use aladhan.methods instead)
 SPECIAL_DAYS = BASE + "specialDays"
 ISLAMIC_MONTHS = BASE + "islamicMonths"
 
 # Date Converters
 H_TO_G = BASE + "hToG"
 G_TO_H = BASE + "gToH"
```

### Comparing `aladhan.py-1.2.0/aladhan/enums.py` & `aladhan.py-1.2.1/aladhan/enums.py`

 * *Files identical despite different names*

### Comparing `aladhan.py-1.2.0/aladhan/exceptions.py` & `aladhan.py-1.2.1/aladhan/exceptions.py`

 * *Files identical despite different names*

### Comparing `aladhan.py-1.2.0/aladhan/http.py` & `aladhan.py-1.2.1/aladhan/http.py`

 * *Files identical despite different names*

### Comparing `aladhan.py-1.2.0/aladhan/methods.py` & `aladhan.py-1.2.1/aladhan/methods.py`

 * *Files identical despite different names*

### Comparing `aladhan.py-1.2.0/aladhan/types.py` & `aladhan.py-1.2.1/aladhan/types.py`

 * *Files identical despite different names*

### Comparing `aladhan.py-1.2.0/aladhan.py.egg-info/PKG-INFO` & `aladhan.py-1.2.1/aladhan.py.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aladhan.py
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python wrapper for the Aladhan prayer times API
 Home-page: https://github.com/HETHAT/aladhan.py
 Author: HETHAT
 Author-email: zhethat@gmail.com
 License: MIT
 Project-URL: Documentation, https://aladhanpy.rtfd.org 
 Project-URL: Issue tracker, https://github.com/HETHAT/aladhan.py/issues
@@ -21,16 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: async
-Provides-Extra: sync
+Provides-Extra: dev
 License-File: LICENSE
 
 ``aladhan.py`` is a pythonic wrapper for the `Aladhan prayer times <https://aladhan.com/prayer-times-api>`_ API.
 
 .. image:: https://img.shields.io/pypi/v/aladhan.py?color=blue
     :target: https://pypi.python.org/pypi/aladhan.py
     :alt: PyPI version info
@@ -51,26 +50,14 @@
 
 To Install ``aladhan.py`` with pip:
 
 .. code:: sh
 
     pip install aladhan.py
 
-To install only with synchronous requirements
-
-.. code:: sh
-
-    pip install aladhan.py[sync]
-
-To install only with asynchronous requirements
-
-.. code:: sh
-
-    pip install aladhan.py[async]
-
 Quick Example
 -------------
 
 .. code:: py
 
     import aladhan
```

### Comparing `aladhan.py-1.2.0/setup.py` & `aladhan.py-1.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,16 +43,15 @@
     requirements = []
     with open(filename, "r", encoding="utf8") as requirements_txt:
         requirements = requirements_txt.read().splitlines()
     return requirements
 
 
 extras_require = {
-    "async": get_requirements("reqs/async-requirements.txt"),
-    "sync": get_requirements("reqs/sync-requirements.txt"),
+    "dev": get_requirements("dev-requirements.txt")
 }
 
 setup(
     name="aladhan.py",
     version=get_version("aladhan"),
     url="https://github.com/HETHAT/aladhan.py",
     license="MIT",
```


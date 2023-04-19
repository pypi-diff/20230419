# Comparing `tmp/webslides-0.5.9.tar.gz` & `tmp/webslides-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webslides-0.5.9.tar", last modified: Mon Apr 17 08:23:39 2023, max compression
+gzip compressed data, was "webslides-0.6.0.tar", last modified: Wed Apr 19 08:26:13 2023, max compression
```

## Comparing `webslides-0.5.9.tar` & `webslides-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 08:23:39.110199 webslides-0.5.9/
--rw-rw-rw-   0        0        0       49 2023-04-17 08:03:59.000000 webslides-0.5.9/MANIFEST.in
--rw-rw-rw-   0        0        0     6763 2023-04-17 08:23:39.109201 webslides-0.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     6421 2023-04-17 05:53:40.000000 webslides-0.5.9/README.md
--rw-rw-rw-   0        0        0       42 2023-04-17 08:23:39.112197 webslides-0.5.9/setup.cfg
--rw-rw-rw-   0        0        0      537 2023-04-17 08:23:36.000000 webslides-0.5.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:23:38.921200 webslides-0.5.9/webslides/
--rw-rw-rw-   0        0        0       56 2023-04-16 16:05:42.000000 webslides-0.5.9/webslides/__init__.py
--rw-rw-rw-   0        0        0     5066 2023-04-17 08:03:59.000000 webslides-0.5.9/webslides/main.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:23:39.036196 webslides-0.5.9/webslides/modules/
-drwxrwxrwx   0        0        0        0 2023-04-17 08:23:39.103200 webslides-0.5.9/webslides/modules/__pycache__/
--rw-rw-rw-   0        0        0     4642 2023-04-17 08:20:03.000000 webslides-0.5.9/webslides/modules/__pycache__/demo.cpython-310.pyc
--rw-rw-rw-   0        0        0     2562 2023-04-16 15:26:29.000000 webslides-0.5.9/webslides/modules/__pycache__/generate.cpython-310.pyc
--rw-rw-rw-   0        0        0     2445 2023-04-16 18:33:07.000000 webslides-0.5.9/webslides/modules/__pycache__/input_validations.cpython-310.pyc
--rw-rw-rw-   0        0        0     1792 2023-04-16 17:27:37.000000 webslides-0.5.9/webslides/modules/__pycache__/other.cpython-310.pyc
--rw-rw-rw-   0        0        0     1927 2023-04-17 05:45:38.000000 webslides-0.5.9/webslides/modules/__pycache__/pagination.cpython-310.pyc
--rw-rw-rw-   0        0        0     6342 2023-04-17 05:45:38.000000 webslides-0.5.9/webslides/modules/__pycache__/tohtml.cpython-310.pyc
--rw-rw-rw-   0        0        0     5840 2023-04-17 08:22:23.000000 webslides-0.5.9/webslides/modules/demo.py
--rw-rw-rw-   0        0        0    11267 2023-04-17 08:19:41.000000 webslides-0.5.9/webslides/modules/df_demo.html
--rw-rw-rw-   0        0        0    14255 2023-04-17 07:31:42.000000 webslides-0.5.9/webslides/modules/folium_demo.html
--rw-rw-rw-   0        0        0     3800 2023-04-15 17:59:58.000000 webslides-0.5.9/webslides/modules/generate.py
--rw-rw-rw-   0        0        0     2383 2023-04-16 15:35:26.000000 webslides-0.5.9/webslides/modules/hello_world.py
--rw-rw-rw-   0        0        0     2824 2023-04-16 17:57:26.000000 webslides-0.5.9/webslides/modules/input_validations.py
--rw-rw-rw-   0        0        0     1724 2023-04-16 16:39:50.000000 webslides-0.5.9/webslides/modules/other.py
--rw-rw-rw-   0        0        0     2998 2023-04-16 18:40:55.000000 webslides-0.5.9/webslides/modules/pagination.py
--rw-rw-rw-   0        0        0     7774 2023-04-16 18:40:55.000000 webslides-0.5.9/webslides/modules/tohtml.py
-drwxrwxrwx   0        0        0        0 2023-04-17 08:23:38.977194 webslides-0.5.9/webslides.egg-info/
--rw-rw-rw-   0        0        0     6763 2023-04-17 08:23:38.000000 webslides-0.5.9/webslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-04-17 08:23:38.000000 webslides-0.5.9/webslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 08:23:38.000000 webslides-0.5.9/webslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-17 08:23:38.000000 webslides-0.5.9/webslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-17 08:23:38.000000 webslides-0.5.9/webslides.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 08:26:13.089781 webslides-0.6.0/
+-rw-rw-rw-   0        0        0       49 2023-04-17 08:03:59.000000 webslides-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6806 2023-04-19 08:26:13.088779 webslides-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6464 2023-04-19 08:10:18.000000 webslides-0.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 08:26:13.089781 webslides-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      537 2023-04-19 08:12:08.000000 webslides-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:26:12.845775 webslides-0.6.0/webslides/
+-rw-rw-rw-   0        0        0       56 2023-04-16 16:05:42.000000 webslides-0.6.0/webslides/__init__.py
+-rw-rw-rw-   0        0        0     5025 2023-04-17 08:28:07.000000 webslides-0.6.0/webslides/main.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:26:13.014781 webslides-0.6.0/webslides/modules/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:26:13.080778 webslides-0.6.0/webslides/modules/__pycache__/
+-rw-rw-rw-   0        0        0     4741 2023-04-19 08:25:34.000000 webslides-0.6.0/webslides/modules/__pycache__/demo.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2562 2023-04-16 15:26:29.000000 webslides-0.6.0/webslides/modules/__pycache__/generate.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2445 2023-04-16 18:33:07.000000 webslides-0.6.0/webslides/modules/__pycache__/input_validations.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1792 2023-04-16 17:27:37.000000 webslides-0.6.0/webslides/modules/__pycache__/other.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1928 2023-04-19 08:10:22.000000 webslides-0.6.0/webslides/modules/__pycache__/pagination.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6342 2023-04-17 05:45:38.000000 webslides-0.6.0/webslides/modules/__pycache__/tohtml.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5950 2023-04-19 08:26:09.000000 webslides-0.6.0/webslides/modules/demo.py
+-rw-rw-rw-   0        0        0    11267 2023-04-17 08:19:41.000000 webslides-0.6.0/webslides/modules/df_demo.html
+-rw-rw-rw-   0        0        0    14255 2023-04-17 07:31:42.000000 webslides-0.6.0/webslides/modules/folium_demo.html
+-rw-rw-rw-   0        0        0     3800 2023-04-15 17:59:58.000000 webslides-0.6.0/webslides/modules/generate.py
+-rw-rw-rw-   0        0        0     2383 2023-04-16 15:35:26.000000 webslides-0.6.0/webslides/modules/hello_world.py
+-rw-rw-rw-   0        0        0     2824 2023-04-16 17:57:26.000000 webslides-0.6.0/webslides/modules/input_validations.py
+-rw-rw-rw-   0        0        0     1724 2023-04-16 16:39:50.000000 webslides-0.6.0/webslides/modules/other.py
+-rw-rw-rw-   0        0        0     2999 2023-04-19 08:10:18.000000 webslides-0.6.0/webslides/modules/pagination.py
+-rw-rw-rw-   0        0        0     7774 2023-04-16 18:40:55.000000 webslides-0.6.0/webslides/modules/tohtml.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:26:12.897776 webslides-0.6.0/webslides.egg-info/
+-rw-rw-rw-   0        0        0     6806 2023-04-19 08:26:12.000000 webslides-0.6.0/webslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-04-19 08:26:12.000000 webslides-0.6.0/webslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 08:26:12.000000 webslides-0.6.0/webslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-19 08:26:12.000000 webslides-0.6.0/webslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-19 08:26:12.000000 webslides-0.6.0/webslides.egg-info/top_level.txt
```

### Comparing `webslides-0.5.9/PKG-INFO` & `webslides-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: webslides
-Version: 0.5.9
+Version: 0.6.0
 Summary: Creates powerpoint like slides in HTML format. Including title page, index page and page navigation.
 Home-page: UNKNOWN
 Author: Derk-Jan Woltjer
 Author-email: derkjan.woltjer@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Webslides
 
 Webslides is a Python package that allows you to create PowerPoint-like slides in HTML format. It provides several advantages over traditional PowerPoint presentations, such as clickable content, interactivity with plotly figures and other elements, and the ability to create and update a presentation using Python.
 
-## Live demo
+## [live demo](https://datadept.nl/webslides/demo.html)
 Here is a [live demo](https://datadept.nl/webslides/demo.html) of an output of Webslides, demonstrating most of its features.
 
 ## Advantages
 
 Some key advantages of using HTML over PowerPoint include:
 
 - Pages can be as long (or short) as needed, which is handy for taller diagrams
```

### Comparing `webslides-0.5.9/README.md` & `webslides-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Webslides
 
 Webslides is a Python package that allows you to create PowerPoint-like slides in HTML format. It provides several advantages over traditional PowerPoint presentations, such as clickable content, interactivity with plotly figures and other elements, and the ability to create and update a presentation using Python.
 
-## Live demo
+## [live demo](https://datadept.nl/webslides/demo.html)
 Here is a [live demo](https://datadept.nl/webslides/demo.html) of an output of Webslides, demonstrating most of its features.
 
 ## Advantages
 
 Some key advantages of using HTML over PowerPoint include:
 
 - Pages can be as long (or short) as needed, which is handy for taller diagrams
```

### Comparing `webslides-0.5.9/setup.py` & `webslides-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="webslides",
-    version="0.5.9",
+    version="0.6.0",
     author="Derk-Jan Woltjer",
     author_email="derkjan.woltjer@gmail.com",
     description="Creates powerpoint like slides in HTML format. Including title page, index page and page navigation.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     licence="MIT License",
     packages=find_packages(),
```

### Comparing `webslides-0.5.9/webslides/main.py` & `webslides-0.6.0/webslides/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,28 +120,27 @@
         # close page
         html = html.replace('<span></span></div>', '</div><span></span>')
 
     ###################
     ## HANDLE OUTPUT ##
     ###################
 
-    # create output directory 'out' if not present
+    # create output directory 'wsout' if not present
     current_working_dir = os.getcwd()
-    # current_working_dir = os.path.abspath(__file__)
     fpath = os.path.join(current_working_dir, 'wsout')
 
     if not os.path.exists(fpath):
         os.makedirs(fpath)
 
     with codecs.open(f"{fpath}/{fname}", "w", encoding='utf-8') as f:
         f.write(html)
-        print(f'output saved as {fname}')
+        print(f'output saved as wsout/{fname}')
 
 
     if open_in_browser:
         # open in browser to check result
         htmlfile = f"{fpath}/{fname}"
         webbrowser.open(htmlfile)
-        print(f'opened in browser {fname}')
+        print(f'opened in browser wsout/{fname}')
 
     return None
```

#### html2text {}

```diff
@@ -43,14 +43,13 @@
 html.replace('', '
 ') # insert content html html = content_to_html(html, page,
 show_topcat=show_topcat, show_subcat=show_subcat,
 show_index_page=show_index_page, show_highlights_page=show_highlights_page,
 show_navi=True) # close page html = html.replace('
 ', '
 ') ################### ## HANDLE OUTPUT ## ################### # create output
-directory 'out' if not present current_working_dir = os.getcwd() #
-current_working_dir = os.path.abspath(__file__) fpath = os.path.join
-(current_working_dir, 'wsout') if not os.path.exists(fpath): os.makedirs(fpath)
-with codecs.open(f"{fpath}/{fname}", "w", encoding='utf-8') as f: f.write(html)
-print(f'output saved as {fname}') if open_in_browser: # open in browser to
-check result htmlfile = f"{fpath}/{fname}" webbrowser.open(htmlfile) print
-(f'opened in browser {fname}') return None
+directory 'wsout' if not present current_working_dir = os.getcwd() fpath =
+os.path.join(current_working_dir, 'wsout') if not os.path.exists(fpath):
+os.makedirs(fpath) with codecs.open(f"{fpath}/{fname}", "w", encoding='utf-8')
+as f: f.write(html) print(f'output saved as wsout/{fname}') if open_in_browser:
+# open in browser to check result htmlfile = f"{fpath}/{fname}" webbrowser.open
+(htmlfile) print(f'opened in browser wsout/{fname}') return None
```

### Comparing `webslides-0.5.9/webslides/modules/__pycache__/demo.cpython-310.pyc` & `webslides-0.6.0/webslides/modules/__pycache__/demo.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 17 08:20:02 2023 UTC, .py size: 5836 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3201 3d64 cc16 0000  o.......2.=d....
+00000000: 6f0d 0d0a 0000 0000 7ca5 3f64 3c17 0000  o.......|.?d<...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6a00 0000 6400  .....@...sj...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a04 6400 6401 6c05 6d06 5a07  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6402 6c08 6d09 5a09 0100 6403  ..d.d.l.m.Z...d.
 00000060: 6404 6c0a 6d0b 5a0b 6d0c 5a0c 0100 6405  d.l.m.Z.m.Z...d.
 00000070: 6406 8400 5a0d 6407 6408 8400 5a0e 6409  d...Z.d.d...Z.d.
@@ -65,227 +65,233 @@
 00000400: 6d6c 721d 0000 0072 1e00 0000 2905 7227  mlr....r....).r'
 00000410: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
 00000420: 0000 da07 6466 5f68 746d 6c72 1900 0000  ....df_htmlr....
 00000430: 7219 0000 0072 1a00 0000 da0c 6465 6d6f  r....r......demo
 00000440: 5f64 665f 6874 6d6c 1d00 0000 722d 0000  _df_html....r-..
 00000450: 0072 2f00 0000 6300 0000 0000 0000 0000  .r/...c.........
 00000460: 0000 0002 0000 000b 0000 0043 0000 0073  ...........C...s
-00000470: d400 0000 6401 6402 6403 6404 6405 9c02  ....d.d.d.d.d...
-00000480: 6406 9c03 7d00 6407 6408 6409 6701 640a  d...}.d.d.d.g.d.
-00000490: 6700 640b a201 640c 9c04 640d 640e 640f  g.d...d...d.d.d.
-000004a0: 6702 7400 8300 6410 6701 640c 9c04 6411  g.t...d.g.d...d.
-000004b0: 6412 6701 7401 8300 6413 6701 640c 9c04  d.g.t...d.g.d...
-000004c0: 6414 6415 6416 6702 7402 6417 6418 6702  d.d.d.g.t.d.d.g.
-000004d0: 640c 9c04 6419 641a 6701 641b 641c 6701  d...d.d.g.d.d.g.
-000004e0: 640c 9c04 6705 6901 641d 641e 641f 6701  d...g.i.d.d.d.g.
-000004f0: 7403 6420 8301 6421 9c03 6422 6423 6701  t.d ..d!..d"d#g.
-00000500: 7403 6424 8301 6425 6701 640c 9c04 6426  t.d$..d%g.d...d&
-00000510: 6427 6701 7404 8300 6428 6701 640c 9c04  d'g.t...d(g.d...
-00000520: 6703 6901 6429 9c02 7d01 7405 7c01 7c00  g.i.d)..}.t.|.|.
-00000530: 642a 642b 642b 642b 642b 642b 642c 642d  d*d+d+d+d+d+d,d-
-00000540: 8d09 0100 642e 5300 292f 7a40 4372 6561  ....d.S.)/z@Crea
-00000550: 7465 7320 646f 6375 6d65 6e74 6174 696f  tes documentatio
-00000560: 6e20 6578 706c 6169 6e69 6e67 2077 6879  n explaining why
-00000570: 2061 6e64 2068 6f77 2074 6f20 7573 6520   and how to use 
-00000580: 7468 6973 2070 6163 6b61 6765 da00 7a17  this package..z.
-00000590: 5765 6273 6c69 6465 7320 446f 6375 6d65  Webslides Docume
-000005a0: 6e74 6174 696f 6e7a b157 6562 736c 6964  ntationz.Webslid
-000005b0: 6573 2069 7320 6120 5079 7468 6f6e 2070  es is a Python p
-000005c0: 6163 6b61 6765 2074 6861 7420 6372 6561  ackage that crea
-000005d0: 7465 7320 4854 4d4c 2070 7265 7365 6e74  tes HTML present
-000005e0: 6174 696f 6e73 203c 623e 6c69 6b65 2074  ations <b>like t
-000005f0: 6869 7320 6f6e 653c 2f62 3e2e 3c62 723e  his one</b>.<br>
-00000600: 4974 2065 6e61 626c 6573 2065 6173 7920  It enables easy 
-00000610: 7368 6172 696e 6720 6f66 2050 7974 686f  sharing of Pytho
-00000620: 6e2d 6765 6e65 7261 7465 6420 636f 6e74  n-generated cont
-00000630: 656e 7420 7375 6368 2061 7320 6368 6172  ent such as char
-00000640: 7473 2c20 6f74 6865 7220 7669 7375 616c  ts, other visual
-00000650: 7320 616e 6420 6461 7461 7a5a 5468 6973  s and datazZThis
-00000660: 2070 7265 7365 6e74 6174 696f 6e20 6465   presentation de
-00000670: 6d6f 6e73 7472 6174 6573 2066 6561 7475  monstrates featu
-00000680: 7265 7320 6f66 2074 6865 2048 544d 4c20  res of the HTML 
-00000690: 666f 726d 6174 2061 6e64 2073 686f 756c  format and shoul
-000006a0: 6420 6865 6c70 2079 6f75 2067 6574 2073  d help you get s
-000006b0: 7461 7274 6564 2902 da05 4162 6f75 74da  tarted)...About.
-000006c0: 0843 6f6e 7465 6e74 7329 03da 0769 6d67  .Contents)...img
-000006d0: 5f75 726c 7210 0000 00da 0773 756d 6d61  _urlr......summa
-000006e0: 7279 7a1a 4164 7661 6e74 6167 6573 206f  ryz.Advantages o
-000006f0: 7665 7220 506f 7765 7270 6f69 6e74 7a12  ver Powerpointz.
-00000700: 4479 6e61 6d69 6320 7061 6765 6c65 6e67  Dynamic pageleng
-00000710: 7468 7a3b 2d20 5061 6765 7320 6361 6e20  thz;- Pages can 
-00000720: 6265 2061 7320 6c6f 6e67 2028 6f72 2073  be as long (or s
-00000730: 686f 7274 2920 6173 206e 6565 6465 642c  hort) as needed,
-00000740: 206c 696b 6520 7468 6973 206f 6e65 2175   like this one!u
-00000750: 3e00 0000 4e6f 7468 696e 6720 6d75 6368  >...Nothing much
-00000760: 206f 6e20 7468 6973 2070 6167 6520 7265   on this page re
-00000770: 616c 6c79 2c20 7468 6174 2773 2077 6879  ally, that's why
-00000780: 2069 7473 2073 6f20 7368 6f72 7420 f09f   its so short ..
-00000790: 9889 2903 7a2a 2d20 616e 6420 6164 6469  ..).z*- and addi
-000007a0: 6e67 2061 2066 6f6f 7465 7220 6361 6e20  ng a footer can 
-000007b0: 6265 2075 7365 6675 6c6c 2074 6f6f 2e2e  be usefull too..
-000007c0: 7a46 2d20 7073 2e20 4861 7665 2079 6f75  zF- ps. Have you
-000007d0: 206e 6f74 6564 2074 6865 2070 6167 6520   noted the page 
-000007e0: 6e61 7669 6761 7469 6f6e 206f 6e20 7468  navigation on th
-000007f0: 6520 746f 7020 7269 6768 7420 6f66 2074  e top right of t
-00000800: 6865 2070 6167 653f 7ab4 2d20 2623 7831  he page?z.- &#x1
-00000810: 4634 4131 3b3a 2074 6869 7320 6d61 726b  F4A1;: this mark
-00000820: 7320 7061 6765 7320 7769 7468 2061 2068  s pages with a h
-00000830: 6967 686c 6967 6874 2e20 4966 2061 2070  ighlight. If a p
-00000840: 6167 6520 6861 7320 6e6f 2068 6967 686c  age has no highl
-00000850: 6967 6874 7320 2872 656d 6172 6b73 2069  ights (remarks i
-00000860: 6e20 6772 6579 2061 7265 6129 2069 7420  n grey area) it 
-00000870: 6973 206e 6f74 2073 686f 776e 2069 6e20  is not shown in 
-00000880: 7468 6520 6869 6768 6c69 6768 7420 7375  the highlight su
-00000890: 6d6d 6172 7920 7061 6765 206e 6f72 206d  mmary page nor m
-000008a0: 6172 6b65 6420 696e 2074 6865 2074 6162  arked in the tab
-000008b0: 6c65 206f 6620 636f 6e74 656e 7473 2904  le of contents).
-000008c0: 7210 0000 00da 0a68 6967 686c 6967 6874  r......highlight
-000008d0: 73da 0462 6f64 79da 0666 6f6f 7465 727a  s..body..footerz
-000008e0: 1349 6e74 6572 6163 7469 7665 2063 6f6e  .Interactive con
-000008f0: 7465 6e74 7a60 2d20 4e61 7469 7665 2050  tentz`- Native P
-00000900: 6c6f 746c 7920 6772 6170 6820 6f6a 6563  lotly graph ojec
-00000910: 7473 2063 616e 2062 6520 696e 7365 7274  ts can be insert
-00000920: 6564 2061 7320 636f 6e74 656e 742c 2061  ed as content, a
-00000930: 6e64 2074 6865 7920 6861 7665 206d 616e  nd they have man
-00000940: 7920 696e 7465 7261 6374 6976 6520 6665  y interactive fe
-00000950: 6174 7572 6573 7a70 2d20 5472 7920 7a6f  atureszp- Try zo
-00000960: 6f6d 696e 6720 696e 2074 6865 2062 7920  oming in the by 
-00000970: 6472 6167 6769 6e67 2061 2077 696e 646f  dragging a windo
-00000980: 7720 696e 2074 6865 2070 6c6f 742e 204f  w in the plot. O
-00000990: 7220 746f 6767 6c65 2076 6973 6962 696c  r toggle visibil
-000009a0: 6974 7920 6f66 2061 2064 6174 6120 7365  ity of a data se
-000009b0: 7269 6573 2076 6961 2074 6865 206c 6567  ries via the leg
-000009c0: 656e 6420 6b65 7973 7a46 2d20 4c69 6e6b  end keyszF- Link
-000009d0: 2074 6f20 506c 6f74 6c79 2067 616c 6c65   to Plotly galle
-000009e0: 7279 203c 6120 6872 6566 3d22 6874 7470  ry <a href="http
-000009f0: 733a 2f2f 706c 6f74 6c79 2e63 6f6d 2f70  s://plotly.com/p
-00000a00: 7974 686f 6e2f 223e 6865 7265 3c2f 613e  ython/">here</a>
-00000a10: 7a1c 416e 7920 4854 4d4c 2063 6f6e 7465  z.Any HTML conte
-00000a20: 6e74 2077 696c 6c20 7265 6e64 6572 7a16  nt will renderz.
-00000a30: 2d20 466f 7220 6578 616d 706c 6520 7468  - For example th
-00000a40: 6973 206d 6170 7a66 2d20 7468 6973 206d  is mapzf- this m
-00000a50: 6170 2077 6173 2063 7265 6174 6564 2077  ap was created w
-00000a60: 6974 6820 466f 6c69 756d 2028 3c61 2068  ith Folium (<a h
-00000a70: 7265 663d 2268 7474 7073 3a2f 2f70 7974  ref="https://pyt
-00000a80: 686f 6e2d 7669 7375 616c 697a 6174 696f  hon-visualizatio
-00000a90: 6e2e 6769 7468 7562 2e69 6f2f 666f 6c69  n.github.io/foli
-00000aa0: 756d 2f22 3e64 6f63 733c 2f61 3e29 7a18  um/">docs</a>)z.
-00000ab0: 5374 796c 6564 2050 616e 6461 7320 4461  Styled Pandas Da
-00000ac0: 7461 6672 616d 6573 7a27 2d20 576f 772c  taframesz'- Wow,
-00000ad0: 206e 6f74 6963 6520 7468 6174 206d 6178   notice that max
-00000ae0: 2076 616c 7565 206d 6172 6b65 6420 7265   value marked re
-00000af0: 647a 2f2d 204e 6f74 2074 6f20 6d65 6e74  dz/- Not to ment
-00000b00: 696f 6e20 7468 6520 6c6f 7765 7374 2076  ion the lowest v
-00000b10: 616c 7565 2c20 6d61 726b 6564 2067 7265  alue, marked gre
-00000b20: 656e 7a60 2d20 7374 796c 696e 6720 6f66  enz`- styling of
-00000b30: 2061 2070 616e 6461 7320 6461 7461 6672   a pandas datafr
-00000b40: 616d 6520 6361 6e20 6265 2064 6f6e 6520  ame can be done 
-00000b50: 6279 2063 7265 6174 696e 6720 6120 7374  by creating a st
-00000b60: 796c 6572 206f 626a 6563 7420 616e 6420  yler object and 
-00000b70: 636f 6e76 6572 7420 7468 6174 2074 6f20  convert that to 
-00000b80: 6874 6d6c 7a5b 2d20 6965 2e20 7374 796c  htmlz[- ie. styl
-00000b90: 6564 5f64 6620 3d20 6466 2e73 7479 6c65  ed_df = df.style
-00000ba0: 2e62 6163 6b67 726f 756e 645f 6772 6164  .background_grad
-00000bb0: 6965 6e74 2863 6d61 703d 2742 6c75 6573  ient(cmap='Blues
-00000bc0: 2729 2061 6e64 2068 746d 6c20 3d20 7374  ') and html = st
-00000bd0: 796c 6564 5f64 662e 746f 5f68 746d 6c28  yled_df.to_html(
-00000be0: 297a 1453 7570 6572 2073 7065 6564 2075  )z.Super speed u
-00000bf0: 7064 6174 6573 217a 692d 2041 206b 6579  pdates!zi- A key
-00000c00: 2061 6476 616e 7461 6765 206f 6620 7468   advantage of th
-00000c10: 6973 2070 7265 7365 6e74 6174 696f 6e20  is presentation 
-00000c20: 666f 726d 206d 6179 2062 6520 7468 6174  form may be that
-00000c30: 2075 7064 6174 6573 206f 6e6c 7920 7265   updates only re
-00000c40: 7175 6972 6520 7468 6520 3c69 3e70 7265  quire the <i>pre
-00000c50: 7373 206f 6620 6120 6275 7474 6f6e 3c2f  ss of a button</
-00000c60: 693e 75dc 0000 0056 6572 7920 6f66 7465  i>u....Very ofte
-00000c70: 6e20 6461 7461 2c20 616e 616c 7973 6973  n data, analysis
-00000c80: 2063 6f6e 6c75 7369 6f6e 7320 616e 6420   conlusions and 
-00000c90: 6f74 6865 7220 636f 6e74 656e 7420 6973  other content is
-00000ca0: 2072 6576 6973 6564 2069 6e20 6765 7474   revised in gett
-00000cb0: 696e 6720 746f 2061 2066 696e 616c 2076  ing to a final v
-00000cc0: 6572 7369 6f6e 206f 6620 6120 7072 6573  ersion of a pres
-00000cd0: 656e 7461 7469 6f6e 2e20 5369 6e63 6520  entation. Since 
-00000ce0: 616c 6c20 6973 2069 6e20 7079 7468 6f6e  all is in python
-00000cf0: 2073 6372 6970 742c 2075 7064 6174 6573   script, updates
-00000d00: 206f 6620 7468 6520 7072 6573 656e 7461   of the presenta
-00000d10: 7469 6f6e 206f 6e6c 7920 7265 7175 6972  tion only requir
-00000d20: 6573 2074 6865 2070 7265 7373 206f 6620  es the press of 
-00000d30: 7468 6520 e296 b620 5275 6e20 6275 7474  the ... Run butt
-00000d40: 6f6e 2e7a 452d 2061 6e64 2070 6167 696e  on.zE- and pagin
-00000d50: 6174 696f 6e20 7769 6c6c 2061 7574 6f6d  ation will autom
-00000d60: 6174 6963 616c 6c79 2061 646a 7573 7420  atically adjust 
-00000d70: 6966 206e 6577 2063 6f6e 7465 6e74 2069  if new content i
-00000d80: 7320 696e 7365 7274 6564 7a0f 4765 7474  s insertedz.Gett
-00000d90: 696e 6720 5374 6172 7465 647a 1249 6e73  ing Startedz.Ins
-00000da0: 7461 6c6c 2061 6e64 2049 6d70 6f72 747a  tall and Importz
-00000db0: 2a2d 204e 6f74 6869 6e67 206e 6577 2068  *- Nothing new h
-00000dc0: 6572 652c 2067 6f6f 6420 6f6c 6420 7069  ere, good old pi
-00000dd0: 7020 696e 7374 616c 6c2e 2e7a 5a23 696e  p install..zZ#in
-00000de0: 7374 616c 6c20 7061 636b 6167 653c 6272  stall package<br
-00000df0: 3e70 6970 2069 6e73 7461 6c6c 2077 6562  >pip install web
-00000e00: 736c 6964 6573 3c62 723e 3c62 723e 2369  slides<br><br>#i
-00000e10: 6d70 6f72 7420 7061 636b 6167 653c 6272  mport package<br
-00000e20: 3e69 6d70 6f72 7420 7765 6273 6c69 6465  >import webslide
-00000e30: 7320 6173 2077 7329 0372 1000 0000 7235  s as ws).r....r5
-00000e40: 0000 0072 3600 0000 7a08 5275 6e20 4465  ...r6...z.Run De
-00000e50: 6d6f 7a36 2d20 7773 2e64 656d 6f28 2920  moz6- ws.demo() 
-00000e60: 7769 6c6c 2067 656e 6572 6174 6520 7468  will generate th
-00000e70: 6520 6874 6d6c 2079 6f75 2061 7265 2072  e html you are r
-00000e80: 6561 6469 6e67 206e 6f77 7a60 2369 6d70  eading nowz`#imp
-00000e90: 6f72 743c 6272 3e69 6d70 6f72 7420 7765  ort<br>import we
-00000ea0: 6273 6c69 6465 7320 6173 2077 733c 6272  bslides as ws<br
-00000eb0: 3e3c 6272 3e23 6372 6561 7465 2061 6e64  ><br>#create and
-00000ec0: 206f 7065 6e20 7468 6973 2064 656d 6f2e   open this demo.
-00000ed0: 6874 6d6c 2069 6e20 6272 6f77 7365 723c  html in browser<
-00000ee0: 6272 3e77 732e 6465 6d6f 2829 7a54 2d20  br>ws.demo()zT- 
-00000ef0: 6874 6d6c 206f 7574 7075 7420 6669 6c65  html output file
-00000f00: 2c20 696e 2074 6869 7320 6361 7365 2027  , in this case '
-00000f10: 6465 6d6f 2e68 746d 6c27 2c20 6973 2061  demo.html', is a
-00000f20: 6c77 6179 7320 7361 7665 6420 746f 2061  lways saved to a
-00000f30: 2064 6972 6563 746f 7279 2027 7773 6f75   directory 'wsou
-00000f40: 7427 7a0b 4865 6c6c 6f20 576f 726c 647a  t'z.Hello Worldz
-00000f50: 372d 2062 6173 6963 2065 7861 6d70 6c65  7- basic example
-00000f60: 2c20 6465 6d6f 6e73 7472 6174 696e 6720  , demonstrating 
-00000f70: 616c 6c20 6176 6169 6c61 626c 6520 7061  all available pa
-00000f80: 7261 6d65 7465 7273 7a60 2d20 4854 4d4c  rametersz`- HTML
-00000f90: 2061 6c6c 6f77 7320 746f 2061 6464 206a   allows to add j
-00000fa0: 6176 6173 6372 6970 7420 746f 6f2c 206c  avascript too, l
-00000fb0: 696b 6520 7468 6520 636f 7079 2062 7574  ike the copy but
-00000fc0: 746f 6e2e 2054 6861 7427 7320 6163 7475  ton. That's actu
-00000fd0: 616c 6c79 206f 6e6c 7920 6f6e 6520 6c69  ally only one li
-00000fe0: 6e65 206f 6620 636f 6465 2902 da03 5748  ne of code)...WH
-00000ff0: 59da 0348 4f57 7a09 6465 6d6f 2e68 746d  Y..HOWz.demo.htm
-00001000: 6c54 4629 09da 0763 6f6e 7465 6e74 da0a  lTF)...content..
-00001010: 7469 746c 655f 7061 6765 7227 0000 00da  title_pager'....
-00001020: 0b73 686f 775f 746f 7063 6174 da0b 7368  .show_topcat..sh
-00001030: 6f77 5f73 7562 6361 74da 0f6f 7065 6e5f  ow_subcat..open_
-00001040: 696e 5f62 726f 7773 6572 da0f 7368 6f77  in_browser..show
-00001050: 5f69 6e64 6578 5f70 6167 65da 1473 686f  _index_page..sho
-00001060: 775f 6869 6768 6c69 6768 7473 5f70 6167  w_highlights_pag
-00001070: 65da 1473 686f 775f 6869 6768 6c69 6768  e..show_highligh
-00001080: 7473 5f6f 6e6c 794e 2906 721b 0000 0072  ts_onlyN).r....r
-00001090: 2c00 0000 722f 0000 0072 0500 0000 7204  ,...r/...r....r.
-000010a0: 0000 0072 0200 0000 2902 723b 0000 0072  ...r....).r;...r
-000010b0: 3a00 0000 7219 0000 0072 1900 0000 721a  :...r....r....r.
-000010c0: 0000 00da 0464 656d 6f26 0000 0073 9800  .....demo&...s..
-000010d0: 0000 0204 0201 0202 0201 04fe 06fd 0209  ................
-000010e0: 0201 0401 0201 0601 04fd 0206 0202 0201  ................
-000010f0: 02fe 0403 0401 04fb 0206 0401 0401 0202  ................
-00001100: 02ff 04fd 0205 0201 0201 02ff 0202 0202  ................
-00001110: 0201 02fe 04fc 0207 0202 02ff 0202 0401  ................
-00001120: 04fc 02e8 02ff 0221 0201 0401 0201 0201  .......!........
-00001130: 02ff 04fd 0205 0401 0201 0201 02ff 0203  ................
-00001140: 02ff 04fc 0206 0401 0401 0202 02ff 04fd  ................
-00001150: 04f5 06de 0435 0201 0201 0201 0201 0201  .....5..........
-00001160: 0201 0201 0201 06f8 040a 7242 0000 0029  ..........rB...)
-00001170: 1172 1f00 0000 da05 6e75 6d70 79da 026e  .r......numpy..n
-00001180: 70da 0670 616e 6461 73da 0270 64da 0e70  p..pandas..pd..p
-00001190: 6c6f 746c 792e 6578 7072 6573 73da 0765  lotly.express..e
-000011a0: 7870 7265 7373 7212 0000 00da 0e77 6562  xpressr......web
-000011b0: 736c 6964 6573 2e6d 6169 6e72 0200 0000  slides.mainr....
-000011c0: da05 6f74 6865 7272 0400 0000 7205 0000  ..otherr....r...
-000011d0: 0072 1b00 0000 722c 0000 0072 2f00 0000  .r....r,...r/...
-000011e0: 7242 0000 0072 1900 0000 7219 0000 0072  rB...r....r....r
-000011f0: 1900 0000 721a 0000 00da 083c 6d6f 6475  ....r......<modu
-00001200: 6c65 3e01 0000 0073 1600 0000 0800 0801  le>....s........
-00001210: 0801 0c01 0c02 1001 0803 080a 0809 0809  ................
-00001220: 0a4c                                     .L
+00000470: d800 0000 6401 6402 6403 6404 6405 6406  ....d.d.d.d.d.d.
+00000480: 9c03 6407 9c03 7d00 6408 6409 640a 6701  ..d...}.d.d.d.g.
+00000490: 640b 6700 640c a201 640d 9c04 640e 640f  d.g.d...d...d.d.
+000004a0: 6410 6702 7400 8300 6411 6701 640d 9c04  d.g.t...d.g.d...
+000004b0: 6412 6413 6701 7401 8300 6414 6701 640d  d.d.g.t...d.g.d.
+000004c0: 9c04 6415 6416 6417 6702 7402 8300 6418  ..d.d.d.g.t...d.
+000004d0: 6419 6702 640d 9c04 641a 641b 6701 641c  d.g.d...d.d.g.d.
+000004e0: 641d 6701 640d 9c04 6705 6901 641e 641f  d.g.d...g.i.d.d.
+000004f0: 6420 6701 7403 6421 8301 6422 9c03 6423  d g.t.d!..d"..d#
+00000500: 6424 6701 7403 6425 8301 6426 6701 640d  d$g.t.d%..d&g.d.
+00000510: 9c04 6427 6428 6701 7404 8300 6429 6701  ..d'd(g.t...d)g.
+00000520: 640d 9c04 6703 6901 642a 9c02 7d01 7405  d...g.i.d*..}.t.
+00000530: 7c01 7c00 642b 642c 642c 642c 642c 642c  |.|.d+d,d,d,d,d,
+00000540: 642d 642e 8d09 0100 642f 5300 2930 7a40  d-d.....d/S.)0z@
+00000550: 4372 6561 7465 7320 646f 6375 6d65 6e74  Creates document
+00000560: 6174 696f 6e20 6578 706c 6169 6e69 6e67  ation explaining
+00000570: 2077 6879 2061 6e64 2068 6f77 2074 6f20   why and how to 
+00000580: 7573 6520 7468 6973 2070 6163 6b61 6765  use this package
+00000590: da00 7a17 5765 6273 6c69 6465 7320 446f  ..z.Webslides Do
+000005a0: 6375 6d65 6e74 6174 696f 6e7a b157 6562  cumentationz.Web
+000005b0: 736c 6964 6573 2069 7320 6120 5079 7468  slides is a Pyth
+000005c0: 6f6e 2070 6163 6b61 6765 2074 6861 7420  on package that 
+000005d0: 6372 6561 7465 7320 4854 4d4c 2070 7265  creates HTML pre
+000005e0: 7365 6e74 6174 696f 6e73 203c 623e 6c69  sentations <b>li
+000005f0: 6b65 2074 6869 7320 6f6e 653c 2f62 3e2e  ke this one</b>.
+00000600: 3c62 723e 4974 2065 6e61 626c 6573 2065  <br>It enables e
+00000610: 6173 7920 7368 6172 696e 6720 6f66 2050  asy sharing of P
+00000620: 7974 686f 6e2d 6765 6e65 7261 7465 6420  ython-generated 
+00000630: 636f 6e74 656e 7420 7375 6368 2061 7320  content such as 
+00000640: 6368 6172 7473 2c20 6f74 6865 7220 7669  charts, other vi
+00000650: 7375 616c 7320 616e 6420 6461 7461 7a5a  suals and datazZ
+00000660: 5468 6973 2070 7265 7365 6e74 6174 696f  This presentatio
+00000670: 6e20 6465 6d6f 6e73 7472 6174 6573 2066  n demonstrates f
+00000680: 6561 7475 7265 7320 6f66 2074 6865 2048  eatures of the H
+00000690: 544d 4c20 666f 726d 6174 2061 6e64 2073  TML format and s
+000006a0: 686f 756c 6420 6865 6c70 2079 6f75 2067  hould help you g
+000006b0: 6574 2073 7461 7274 6564 7a55 3c61 2068  et startedzU<a h
+000006c0: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+000006d0: 692e 6f72 672f 7072 6f6a 6563 742f 7765  i.org/project/we
+000006e0: 6273 6c69 6465 732f 223e 6874 7470 733a  bslides/">https:
+000006f0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000700: 6374 2f77 6562 736c 6964 6573 2f3c 2f61  ct/webslides/</a
+00000710: 3e29 03da 0541 626f 7574 da08 436f 6e74  >)...About..Cont
+00000720: 656e 7473 da04 5079 5069 2903 da07 696d  ents..PyPi)...im
+00000730: 675f 7572 6c72 1000 0000 da07 7375 6d6d  g_urlr......summ
+00000740: 6172 797a 1a41 6476 616e 7461 6765 7320  aryz.Advantages 
+00000750: 6f76 6572 2050 6f77 6572 706f 696e 747a  over Powerpointz
+00000760: 1244 796e 616d 6963 2070 6167 656c 656e  .Dynamic pagelen
+00000770: 6774 687a 3b2d 2050 6167 6573 2063 616e  gthz;- Pages can
+00000780: 2062 6520 6173 206c 6f6e 6720 286f 7220   be as long (or 
+00000790: 7368 6f72 7429 2061 7320 6e65 6564 6564  short) as needed
+000007a0: 2c20 6c69 6b65 2074 6869 7320 6f6e 6521  , like this one!
+000007b0: 753e 0000 004e 6f74 6869 6e67 206d 7563  u>...Nothing muc
+000007c0: 6820 6f6e 2074 6869 7320 7061 6765 2072  h on this page r
+000007d0: 6561 6c6c 792c 2074 6861 7427 7320 7768  eally, that's wh
+000007e0: 7920 6974 7320 736f 2073 686f 7274 20f0  y its so short .
+000007f0: 9f98 8929 037a 2a2d 2061 6e64 2061 6464  ...).z*- and add
+00000800: 696e 6720 6120 666f 6f74 6572 2063 616e  ing a footer can
+00000810: 2062 6520 7573 6566 756c 6c20 746f 6f2e   be usefull too.
+00000820: 2e7a 462d 2070 732e 2048 6176 6520 796f  .zF- ps. Have yo
+00000830: 7520 6e6f 7465 6420 7468 6520 7061 6765  u noted the page
+00000840: 206e 6176 6967 6174 696f 6e20 6f6e 2074   navigation on t
+00000850: 6865 2074 6f70 2072 6967 6874 206f 6620  he top right of 
+00000860: 7468 6520 7061 6765 3f7a b42d 2026 2378  the page?z.- &#x
+00000870: 3146 3441 313b 3a20 7468 6973 206d 6172  1F4A1;: this mar
+00000880: 6b73 2070 6167 6573 2077 6974 6820 6120  ks pages with a 
+00000890: 6869 6768 6c69 6768 742e 2049 6620 6120  highlight. If a 
+000008a0: 7061 6765 2068 6173 206e 6f20 6869 6768  page has no high
+000008b0: 6c69 6768 7473 2028 7265 6d61 726b 7320  lights (remarks 
+000008c0: 696e 2067 7265 7920 6172 6561 2920 6974  in grey area) it
+000008d0: 2069 7320 6e6f 7420 7368 6f77 6e20 696e   is not shown in
+000008e0: 2074 6865 2068 6967 686c 6967 6874 2073   the highlight s
+000008f0: 756d 6d61 7279 2070 6167 6520 6e6f 7220  ummary page nor 
+00000900: 6d61 726b 6564 2069 6e20 7468 6520 7461  marked in the ta
+00000910: 626c 6520 6f66 2063 6f6e 7465 6e74 7329  ble of contents)
+00000920: 0472 1000 0000 da0a 6869 6768 6c69 6768  .r......highligh
+00000930: 7473 da04 626f 6479 da06 666f 6f74 6572  ts..body..footer
+00000940: 7a13 496e 7465 7261 6374 6976 6520 636f  z.Interactive co
+00000950: 6e74 656e 747a 602d 204e 6174 6976 6520  ntentz`- Native 
+00000960: 506c 6f74 6c79 2067 7261 7068 206f 6a65  Plotly graph oje
+00000970: 6374 7320 6361 6e20 6265 2069 6e73 6572  cts can be inser
+00000980: 7465 6420 6173 2063 6f6e 7465 6e74 2c20  ted as content, 
+00000990: 616e 6420 7468 6579 2068 6176 6520 6d61  and they have ma
+000009a0: 6e79 2069 6e74 6572 6163 7469 7665 2066  ny interactive f
+000009b0: 6561 7475 7265 737a 702d 2054 7279 207a  eatureszp- Try z
+000009c0: 6f6f 6d69 6e67 2069 6e20 7468 6520 6279  ooming in the by
+000009d0: 2064 7261 6767 696e 6720 6120 7769 6e64   dragging a wind
+000009e0: 6f77 2069 6e20 7468 6520 706c 6f74 2e20  ow in the plot. 
+000009f0: 4f72 2074 6f67 676c 6520 7669 7369 6269  Or toggle visibi
+00000a00: 6c69 7479 206f 6620 6120 6461 7461 2073  lity of a data s
+00000a10: 6572 6965 7320 7669 6120 7468 6520 6c65  eries via the le
+00000a20: 6765 6e64 206b 6579 737a 462d 204c 696e  gend keyszF- Lin
+00000a30: 6b20 746f 2050 6c6f 746c 7920 6761 6c6c  k to Plotly gall
+00000a40: 6572 7920 3c61 2068 7265 663d 2268 7474  ery <a href="htt
+00000a50: 7073 3a2f 2f70 6c6f 746c 792e 636f 6d2f  ps://plotly.com/
+00000a60: 7079 7468 6f6e 2f22 3e68 6572 653c 2f61  python/">here</a
+00000a70: 3e7a 1c41 6e79 2048 544d 4c20 636f 6e74  >z.Any HTML cont
+00000a80: 656e 7420 7769 6c6c 2072 656e 6465 727a  ent will renderz
+00000a90: 162d 2046 6f72 2065 7861 6d70 6c65 2074  .- For example t
+00000aa0: 6869 7320 6d61 707a 662d 2074 6869 7320  his mapzf- this 
+00000ab0: 6d61 7020 7761 7320 6372 6561 7465 6420  map was created 
+00000ac0: 7769 7468 2046 6f6c 6975 6d20 283c 6120  with Folium (<a 
+00000ad0: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+00000ae0: 7468 6f6e 2d76 6973 7561 6c69 7a61 7469  thon-visualizati
+00000af0: 6f6e 2e67 6974 6875 622e 696f 2f66 6f6c  on.github.io/fol
+00000b00: 6975 6d2f 223e 646f 6373 3c2f 613e 297a  ium/">docs</a>)z
+00000b10: 1853 7479 6c65 6420 5061 6e64 6173 2044  .Styled Pandas D
+00000b20: 6174 6166 7261 6d65 737a 272d 2057 6f77  ataframesz'- Wow
+00000b30: 2c20 6e6f 7469 6365 2074 6861 7420 6d61  , notice that ma
+00000b40: 7820 7661 6c75 6520 6d61 726b 6564 2072  x value marked r
+00000b50: 6564 7a2f 2d20 4e6f 7420 746f 206d 656e  edz/- Not to men
+00000b60: 7469 6f6e 2074 6865 206c 6f77 6573 7420  tion the lowest 
+00000b70: 7661 6c75 652c 206d 6172 6b65 6420 6772  value, marked gr
+00000b80: 6565 6e7a 602d 2073 7479 6c69 6e67 206f  eenz`- styling o
+00000b90: 6620 6120 7061 6e64 6173 2064 6174 6166  f a pandas dataf
+00000ba0: 7261 6d65 2063 616e 2062 6520 646f 6e65  rame can be done
+00000bb0: 2062 7920 6372 6561 7469 6e67 2061 2073   by creating a s
+00000bc0: 7479 6c65 7220 6f62 6a65 6374 2061 6e64  tyler object and
+00000bd0: 2063 6f6e 7665 7274 2074 6861 7420 746f   convert that to
+00000be0: 2068 746d 6c7a 5b2d 2069 652e 2073 7479   htmlz[- ie. sty
+00000bf0: 6c65 645f 6466 203d 2064 662e 7374 796c  led_df = df.styl
+00000c00: 652e 6261 636b 6772 6f75 6e64 5f67 7261  e.background_gra
+00000c10: 6469 656e 7428 636d 6170 3d27 426c 7565  dient(cmap='Blue
+00000c20: 7327 2920 616e 6420 6874 6d6c 203d 2073  s') and html = s
+00000c30: 7479 6c65 645f 6466 2e74 6f5f 6874 6d6c  tyled_df.to_html
+00000c40: 2829 7a14 5375 7065 7220 7370 6565 6420  ()z.Super speed 
+00000c50: 7570 6461 7465 7321 7a69 2d20 4120 6b65  updates!zi- A ke
+00000c60: 7920 6164 7661 6e74 6167 6520 6f66 2074  y advantage of t
+00000c70: 6869 7320 7072 6573 656e 7461 7469 6f6e  his presentation
+00000c80: 2066 6f72 6d20 6d61 7920 6265 2074 6861   form may be tha
+00000c90: 7420 7570 6461 7465 7320 6f6e 6c79 2072  t updates only r
+00000ca0: 6571 7569 7265 2074 6865 203c 693e 7072  equire the <i>pr
+00000cb0: 6573 7320 6f66 2061 2062 7574 746f 6e3c  ess of a button<
+00000cc0: 2f69 3e75 dc00 0000 5665 7279 206f 6674  /i>u....Very oft
+00000cd0: 656e 2064 6174 612c 2061 6e61 6c79 7369  en data, analysi
+00000ce0: 7320 636f 6e6c 7573 696f 6e73 2061 6e64  s conlusions and
+00000cf0: 206f 7468 6572 2063 6f6e 7465 6e74 2069   other content i
+00000d00: 7320 7265 7669 7365 6420 696e 2067 6574  s revised in get
+00000d10: 7469 6e67 2074 6f20 6120 6669 6e61 6c20  ting to a final 
+00000d20: 7665 7273 696f 6e20 6f66 2061 2070 7265  version of a pre
+00000d30: 7365 6e74 6174 696f 6e2e 2053 696e 6365  sentation. Since
+00000d40: 2061 6c6c 2069 7320 696e 2070 7974 686f   all is in pytho
+00000d50: 6e20 7363 7269 7074 2c20 7570 6461 7465  n script, update
+00000d60: 7320 6f66 2074 6865 2070 7265 7365 6e74  s of the present
+00000d70: 6174 696f 6e20 6f6e 6c79 2072 6571 7569  ation only requi
+00000d80: 7265 7320 7468 6520 7072 6573 7320 6f66  res the press of
+00000d90: 2074 6865 20e2 96b6 2052 756e 2062 7574   the ... Run but
+00000da0: 746f 6e2e 7a45 2d20 616e 6420 7061 6769  ton.zE- and pagi
+00000db0: 6e61 7469 6f6e 2077 696c 6c20 6175 746f  nation will auto
+00000dc0: 6d61 7469 6361 6c6c 7920 6164 6a75 7374  matically adjust
+00000dd0: 2069 6620 6e65 7720 636f 6e74 656e 7420   if new content 
+00000de0: 6973 2069 6e73 6572 7465 647a 0f47 6574  is insertedz.Get
+00000df0: 7469 6e67 2053 7461 7274 6564 7a12 496e  ting Startedz.In
+00000e00: 7374 616c 6c20 616e 6420 496d 706f 7274  stall and Import
+00000e10: 7a2a 2d20 4e6f 7468 696e 6720 6e65 7720  z*- Nothing new 
+00000e20: 6865 7265 2c20 676f 6f64 206f 6c64 2070  here, good old p
+00000e30: 6970 2069 6e73 7461 6c6c 2e2e 7a5a 2369  ip install..zZ#i
+00000e40: 6e73 7461 6c6c 2070 6163 6b61 6765 3c62  nstall package<b
+00000e50: 723e 7069 7020 696e 7374 616c 6c20 7765  r>pip install we
+00000e60: 6273 6c69 6465 733c 6272 3e3c 6272 3e23  bslides<br><br>#
+00000e70: 696d 706f 7274 2070 6163 6b61 6765 3c62  import package<b
+00000e80: 723e 696d 706f 7274 2077 6562 736c 6964  r>import webslid
+00000e90: 6573 2061 7320 7773 2903 7210 0000 0072  es as ws).r....r
+00000ea0: 3600 0000 7237 0000 007a 0852 756e 2044  6...r7...z.Run D
+00000eb0: 656d 6f7a 362d 2077 732e 6465 6d6f 2829  emoz6- ws.demo()
+00000ec0: 2077 696c 6c20 6765 6e65 7261 7465 2074   will generate t
+00000ed0: 6865 2068 746d 6c20 796f 7520 6172 6520  he html you are 
+00000ee0: 7265 6164 696e 6720 6e6f 777a 6023 696d  reading nowz`#im
+00000ef0: 706f 7274 3c62 723e 696d 706f 7274 2077  port<br>import w
+00000f00: 6562 736c 6964 6573 2061 7320 7773 3c62  ebslides as ws<b
+00000f10: 723e 3c62 723e 2363 7265 6174 6520 616e  r><br>#create an
+00000f20: 6420 6f70 656e 2074 6869 7320 6465 6d6f  d open this demo
+00000f30: 2e68 746d 6c20 696e 2062 726f 7773 6572  .html in browser
+00000f40: 3c62 723e 7773 2e64 656d 6f28 297a 542d  <br>ws.demo()zT-
+00000f50: 2068 746d 6c20 6f75 7470 7574 2066 696c   html output fil
+00000f60: 652c 2069 6e20 7468 6973 2063 6173 6520  e, in this case 
+00000f70: 2764 656d 6f2e 6874 6d6c 272c 2069 7320  'demo.html', is 
+00000f80: 616c 7761 7973 2073 6176 6564 2074 6f20  always saved to 
+00000f90: 6120 6469 7265 6374 6f72 7920 2777 736f  a directory 'wso
+00000fa0: 7574 277a 0b48 656c 6c6f 2057 6f72 6c64  ut'z.Hello World
+00000fb0: 7a37 2d20 6261 7369 6320 6578 616d 706c  z7- basic exampl
+00000fc0: 652c 2064 656d 6f6e 7374 7261 7469 6e67  e, demonstrating
+00000fd0: 2061 6c6c 2061 7661 696c 6162 6c65 2070   all available p
+00000fe0: 6172 616d 6574 6572 737a 602d 2048 544d  arametersz`- HTM
+00000ff0: 4c20 616c 6c6f 7773 2074 6f20 6164 6420  L allows to add 
+00001000: 6a61 7661 7363 7269 7074 2074 6f6f 2c20  javascript too, 
+00001010: 6c69 6b65 2074 6865 2063 6f70 7920 6275  like the copy bu
+00001020: 7474 6f6e 2e20 5468 6174 2773 2061 6374  tton. That's act
+00001030: 7561 6c6c 7920 6f6e 6c79 206f 6e65 206c  ually only one l
+00001040: 696e 6520 6f66 2063 6f64 6529 02da 0357  ine of code)...W
+00001050: 4859 da03 484f 577a 0964 656d 6f2e 6874  HY..HOWz.demo.ht
+00001060: 6d6c 5446 2909 da07 636f 6e74 656e 74da  mlTF)...content.
+00001070: 0a74 6974 6c65 5f70 6167 6572 2700 0000  .title_pager'...
+00001080: da0b 7368 6f77 5f74 6f70 6361 74da 0b73  ..show_topcat..s
+00001090: 686f 775f 7375 6263 6174 da0f 6f70 656e  how_subcat..open
+000010a0: 5f69 6e5f 6272 6f77 7365 72da 0f73 686f  _in_browser..sho
+000010b0: 775f 696e 6465 785f 7061 6765 da14 7368  w_index_page..sh
+000010c0: 6f77 5f68 6967 686c 6967 6874 735f 7061  ow_highlights_pa
+000010d0: 6765 da14 7368 6f77 5f68 6967 686c 6967  ge..show_highlig
+000010e0: 6874 735f 6f6e 6c79 4e29 0672 1b00 0000  hts_onlyN).r....
+000010f0: 722c 0000 0072 2f00 0000 7205 0000 0072  r,...r/...r....r
+00001100: 0400 0000 7202 0000 0029 0272 3c00 0000  ....r....).r<...
+00001110: 723b 0000 0072 1900 0000 7219 0000 0072  r;...r....r....r
+00001120: 1a00 0000 da04 6465 6d6f 2600 0000 739a  ......demo&...s.
+00001130: 0000 0002 0402 0102 0202 0102 0104 fd06  ................
+00001140: fd02 0a02 0104 0102 0106 0104 fd02 0602  ................
+00001150: 0202 0102 fe04 0304 0104 fb02 0604 0104  ................
+00001160: 0102 0202 ff04 fd02 0502 0102 0102 ff04  ................
+00001170: 0202 0202 0102 fe04 fc02 0702 0202 ff02  ................
+00001180: 0204 0104 fc02 e802 ff02 2102 0104 0102  ..........!.....
+00001190: 0102 0102 ff04 fd02 0504 0102 0102 0102  ................
+000011a0: ff02 0302 ff04 fc02 0604 0104 0102 0202  ................
+000011b0: ff04 fd04 f506 de04 3502 0102 0102 0102  ........5.......
+000011c0: 0102 0102 0102 0102 0106 f804 0a72 4300  .............rC.
+000011d0: 0000 2911 721f 0000 00da 056e 756d 7079  ..).r......numpy
+000011e0: da02 6e70 da06 7061 6e64 6173 da02 7064  ..np..pandas..pd
+000011f0: da0e 706c 6f74 6c79 2e65 7870 7265 7373  ..plotly.express
+00001200: da07 6578 7072 6573 7372 1200 0000 da0e  ..expressr......
+00001210: 7765 6273 6c69 6465 732e 6d61 696e 7202  webslides.mainr.
+00001220: 0000 00da 056f 7468 6572 7204 0000 0072  .....otherr....r
+00001230: 0500 0000 721b 0000 0072 2c00 0000 722f  ....r....r,...r/
+00001240: 0000 0072 4300 0000 7219 0000 0072 1900  ...rC...r....r..
+00001250: 0000 7219 0000 0072 1a00 0000 da08 3c6d  ..r....r......<m
+00001260: 6f64 756c 653e 0100 0000 7316 0000 0008  odule>....s.....
+00001270: 0008 0108 010c 010c 0210 0108 0308 0a08  ................
+00001280: 0908 090a 4d                             ....M
```

### Comparing `webslides-0.5.9/webslides/modules/__pycache__/generate.cpython-310.pyc` & `webslides-0.6.0/webslides/modules/__pycache__/generate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `webslides-0.5.9/webslides/modules/__pycache__/input_validations.cpython-310.pyc` & `webslides-0.6.0/webslides/modules/__pycache__/input_validations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `webslides-0.5.9/webslides/modules/__pycache__/other.cpython-310.pyc` & `webslides-0.6.0/webslides/modules/__pycache__/other.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `webslides-0.5.9/webslides/modules/__pycache__/pagination.cpython-310.pyc` & `webslides-0.6.0/webslides/modules/__pycache__/pagination.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 16 18:40:55 2023 UTC, .py size: 2998 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-00000000: 6f0d 0d0a 0000 0000 3741 3c64 b60b 0000  o.......7A<d....
+00000000: 6f0d 0d0a 0000 0000 eaa1 3f64 b70b 0000  o.........?d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6402 6403 8400 5a02 6401  d.l.Z.d.d...Z.d.
 00000040: 5300 2904 e900 0000 004e 6302 0000 0000  S.)......Nc.....
 00000050: 0000 0000 0000 000a 0000 0006 0000 0003  ................
 00000060: 0000 0073 3202 0000 7400 8300 7d02 7c00  ...s2...t...}.|.
 00000070: a001 a100 4400 5d33 5c02 7d03 7d04 7c04  ....D.]3\.}.}.|.
 00000080: a001 a100 4400 5d2a 5c02 7d05 7d06 7c06  ....D.]*\.}.}.|.
 00000090: 4400 5d23 7d07 7c07 a002 a100 7d08 7c03  D.]#}.|.....}.|.
 000000a0: 7c08 6401 3c00 7c05 7c08 6402 3c00 6403  |.d.<.|.|.d.<.d.
 000000b0: 7c08 7601 722b 6404 7c08 6403 3c00 6405  |.v.r+d.|.d.<.d.
 000000c0: 7c08 7601 7233 6404 7c08 6405 3c00 7c02  |.v.r3d.|.d.<.|.
 000000d0: a003 7c08 a101 0100 7115 710f 7107 7404  ..|.....q.q.q.t.
 000000e0: a005 7c02 a101 7d09 6406 7c09 6a06 7600  ..|...}.d.|.j.v.
-000000f0: 724c 7c09 7c09 6a07 6407 6b02 1900 7d09  rL|.|.j.d.k...}.
-00000100: 7c09 6a08 7c09 6408 3c00 7c09 6a09 6407  |.j.|.d.<.|.j.d.
-00000110: 6409 8d01 7d09 6401 7c09 6a06 7600 7264  d...}.d.|.j.v.rd
-00000120: 7c09 6a0a a00b 640a a101 7c09 640b 3c00  |.j...d...|.d.<.
+000000f0: 724c 7c09 7c09 6a07 6407 6b03 1900 7d09  rL|.|.j.d.k...}.
+00000100: 7c09 6a08 7c09 6408 3c00 7c09 6a09 6409  |.j.|.d.<.|.j.d.
+00000110: 640a 8d01 7d09 6401 7c09 6a06 7600 7264  d...}.d.|.j.v.rd
+00000120: 7c09 6a0a a00b 640b a101 7c09 640c 3c00  |.j...d...|.d.<.
 00000130: 6402 7c09 6a06 7600 7271 7c09 6a0c a00b  d.|.j.v.rq|.j...
-00000140: 640a a101 7c09 640c 3c00 6405 7c09 6a06  d...|.d.<.d.|.j.
-00000150: 7600 7281 7c09 6a0d 640d 640e 8400 640a  v.r.|.j.d.d...d.
-00000160: 640f 8d02 7c09 6410 3c00 7c09 6a08 640a  d...|.d.<.|.j.d.
-00000170: 1700 7c09 6411 3c00 6405 7c09 6a06 7600  ..|.d.<.d.|.j.v.
+00000140: 640b a101 7c09 640d 3c00 6405 7c09 6a06  d...|.d.<.d.|.j.
+00000150: 7600 7281 7c09 6a0d 640e 640f 8400 640b  v.r.|.j.d.d...d.
+00000160: 6410 8d02 7c09 6411 3c00 7c09 6a08 640b  d...|.d.<.|.j.d.
+00000170: 1700 7c09 6412 3c00 6405 7c09 6a06 7600  ..|.d.<.d.|.j.v.
 00000180: 9001 7212 7c09 6a0e 7c09 6a0f 1400 7c09  ..r.|.j.|.j...|.
-00000190: 6412 3c00 7c09 6a10 a011 a100 7c09 6413  d.<.|.j.....|.d.
-000001a0: 3c00 7c09 6a12 a00b 640a a101 7c09 6414  <.|.j...d...|.d.
-000001b0: 3c00 7c09 6a10 a013 6415 6416 a102 7c09  <.|.j...d.d...|.
-000001c0: 6417 3c00 7c09 6a14 6404 6404 6418 8503  d.<.|.j.d.d.d...
-000001d0: 6417 6602 1900 a015 a100 6404 6404 6418  d.f.......d.d.d.
-000001e0: 8503 1900 7c09 6419 3c00 7c09 6a16 a00b  ....|.d.<.|.j...
-000001f0: 6418 a101 a017 641a a101 7c09 641b 3c00  d.....d...|.d.<.
-00000200: 7c09 6414 1900 a018 6415 a101 7c09 6414  |.d.....d...|.d.
-00000210: 3c00 7c09 641b 1900 a018 6415 a101 7c09  <.|.d.....d...|.
-00000220: 641b 3c00 7419 741a 7c09 6a0f 7c09 6a1b  d.<.t.t.|.j.|.j.
-00000230: 8302 8301 8900 641c 8800 6415 3c00 641c  ......d...d.<.d.
-00000240: 8800 6416 3c00 7c09 6a0d 8700 6601 641d  ..d.<.|.j...f.d.
-00000250: 640e 8408 640a 640f 8d02 7c09 641e 3c00  d...d.d...|.d.<.
-00000260: 7c09 6a0d 8700 6601 641f 640e 8408 640a  |.j...f.d.d...d.
-00000270: 640f 8d02 7c09 6420 3c00 7c09 6a1c 6700  d...|.d <.|.j.g.
-00000280: 6421 a201 640a 640f 8d02 7d09 7c09 a018  d!..d.d...}.|...
-00000290: 641c a101 7d09 7c09 5300 2922 7a96 0a20  d...}.|.S.)"z.. 
+00000190: 6413 3c00 7c09 6a10 a011 a100 7c09 6414  d.<.|.j.....|.d.
+000001a0: 3c00 7c09 6a12 a00b 640b a101 7c09 6415  <.|.j...d...|.d.
+000001b0: 3c00 7c09 6a10 a013 6416 6417 a102 7c09  <.|.j...d.d...|.
+000001c0: 6418 3c00 7c09 6a14 6404 6404 6419 8503  d.<.|.j.d.d.d...
+000001d0: 6418 6602 1900 a015 a100 6404 6404 6419  d.f.......d.d.d.
+000001e0: 8503 1900 7c09 641a 3c00 7c09 6a16 a00b  ....|.d.<.|.j...
+000001f0: 6419 a101 a017 641b a101 7c09 641c 3c00  d.....d...|.d.<.
+00000200: 7c09 6415 1900 a018 6416 a101 7c09 6415  |.d.....d...|.d.
+00000210: 3c00 7c09 641c 1900 a018 6416 a101 7c09  <.|.d.....d...|.
+00000220: 641c 3c00 7419 741a 7c09 6a0f 7c09 6a1b  d.<.t.t.|.j.|.j.
+00000230: 8302 8301 8900 641d 8800 6416 3c00 641d  ......d...d.<.d.
+00000240: 8800 6417 3c00 7c09 6a0d 8700 6601 641e  ..d.<.|.j...f.d.
+00000250: 640f 8408 640b 6410 8d02 7c09 641f 3c00  d...d.d...|.d.<.
+00000260: 7c09 6a0d 8700 6601 6420 640f 8408 640b  |.j...f.d d...d.
+00000270: 6410 8d02 7c09 6421 3c00 7c09 6a1c 6700  d...|.d!<.|.j.g.
+00000280: 6422 a201 640b 6410 8d02 7d09 7c09 a018  d"..d.d...}.|...
+00000290: 641d a101 7d09 7c09 5300 2923 7a96 0a20  d...}.|.S.)#z.. 
 000002a0: 2020 203a 7061 7261 6d20 7061 6765 6461     :param pageda
 000002b0: 7461 3a20 6c69 7374 206f 6620 6469 6374  ta: list of dict
 000002c0: 7320 7769 7468 2063 6f6e 6669 6720 616e  s with config an
 000002d0: 6420 636f 6e74 656e 7473 2070 6572 2070  d contents per p
 000002e0: 6167 650a 2020 2020 3a72 6574 7572 6e3a  age.    :return:
 000002f0: 2064 6620 7769 7468 2070 6167 696e 6174   df with paginat
 00000300: 696f 6e20 6461 7461 2c20 6c69 6b65 2070  ion data, like p
 00000310: 6167 656e 756d 6265 722c 2063 6174 6567  agenumber, categ
 00000320: 6f72 792c 2070 6167 6520 6f72 6465 720a  ory, page order.
 00000330: 2020 2020 da06 746f 7063 6174 da06 7375      ..topcat..su
 00000340: 6263 6174 da06 666f 6f74 6572 4eda 0a68  bcat..footerN..h
-00000350: 6967 686c 6967 6874 73da 0473 686f 7754  ighlights..showT
-00000360: da07 7061 6765 6b65 7929 01da 0464 726f  ..pagekey)...dro
-00000370: 70e9 0100 0000 da09 6e65 7874 5f74 6361  p.......next_tca
-00000380: 74da 096e 6578 745f 7363 6174 6301 0000  t..next_scatc...
-00000390: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-000003a0: 0053 0000 0073 1000 0000 7c00 6401 1900  .S...s....|.d...
-000003b0: 7206 6402 5300 6403 5300 2904 4e72 0500  r.d.S.d.S.).Nr..
-000003c0: 0000 5446 a900 a901 da01 7872 0c00 0000  ..TF......xr....
-000003d0: 720c 0000 00fa 5343 3a5c 5573 6572 735c  r.....SC:\Users\
-000003e0: 6465 726b 2d6a 616e 2e77 6f6c 746a 6572  derk-jan.woltjer
-000003f0: 5c50 7963 6861 726d 5072 6f6a 6563 7473  \PycharmProjects
-00000400: 5c77 6562 736c 6964 6573 5c77 6562 736c  \webslides\websl
-00000410: 6964 6573 5c6d 6f64 756c 6573 5c70 6167  ides\modules\pag
-00000420: 696e 6174 696f 6e2e 7079 da08 3c6c 616d  ination.py..<lam
-00000430: 6264 613e 2c00 0000 7302 0000 0010 007a  bda>,...s......z
-00000440: 2170 6167 696e 6174 696f 6e5f 6461 7461  !pagination_data
-00000450: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-00000460: 613e 2901 da04 6178 6973 da09 6869 6768  a>)...axis..high
-00000470: 6c69 6768 74da 0670 6167 656e 6fda 0768  light..pageno..h
-00000480: 6c5f 7061 6765 da06 686c 5f6d 6178 da07  l_page..hl_max..
-00000490: 686c 5f70 7265 7672 0100 0000 e963 0000  hl_prevr.....c..
-000004a0: 00da 0868 6c5f 7061 6765 32e9 ffff ffff  ...hl_page2.....
-000004b0: da06 686c 5f6d 696e da05 496e 7436 34da  ..hl_min..Int64.
-000004c0: 0768 6c5f 6e65 7874 da00 6301 0000 0000  .hl_next..c.....
-000004d0: 0000 0000 0000 0001 0000 0003 0000 0013  ................
-000004e0: 0000 00f3 0c00 0000 8800 7c00 6401 1900  ..........|.d...
-000004f0: 1900 5300 2902 4e72 1600 0000 720c 0000  ..S.).Nr....r...
-00000500: 0072 0d00 0000 a901 7207 0000 0072 0c00  .r......r....r..
-00000510: 0000 720f 0000 0072 1000 0000 4600 0000  ..r....r....F...
-00000520: f302 0000 000c 00da 0b68 6c5f 7072 6576  .........hl_prev
-00000530: 5f6b 6579 6301 0000 0000 0000 0000 0000  _keyc...........
-00000540: 0001 0000 0003 0000 0013 0000 0072 1e00  .............r..
-00000550: 0000 2902 4e72 1c00 0000 720c 0000 0072  ..).Nr....r....r
-00000560: 0d00 0000 721f 0000 0072 0c00 0000 720f  ....r....r....r.
-00000570: 0000 0072 1000 0000 4700 0000 7220 0000  ...r....G...r ..
-00000580: 00da 0b68 6c5f 6e65 7874 5f6b 6579 2906  ...hl_next_key).
-00000590: 7214 0000 0072 1500 0000 7218 0000 0072  r....r....r....r
-000005a0: 1a00 0000 721c 0000 0072 1600 0000 291d  ....r....r....).
-000005b0: da04 6c69 7374 da05 6974 656d 73da 0463  ..list..items..c
-000005c0: 6f70 79da 0661 7070 656e 64da 0270 64da  opy..append..pd.
-000005d0: 0944 6174 6146 7261 6d65 da07 636f 6c75  .DataFrame..colu
-000005e0: 6d6e 7372 0600 0000 da05 696e 6465 78da  mnsr......index.
-000005f0: 0b72 6573 6574 5f69 6e64 6578 7202 0000  .reset_indexr...
-00000600: 00da 0573 6869 6674 7203 0000 00da 0561  ...shiftr......a
-00000610: 7070 6c79 7212 0000 0072 1300 0000 7214  pplyr....r....r.
-00000620: 0000 00da 0663 756d 6d61 7872 1500 0000  .....cummaxr....
-00000630: da07 7265 706c 6163 65da 036c 6f63 da06  ..replace..loc..
-00000640: 6375 6d6d 696e 721a 0000 00da 0661 7374  cumminr......ast
-00000650: 7970 65da 0666 696c 6c6e 61da 0464 6963  ype..fillna..dic
-00000660: 74da 037a 6970 7207 0000 0072 0800 0000  t..zipr....r....
-00000670: 290a da07 636f 6e74 656e 74da 1473 686f  )...content..sho
-00000680: 775f 6869 6768 6c69 6768 7473 5f6f 6e6c  w_highlights_onl
-00000690: 79da 0464 6174 6172 0200 0000 5a07 7375  y..datar....Z.su
-000006a0: 6263 6174 7372 0300 0000 7224 0000 00da  bcatsr....r$....
-000006b0: 0469 7465 6d5a 0969 7465 6d5f 636f 7079  .itemZ.item_copy
-000006c0: da02 6466 720c 0000 0072 1f00 0000 720f  ..dfr....r....r.
-000006d0: 0000 00da 0f70 6167 696e 6174 696f 6e5f  .....pagination_
-000006e0: 6461 7461 0400 0000 7356 0000 0006 0610  data....sV......
-000006f0: 0110 0108 0108 0108 0108 0108 0308 0108  ................
-00000700: 0108 010c 0202 f502 ff0a 0e0a 040e 010a  ................
-00000710: 020c 010a 0210 010a 0110 010a 0316 020e  ................
-00000720: 030c 0210 010e 0310 0112 0326 0116 0112  ...........&....
-00000730: 0412 0112 0308 0108 011a 011a 0112 030a  ................
-00000740: 0404 0272 3b00 0000 2903 da06 7061 6e64  ...r;...)...pand
-00000750: 6173 7227 0000 0072 3b00 0000 720c 0000  asr'...r;...r...
-00000760: 0072 0c00 0000 720c 0000 0072 0f00 0000  .r....r....r....
-00000770: da08 3c6d 6f64 756c 653e 0100 0000 7304  ..<module>....s.
-00000780: 0000 0008 000c 03                        .......
+00000350: 6967 686c 6967 6874 73da 0473 686f 7746  ighlights..showF
+00000360: da07 7061 6765 6b65 7954 2901 da04 6472  ..pagekeyT)...dr
+00000370: 6f70 e901 0000 00da 096e 6578 745f 7463  op.......next_tc
+00000380: 6174 da09 6e65 7874 5f73 6361 7463 0100  at..next_scatc..
+00000390: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+000003a0: 0000 5300 0000 7310 0000 007c 0064 0119  ..S...s....|.d..
+000003b0: 0072 0664 0253 0064 0353 0029 044e 7205  .r.d.S.d.S.).Nr.
+000003c0: 0000 0054 46a9 00a9 01da 0178 720c 0000  ...TF......xr...
+000003d0: 0072 0c00 0000 fa53 433a 5c55 7365 7273  .r.....SC:\Users
+000003e0: 5c64 6572 6b2d 6a61 6e2e 776f 6c74 6a65  \derk-jan.woltje
+000003f0: 725c 5079 6368 6172 6d50 726f 6a65 6374  r\PycharmProject
+00000400: 735c 7765 6273 6c69 6465 735c 7765 6273  s\webslides\webs
+00000410: 6c69 6465 735c 6d6f 6475 6c65 735c 7061  lides\modules\pa
+00000420: 6769 6e61 7469 6f6e 2e70 79da 083c 6c61  gination.py..<la
+00000430: 6d62 6461 3e2c 0000 0073 0200 0000 1000  mbda>,...s......
+00000440: 7a21 7061 6769 6e61 7469 6f6e 5f64 6174  z!pagination_dat
+00000450: 612e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  a.<locals>.<lamb
+00000460: 6461 3e29 01da 0461 7869 73da 0968 6967  da>)...axis..hig
+00000470: 686c 6967 6874 da06 7061 6765 6e6f da07  hlight..pageno..
+00000480: 686c 5f70 6167 65da 0668 6c5f 6d61 78da  hl_page..hl_max.
+00000490: 0768 6c5f 7072 6576 7201 0000 00e9 6300  .hl_prevr.....c.
+000004a0: 0000 da08 686c 5f70 6167 6532 e9ff ffff  ....hl_page2....
+000004b0: ffda 0668 6c5f 6d69 6eda 0549 6e74 3634  ...hl_min..Int64
+000004c0: da07 686c 5f6e 6578 74da 0063 0100 0000  ..hl_next..c....
+000004d0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+000004e0: 1300 0000 f30c 0000 0088 007c 0064 0119  ...........|.d..
+000004f0: 0019 0053 0029 024e 7216 0000 0072 0c00  ...S.).Nr....r..
+00000500: 0000 720d 0000 00a9 0172 0700 0000 720c  ..r......r....r.
+00000510: 0000 0072 0f00 0000 7210 0000 0046 0000  ...r....r....F..
+00000520: 00f3 0200 0000 0c00 da0b 686c 5f70 7265  ..........hl_pre
+00000530: 765f 6b65 7963 0100 0000 0000 0000 0000  v_keyc..........
+00000540: 0000 0100 0000 0300 0000 1300 0000 721e  ..............r.
+00000550: 0000 0029 024e 721c 0000 0072 0c00 0000  ...).Nr....r....
+00000560: 720d 0000 0072 1f00 0000 720c 0000 0072  r....r....r....r
+00000570: 0f00 0000 7210 0000 0047 0000 0072 2000  ....r....G...r .
+00000580: 0000 da0b 686c 5f6e 6578 745f 6b65 7929  ....hl_next_key)
+00000590: 0672 1400 0000 7215 0000 0072 1800 0000  .r....r....r....
+000005a0: 721a 0000 0072 1c00 0000 7216 0000 0029  r....r....r....)
+000005b0: 1dda 046c 6973 74da 0569 7465 6d73 da04  ...list..items..
+000005c0: 636f 7079 da06 6170 7065 6e64 da02 7064  copy..append..pd
+000005d0: da09 4461 7461 4672 616d 65da 0763 6f6c  ..DataFrame..col
+000005e0: 756d 6e73 7206 0000 00da 0569 6e64 6578  umnsr......index
+000005f0: da0b 7265 7365 745f 696e 6465 7872 0200  ..reset_indexr..
+00000600: 0000 da05 7368 6966 7472 0300 0000 da05  ....shiftr......
+00000610: 6170 706c 7972 1200 0000 7213 0000 0072  applyr....r....r
+00000620: 1400 0000 da06 6375 6d6d 6178 7215 0000  ......cummaxr...
+00000630: 00da 0772 6570 6c61 6365 da03 6c6f 63da  ...replace..loc.
+00000640: 0663 756d 6d69 6e72 1a00 0000 da06 6173  .cumminr......as
+00000650: 7479 7065 da06 6669 6c6c 6e61 da04 6469  type..fillna..di
+00000660: 6374 da03 7a69 7072 0700 0000 7208 0000  ct..zipr....r...
+00000670: 0029 0ada 0763 6f6e 7465 6e74 da14 7368  .)...content..sh
+00000680: 6f77 5f68 6967 686c 6967 6874 735f 6f6e  ow_highlights_on
+00000690: 6c79 da04 6461 7461 7202 0000 005a 0773  ly..datar....Z.s
+000006a0: 7562 6361 7473 7203 0000 0072 2400 0000  ubcatsr....r$...
+000006b0: da04 6974 656d 5a09 6974 656d 5f63 6f70  ..itemZ.item_cop
+000006c0: 79da 0264 6672 0c00 0000 721f 0000 0072  y..dfr....r....r
+000006d0: 0f00 0000 da0f 7061 6769 6e61 7469 6f6e  ......pagination
+000006e0: 5f64 6174 6104 0000 0073 5600 0000 0606  _data....sV.....
+000006f0: 1001 1001 0801 0801 0801 0801 0803 0801  ................
+00000700: 0801 0801 0c02 02f5 02ff 0a0e 0a04 0e01  ................
+00000710: 0a02 0c01 0a02 1001 0a01 1001 0a03 1602  ................
+00000720: 0e03 0c02 1001 0e03 1001 1203 2601 1601  ............&...
+00000730: 1204 1201 1203 0801 0801 1a01 1a01 1203  ................
+00000740: 0a04 0402 723b 0000 0029 03da 0670 616e  ....r;...)...pan
+00000750: 6461 7372 2700 0000 723b 0000 0072 0c00  dasr'...r;...r..
+00000760: 0000 720c 0000 0072 0c00 0000 720f 0000  ..r....r....r...
+00000770: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000780: 0400 0000 0800 0c03                      ........
```

### Comparing `webslides-0.5.9/webslides/modules/__pycache__/tohtml.cpython-310.pyc` & `webslides-0.6.0/webslides/modules/__pycache__/tohtml.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `webslides-0.5.9/webslides/modules/demo.py` & `webslides-0.6.0/webslides/modules/demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
     """Creates documentation explaining why and how to use this package"""
 
     title_page = {
         'img_url': '',
         'title': 'Webslides Documentation',
         'summary': {
             'About': 'Webslides is a Python package that creates HTML presentations <b>like this one</b>.<br>It enables easy sharing of Python-generated content such as charts, other visuals and data',
-            'Contents': 'This presentation demonstrates features of the HTML format and should help you get started'}
+            'Contents': 'This presentation demonstrates features of the HTML format and should help you get started',
+            'PyPi': '<a href="https://pypi.org/project/webslides/">https://pypi.org/project/webslides/</a>'}
     }
 
     content = {
         'WHY': {'Advantages over Powerpoint':
                     [{'title': 'Dynamic pagelength',
                       'highlights': ['- Pages can be as long (or short) as needed, like this one!'],
                       'body': 'Nothing much on this page really, that\'s why its so short 😉',
```

#### html2text {}

```diff
@@ -12,26 +12,27 @@
 fpath = os.path.join(current_dir, fname) with open(fpath, 'r') as f: df_html =
 f.read() return df_html def demo(): """Creates documentation explaining why and
 how to use this package""" title_page = { 'img_url': '', 'title': 'Webslides
 Documentation', 'summary': { 'About': 'Webslides is a Python package that
 creates HTML presentations like this one.
 It enables easy sharing of Python-generated content such as charts, other
 visuals and data', 'Contents': 'This presentation demonstrates features of the
-HTML format and should help you get started'} } content = { 'WHY': {'Advantages
-over Powerpoint': [{'title': 'Dynamic pagelength', 'highlights': ['- Pages can
-be as long (or short) as needed, like this one!'], 'body': 'Nothing much on
-this page really, that\'s why its so short ð', 'footer': ['- and adding a
-footer can be usefull too..', '- ps. Have you noted the page navigation on the
-top right of the page?', '- &#x1F4A1;: this marks pages with a highlight. If a
-page has no highlights (remarks in grey area) it is not shown in the highlight
-summary page nor marked in the table of contents']}, {'title': 'Interactive
-content', 'highlights': [ '- Native Plotly graph ojects can be inserted as
-content, and they have many interactive features', '- Try zooming in the by
-dragging a window in the plot. Or toggle visibility of a data series via the
-legend keys'], 'body': demo_plotly_fig(), 'footer': ['- Link to Plotly gallery
+HTML format and should help you get started', 'PyPi': 'https://pypi.org/
+project/webslides/'} } content = { 'WHY': {'Advantages over Powerpoint': [
+{'title': 'Dynamic pagelength', 'highlights': ['- Pages can be as long (or
+short) as needed, like this one!'], 'body': 'Nothing much on this page really,
+that\'s why its so short ð', 'footer': ['- and adding a footer can be
+usefull too..', '- ps. Have you noted the page navigation on the top right of
+the page?', '- &#x1F4A1;: this marks pages with a highlight. If a page has no
+highlights (remarks in grey area) it is not shown in the highlight summary page
+nor marked in the table of contents']}, {'title': 'Interactive content',
+'highlights': [ '- Native Plotly graph ojects can be inserted as content, and
+they have many interactive features', '- Try zooming in the by dragging a
+window in the plot. Or toggle visibility of a data series via the legend
+keys'], 'body': demo_plotly_fig(), 'footer': ['- Link to Plotly gallery
 here']}, {'title': 'Any HTML content will render', 'highlights': ['- For
 example this map'], 'body': demo_folium_html(), 'footer': [ '- this map was
 created with Folium (docs)']}, {'title': 'Styled Pandas Dataframes',
 'highlights': ['- Wow, notice that max value marked red', '- Not to mention the
 lowest value, marked green'], 'body': demo_df_html(), 'footer': [ '- styling of
 a pandas dataframe can be done by creating a styler object and convert that to
 html', '- ie. styled_df = df.style.background_gradient(cmap=\'Blues\') and html
```

### Comparing `webslides-0.5.9/webslides/modules/df_demo.html` & `webslides-0.6.0/webslides/modules/df_demo.html`

 * *Files identical despite different names*

### Comparing `webslides-0.5.9/webslides/modules/folium_demo.html` & `webslides-0.6.0/webslides/modules/folium_demo.html`

 * *Files identical despite different names*

### Comparing `webslides-0.5.9/webslides/modules/generate.py` & `webslides-0.6.0/webslides/modules/generate.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.9/webslides/modules/hello_world.py` & `webslides-0.6.0/webslides/modules/hello_world.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.9/webslides/modules/input_validations.py` & `webslides-0.6.0/webslides/modules/input_validations.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.9/webslides/modules/other.py` & `webslides-0.6.0/webslides/modules/other.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.9/webslides/modules/pagination.py` & `webslides-0.6.0/webslides/modules/pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                 data.append(item_copy)
 
     df = pd.DataFrame(data)
 
     # only keep page to be shown
     # nb. if shown is not defined for any of the content pages all pages will be shown
     if 'show' in df.columns:
-        df = df[df.show == True]
+        df = df[df.show != False]
 
     df['pagekey'] = df.index
     df = df.reset_index(drop=True)
 
     if 'topcat' in df.columns:
         df['next_tcat'] = df.topcat.shift(1)
     if 'subcat' in df.columns:
```

### Comparing `webslides-0.5.9/webslides/modules/tohtml.py` & `webslides-0.6.0/webslides/modules/tohtml.py`

 * *Files identical despite different names*

### Comparing `webslides-0.5.9/webslides.egg-info/PKG-INFO` & `webslides-0.6.0/webslides.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: webslides
-Version: 0.5.9
+Version: 0.6.0
 Summary: Creates powerpoint like slides in HTML format. Including title page, index page and page navigation.
 Home-page: UNKNOWN
 Author: Derk-Jan Woltjer
 Author-email: derkjan.woltjer@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Webslides
 
 Webslides is a Python package that allows you to create PowerPoint-like slides in HTML format. It provides several advantages over traditional PowerPoint presentations, such as clickable content, interactivity with plotly figures and other elements, and the ability to create and update a presentation using Python.
 
-## Live demo
+## [live demo](https://datadept.nl/webslides/demo.html)
 Here is a [live demo](https://datadept.nl/webslides/demo.html) of an output of Webslides, demonstrating most of its features.
 
 ## Advantages
 
 Some key advantages of using HTML over PowerPoint include:
 
 - Pages can be as long (or short) as needed, which is handy for taller diagrams
```

### Comparing `webslides-0.5.9/webslides.egg-info/SOURCES.txt` & `webslides-0.6.0/webslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/mkdocs-roamlinks-plugin-0.3.0.tar.gz` & `tmp/mkdocs-roamlinks-plugin-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-roamlinks-plugin-0.3.0.tar", last modified: Wed Mar 29 04:16:01 2023, max compression
+gzip compressed data, was "mkdocs-roamlinks-plugin-0.3.1.tar", last modified: Wed Apr 19 11:13:29 2023, max compression
```

## Comparing `mkdocs-roamlinks-plugin-0.3.0.tar` & `mkdocs-roamlinks-plugin-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-29 04:16:01.403193 mkdocs-roamlinks-plugin-0.3.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1056 2023-03-11 15:33:06.000000 mkdocs-roamlinks-plugin-0.3.0/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      774 2023-03-29 04:16:01.403193 mkdocs-roamlinks-plugin-0.3.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1512 2023-03-29 04:14:52.000000 mkdocs-roamlinks-plugin-0.3.0/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-29 04:16:01.403193 mkdocs-roamlinks-plugin-0.3.0/mkdocs_roamlinks_plugin/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-03-11 15:33:06.000000 mkdocs-roamlinks-plugin-0.3.0/mkdocs_roamlinks_plugin/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7664 2023-03-29 04:14:07.000000 mkdocs-roamlinks-plugin-0.3.0/mkdocs_roamlinks_plugin/plugin.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-29 04:16:01.403193 mkdocs-roamlinks-plugin-0.3.0/mkdocs_roamlinks_plugin.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      774 2023-03-29 04:16:01.000000 mkdocs-roamlinks-plugin-0.3.0/mkdocs_roamlinks_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      429 2023-03-29 04:16:01.000000 mkdocs-roamlinks-plugin-0.3.0/mkdocs_roamlinks_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-03-29 04:16:01.000000 mkdocs-roamlinks-plugin-0.3.0/mkdocs_roamlinks_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       76 2023-03-29 04:16:01.000000 mkdocs-roamlinks-plugin-0.3.0/mkdocs_roamlinks_plugin.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       28 2023-03-29 04:16:01.000000 mkdocs-roamlinks-plugin-0.3.0/mkdocs_roamlinks_plugin.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       30 2023-03-29 04:16:01.000000 mkdocs-roamlinks-plugin-0.3.0/mkdocs_roamlinks_plugin.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       79 2023-03-29 04:16:01.403193 mkdocs-roamlinks-plugin-0.3.0/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1134 2023-03-29 04:15:00.000000 mkdocs-roamlinks-plugin-0.3.0/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-03-29 04:16:01.403193 mkdocs-roamlinks-plugin-0.3.0/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-03-29 04:14:07.000000 mkdocs-roamlinks-plugin-0.3.0/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5273 2023-03-29 04:14:07.000000 mkdocs-roamlinks-plugin-0.3.0/tests/test_plugin.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-19 11:13:29.861666 mkdocs-roamlinks-plugin-0.3.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1056 2023-03-11 15:33:06.000000 mkdocs-roamlinks-plugin-0.3.1/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      774 2023-04-19 11:13:29.861666 mkdocs-roamlinks-plugin-0.3.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1514 2023-04-01 07:10:16.000000 mkdocs-roamlinks-plugin-0.3.1/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-19 11:13:29.857666 mkdocs-roamlinks-plugin-0.3.1/mkdocs_roamlinks_plugin/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-03-11 15:33:06.000000 mkdocs-roamlinks-plugin-0.3.1/mkdocs_roamlinks_plugin/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7666 2023-04-19 11:09:37.000000 mkdocs-roamlinks-plugin-0.3.1/mkdocs_roamlinks_plugin/plugin.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-19 11:13:29.861666 mkdocs-roamlinks-plugin-0.3.1/mkdocs_roamlinks_plugin.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      774 2023-04-19 11:13:29.000000 mkdocs-roamlinks-plugin-0.3.1/mkdocs_roamlinks_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      429 2023-04-19 11:13:29.000000 mkdocs-roamlinks-plugin-0.3.1/mkdocs_roamlinks_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-19 11:13:29.000000 mkdocs-roamlinks-plugin-0.3.1/mkdocs_roamlinks_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       76 2023-04-19 11:13:29.000000 mkdocs-roamlinks-plugin-0.3.1/mkdocs_roamlinks_plugin.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       28 2023-04-19 11:13:29.000000 mkdocs-roamlinks-plugin-0.3.1/mkdocs_roamlinks_plugin.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       30 2023-04-19 11:13:29.000000 mkdocs-roamlinks-plugin-0.3.1/mkdocs_roamlinks_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       79 2023-04-19 11:13:29.865666 mkdocs-roamlinks-plugin-0.3.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1134 2023-04-19 11:12:24.000000 mkdocs-roamlinks-plugin-0.3.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-19 11:13:29.861666 mkdocs-roamlinks-plugin-0.3.1/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-03-29 04:14:07.000000 mkdocs-roamlinks-plugin-0.3.1/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5273 2023-04-19 11:09:24.000000 mkdocs-roamlinks-plugin-0.3.1/tests/test_plugin.py
```

### Comparing `mkdocs-roamlinks-plugin-0.3.0/LICENSE` & `mkdocs-roamlinks-plugin-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-roamlinks-plugin-0.3.0/PKG-INFO` & `mkdocs-roamlinks-plugin-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-roamlinks-plugin
-Version: 0.3.0
+Version: 0.3.1
 Summary: An MkDocs plugin
 Home-page: https://github.com/Jackiexiao/mkdocs-roamlinks-plugin
 Author: jackiexiao
 Author-email: 707610215@qq.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-roamlinks-plugin-0.3.0/README.md` & `mkdocs-roamlinks-plugin-0.3.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 | ----------------------- | ----------------------------------- |
 | `[Git Flow](git_flow.md)` | `[Git Flow](../software/git_flow.md)` |
 | `[[Git Flow]]`            | `[Git Flow](../software/git_flow.md)` |
 | `[[software/Git Flow]]`   | `[software/Git Flow](../software/git_flow.md)` |
 | `![[image.png]]`           | `![image.png](../image/imag.png)`      |
 | `[[#Heading identifiers]]` | `[Heading identifiers in HTML](#heading-identifiers-in-html)`|
 | `[[Git Flow#Heading]]`     |  `[Git Flow](../software/git_flow.md#heading)` |
-| `![[image.png|Description|800x600]]` | `![Description](image.png){ width="600"; height="800" }` |
+| `![[image.png\|Description\|800x600]]` | `![Description](image.png){ width="600"; height="800" }` |
 
 
 ## TODO
 
 - [ ] convert admonition, for example
 
 [obsidian style admonition](https://help.obsidian.md/How+to/Use+callouts)
```

### Comparing `mkdocs-roamlinks-plugin-0.3.0/mkdocs_roamlinks_plugin/plugin.py` & `mkdocs-roamlinks-plugin-0.3.1/mkdocs_roamlinks_plugin/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # For Regex, match groups are:
 #       0: Whole roamlike link e.g. [[filename#title|alias|widthxheight]]
 #       1: Filename e.g. filename.md
 #       2: #title
 #       3: alias
 #       4: width
 #       5: height
-ROAMLINK_RE = r"""\[\[(.*?)(\#.*?)?(?:\|([\D][^\|]+[\d]*))?(?:\|(\d+)(?:x(\d+))?)?\]\]"""
+ROAMLINK_RE = r"""\[\[(.*?)(\#.*?)?(?:\|([\D][^\|\]]+[\d]*))?(?:\|(\d+)(?:x(\d+))?)?\]\]"""
 
 class AutoLinkReplacer:
     def __init__(self, base_docs_url, page_url):
         self.base_docs_url = base_docs_url
         self.page_url = page_url
 
     def __call__(self, match):
```

### Comparing `mkdocs-roamlinks-plugin-0.3.0/mkdocs_roamlinks_plugin.egg-info/PKG-INFO` & `mkdocs-roamlinks-plugin-0.3.1/mkdocs_roamlinks_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-roamlinks-plugin
-Version: 0.3.0
+Version: 0.3.1
 Summary: An MkDocs plugin
 Home-page: https://github.com/Jackiexiao/mkdocs-roamlinks-plugin
 Author: jackiexiao
 Author-email: 707610215@qq.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs-roamlinks-plugin-0.3.0/setup.py` & `mkdocs-roamlinks-plugin-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-roamlinks-plugin',
-    version='0.3.0',
+    version='0.3.1',
     description='An MkDocs plugin',
     long_description='An MkDocs plugin that automagically generates relative links and convert roamlike links for foam and obsidian between markdown pages',
     keywords='mkdocs',
     url= 'https://github.com/Jackiexiao/mkdocs-roamlinks-plugin',
     author='jackiexiao',
     author_email='707610215@qq.com',
     license='MIT',
```

### Comparing `mkdocs-roamlinks-plugin-0.3.0/tests/test_plugin.py` & `mkdocs-roamlinks-plugin-0.3.1/tests/test_plugin.py`

 * *Files identical despite different names*


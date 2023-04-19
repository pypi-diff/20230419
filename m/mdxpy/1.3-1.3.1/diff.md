# Comparing `tmp/mdxpy-1.3.tar.gz` & `tmp/mdxpy-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdxpy-1.3.tar", last modified: Fri Apr 14 13:03:11 2023, max compression
+gzip compressed data, was "mdxpy-1.3.1.tar", last modified: Wed Apr 19 16:51:43 2023, max compression
```

## Comparing `mdxpy-1.3.tar` & `mdxpy-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 13:03:11.512216 mdxpy-1.3/
--rw-rw-rw-   0        0        0       88 2020-05-07 19:15:45.000000 mdxpy-1.3/.gitignore
--rw-rw-rw-   0        0        0     1099 2020-04-25 16:07:06.000000 mdxpy-1.3/LICENSE
--rw-rw-rw-   0        0        0     9292 2023-04-14 13:03:11.512216 mdxpy-1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-14 13:03:11.505698 mdxpy-1.3/images/
--rw-rw-rw-   0        0        0    65252 2020-05-07 21:01:00.000000 mdxpy-1.3/images/logo.png
-drwxrwxrwx   0        0        0        0 2023-04-14 13:03:11.512216 mdxpy-1.3/mdxpy/
--rw-rw-rw-   0        0        0      192 2022-10-09 19:46:22.000000 mdxpy-1.3/mdxpy/__init__.py
--rw-rw-rw-   0        0        0    49610 2023-04-05 20:27:37.000000 mdxpy-1.3/mdxpy/mdx.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:03:11.512216 mdxpy-1.3/mdxpy.egg-info/
--rw-rw-rw-   0        0        0     9292 2023-04-14 13:03:11.000000 mdxpy-1.3/mdxpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-14 13:03:11.000000 mdxpy-1.3/mdxpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 13:03:11.000000 mdxpy-1.3/mdxpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-14 13:03:11.000000 mdxpy-1.3/mdxpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-01-19 11:32:22.000000 mdxpy-1.3/pyproject.toml
--rw-rw-rw-   0        0        0     8260 2022-10-10 13:17:58.000000 mdxpy-1.3/readme.md
--rw-rw-rw-   0        0        0       42 2023-04-14 13:03:11.512216 mdxpy-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1334 2023-04-04 20:28:04.000000 mdxpy-1.3/setup.py
--rw-rw-rw-   0        0        0    47119 2023-04-05 20:31:29.000000 mdxpy-1.3/test.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:51:43.009164 mdxpy-1.3.1/
+-rw-rw-rw-   0        0        0       88 2020-05-07 19:15:45.000000 mdxpy-1.3.1/.gitignore
+-rw-rw-rw-   0        0        0     1099 2020-04-25 16:07:06.000000 mdxpy-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     9294 2023-04-19 16:51:43.009164 mdxpy-1.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-19 16:51:43.009164 mdxpy-1.3.1/images/
+-rw-rw-rw-   0        0        0    65252 2020-05-07 21:01:00.000000 mdxpy-1.3.1/images/logo.png
+drwxrwxrwx   0        0        0        0 2023-04-19 16:51:43.009164 mdxpy-1.3.1/mdxpy/
+-rw-rw-rw-   0        0        0      192 2022-10-09 19:46:22.000000 mdxpy-1.3.1/mdxpy/__init__.py
+-rw-rw-rw-   0        0        0    49608 2023-04-19 16:49:06.000000 mdxpy-1.3.1/mdxpy/mdx.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:51:43.009164 mdxpy-1.3.1/mdxpy.egg-info/
+-rw-rw-rw-   0        0        0     9294 2023-04-19 16:51:42.000000 mdxpy-1.3.1/mdxpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-04-19 16:51:42.000000 mdxpy-1.3.1/mdxpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 16:51:42.000000 mdxpy-1.3.1/mdxpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 16:51:42.000000 mdxpy-1.3.1/mdxpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-01-19 11:32:22.000000 mdxpy-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0     8260 2022-10-10 13:17:58.000000 mdxpy-1.3.1/readme.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 16:51:43.009164 mdxpy-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1336 2023-04-19 16:48:52.000000 mdxpy-1.3.1/setup.py
+-rw-rw-rw-   0        0        0    47119 2023-04-19 16:48:43.000000 mdxpy-1.3.1/test.py
```

### Comparing `mdxpy-1.3/LICENSE` & `mdxpy-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mdxpy-1.3/PKG-INFO` & `mdxpy-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdxpy
-Version: 1.3
+Version: 1.3.1
 Summary: A simple, yet elegant MDX library for TM1
 Home-page: https://github.com/cubewise-code/mdxpy
 Maintainer: Marius Wirtz
 Maintainer-email: MWirtz@cubewise.com
 License: MIT-LICENSE
 Keywords: MDX,TM1,IBM Cognos TM1,Planning Analytics,PA,Cognos
 Platform: any
```

### Comparing `mdxpy-1.3/images/logo.png` & `mdxpy-1.3.1/images/logo.png`

 * *Files identical despite different names*

### Comparing `mdxpy-1.3/mdxpy/mdx.py` & `mdxpy-1.3.1/mdxpy/mdx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1250,16 +1250,16 @@
         head_by_axis_position = {0: head_columns, 1: head_rows}
         tail_by_axis_position = {0: tail_columns, 1: tail_rows}
 
         mdx_axes = ",\r\n".join(
             self._axis_mdx(
                 position,
                 # default for head, tail is False for axes beyond rows and columns
-                head=head_by_axis_position.get(position, False),
-                tail=tail_by_axis_position.get(position, False),
+                head=head_by_axis_position.get(position, None),
+                tail=tail_by_axis_position.get(position, None),
                 skip_dimension_properties=skip_dimension_properties)
             for position
             in self.axes)
 
         mdx_where = "\r\nWHERE " + self._where.to_mdx() if not self._where.is_empty() else ""
 
         return f"""{mdx_with if self.calculated_members else ""}SELECT\r\n{mdx_axes}\r\nFROM [{self.cube}]{mdx_where}"""
```

### Comparing `mdxpy-1.3/mdxpy.egg-info/PKG-INFO` & `mdxpy-1.3.1/mdxpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdxpy
-Version: 1.3
+Version: 1.3.1
 Summary: A simple, yet elegant MDX library for TM1
 Home-page: https://github.com/cubewise-code/mdxpy
 Maintainer: Marius Wirtz
 Maintainer-email: MWirtz@cubewise.com
 License: MIT-LICENSE
 Keywords: MDX,TM1,IBM Cognos TM1,Planning Analytics,PA,Cognos
 Platform: any
```

### Comparing `mdxpy-1.3/readme.md` & `mdxpy-1.3.1/readme.md`

 * *Files identical despite different names*

### Comparing `mdxpy-1.3/setup.py` & `mdxpy-1.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 DESCRIPTION = open('readme.md').read()
 
 setup(
     name="mdxpy",
-    version='1.3',
+    version='1.3.1',
     maintainer='Marius Wirtz',
     maintainer_email='MWirtz@cubewise.com',
     license="MIT-LICENSE",
     url='https://github.com/cubewise-code/mdxpy',
     platforms=["any"],
     description="A simple, yet elegant MDX library for TM1",
     long_description=DESCRIPTION,
```

### Comparing `mdxpy-1.3/test.py` & `mdxpy-1.3.1/test.py`

 * *Files identical despite different names*


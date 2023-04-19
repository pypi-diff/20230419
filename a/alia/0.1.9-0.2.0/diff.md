# Comparing `tmp/alia-0.1.9.tar.gz` & `tmp/alia-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alia-0.1.9.tar", last modified: Tue Apr 18 16:52:30 2023, max compression
+gzip compressed data, was "alia-0.2.0.tar", last modified: Wed Apr 19 20:15:41 2023, max compression
```

## Comparing `alia-0.1.9.tar` & `alia-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-18 16:52:30.117637 alia-0.1.9/
--rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.1.9/LICENSE
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-18 16:52:30.117315 alia-0.1.9/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 19:00:09.000000 alia-0.1.9/README.md
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-18 16:52:30.114095 alia-0.1.9/alia/
--rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.1.9/alia/__init__.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    14246 2023-03-23 19:42:40.000000 alia-0.1.9/alia/colors.py
--rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.1.9/alia/df_tools.py
--rw-r--r--   0 aliavictor   (502) staff       (20)    26066 2023-04-18 16:51:02.000000 alia-0.1.9/alia/tools.py
-drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-18 16:52:30.116850 alia-0.1.9/alia.egg-info/
--rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-18 16:52:30.000000 alia-0.1.9/alia.egg-info/PKG-INFO
--rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-04-18 16:52:30.000000 alia-0.1.9/alia.egg-info/SOURCES.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-04-18 16:52:30.000000 alia-0.1.9/alia.egg-info/dependency_links.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       74 2023-04-18 16:52:30.000000 alia-0.1.9/alia.egg-info/requires.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-04-18 16:52:30.000000 alia-0.1.9/alia.egg-info/top_level.txt
--rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-04-18 16:52:30.117719 alia-0.1.9/setup.cfg
--rw-r--r--   0 aliavictor   (502) staff       (20)      884 2023-04-18 16:51:49.000000 alia-0.1.9/setup.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-19 20:15:41.703047 alia-0.2.0/
+-rw-r--r--   0 aliavictor   (502) staff       (20)     1066 2023-03-23 20:16:29.000000 alia-0.2.0/LICENSE
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-19 20:15:41.702651 alia-0.2.0/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 19:00:09.000000 alia-0.2.0/README.md
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-19 20:15:41.700223 alia-0.2.0/alia/
+-rw-r--r--   0 aliavictor   (502) staff       (20)        0 2023-03-23 18:58:43.000000 alia-0.2.0/alia/__init__.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    17437 2023-04-19 20:09:36.000000 alia-0.2.0/alia/colors.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)     5598 2023-04-05 19:22:12.000000 alia-0.2.0/alia/df_tools.py
+-rw-r--r--   0 aliavictor   (502) staff       (20)    27520 2023-04-19 20:13:35.000000 alia-0.2.0/alia/tools.py
+drwxr-xr-x   0 aliavictor   (502) staff       (20)        0 2023-04-19 20:15:41.702275 alia-0.2.0/alia.egg-info/
+-rw-r--r--   0 aliavictor   (502) staff       (20)      570 2023-04-19 20:15:41.000000 alia-0.2.0/alia.egg-info/PKG-INFO
+-rw-r--r--   0 aliavictor   (502) staff       (20)      228 2023-04-19 20:15:41.000000 alia-0.2.0/alia.egg-info/SOURCES.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        1 2023-04-19 20:15:41.000000 alia-0.2.0/alia.egg-info/dependency_links.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       81 2023-04-19 20:15:41.000000 alia-0.2.0/alia.egg-info/requires.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)        5 2023-04-19 20:15:41.000000 alia-0.2.0/alia.egg-info/top_level.txt
+-rw-r--r--   0 aliavictor   (502) staff       (20)       38 2023-04-19 20:15:41.703170 alia-0.2.0/setup.cfg
+-rw-r--r--   0 aliavictor   (502) staff       (20)      902 2023-04-19 20:12:22.000000 alia-0.2.0/setup.py
```

### Comparing `alia-0.1.9/LICENSE` & `alia-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alia-0.1.9/PKG-INFO` & `alia-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alia
-Version: 0.1.9
+Version: 0.2.0
 Summary: A collection of random helper tools to make life easier
 Home-page: https://github.com/aliavictor/alia
 Author: Alia
 Author-email: alia.jo.victor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alia-0.1.9/alia/colors.py` & `alia-0.2.0/alia/colors.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 from sty import fg, bg, ef, rs
 from datetime import datetime
 import re
 
 
 def color_opts(x=None):
-    """
-    When nothing is passed entire list of sty's color options with their corresponding numbers are returned.
-    Alternatively you can pass a specific number to see what color it corresponds to in sty.
-    """
+    """Previews sty colors. When nothing is passed entire list of `sty` color options with 
+    their corresponding numbers are returned. Alternatively you can pass a specific number 
+    to see what color it corresponds to in `sty`.
+    
+    Args:
+        x (int): `sty` color code to preview (optional)
+    
+    Returns:
+        Nothing (just prints)."""
     if x is None:
         for i in range(256):
             print(fg(i) + "fg({0})".format(i) + rs.all)
         return None
     else:
         print(fg(int(x)) + "fg({0})".format(x) + rs.all)
 
 
 def blue(x, ts=True, r=False):
-    """
-    x: input text
-    ts: whether or not to include current timestamp (default True)
-    r: when True returns actual compiled object, when False (default) nothing is returned only printed
-    """
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Prints the passed string in blue.
+    
+    Args:
+        x (str): Input text
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+    
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         x = f'{x} [{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}]'
     out = (
         fg(33)
         + und_rgx2.sub(
             rs.all + fg(33),
             und_rgx.sub(ef.u, bold_rgx2.sub(rs.all + fg(33), bold_rgx.sub(ef.bold, x))),
@@ -39,23 +48,27 @@
     if r:
         return out
     else:
         print(out)
 
 
 def light_blue(x, ts=True, r=False):
-    """
-    x: input text
-    ts: whether or not to include current timestamp (default True)
-    r: when True returns actual compiled object, when False (default) nothing is returned only printed
-    """
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Prints the passed string in light blue.
+
+    Args:
+        x (str): Input text
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         x = f'{x} [{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}]'
     out = (
         fg(39)
         + und_rgx2.sub(
             rs.all + fg(39),
             und_rgx.sub(ef.u, bold_rgx2.sub(rs.all + fg(39), bold_rgx.sub(ef.bold, x))),
@@ -65,23 +78,27 @@
     if r:
         return out
     else:
         print(out)
 
 
 def teal(x, ts=True, r=False):
-    """
-    x: input text
-    ts: whether or not to include current timestamp (default True)
-    r: when True returns actual compiled object, when False (default) nothing is returned only printed
-    """
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Prints the passed string in teal.
+
+    Args:
+        x (str): Input text
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         x = f'{x} [{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}]'
     out = (
         fg(30)
         + und_rgx2.sub(
             rs.all + fg(30),
             und_rgx.sub(ef.u, bold_rgx2.sub(rs.all + fg(30), bold_rgx.sub(ef.bold, x))),
@@ -91,23 +108,27 @@
     if r:
         return out
     else:
         print(out)
 
 
 def light_teal(x, ts=True, r=False):
-    """
-    x: input text
-    ts: whether or not to include current timestamp (default True)
-    r: when True returns actual compiled object, when False (default) nothing is returned only printed
-    """
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Prints the passed string in light teal.
+
+    Args:
+        x (str): Input text
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         x = f'{x} [{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}]'
     out = (
         fg(32)
         + und_rgx2.sub(
             rs.all + fg(32),
             und_rgx.sub(ef.u, bold_rgx2.sub(rs.all + fg(32), bold_rgx.sub(ef.bold, x))),
@@ -117,23 +138,27 @@
     if r:
         return out
     else:
         print(out)
 
 
 def gray(x, ts=True, r=False):
-    """
-    x: input text
-    ts: whether or not to include current timestamp (default True)
-    r: when True returns actual compiled object, when False (default) nothing is returned only printed
-    """
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Prints the passed string in gray.
+
+    Args:
+        x (str): Input text
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         x = f'{x} [{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}]'
     out = (
         fg(246)
         + und_rgx2.sub(
             rs.all + fg(246),
             und_rgx.sub(
@@ -145,23 +170,27 @@
     if r:
         return out
     else:
         print(out)
 
 
 def red(x, ts=True, r=False):
-    """
-    x: input text
-    ts: whether or not to include current timestamp (default True)
-    r: when True returns actual compiled object, when False (default) nothing is returned only printed
-    """
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Prints the passed string in red.
+
+    Args:
+        x (str): Input text
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         x = f'{x} [{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}]'
     out = (
         fg(196)
         + und_rgx2.sub(
             rs.all + fg(196),
             und_rgx.sub(
@@ -173,23 +202,27 @@
     if r:
         return out
     else:
         print(out)
 
 
 def dark_red(x, ts=True, r=False):
-    """
-    x: input text
-    ts: whether or not to include current timestamp (default True)
-    r: when True returns actual compiled object, when False (default) nothing is returned only printed
-    """
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Prints the passed string in dark red.
+
+    Args:
+        x (str): Input text
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         x = f'{x} [{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}]'
     out = (
         fg(160)
         + und_rgx2.sub(
             rs.all + fg(160),
             und_rgx.sub(
@@ -201,23 +234,27 @@
     if r:
         return out
     else:
         print(out)
 
 
 def green(x, ts=True, r=False):
-    """
-    x: input text
-    ts: whether or not to include current timestamp (default True)
-    r: when True returns actual compiled object, when False (default) nothing is returned only printed
-    """
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Prints the passed string in green.
+
+    Args:
+        x (str): Input text
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         x = f'{x} [{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}]'
     out = (
         fg(40)
         + und_rgx2.sub(
             rs.all + fg(40),
             und_rgx.sub(ef.u, bold_rgx2.sub(rs.all + fg(40), bold_rgx.sub(ef.bold, x))),
@@ -227,23 +264,27 @@
     if r:
         return out
     else:
         print(out)
 
 
 def light_green(x, ts=True, r=False):
-    """
-    x: input text
-    ts: whether or not to include current timestamp (default True)
-    r: when True returns actual compiled object, when False (default) nothing is returned only printed
-    """
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Prints the passed string in light green.
+
+    Args:
+        x (str): Input text
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         x = f'{x} [{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}]'
     out = (
         fg(30)
         + und_rgx2.sub(
             rs.all + fg(30),
             und_rgx.sub(ef.u, bold_rgx2.sub(rs.all + fg(30), bold_rgx.sub(ef.bold, x))),
@@ -253,23 +294,27 @@
     if r:
         return out
     else:
         print(out)
 
 
 def purple(x, ts=True, r=False):
-    """
-    x: input text
-    ts: whether or not to include current timestamp (default True)
-    r: when True returns actual compiled object, when False (default) nothing is returned only printed
-    """
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Prints the passed string in purple.
+
+    Args:
+        x (str): Input text
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         x = f'{x} [{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}]'
     out = (
         fg(57)
         + und_rgx2.sub(
             rs.all + fg(57),
             und_rgx.sub(ef.u, bold_rgx2.sub(rs.all + fg(57), bold_rgx.sub(ef.bold, x))),
@@ -279,23 +324,27 @@
     if r:
         return out
     else:
         print(out)
 
 
 def violet(x, ts=True, r=False):
-    """
-    x: input text
-    ts: whether or not to include current timestamp (default True)
-    r: when True returns actual compiled object, when False (default) nothing is returned only printed
-    """
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Prints the passed string in violet.
+
+    Args:
+        x (str): Input text
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         x = f'{x} [{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}]'
     out = (
         fg(63)
         + und_rgx2.sub(
             rs.all + fg(63),
             und_rgx.sub(ef.u, bold_rgx2.sub(rs.all + fg(63), bold_rgx.sub(ef.bold, x))),
@@ -305,23 +354,27 @@
     if r:
         return out
     else:
         print(out)
 
 
 def magenta(x, ts=True, r=False):
-    """
-    x: input text
-    ts: whether or not to include current timestamp (default True)
-    r: when True returns actual compiled object, when False (default) nothing is returned only printed
-    """
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Prints the passed string in magenta.
+
+    Args:
+        x (str): Input text
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         x = f'{x} [{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}]'
     out = (
         fg(198)
         + und_rgx2.sub(
             rs.all + fg(198),
             und_rgx.sub(
@@ -333,23 +386,27 @@
     if r:
         return out
     else:
         print(out)
 
 
 def pink(x, ts=True, r=False):
-    """
-    x: input text
-    ts: whether or not to include current timestamp (default True)
-    r: when True returns actual compiled object, when False (default) nothing is returned only printed
-    """
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Prints the passed string in pink.
+
+    Args:
+        x (str): Input text
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         x = f'{x} [{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}]'
     out = (
         fg(200)
         + und_rgx2.sub(
             rs.all + fg(200),
             und_rgx.sub(
@@ -361,23 +418,27 @@
     if r:
         return out
     else:
         print(out)
 
 
 def light_pink(x, ts=True, r=False):
-    """
-    x: input text
-    ts: whether or not to include current timestamp (default True)
-    r: when True returns actual compiled object, when False (default) nothing is returned only printed
-    """
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Prints the passed string in light pink.
+
+    Args:
+        x (str): Input text
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         x = f'{x} [{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}]'
     out = (
         fg(205)
         + und_rgx2.sub(
             rs.all + fg(205),
             und_rgx.sub(
@@ -389,23 +450,27 @@
     if r:
         return out
     else:
         print(out)
 
 
 def orange(x, ts=True, r=False):
-    """
-    x: input text
-    ts: whether or not to include current timestamp (default True)
-    r: when True returns actual compiled object, when False (default) nothing is returned only printed
-    """
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Prints the passed string in orange.
+
+    Args:
+        x (str): Input text
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         x = f'{x} [{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}]'
     out = (
         fg(202)
         + und_rgx2.sub(
             rs.all + fg(202),
             und_rgx.sub(
@@ -417,19 +482,28 @@
     if r:
         return out
     else:
         print(out)
 
 
 def pcolor(x, cid, ts=True, r=False):
-    """Same as all color printing functions, just lets you pass specific color ID (from color_opts())."""
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Prints the passed string in the color code that's passed.
+
+    Args:
+        x (str): Input text
+        cid (int): `sty` color integer
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         x = f'{x} [{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}]'
     out = (
         fg(cid)
         + und_rgx2.sub(
             rs.all + fg(cid),
             und_rgx.sub(
@@ -441,24 +515,31 @@
     if r:
         return out
     else:
         print(out)
 
 
 def pprint(x, ts=True, r=False):
-    """
-    Identical to other color functions, except you have more control over the string color(s).
-    Example: '<33>Hello world!</33>' would print the string 'Hello world!' in the corresponding sty color value (blue)
-    """
-    color_rgx1 = re.compile("<([\d{,2}]*)>")
-    color_rgx2 = re.compile("<\/([\d{,2]*)>")
-    bold_rgx = re.compile("(<b>)", re.IGNORECASE)
-    bold_rgx2 = re.compile("(<\/b>)", re.IGNORECASE)
-    und_rgx = re.compile("(<u>)", re.IGNORECASE)
-    und_rgx2 = re.compile("(<\/u>)", re.IGNORECASE)
+    """Identical to other color functions, except you have more control over the string color(s).
+    Example: '<33>Hello world!</33>' would print the string 'Hello world!' in the corresponding 
+    `sty` color value (blue)
+
+    Args:
+        x (str): Input text
+        ts (bool): Whether or not to include current timestamp (default True)
+        r (bool): When True returns actual compiled object, when False nothing is returned only printed
+
+    Returns:
+        Either a compiled `re` object or nothing depending on the r parameter."""
+    color_rgx1 = re.compile(r"<([\d{,2}]*)>")
+    color_rgx2 = re.compile(r"<\/([\d{,2]*)>")
+    bold_rgx = re.compile(r"(<b>)", re.IGNORECASE)
+    bold_rgx2 = re.compile(r"(<\/b>)", re.IGNORECASE)
+    und_rgx = re.compile(r"(<u>)", re.IGNORECASE)
+    und_rgx2 = re.compile(r"(<\/u>)", re.IGNORECASE)
     if ts:
         tstmp = (
             fg(246) + "[" + datetime.now().strftime("%Y-%m-%d %H:%M:%S") + "]" + rs.fg
         )
         x = f"{x} {tstmp}"
     out = color_rgx2.sub(
         rs.fg,
```

### Comparing `alia-0.1.9/alia/df_tools.py` & `alia-0.2.0/alia/df_tools.py`

 * *Files identical despite different names*

### Comparing `alia-0.1.9/alia/tools.py` & `alia-0.2.0/alia/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import base64
 import calendar
+import csv
 import difflib
 import os
 import pickle
 from datetime import datetime, date, timedelta
 
 import pandas as pd
 import pyperclip
+from cryptography.fernet import Fernet
 from dateutil.parser import parse
 
 from .colors import *
 
 
 def clipboard(string):
     """Copies text to clipboard so it can be pasted anywhere.
@@ -26,15 +28,15 @@
 
 def save_obj(obj, filename, mode="wb"):
     """Saves an object to a file by pickling it.
 
     Args:
         obj (any type): Object to save
         filename (str): Filename to save the object as
-        mode (str): Which file mode to use ('wb' by default, 'a' to append)
+        mode (str): Which file mode to use ('wb' by default, 'ab' to append)
 
     Returns:
         Nothing."""
     if ".pkl" not in filename:
         filename = f"{filename.strip()}.pkl"
 
     with open(filename, mode) as f:
@@ -53,14 +55,29 @@
         An un-pickled object."""
     with open(filename, "rb") as f:
         obj = pickle.load(f)
 
     return obj
 
 
+def read_csv(file_path):
+    """Reads a CSV file.
+
+    Args:
+        file_path (str): Path to the CSV file to read
+
+    Returns:
+        A list of dictionaries where each dictionary represents a row of the CSV."""
+    with open(file_path, "r", newline="") as file:
+        reader = csv.DictReader(file)
+        rows = [{k: v.strip() for k, v in row.items()} for row in reader]
+
+    return rows
+
+
 def b64encode(obj, encoding="utf-8"):
     """Encodes an object using the base64 library.
 
     Args:
         obj (any type): Object to encode
         encoding (str): Encoding to use (utf-8 by default)
 
@@ -68,14 +85,43 @@
         An encoded string representing the given object."""
     if isinstance(obj, str):
         return base64.b64encode(bytes(obj, encoding)).decode(encoding)
     else:
         return base64.b64encode(obj).decode(encoding)
 
 
+def encrypt(string):
+    """Uses Fernet 128-bit encryption to encrypt the passed string
+
+    Args:
+        string (str): String to encrypt
+
+    Returns:
+        encrypted_str (bytes): Encrypted string
+        key (bytes): Associated encryption key (keep private!)"""
+    key = Fernet.generate_key()
+    f = Fernet(key)
+    encrypted_str = f.encrypt(string.encode())
+
+    return encrypted_str, key
+
+
+def decrypt(encrypted_str, key):
+    """Decrypts an encrypted bytes string using Fernet.
+
+    Args:
+        encrypted_str (bytes): Encrypted bytes string to decrypt
+        key (bytes): Associated encryption key
+
+    Returns:
+        A decrypted string."""
+    f = Fernet(key)
+    return f.decrypt(encrypted_str).decode()
+
+
 def tformat(date_obj, style=None):
     """Formats a date or datetime object as a string with the given style.
     When style=None default datetime format is %Y-%m-%d %H:%M:%S and default date format is %Y-%m-%d.
 
     Args:
         date_obj (date, datetime): Date or datetime object to format
         style (str): Desired datetime format (i.e. %Y-%m-%d)
@@ -490,25 +536,31 @@
     Returns:
         True if the given number is even, False if it's odd."""
     if not isinstance(num, int):
         num = int(num.replace(",", ""))
     return (num % 2) == 0
 
 
-def regex(string, pattern):
-    """Performs a regex extration of a given string.
+def regex(string, pattern, ignore_case=False):
+    """Performs a regex extraction of a given string.
 
     Args:
         string (str, re.compile): String or compiled re object to reference
         pattern (str): Regex pattern to search the string with
+        ignore_case (bool): Whether or not to use re.IGNORECASE
 
     Returns:
         A string of the output of the passed regex."""
-    if type(pattern) == str:
-        return re.search(pattern, string).group(1)
+    if isinstance(pattern, str):
+        if ignore_case:
+            return re.search(pattern, string, re.IGNORECASE).group(1)
+        else:
+            return re.search(pattern, string).group(1)
+    elif ignore_case:
+        return pattern.search(string, re.IGNORECASE).group(1)
     else:
         return pattern.search(string).group(1)
 
 
 def str_dedupe(txt):
     """Removes duplicate substrings from a string.
```

### Comparing `alia-0.1.9/alia.egg-info/PKG-INFO` & `alia-0.2.0/alia.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alia
-Version: 0.1.9
+Version: 0.2.0
 Summary: A collection of random helper tools to make life easier
 Home-page: https://github.com/aliavictor/alia
 Author: Alia
 Author-email: alia.jo.victor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alia-0.1.9/setup.py` & `alia-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name="alia",
-    version="0.1.9",
+    version="0.2.0",
     description="A collection of random helper tools to make life easier",
     author="Alia",
     author_email="alia.jo.victor@gmail.com",
     url="https://github.com/aliavictor/alia",
     packages=find_packages(),
     install_requires=[
         # i.e. 'numpy>=1.18.0'
         "numpy",
         "pandas",
         "requests",
         "python-dotenv",
         "sty",
         "pyperclip",
         "python-dateutil",
-        "ipython"
+        "ipython",
+        "fernet"
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```


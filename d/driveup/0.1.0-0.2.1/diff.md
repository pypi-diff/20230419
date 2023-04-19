# Comparing `tmp/driveup-0.1.0.tar.gz` & `tmp/driveup-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "driveup-0.1.0.tar", last modified: Wed Apr 19 10:52:02 2023, max compression
+gzip compressed data, was "driveup-0.2.1.tar", last modified: Wed Apr 19 12:25:30 2023, max compression
```

## Comparing `driveup-0.1.0.tar` & `driveup-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 10:52:02.266795 driveup-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-04-19 10:52:02.241863 driveup-0.1.0/Driveup/
--rw-rw-rw-   0        0        0        0 2023-04-19 10:32:16.000000 driveup-0.1.0/Driveup/__init__.py
--rw-rw-rw-   0        0        0     1089 2023-04-19 09:05:25.000000 driveup-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      170 2023-04-19 10:52:02.261807 driveup-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-04-19 10:42:26.000000 driveup-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 10:52:02.258816 driveup-0.1.0/driveup.egg-info/
--rw-rw-rw-   0        0        0      170 2023-04-19 10:52:02.000000 driveup-0.1.0/driveup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-04-19 10:52:02.000000 driveup-0.1.0/driveup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 10:52:02.000000 driveup-0.1.0/driveup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 10:52:02.000000 driveup-0.1.0/driveup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 10:52:02.000000 driveup-0.1.0/driveup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 10:52:02.266795 driveup-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      290 2023-04-19 10:41:48.000000 driveup-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:25:30.934874 driveup-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:25:30.934874 driveup-0.2.1/Driveup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 12:25:19.000000 driveup-0.2.1/Driveup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-19 12:25:19.000000 driveup-0.2.1/Driveup/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 12:25:19.000000 driveup-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-19 12:25:30.934874 driveup-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 12:25:19.000000 driveup-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:25:30.934874 driveup-0.2.1/driveup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-19 12:25:30.000000 driveup-0.2.1/driveup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-19 12:25:30.000000 driveup-0.2.1/driveup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:25:30.000000 driveup-0.2.1/driveup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 12:25:30.000000 driveup-0.2.1/driveup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 12:25:30.000000 driveup-0.2.1/driveup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 12:25:30.934874 driveup-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-19 12:25:19.000000 driveup-0.2.1/setup.py
```

### Comparing `driveup-0.1.0/LICENSE` & `driveup-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Raúl Martín
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Raúl Martín
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```


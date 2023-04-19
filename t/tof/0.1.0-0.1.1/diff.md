# Comparing `tmp/tof-0.1.0.tar.gz` & `tmp/tof-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tof-0.1.0.tar", last modified: Wed Apr 19 12:53:12 2023, max compression
+gzip compressed data, was "tof-0.1.1.tar", last modified: Wed Apr 19 15:38:46 2023, max compression
```

## Comparing `tof-0.1.0.tar` & `tof-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-19 12:53:12.630288 tof-0.1.0/
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     1492 2023-04-19 10:45:19.000000 tof-0.1.0/LICENSE
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      508 2023-04-19 12:53:12.630288 tof-0.1.0/PKG-INFO
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)       70 2023-04-19 10:45:19.000000 tof-0.1.0/README.md
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      707 2023-04-19 10:48:19.000000 tof-0.1.0/pyproject.toml
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)       38 2023-04-19 12:53:12.630288 tof-0.1.0/setup.cfg
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-19 12:53:12.626288 tof-0.1.0/src/
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-19 12:53:12.626288 tof-0.1.0/src/tof/
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      110 2023-04-19 10:46:01.000000 tof-0.1.0/src/tof/__init__.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     9214 2023-04-19 10:46:01.000000 tof-0.1.0/src/tof/chopper.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      765 2023-04-19 10:46:01.000000 tof-0.1.0/src/tof/detector.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     2832 2023-04-19 10:46:01.000000 tof-0.1.0/src/tof/model.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      978 2023-04-19 10:46:01.000000 tof-0.1.0/src/tof/pulse.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      131 2023-04-19 10:46:01.000000 tof-0.1.0/src/tof/tools.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      600 2023-04-19 10:46:01.000000 tof-0.1.0/src/tof/units.py
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-19 12:53:12.626288 tof-0.1.0/src/tof.egg-info/
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      508 2023-04-19 12:53:12.000000 tof-0.1.0/src/tof.egg-info/PKG-INFO
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      464 2023-04-19 12:53:12.000000 tof-0.1.0/src/tof.egg-info/SOURCES.txt
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)        1 2023-04-19 12:53:12.000000 tof-0.1.0/src/tof.egg-info/dependency_links.txt
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)       37 2023-04-19 12:53:12.000000 tof-0.1.0/src/tof.egg-info/requires.txt
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)        4 2023-04-19 12:53:12.000000 tof-0.1.0/src/tof.egg-info/top_level.txt
+drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-19 15:38:46.813551 tof-0.1.1/
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     1492 2023-04-19 10:45:19.000000 tof-0.1.1/LICENSE
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      552 2023-04-19 15:38:46.813551 tof-0.1.1/PKG-INFO
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      114 2023-04-19 12:55:35.000000 tof-0.1.1/README.md
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      707 2023-04-19 15:38:08.000000 tof-0.1.1/pyproject.toml
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)       38 2023-04-19 15:38:46.813551 tof-0.1.1/setup.cfg
+drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-19 15:38:46.809551 tof-0.1.1/src/
+drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-19 15:38:46.813551 tof-0.1.1/src/tof/
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      110 2023-04-19 10:46:01.000000 tof-0.1.1/src/tof/__init__.py
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     9291 2023-04-19 15:26:55.000000 tof-0.1.1/src/tof/chopper.py
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      909 2023-04-19 15:26:15.000000 tof-0.1.1/src/tof/detector.py
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)    13930 2023-04-19 14:10:18.000000 tof-0.1.1/src/tof/facilities.py
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     3899 2023-04-19 15:29:51.000000 tof-0.1.1/src/tof/model.py
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     3006 2023-04-19 15:27:13.000000 tof-0.1.1/src/tof/pulse.py
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      131 2023-04-19 10:46:01.000000 tof-0.1.1/src/tof/tools.py
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      600 2023-04-19 10:46:01.000000 tof-0.1.1/src/tof/units.py
+drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-19 15:38:46.813551 tof-0.1.1/src/tof.egg-info/
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      552 2023-04-19 15:38:46.000000 tof-0.1.1/src/tof.egg-info/PKG-INFO
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      510 2023-04-19 15:38:46.000000 tof-0.1.1/src/tof.egg-info/SOURCES.txt
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)        1 2023-04-19 15:38:46.000000 tof-0.1.1/src/tof.egg-info/dependency_links.txt
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)       37 2023-04-19 15:38:46.000000 tof-0.1.1/src/tof.egg-info/requires.txt
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)        4 2023-04-19 15:38:46.000000 tof-0.1.1/src/tof.egg-info/top_level.txt
```

### Comparing `tof-0.1.0/LICENSE` & `tof-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tof-0.1.0/pyproject.toml` & `tof-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tof"
-version = "0.1.0"
+version = "0.1.1"
 description = "A simple tool to create time-of-flight chopper cascade diagrams"
 license = {text = "BSD-3-Clause"}
 authors = [{name = "Neil Vaytet"}]
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: BSD License",
```

### Comparing `tof-0.1.0/src/tof/chopper.py` & `tof-0.1.1/src/tof/chopper.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,23 +56,25 @@
     def close_times(self):
         return (self.close + self.phase) / self.omega
 
     @property
     def tofs(self):
         return units.s_to_us(self._arrival_times[self._mask])
 
-    def hist(self, bins=100):
+    def hist(self, bins=300):
         return np.histogram(self.tofs, bins=bins)
 
-    def plot(self, bins=100):
+    def plot(self, bins=300):
         h, edges = self.hist(bins=bins)
         fig, ax = plt.subplots()
         x = np.concatenate([edges, edges[-1:]])
         y = np.concatenate([[0], h, [0]])
         ax.step(x, y)
+        ax.set_xlabel('Time-of-flight (us)')
+        ax.set_ylabel('Counts')
         return Plot(fig=fig, ax=ax)
 
     def __repr__(self):
         return (
             f"Chopper(name={self.name}, distance={self.distance}, "
             f"frequency={self.frequency}, phase={self.phase}, "
             f"cutouts={len(self.open)})"
```

### Comparing `tof-0.1.0/src/tof/detector.py` & `tof-0.1.1/src/tof/detector.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 
 
 from .tools import Plot
 from .units import s_to_us
 
 
 class Detector:
-    def __init__(self, distance: float = 0.0):
+    def __init__(self, distance: float = 0.0, name: str = "detector"):
         self.distance = distance
+        self.name = name
         self._arrival_times = None
         self._mask = None
 
     @property
     def tofs(self):
         return s_to_us(self._arrival_times[self._mask])
 
-    def hist(self, bins=100):
+    def hist(self, bins=300):
         return np.histogram(self.tofs, bins=bins)
 
-    def plot(self, bins=100):
+    def plot(self, bins=300):
         h, edges = self.hist(bins=bins)
         fig, ax = plt.subplots()
         x = np.concatenate([edges, edges[-1:]])
         y = np.concatenate([[0], h, [0]])
         ax.step(x, y)
+        ax.set_xlabel('Time-of-flight (us)')
+        ax.set_ylabel('Counts')
         return Plot(fig=fig, ax=ax)
 
     def __repr__(self):
-        return f"Detector(distance={self.distance})"
+        return f"Detector(name={self.name}, distance={self.distance})"
```

### Comparing `tof-0.1.0/src/tof/units.py` & `tof-0.1.1/src/tof/units.py`

 * *Files identical despite different names*


# Comparing `tmp/tof-0.1.1.tar.gz` & `tmp/tof-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tof-0.1.1.tar", last modified: Wed Apr 19 15:38:46 2023, max compression
+gzip compressed data, was "tof-0.1.2.tar", last modified: Wed Apr 19 18:35:50 2023, max compression
```

## Comparing `tof-0.1.1.tar` & `tof-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-19 15:38:46.813551 tof-0.1.1/
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     1492 2023-04-19 10:45:19.000000 tof-0.1.1/LICENSE
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      552 2023-04-19 15:38:46.813551 tof-0.1.1/PKG-INFO
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      114 2023-04-19 12:55:35.000000 tof-0.1.1/README.md
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      707 2023-04-19 15:38:08.000000 tof-0.1.1/pyproject.toml
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)       38 2023-04-19 15:38:46.813551 tof-0.1.1/setup.cfg
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-19 15:38:46.809551 tof-0.1.1/src/
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-19 15:38:46.813551 tof-0.1.1/src/tof/
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      110 2023-04-19 10:46:01.000000 tof-0.1.1/src/tof/__init__.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     9291 2023-04-19 15:26:55.000000 tof-0.1.1/src/tof/chopper.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      909 2023-04-19 15:26:15.000000 tof-0.1.1/src/tof/detector.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)    13930 2023-04-19 14:10:18.000000 tof-0.1.1/src/tof/facilities.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     3899 2023-04-19 15:29:51.000000 tof-0.1.1/src/tof/model.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     3006 2023-04-19 15:27:13.000000 tof-0.1.1/src/tof/pulse.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      131 2023-04-19 10:46:01.000000 tof-0.1.1/src/tof/tools.py
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      600 2023-04-19 10:46:01.000000 tof-0.1.1/src/tof/units.py
-drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-19 15:38:46.813551 tof-0.1.1/src/tof.egg-info/
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      552 2023-04-19 15:38:46.000000 tof-0.1.1/src/tof.egg-info/PKG-INFO
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      510 2023-04-19 15:38:46.000000 tof-0.1.1/src/tof.egg-info/SOURCES.txt
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)        1 2023-04-19 15:38:46.000000 tof-0.1.1/src/tof.egg-info/dependency_links.txt
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)       37 2023-04-19 15:38:46.000000 tof-0.1.1/src/tof.egg-info/requires.txt
--rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)        4 2023-04-19 15:38:46.000000 tof-0.1.1/src/tof.egg-info/top_level.txt
+drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-19 18:35:50.507031 tof-0.1.2/
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      150 2023-04-19 18:21:44.000000 tof-0.1.2/.flake8
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     1492 2023-04-19 16:26:58.000000 tof-0.1.2/LICENSE
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      552 2023-04-19 18:35:50.507031 tof-0.1.2/PKG-INFO
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      114 2023-04-19 16:26:58.000000 tof-0.1.2/README.md
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      707 2023-04-19 18:33:21.000000 tof-0.1.2/pyproject.toml
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)       38 2023-04-19 18:35:50.507031 tof-0.1.2/setup.cfg
+drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-19 18:35:50.507031 tof-0.1.2/src/
+drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-19 18:35:50.507031 tof-0.1.2/src/tof/
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      239 2023-04-19 18:34:06.000000 tof-0.1.2/src/tof/__init__.py
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     2024 2023-04-19 18:34:03.000000 tof-0.1.2/src/tof/chopper.py
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     1120 2023-04-19 18:34:11.000000 tof-0.1.2/src/tof/detector.py
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)    14038 2023-04-19 18:34:36.000000 tof-0.1.2/src/tof/facilities.py
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     4198 2023-04-19 18:34:16.000000 tof-0.1.2/src/tof/model.py
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)     3176 2023-04-19 18:34:32.000000 tof-0.1.2/src/tof/pulse.py
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      240 2023-04-19 18:34:24.000000 tof-0.1.2/src/tof/tools.py
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      666 2023-04-19 18:34:46.000000 tof-0.1.2/src/tof/units.py
+drwxrwxr-x   0 nvaytet   (1000) nvaytet   (1000)        0 2023-04-19 18:35:50.507031 tof-0.1.2/src/tof.egg-info/
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      552 2023-04-19 18:35:50.000000 tof-0.1.2/src/tof.egg-info/PKG-INFO
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)      518 2023-04-19 18:35:50.000000 tof-0.1.2/src/tof.egg-info/SOURCES.txt
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)        1 2023-04-19 18:35:50.000000 tof-0.1.2/src/tof.egg-info/dependency_links.txt
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)       37 2023-04-19 18:35:50.000000 tof-0.1.2/src/tof.egg-info/requires.txt
+-rw-rw-r--   0 nvaytet   (1000) nvaytet   (1000)        4 2023-04-19 18:35:50.000000 tof-0.1.2/src/tof.egg-info/top_level.txt
```

### Comparing `tof-0.1.1/LICENSE` & `tof-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tof-0.1.1/PKG-INFO` & `tof-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tof
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple tool to create time-of-flight chopper cascade diagrams
 Author: Neil Vaytet
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tof-0.1.1/pyproject.toml` & `tof-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tof"
-version = "0.1.1"
+version = "0.1.2"
 description = "A simple tool to create time-of-flight chopper cascade diagrams"
 license = {text = "BSD-3-Clause"}
 authors = [{name = "Neil Vaytet"}]
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: BSD License",
```

### Comparing `tof-0.1.1/src/tof/detector.py` & `tof-0.1.2/src/tof/detector.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-License-Identifier: BSD-3-Clause
+# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+
 import numpy as np
 import matplotlib.pyplot as plt
 
 
 from .tools import Plot
 from .units import s_to_us
 
@@ -22,13 +25,15 @@
 
     def plot(self, bins=300):
         h, edges = self.hist(bins=bins)
         fig, ax = plt.subplots()
         x = np.concatenate([edges, edges[-1:]])
         y = np.concatenate([[0], h, [0]])
         ax.step(x, y)
+        ax.fill_between(x, 0, y, step="pre", alpha=0.5)
         ax.set_xlabel('Time-of-flight (us)')
         ax.set_ylabel('Counts')
+        ax.set_title(f"Detector: {self.name}")
         return Plot(fig=fig, ax=ax)
 
     def __repr__(self):
         return f"Detector(name={self.name}, distance={self.distance})"
```

### Comparing `tof-0.1.1/src/tof/facilities.py` & `tof-0.1.2/src/tof/facilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-License-Identifier: BSD-3-Clause
+# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+
 import numpy as np
 
 ess = {
     'time': np.array(
         [
             [1.24378109e-05, 3.35837383e-04],
             [3.73134328e-05, 7.11462527e-04],
```

### Comparing `tof-0.1.1/src/tof/model.py` & `tof-0.1.2/src/tof/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,32 @@
+# SPDX-License-Identifier: BSD-3-Clause
+# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+
 from itertools import chain
 
 import numpy as np
 from matplotlib.collections import LineCollection
 import matplotlib.pyplot as plt
 
 from .detector import Detector
-from .pulse import Pulse
 from .tools import Plot
 from .units import s_to_us
 
 
 class Model:
     def __init__(self, choppers, detectors, pulse):
         self.choppers = choppers
         if not isinstance(self.choppers, dict):
             self.choppers = {self.choppers.name: self.choppers}
         self.detectors = detectors
         if not isinstance(self.detectors, dict):
             self.detectors = {self.detectors.name: self.detectors}
         self.pulse = pulse
 
-    def ray_trace(self, npulses=1):
+    def run(self, npulses=1):
         # TODO: ray-trace multiple pulses
         components = sorted(
             chain(self.choppers.values(), self.detectors.values()),
             key=lambda c: c.distance,
         )
 
         initial_mask = np.full_like(self.pulse.birth_times, True, dtype=bool)
@@ -39,32 +41,30 @@
             tc = comp.close_times
             for i in range(len(to)):
                 m |= (t > to[i]) & (t < tc[i])
             combined = initial_mask & m
             comp._mask = combined
             initial_mask = combined
 
-        # self.detector._arrival_times = (
-        #     self.pulse.birth_times + self.detector.distance / self.pulse.speeds
-        # )
-        # self.detector._mask = initial_mask
-
-    def plot(self, nrays=1000):
+    def plot(self, max_rays=1000):
         fig, ax = plt.subplots()
-
         furthest_detector = max(self.detectors.values(), key=lambda d: d.distance)
-
         tofs = furthest_detector.tofs
         tof_max = tofs.max()
-        inds = np.random.choice(len(tofs), size=nrays, replace=False)
+        if (max_rays is not None) and (len(tofs) > max_rays):
+            inds = np.random.choice(len(tofs), size=max_rays, replace=False)
+        else:
+            inds = slice(None)
+
         # Plot rays
         x0 = s_to_us(self.pulse.birth_times[furthest_detector._mask][inds]).reshape(
             -1, 1
         )
         x1 = tofs[inds].reshape(-1, 1)
+        nrays = x0.size
         y0 = np.zeros(nrays).reshape(-1, 1)
         y1 = np.full(nrays, furthest_detector.distance).reshape(-1, 1)
         segments = np.concatenate(
             (
                 np.concatenate((x0, y0), axis=1).reshape(-1, 1, 2),
                 np.concatenate((x1, y1), axis=1).reshape(-1, 1, 2),
             ),
@@ -73,31 +73,40 @@
         coll = LineCollection(segments, cmap=plt.cm.gist_rainbow_r)
         coll.set_array(
             (self.pulse.wavelengths[furthest_detector._mask][inds] - self.pulse.lmin)
             / (self.pulse.lmax - self.pulse.lmin)
         )
         ax.add_collection(coll)
         # Plot choppers
-        for name, ch in self.choppers.items():
+        for ch in self.choppers.values():
             x0 = s_to_us(ch.open_times)
             x1 = s_to_us(ch.close_times)
             x = np.empty(3 * x0.size, dtype=x0.dtype)
             x[0::3] = x0
             x[1::3] = 0.5 * (x0 + x1)
             x[2::3] = x1
             x = np.concatenate([[0], x, [tof_max]])
             y = np.full_like(x, ch.distance)
             y[2::3] = None
             ax.plot(x, y, color="k")
-            ax.text(tof_max, ch.distance, name, ha="right", va="bottom", color="k")
+            ax.text(tof_max, ch.distance, ch.name, ha="right", va="bottom", color="k")
 
         # Plot detectors
-        for name, det in self.detectors.items():
+        for det in self.detectors.values():
             ax.plot([0, tof_max], [det.distance] * 2, color="gray", lw=3)
-            ax.text(0, det.distance, name, ha="left", va="bottom", color="gray")
+            ax.text(0, det.distance, det.name, ha="left", va="bottom", color="gray")
+
+        # Plot pulse
+        ax.plot(
+            [s_to_us(self.pulse.tmin), s_to_us(self.pulse.tmax)],
+            [0, 0],
+            color="gray",
+            lw=3,
+        )
+        ax.text(s_to_us(self.pulse.tmin), 0, "Pulse", ha="left", va="top", color="gray")
 
         ax.set_xlabel("Time-of-flight (us)")
         ax.set_ylabel("Distance (m)")
         return Plot(fig=fig, ax=ax)
 
     def __repr__(self):
         return (
```

### Comparing `tof-0.1.1/src/tof/pulse.py` & `tof-0.1.2/src/tof/pulse.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# SPDX-License-Identifier: BSD-3-Clause
+# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+
 import numpy as np
 import matplotlib.pyplot as plt
 
 from . import facilities
 from .tools import Plot
 from . import units
 
@@ -10,15 +13,15 @@
     def __init__(
         self,
         tmin: float = None,
         tmax: float = None,
         lmin: float = None,
         lmax: float = None,
         neutrons=1_000_000,
-        kind="ess",
+        kind=None,
         p_wav=None,
         p_time=None,
         sampling_resolution=10000,
     ):
         self.kind = kind
         self.neutrons = neutrons
 
@@ -74,12 +77,13 @@
         for i, (data, label) in enumerate(
             zip([self.birth_times, self.wavelengths], ["Time", "Wavelength"])
         ):
             h, edges = np.histogram(data, bins=bins)
             x = np.concatenate([edges, edges[-1:]])
             y = np.concatenate([[0], h, [0]])
             ax[i].step(x, y)
+            ax[i].fill_between(x, 0, y, step="pre", alpha=0.5)
             ax[i].set_xlabel(label)
             ax[i].set_ylabel("Counts")
         size = fig.get_size_inches()
         fig.set_size_inches(size[0] * 2, size[1])
         return Plot(fig=fig, ax=ax)
```

### Comparing `tof-0.1.1/src/tof/units.py` & `tof-0.1.2/src/tof/units.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+# SPDX-License-Identifier: BSD-3-Clause
+# Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
+
 import numpy as np
 
 mass = 1.674927471e-27  # Neutron mass in kg
 alpha = 2.5278e-4  # Neutron mass over Planck constant
 mev = 1.602176634e-22  # meV to Joule
-# angstrom = 1.0e-10  # Angstrom to meter
 
 
 def deg_to_rad(x):
     return np.radians(x)
 
 
 def rad_to_deg(x):
```

### Comparing `tof-0.1.1/src/tof.egg-info/PKG-INFO` & `tof-0.1.2/src/tof.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tof
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple tool to create time-of-flight chopper cascade diagrams
 Author: Neil Vaytet
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```


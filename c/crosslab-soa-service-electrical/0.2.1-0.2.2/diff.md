# Comparing `tmp/crosslab_soa_service_electrical-0.2.1.tar.gz` & `tmp/crosslab_soa_service_electrical-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_soa_service_electrical-0.2.1.tar", last modified: Tue Feb 21 23:52:17 2023, max compression
+gzip compressed data, was "crosslab_soa_service_electrical-0.2.2.tar", last modified: Wed Apr 19 18:30:49 2023, max compression
```

## Comparing `crosslab_soa_service_electrical-0.2.1.tar` & `crosslab_soa_service_electrical-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:52:17.881141 crosslab_soa_service_electrical-0.2.1/
--rw-r--r--   0 dev       (1000) docker-host   (967)      355 2023-02-21 23:52:17.881141 crosslab_soa_service_electrical-0.2.1/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.1/pyproject.toml
--rw-r--r--   0 dev       (1000) docker-host   (967)      585 2023-02-21 23:52:17.881141 crosslab_soa_service_electrical-0.2.1/setup.cfg
--rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.1/setup.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:52:17.881141 crosslab_soa_service_electrical-0.2.1/src/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:52:17.881141 crosslab_soa_service_electrical-0.2.1/src/crosslab/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:52:17.881141 crosslab_soa_service_electrical-0.2.1/src/crosslab/soa_services/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:52:17.881141 crosslab_soa_service_electrical-0.2.1/src/crosslab/soa_services/electrical/
--rw-r--r--   0 dev       (1000) docker-host   (967)      256 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.1/src/crosslab/soa_services/electrical/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     3604 2023-02-10 10:19:30.000000 crosslab_soa_service_electrical-0.2.1/src/crosslab/soa_services/electrical/electrical_connection_service.py
--rw-r--r--   0 dev       (1000) docker-host   (967)      745 2023-02-10 10:19:30.000000 crosslab_soa_service_electrical-0.2.1/src/crosslab/soa_services/electrical/messages.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.1/src/crosslab/soa_services/electrical/py.typed
--rw-r--r--   0 dev       (1000) docker-host   (967)      614 2023-02-10 10:19:30.000000 crosslab_soa_service_electrical-0.2.1/src/crosslab/soa_services/electrical/signal_interface.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:52:17.881141 crosslab_soa_service_electrical-0.2.1/src/crosslab/soa_services/electrical/signal_interfaces/
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.1/src/crosslab/soa_services/electrical/signal_interfaces/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)     2867 2023-02-10 10:19:30.000000 crosslab_soa_service_electrical-0.2.1/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:52:17.881141 crosslab_soa_service_electrical-0.2.1/src/crosslab_soa_service_electrical.egg-info/
--rw-r--r--   0 dev       (1000) docker-host   (967)      355 2023-02-21 23:52:17.000000 crosslab_soa_service_electrical-0.2.1/src/crosslab_soa_service_electrical.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)      747 2023-02-21 23:52:17.000000 crosslab_soa_service_electrical-0.2.1/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-02-21 23:52:17.000000 crosslab_soa_service_electrical-0.2.1/src/crosslab_soa_service_electrical.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-02-21 23:52:17.000000 crosslab_soa_service_electrical-0.2.1/src/crosslab_soa_service_electrical.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-02-21 23:52:17.000000 crosslab_soa_service_electrical-0.2.1/src/crosslab_soa_service_electrical.egg-info/top_level.txt
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:52:17.881141 crosslab_soa_service_electrical-0.2.1/tests/
--rw-r--r--   0 dev       (1000) docker-host   (967)     3751 2023-02-10 10:19:30.000000 crosslab_soa_service_electrical-0.2.1/tests/test_gpio.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:30:49.366616 crosslab_soa_service_electrical-0.2.2/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      355 2023-04-19 18:30:49.366616 crosslab_soa_service_electrical-0.2.2/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.2/pyproject.toml
+-rw-r--r--   0 dev       (1000) docker-host   (967)      585 2023-04-19 18:30:49.366616 crosslab_soa_service_electrical-0.2.2/setup.cfg
+-rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.2/setup.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:30:49.363283 crosslab_soa_service_electrical-0.2.2/src/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:30:49.363283 crosslab_soa_service_electrical-0.2.2/src/crosslab/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:30:49.363283 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:30:49.363283 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      256 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     5204 2023-04-19 13:37:16.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/electrical_connection_service.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      745 2023-02-10 10:19:30.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/messages.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/py.typed
+-rw-r--r--   0 dev       (1000) docker-host   (967)      614 2023-04-12 09:26:55.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/signal_interface.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:30:49.363283 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/signal_interfaces/
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-10 09:58:35.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/signal_interfaces/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)     2876 2023-04-19 13:37:16.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:30:49.363283 crosslab_soa_service_electrical-0.2.2/src/crosslab_soa_service_electrical.egg-info/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      355 2023-04-19 18:30:49.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab_soa_service_electrical.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)      770 2023-04-19 18:30:49.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-04-19 18:30:49.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab_soa_service_electrical.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)       25 2023-04-19 18:30:49.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab_soa_service_electrical.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-04-19 18:30:49.000000 crosslab_soa_service_electrical-0.2.2/src/crosslab_soa_service_electrical.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:30:49.363283 crosslab_soa_service_electrical-0.2.2/tests/
+-rw-r--r--   0 dev       (1000) docker-host   (967)     4076 2023-04-19 13:37:16.000000 crosslab_soa_service_electrical-0.2.2/tests/test_gpio.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      810 2023-04-19 13:37:16.000000 crosslab_soa_service_electrical-0.2.2/tests/test_standard.py
```

### Comparing `crosslab_soa_service_electrical-0.2.1/setup.cfg` & `crosslab_soa_service_electrical-0.2.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_soa_service_electrical
-version = 0.2.1
+version = 0.2.2
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab SOA Electrical Service
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
```

### Comparing `crosslab_soa_service_electrical-0.2.1/src/crosslab/soa_services/electrical/messages.py` & `crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/messages.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.1/src/crosslab/soa_services/electrical/signal_interface.py` & `crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/signal_interface.py`

 * *Files identical despite different names*

### Comparing `crosslab_soa_service_electrical-0.2.1/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py` & `crosslab_soa_service_electrical-0.2.2/src/crosslab/soa_services/electrical/signal_interfaces/gpio.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Dict, List
+from typing import Dict, List, Optional
 
 from crosslab.soa_services.electrical import (
     ConstructableSignalInterface,
     SignalInterface,
 )
 from crosslab.soa_services.electrical.messages import (
     GPIOInterfaceConfig,
@@ -18,54 +18,52 @@
     state: State
 
 
 class GPIOInterface(SignalInterface):
     driverStates: Dict[str, State]
     interfaceType = "gpio"
     signalState: State
+    configuration: GPIOInterfaceConfig  # TODO: Deprecate this
+
+    _driverState: State = "unknown"
+    _driver: Optional[str] = None
 
     def __init__(self, configuration: GPIOInterfaceConfig):
         super().__init__()
         self.driverStates = dict()
         self.signalState = "unknown"
         self.configuration = configuration
+        if configuration.get("direction", "inout") != "in":
+            self._driver = configuration.get("driver", "default")
 
     def changeDriver(self, state: State):
-        data = GPIOInterfaceData(
-            driver=self.configuration.get("driver", "pc"), state=state
-        )
-        self.emit("upstreamData", data)
-        self.downstreamData(data)
+        if self._driver:
+            self._driverState = state
+            data = GPIOInterfaceData(driver=self._driver, state=state)
+            self.emit("upstreamData", data)
+            self.downstreamData(data)
 
     def retransmit(self):
-        if "pc" in self.driverStates:
-            self.emit(
-                "upstreamData",
-                GPIOInterfaceData(
-                    driver=self.configuration.get("driver", "pc"),
-                    state=self.driverStates["pc"],
-                ),
-            )
-        else:
+        if self._driver:
             self.emit(
                 "upstreamData",
                 GPIOInterfaceData(
-                    driver=self.configuration.get("driver", "pc"),
-                    state="unknown",
+                    driver=self._driver,
+                    state=self._driverState,
                 ),
             )
 
     def downstreamData(self, data: GPIOInterfaceData):
         self.driverStates[data.get("driver", "default")] = data["state"]
         self.evaluateSignalState()
 
     def evaluateSignalState(self):
         states = set(self.driverStates.values())
 
-        newState: State = "unknown"
+        newState: State = "highZ"
         if "error" in states:
             newState = "error"
         elif "strongH" in states and "strongL" in states:
             newState = "error"
         elif "unknown" in states:
             newState = "unknown"
         elif "strongH" in states:
```

### Comparing `crosslab_soa_service_electrical-0.2.1/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt` & `crosslab_soa_service_electrical-0.2.2/src/crosslab_soa_service_electrical.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 src/crosslab/soa_services/electrical/signal_interfaces/__init__.py
 src/crosslab/soa_services/electrical/signal_interfaces/gpio.py
 src/crosslab_soa_service_electrical.egg-info/PKG-INFO
 src/crosslab_soa_service_electrical.egg-info/SOURCES.txt
 src/crosslab_soa_service_electrical.egg-info/dependency_links.txt
 src/crosslab_soa_service_electrical.egg-info/requires.txt
 src/crosslab_soa_service_electrical.egg-info/top_level.txt
-tests/test_gpio.py
+tests/test_gpio.py
+tests/test_standard.py
```


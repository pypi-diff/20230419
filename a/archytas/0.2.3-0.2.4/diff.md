# Comparing `tmp/archytas-0.2.3.tar.gz` & `tmp/archytas-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archytas-0.2.3.tar", max compression
+gzip compressed data, was "archytas-0.2.4.tar", max compression
```

## Comparing `archytas-0.2.3.tar` & `archytas-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    32472 2023-04-19 16:53:36.933413 archytas-0.2.3/LICENSE
--rw-r--r--   0        0        0     2577 2023-04-19 16:53:36.933413 archytas-0.2.3/README.md
--rw-r--r--   0        0        0        0 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/__init__.py
--rw-r--r--   0        0        0     3214 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/agent.py
--rw-r--r--   0        0        0      513 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/auth.py
--rw-r--r--   0        0        0     8468 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/demo_tools.py
--rw-r--r--   0        0        0     3583 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/prompt.py
--rw-r--r--   0        0        0     5866 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/react.py
--rw-r--r--   0        0        0     1055 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/repl.py
--rw-r--r--   0        0        0    17591 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/tool_utils.py
--rw-r--r--   0        0        0     1778 2023-04-19 16:53:36.933413 archytas-0.2.3/archytas/tools.py
--rw-r--r--   0        0        0      758 2023-04-19 16:53:36.937413 archytas-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3369 1970-01-01 00:00:00.000000 archytas-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    32472 2023-04-19 17:23:26.520856 archytas-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2577 2023-04-19 17:23:26.520856 archytas-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/__init__.py
+-rw-r--r--   0        0        0     3214 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/agent.py
+-rw-r--r--   0        0        0      513 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/auth.py
+-rw-r--r--   0        0        0     8997 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/demo_tools.py
+-rw-r--r--   0        0        0     3583 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/prompt.py
+-rw-r--r--   0        0        0     5866 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/react.py
+-rw-r--r--   0        0        0     1055 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/repl.py
+-rw-r--r--   0        0        0    17591 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/tool_utils.py
+-rw-r--r--   0        0        0     1778 2023-04-19 17:23:26.520856 archytas-0.2.4/archytas/tools.py
+-rw-r--r--   0        0        0      758 2023-04-19 17:23:26.524856 archytas-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3369 1970-01-01 00:00:00.000000 archytas-0.2.4/PKG-INFO
```

### Comparing `archytas-0.2.3/LICENSE` & `archytas-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `archytas-0.2.3/README.md` & `archytas-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `archytas-0.2.3/archytas/agent.py` & `archytas-0.2.4/archytas/agent.py`

 * *Files identical despite different names*

### Comparing `archytas-0.2.3/archytas/auth.py` & `archytas-0.2.4/archytas/auth.py`

 * *Files identical despite different names*

### Comparing `archytas-0.2.3/archytas/demo_tools.py` & `archytas-0.2.4/archytas/demo_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -294,16 +294,18 @@
 
 
 @toolset()
 class ModelSimulation:
     """
     Simple example of a SIR model simulation
     """
-    def __init__(self):
-        self.parameters = {'alpha': 0.5, 'beta': 0.25, 'gamma': 0.75, 'S': 1000, 'I': 1, 'R': 0}
+    def __init__(self, dt=0.1):
+        self._default_parameters = {'beta': 0.002, 'gamma': 0.1, 'S': 990, 'I': 10, 'R': 0}
+        self.parameters = self._default_parameters.copy()
+        self.dt = dt
 
     @tool()
     def get_model_parameters(self) -> dict:
         """
         Get the model parameters
 
         Returns:
@@ -329,20 +331,33 @@
 
         Args:
             steps (int): The number of steps to run the model for. Defaults to 100.
 
         Returns:
             dict: The model results in the form {param0: value0, param1: value1, ...}
         """
-        for i in range(steps):
-            self.parameters['S'] -= self.parameters['alpha']*self.parameters['S']*self.parameters['I']
-            self.parameters['I'] += self.parameters['alpha']*self.parameters['S']*self.parameters['I'] - self.parameters['beta']*self.parameters['I']
-            self.parameters['R'] += self.parameters['beta']*self.parameters['I']
+        S_new, I_new, R_new = self.parameters['S'], self.parameters['I'], self.parameters['R']
+        beta, gamma = self.parameters['beta'], self.parameters['gamma']
+        population = S_new + I_new + R_new
+
+        for _ in range(steps):
+            S_old, I_old, R_old = S_new, I_new, R_new
+            dS = -beta * S_old * I_old
+            dI = beta * S_old * I_old - gamma * I_old
+            dR = gamma * I_old
+
+            S_new = max(0, min(S_old + self.dt*dS, population))
+            I_new = max(0, min(I_old + self.dt*dI, population))
+            R_new = max(0, min(R_old + self.dt*dR, population))
+
+            # Ensure the total population remains constant
+            total_error = population - (S_new + I_new + R_new)
+            R_new += total_error
 
+        self.parameters['S'], self.parameters['I'], self.parameters['R'] = S_new, I_new, R_new
         return self.parameters
 
-    @tool()
     def reset_model(self):
         """
         Reset the model to the initial parameters
         """
-        self.parameters = {'alpha': 0.5, 'beta': 0.25, 'gamma': 0.75, 'S': 1000, 'I': 1, 'R': 0}
+        self.parameters = self._default_parameters.copy()
```

### Comparing `archytas-0.2.3/archytas/prompt.py` & `archytas-0.2.4/archytas/prompt.py`

 * *Files identical despite different names*

### Comparing `archytas-0.2.3/archytas/react.py` & `archytas-0.2.4/archytas/react.py`

 * *Files identical despite different names*

### Comparing `archytas-0.2.3/archytas/repl.py` & `archytas-0.2.4/archytas/repl.py`

 * *Files identical despite different names*

### Comparing `archytas-0.2.3/archytas/tool_utils.py` & `archytas-0.2.4/archytas/tool_utils.py`

 * *Files identical despite different names*

### Comparing `archytas-0.2.3/archytas/tools.py` & `archytas-0.2.4/archytas/tools.py`

 * *Files identical despite different names*

### Comparing `archytas-0.2.3/pyproject.toml` & `archytas-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archytas"
-version = "0.2.3"
+version = "0.2.4"
 description = "A library for pairing LLM agents with tools so they perform open ended tasks"
 authors = ["David Andrew Samson <david.andrew.engineer@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [project.urls]
 "Homepage" = "https://github.com/jataware/archytas"
```

### Comparing `archytas-0.2.3/PKG-INFO` & `archytas-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archytas
-Version: 0.2.3
+Version: 0.2.4
 Summary: A library for pairing LLM agents with tools so they perform open ended tasks
 License: GPL-3.0-or-later
 Author: David Andrew Samson
 Author-email: david.andrew.engineer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```


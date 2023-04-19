# Comparing `tmp/isqlab-0.3.0.tar.gz` & `tmp/isqlab-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isqlab-0.3.0.tar", last modified: Tue Apr 11 06:59:12 2023, max compression
+gzip compressed data, was "isqlab-0.3.1.tar", last modified: Wed Apr 19 07:45:40 2023, max compression
```

## Comparing `isqlab-0.3.0.tar` & `isqlab-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-11 06:59:12.607251 isqlab-0.3.0/
--rw-r--r--   0 yangys    (1000) yangys    (1000)     1151 2023-04-11 06:59:12.607251 isqlab-0.3.0/PKG-INFO
--rw-r--r--   0 yangys    (1000) yangys    (1000)      610 2023-04-11 06:59:01.000000 isqlab-0.3.0/README.md
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-11 06:59:12.607251 isqlab-0.3.0/isqlab/
--rw-r--r--   0 yangys    (1000) yangys    (1000)      442 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/__init__.py
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-11 06:59:12.607251 isqlab-0.3.0/isqlab/circuits/
--rw-r--r--   0 yangys    (1000) yangys    (1000)       44 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/circuits/__init__.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)    20874 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/circuits/quantum_circuit.py
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-11 06:59:12.607251 isqlab-0.3.0/isqlab/linkers/
--rw-r--r--   0 yangys    (1000) yangys    (1000)       38 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/linkers/__init__.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)    10356 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/linkers/torch_linker.py
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-11 06:59:12.607251 isqlab-0.3.0/isqlab/neural_networks/
--rw-r--r--   0 yangys    (1000) yangys    (1000)       42 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/neural_networks/__init__.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     8563 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/neural_networks/neural_network.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     1452 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/neural_networks/qnn_autograd.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     1351 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/neural_networks/qnn_jax.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     4143 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/neural_networks/qnn_simulator.py
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-11 06:59:12.607251 isqlab-0.3.0/isqlab/vqe/
--rw-r--r--   0 yangys    (1000) yangys    (1000)       53 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/vqe/__init__.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     6876 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/vqe/chem.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     1581 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/vqe/hamiltonian_measure.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     3499 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/vqe/kupccgsd.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)    10721 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/vqe/ucc.py
--rw-r--r--   0 yangys    (1000) yangys    (1000)     3391 2023-04-11 06:59:01.000000 isqlab-0.3.0/isqlab/vqe/uccsd.py
-drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-11 06:59:12.607251 isqlab-0.3.0/isqlab.egg-info/
--rw-r--r--   0 yangys    (1000) yangys    (1000)     1151 2023-04-11 06:59:12.000000 isqlab-0.3.0/isqlab.egg-info/PKG-INFO
--rw-r--r--   0 yangys    (1000) yangys    (1000)      614 2023-04-11 06:59:12.000000 isqlab-0.3.0/isqlab.egg-info/SOURCES.txt
--rw-r--r--   0 yangys    (1000) yangys    (1000)        1 2023-04-11 06:59:12.000000 isqlab-0.3.0/isqlab.egg-info/dependency_links.txt
--rw-r--r--   0 yangys    (1000) yangys    (1000)        7 2023-04-11 06:59:12.000000 isqlab-0.3.0/isqlab.egg-info/top_level.txt
--rw-r--r--   0 yangys    (1000) yangys    (1000)      107 2023-04-11 06:59:12.607251 isqlab-0.3.0/setup.cfg
--rw-r--r--   0 yangys    (1000) yangys    (1000)      752 2023-04-11 06:59:01.000000 isqlab-0.3.0/setup.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-19 07:45:40.497273 isqlab-0.3.1/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     1157 2023-04-19 07:45:40.497273 isqlab-0.3.1/PKG-INFO
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      616 2023-04-19 07:45:31.000000 isqlab-0.3.1/README.md
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-19 07:45:40.487273 isqlab-0.3.1/isqlab/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      511 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/__init__.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-19 07:45:40.497273 isqlab-0.3.1/isqlab/circuits/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)       65 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/circuits/__init__.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)    23487 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/circuits/quantum_circuit.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-19 07:45:40.497273 isqlab-0.3.1/isqlab/linkers/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)       38 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/linkers/__init__.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)    10356 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/linkers/torch_linker.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-19 07:45:40.497273 isqlab-0.3.1/isqlab/neural_networks/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      148 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/neural_networks/__init__.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     8563 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/neural_networks/neural_network.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     1452 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/neural_networks/qnn_autograd.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     1351 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/neural_networks/qnn_jax.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     4143 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/neural_networks/qnn_simulator.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-19 07:45:40.497273 isqlab-0.3.1/isqlab/vqe/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      130 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/vqe/__init__.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     6876 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/vqe/chem.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     4181 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/vqe/hamiltonian_measure.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     3499 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/vqe/kupccgsd.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     2534 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/vqe/symmetry_preserving.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)    10713 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/vqe/ucc.py
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     3391 2023-04-19 07:45:31.000000 isqlab-0.3.1/isqlab/vqe/uccsd.py
+drwxr-xr-x   0 yangys    (1000) yangys    (1000)        0 2023-04-19 07:45:40.497273 isqlab-0.3.1/isqlab.egg-info/
+-rw-r--r--   0 yangys    (1000) yangys    (1000)     1157 2023-04-19 07:45:40.000000 isqlab-0.3.1/isqlab.egg-info/PKG-INFO
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      648 2023-04-19 07:45:40.000000 isqlab-0.3.1/isqlab.egg-info/SOURCES.txt
+-rw-r--r--   0 yangys    (1000) yangys    (1000)        1 2023-04-19 07:45:40.000000 isqlab-0.3.1/isqlab.egg-info/dependency_links.txt
+-rw-r--r--   0 yangys    (1000) yangys    (1000)        7 2023-04-19 07:45:40.000000 isqlab-0.3.1/isqlab.egg-info/top_level.txt
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      107 2023-04-19 07:45:40.497273 isqlab-0.3.1/setup.cfg
+-rw-r--r--   0 yangys    (1000) yangys    (1000)      752 2023-04-19 07:45:31.000000 isqlab-0.3.1/setup.py
```

### Comparing `isqlab-0.3.0/PKG-INFO` & `isqlab-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isqlab
-Version: 0.3.0
+Version: 0.3.1
 Summary: application modules for isq
 Home-page: UNKNOWN
 Author: Yusheng Yang
 Author-email: yangys@arclightquantum.com
 License: UNKNOWN
 Description: Isqlab is a Python library for isQ.
         
@@ -21,17 +21,17 @@
         ## Installation
         
         Isqlab requires Python version 3.8 and above. Installation of isqlab can be done using:
         
         ```console
         git clone http://www.arclighttest.cn:8090/yangys/isqlab.git
         cd isqlab
-        python setup.py bdist_wheel
+        python setup.py bdist_wheel sdist
         cd dist
-        pip install isqlab-0.1.0-py3-none-any.whl
+        pip install isqlab-0.3.1-py3-none-any.whl
         ```
         
         ## Getting started
         
         See examples.
         
         ## Authors
```

### Comparing `isqlab-0.3.0/README.md` & `isqlab-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 ## Installation
 
 Isqlab requires Python version 3.8 and above. Installation of isqlab can be done using:
 
 ```console
 git clone http://www.arclighttest.cn:8090/yangys/isqlab.git
 cd isqlab
-python setup.py bdist_wheel
+python setup.py bdist_wheel sdist
 cd dist
-pip install isqlab-0.1.0-py3-none-any.whl
+pip install isqlab-0.3.1-py3-none-any.whl
 ```
 
 ## Getting started
 
 See examples.
 
 ## Authors
```

### Comparing `isqlab-0.3.0/isqlab/circuits/quantum_circuit.py` & `isqlab-0.3.1/isqlab/circuits/quantum_circuit.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,34 +2,41 @@
 # (C) Copyright ArcLight Quantum 2023.
 # This code is licensed under the MIT License.
 
 """Quantum circuit object."""
 
 from isq import LocalDevice, quantumCor
 from isq.device import Device
+from isq.drawer import Drawer
 from typing import Callable, Union, Sequence, Literal, Optional
 from functools import partial
 import numpy as np
 import itertools
 import time
 
 
 try:
     import jax.numpy as jnp
     HAS_JAX = True
 except Exception:
     HAS_JAX = False
 
 try:
+    import torch
+    HAS_TORCH = True
+except Exception:
+    HAS_TORCH = False
+
+try:
     from autograd import numpy as anp
     HAS_AUTOGRAD = True
 except Exception:
     HAS_AUTOGRAD = False
 
-SIMULATOR_METHOD = Literal["simulator", "autograd", "jax"]
+SIMULATOR_METHOD = Literal["simulator", "autograd", "jax", "torch", "pytorch"]
 
 
 class QuantumCircuitError(Exception):
     """
     Quantum circuits error.
     """
     pass
@@ -41,18 +48,18 @@
 
     """
 
     def __init__(
         self,
         num_qubits: Optional[int] = None,
         backend: Device = LocalDevice(),
-        method: SIMULATOR_METHOD = "autograd",  # simulator, autograd, jax
+        method: SIMULATOR_METHOD = "autograd",
         dict_format: bool = False,
-        run_time: int = 600,
         sleep_time: int = 3,
+        run_time: Optional[int] = None,
     ) -> None:
 
         self.use_hardware = False
         self.run_time = None
         self.sleep_time = None
         if not isinstance(backend, LocalDevice):
             self.use_hardware = True
@@ -64,14 +71,18 @@
             if not HAS_JAX:
                 raise QuantumCircuitError("Jax is not installed.")
 
         if method == "autograd":
             if not HAS_AUTOGRAD:
                 raise QuantumCircuitError("Autograd is not installed.")
 
+        if method in ["torch", "pytorch"]:
+            if not HAS_TORCH:
+                raise QuantumCircuitError("Pytorch is not installed.")
+
         self._circuit_recording = []  # to record isqfile
         self._measure_recording = []  # to recoed measurement
 
         self.backend = backend
         self.method = method
         self.dict_format = dict_format
 
@@ -94,19 +105,29 @@
     def __getitem__(self, key: int) -> str:
         return self.circuit[key]
 
     @property
     def circuit(self) -> list:
         return self._circuit_recording + self._measure_recording
 
+    def qir(self, **kw) -> str:
+        if kw is None:
+            return self.backend.compile_to_ir(self.__repr__())
+        self.backend.compile_with_par(self.__repr__(), **kw)
+        return self.backend.get_ir()
+
     def extend(
         self,
         circuit: "QuantumCircuit",
+        remove_qbit_def: bool = True,
     ) -> None:
-        self._circuit_recording.extend(circuit._circuit_recording[1:])
+        if remove_qbit_def:
+            self._circuit_recording.extend(circuit._circuit_recording[1:])
+        else:
+            self._circuit_recording.extend(circuit._circuit_recording)
 
     def insert(
         self,
         start: int,
         end: int,
         reverse: bool = True
     ) -> None:
@@ -132,139 +153,224 @@
         func(*args, **kw)
         end = self.idx
         insert_list = self[start:end][::-1]
         for i in range(end-start):
             _ = self._circuit_recording.pop()
         self._circuit_recording.extend(insert_list)
 
-    def _qbit_init(self, num_qubits: int) -> None:
+    def _qbit_init(
+        self,
+        num_qubits: int,
+    ) -> None:
         """
         Qubits initialization.
         """
         if num_qubits < 0:
             raise QuantumCircuitError(
                 f"Number of inputs cannot be negative: {num_qubits}!")
 
         self._circuit_recording.append(f"qbit q[{num_qubits}];")
 
-    def _one_qubit_op(self, qubit_idx: int, operation: str) -> None:
+    def _one_qubit_op(
+        self,
+        qubit_idx: int,
+        operation: str,
+    ) -> None:
         """
         General one qubit operations.
         """
         self._circuit_recording.append(f"{operation}(q[{qubit_idx}]);")
 
-    def h(self, qubit_idx: int):
+    def h(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "H"
         self._one_qubit_op(qubit_idx, operation)
 
-    def x(self, qubit_idx: int):
+    def x(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "X"
         self._one_qubit_op(qubit_idx, operation)
 
-    def y(self, qubit_idx: int):
+    def y(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "Y"
         self._one_qubit_op(qubit_idx, operation)
 
-    def z(self, qubit_idx: int):
+    def z(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "Z"
         self._one_qubit_op(qubit_idx, operation)
 
-    def s(self, qubit_idx: int):
+    def s(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "S"
         self._one_qubit_op(qubit_idx, operation)
 
-    def sd(self, qubit_idx: int):
+    def sd(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "SD"
         self._one_qubit_op(qubit_idx, operation)
 
-    def t(self, qubit_idx: int):
+    def t(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "T"
         self._one_qubit_op(qubit_idx, operation)
 
-    def td(self, qubit_idx: int):
+    def td(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "TD"
         self._one_qubit_op(qubit_idx, operation)
 
-    def x2p(self, qubit_idx: int):
+    def x2p(
+        self,
+        qubit_idx: int,
+    ) -> None:
         """X rotate pi/2"""
         operation = "X2P"
         self._one_qubit_op(qubit_idx, operation)
 
-    def x2m(self, qubit_idx: int):
+    def x2m(
+        self,
+        qubit_idx: int,
+    ) -> None:
         """X rotate -pi/2"""
         operation = "X2M"
         self._one_qubit_op(qubit_idx, operation)
 
-    def y2p(self, qubit_idx: int):
+    def y2p(
+        self,
+        qubit_idx: int,
+    ) -> None:
         """Y rotate pi/2"""
         operation = "Y2P"
         self._one_qubit_op(qubit_idx, operation)
 
-    def y2m(self, qubit_idx: int):
+    def y2m(
+        self,
+        qubit_idx: int,
+    ) -> None:
         """Y rotate -pi/2"""
         operation = "Y2M"
         self._one_qubit_op(qubit_idx, operation)
 
-    def m(self, qubit_idx: int):
+    def m(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "M"
         self._one_qubit_op(qubit_idx, operation)
 
-    def H(self, qubit_idx: int):
+    def H(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "H"
         self._one_qubit_op(qubit_idx, operation)
 
-    def X(self, qubit_idx: int):
+    def X(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "X"
         self._one_qubit_op(qubit_idx, operation)
 
-    def Y(self, qubit_idx: int):
+    def Y(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "Y"
         self._one_qubit_op(qubit_idx, operation)
 
-    def Z(self, qubit_idx: int):
+    def Z(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "Z"
         self._one_qubit_op(qubit_idx, operation)
 
-    def S(self, qubit_idx: int):
+    def S(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "S"
         self._one_qubit_op(qubit_idx, operation)
 
-    def SD(self, qubit_idx: int):
+    def SD(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "SD"
         self._one_qubit_op(qubit_idx, operation)
 
-    def T(self, qubit_idx: int):
+    def T(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "T"
         self._one_qubit_op(qubit_idx, operation)
 
-    def TD(self, qubit_idx: int):
+    def TD(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "TD"
         self._one_qubit_op(qubit_idx, operation)
 
-    def X2P(self, qubit_idx: int):
+    def X2P(
+        self,
+        qubit_idx: int,
+    ) -> None:
         """X rotate pi/2"""
         operation = "X2P"
         self._one_qubit_op(qubit_idx, operation)
 
-    def X2M(self, qubit_idx: int):
+    def X2M(
+        self,
+        qubit_idx: int,
+    ) -> None:
         """X rotate -pi/2"""
         operation = "X2M"
         self._one_qubit_op(qubit_idx, operation)
 
-    def Y2P(self, qubit_idx: int):
+    def Y2P(
+        self,
+        qubit_idx: int,
+    ) -> None:
         """Y rotate pi/2"""
         operation = "Y2P"
         self._one_qubit_op(qubit_idx, operation)
 
-    def Y2M(self, qubit_idx: int):
+    def Y2M(
+        self,
+        qubit_idx: int,
+    ) -> None:
         """Y rotate -pi/2"""
         operation = "Y2M"
         self._one_qubit_op(qubit_idx, operation)
 
-    def M(self, qubit_idx: int):
+    def M(
+        self,
+        qubit_idx: int,
+    ) -> None:
         operation = "M"
         self._one_qubit_op(qubit_idx, operation)
 
     def _two_qubits_op(
         self,
         qubit_control: int,
         qubit_target: int,
@@ -272,43 +378,75 @@
     ) -> None:
         """
         General two qubit operations.
         """
         self._circuit_recording.append(
             f"{operation}(q[{qubit_control}], q[{qubit_target}]);")
 
-    def cnot(self, qubit_control: int, qubit_target: int):
+    def cnot(
+        self,
+        qubit_control: int,
+        qubit_target: int,
+    ) -> None:
         operation = "CNOT"
         self._two_qubits_op(qubit_control, qubit_target, operation)
 
-    def cx(self, qubit_control: int, qubit_target: int):
+    def cx(
+        self,
+        qubit_control: int,
+        qubit_target: int,
+    ) -> None:
         operation = "CX"
         self._two_qubits_op(qubit_control, qubit_target, operation)
 
-    def cy(self, qubit_control: int, qubit_target: int):
+    def cy(
+        self,
+        qubit_control: int,
+        qubit_target: int,
+    ) -> None:
         operation = "CY"
         self._two_qubits_op(qubit_control, qubit_target, operation)
 
-    def cz(self, qubit_control: int, qubit_target: int):
+    def cz(
+        self,
+        qubit_control: int,
+        qubit_target: int,
+    ) -> None:
         operation = "CZ"
         self._two_qubits_op(qubit_control, qubit_target, operation)
 
-    def CNOT(self, qubit_control: int, qubit_target: int):
+    def CNOT(
+        self,
+        qubit_control: int,
+        qubit_target: int,
+    ) -> None:
         operation = "CNOT"
         self._two_qubits_op(qubit_control, qubit_target, operation)
 
-    def CX(self, qubit_control: int, qubit_target: int):
+    def CX(
+        self,
+        qubit_control: int,
+        qubit_target: int,
+    ) -> None:
         operation = "CX"
         self._two_qubits_op(qubit_control, qubit_target, operation)
 
-    def CY(self, qubit_control: int, qubit_target: int):
+    def CY(
+        self,
+        qubit_control: int,
+        qubit_target: int,
+    ) -> None:
         operation = "CY"
         self._two_qubits_op(qubit_control, qubit_target, operation)
 
-    def CZ(self, qubit_control: int, qubit_target: int):
+    def CZ(
+        self,
+        qubit_control: int,
+        qubit_target: int,
+    ) -> None:
         operation = "CZ"
         self._two_qubits_op(qubit_control, qubit_target, operation)
 
     def _rotate_gate(
         self,
         param: Union[float, str],
         qubit_idx: int,
@@ -316,35 +454,59 @@
     ) -> None:
         """
         General rotion operations.
         """
         self._circuit_recording.append(
             f"{operation}({param}, q[{qubit_idx}]);")
 
-    def rx(self, param: Union[float, str], qubit_idx: int):
+    def rx(
+        self,
+        param: Union[float, str],
+        qubit_idx: int,
+    ) -> None:
         operation = "RX"
         self._rotate_gate(param, qubit_idx, operation)
 
-    def ry(self, param: Union[float, str], qubit_idx: int):
+    def ry(
+        self,
+        param: Union[float, str],
+        qubit_idx: int,
+    ) -> None:
         operation = "RY"
         self._rotate_gate(param, qubit_idx, operation)
 
-    def rz(self, param: Union[float, str], qubit_idx: int):
+    def rz(
+        self,
+        param: Union[float, str],
+        qubit_idx: int,
+    ) -> None:
         operation = "RZ"
         self._rotate_gate(param, qubit_idx, operation)
 
-    def RX(self, param: Union[float, str], qubit_idx: int):
+    def RX(
+        self,
+        param: Union[float, str],
+        qubit_idx: int,
+    ) -> None:
         operation = "RX"
         self._rotate_gate(param, qubit_idx, operation)
 
-    def RY(self, param: Union[float, str], qubit_idx: int):
+    def RY(
+        self,
+        param: Union[float, str],
+        qubit_idx: int,
+    ) -> None:
         operation = "RY"
         self._rotate_gate(param, qubit_idx, operation)
 
-    def RZ(self, param: Union[float, str], qubit_idx: int):
+    def RZ(
+        self,
+        param: Union[float, str],
+        qubit_idx: int,
+    ) -> None:
         operation = "RZ"
         self._rotate_gate(param, qubit_idx, operation)
 
     def add_gate(
         self,
         gate_name: str,
         matrix: Union[list, np.ndarray],
@@ -413,36 +575,40 @@
 
         elif self.method == "autograd":
             return self.backend.probs(self.__repr__(), mod=0, **params)
 
         elif self.method == "jax":
             return self.backend.probs(self.__repr__(), mod=1, **params)
 
+        elif self.method in ["torch", "pytorch"]:
+            return self.backend.probs(self.__repr__(), mod=2, **params)
+
         else:
             raise NotImplementedError("Undefined method.")
 
     def _measure_hardware(self, **params) -> dict:
         """Using quantum hardwares."""
         from isq import TaskState
         task = self.backend.run(self.__repr__(), **params)
         self.task_cancel = task.cancel
         # Expose the cancel API
-        end_time = time.time() + self.run_time
-        while task.state == TaskState.WAIT and time.time() < end_time:
-            if task.state == TaskState.COMPLETE:
-                task.result()
-            elif task.state == TaskState.CANCEL:
-                raise QuantumCircuitError("Task was canceled.")
-            elif task.state == TaskState.FAIL:
-                raise QuantumCircuitError("Task was failed.")
+        start_time = time.time()
+        while task.state == TaskState.WAIT:
+            task.result()
             # Wait for a period of time before doing an http request
             time.sleep(self.sleep_time)
+            if self.run_time is not None:
+                if time.time() > start_time + self.run_time:
+                    break
         return task
 
-    def _dict2array(self, result_dicts: dict) -> np.ndarray:
+    def _dict2array(
+        self,
+        result_dicts: dict,
+    ) -> np.ndarray:
         """
         Transfer measurement results from Dict to Array.
         """
         shots = self.backend.shots
         # results_list = [0.0] * (2 ** self._len_qubit_measure)
         results_arrays = np.zeros(2 ** self._len_qubit_measure)
 
@@ -464,34 +630,35 @@
             gates = gate_name[0::2]
             locations = [int(location) for location in gate_name[1::2]]
 
             if not len(locations) == len(set(locations)):
                 raise ValueError("Error pauli measurement.")
 
             for i in range(len(gates)):
-                if gates[i] == 'X' or gates[i] == 'x':
+                if gates[i] in ["x", "X"]:
                     self._measure_recording.append(
                         f"H(q[{locations[i]}]);",
                     )
                     self._measure_recording.append(
                         f"M(q[{locations[i]}]);",
                     )
-                elif gates[i] == 'Y' or gates[i] == 'y':
+                elif gates[i] in ["y", "Y"]:
                     self._measure_recording.append(
                         f"X2P(q[{locations[i]}]);",
                     )
                     self._measure_recording.append(
                         f"M(q[{locations[i]}]);",
                     )
-                elif gates[i] == 'Z' or gates[i] == 'z':
+                elif gates[i] in ["z", "Z"]:
                     self._measure_recording.append(
                         f"M(q[{locations[i]}]);",
                     )
                 else:
-                    raise ValueError("Please input correct Pauli gates.")
+                    raise ValueError(
+                        f"Please input correct Pauli gates instead of {gates[i]}.")
 
         elif format == "openfermion":
             for single_gate in gate_name:
                 if single_gate[1] == "X":
                     self._measure_recording.append(
                         f"H(q[{single_gate[0]}]);",
                     )
@@ -540,23 +707,33 @@
             return result
 
         elif self.method == "autograd":
             measure_result_list = self.backend.probs(
                 self.__repr__(), mod=0, **params)
             parity = [(-1) ** (str(bin(int(index))).count("1") % 2)
                       for index in range(len(measure_result_list))]
-            return anp.dot(anp.array(measure_result_list), anp.array(parity))
+            return anp.dot(measure_result_list, anp.array(parity))
 
         elif self.method == "jax":
             measure_result_list = self.backend.probs(
                 self.__repr__(), mod=1, **params)
             parity = [(-1) ** (str(bin(int(index))).count("1") % 2)
                       for index in range(len(measure_result_list))]
             return jnp.vdot(jnp.array(measure_result_list), jnp.array(parity))
 
+        elif self.method in ["torch", "pytorch"]:
+            measure_result_list = self.backend.probs(
+                self.__repr__(), mod=2, **params)
+            parity = [(-1) ** (str(bin(int(index))).count("1") % 2)
+                      for index in range(len(measure_result_list))]
+            return torch.dot(
+                measure_result_list,
+                torch.tensor(parity).type_as(measure_result_list),
+            )
+
         else:
             raise NotImplementedError("Undefined method.")
 
     def str2circuit(
         self,
         isq_str: str,
         remove_qbit_def: bool = False,
@@ -673,7 +850,15 @@
 
     def cmt(self, comments: Optional[str] = None) -> None:
         """Add comments"""
         if comments is None:
             self._circuit_recording.append("")
         elif isinstance(comments, str):
             self._circuit_recording.append(f"// {comments}")
+
+    def draw(
+        self,
+        show_param: bool = False,
+        **kw,
+    ) -> None:
+        drawer = Drawer(showparam=show_param)
+        drawer.plot(self.qir(**kw))
```

### Comparing `isqlab-0.3.0/isqlab/linkers/torch_linker.py` & `isqlab-0.3.1/isqlab/linkers/torch_linker.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.0/isqlab/neural_networks/neural_network.py` & `isqlab-0.3.1/isqlab/neural_networks/neural_network.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.0/isqlab/neural_networks/qnn_autograd.py` & `isqlab-0.3.1/isqlab/neural_networks/qnn_autograd.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.0/isqlab/neural_networks/qnn_jax.py` & `isqlab-0.3.1/isqlab/neural_networks/qnn_jax.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.0/isqlab/neural_networks/qnn_simulator.py` & `isqlab-0.3.1/isqlab/neural_networks/qnn_simulator.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.0/isqlab/vqe/chem.py` & `isqlab-0.3.1/isqlab/vqe/chem.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.0/isqlab/vqe/kupccgsd.py` & `isqlab-0.3.1/isqlab/vqe/kupccgsd.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.0/isqlab/vqe/ucc.py` & `isqlab-0.3.1/isqlab/vqe/ucc.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         n_qubits: int,
         n_elec: int,
         init_state: Union[QuantumCircuit, str] = "hf",
     ) -> QuantumCircuit:
 
         if isinstance(init_state, QuantumCircuit):
             return init_state
-        if init_state == "hf" or init_state == "HF":
+        if init_state in ["hf", "Hf", "HF"]:
             circuit = QuantumCircuit(n_qubits)
             for i in range(n_elec // 2):
                 circuit.X(i)
                 circuit.X(n_qubits // 2 + i)
 
         return circuit
```

### Comparing `isqlab-0.3.0/isqlab/vqe/uccsd.py` & `isqlab-0.3.1/isqlab/vqe/uccsd.py`

 * *Files identical despite different names*

### Comparing `isqlab-0.3.0/isqlab.egg-info/PKG-INFO` & `isqlab-0.3.1/isqlab.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isqlab
-Version: 0.3.0
+Version: 0.3.1
 Summary: application modules for isq
 Home-page: UNKNOWN
 Author: Yusheng Yang
 Author-email: yangys@arclightquantum.com
 License: UNKNOWN
 Description: Isqlab is a Python library for isQ.
         
@@ -21,17 +21,17 @@
         ## Installation
         
         Isqlab requires Python version 3.8 and above. Installation of isqlab can be done using:
         
         ```console
         git clone http://www.arclighttest.cn:8090/yangys/isqlab.git
         cd isqlab
-        python setup.py bdist_wheel
+        python setup.py bdist_wheel sdist
         cd dist
-        pip install isqlab-0.1.0-py3-none-any.whl
+        pip install isqlab-0.3.1-py3-none-any.whl
         ```
         
         ## Getting started
         
         See examples.
         
         ## Authors
```

### Comparing `isqlab-0.3.0/isqlab.egg-info/SOURCES.txt` & `isqlab-0.3.1/isqlab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,10 @@
 isqlab/neural_networks/qnn_autograd.py
 isqlab/neural_networks/qnn_jax.py
 isqlab/neural_networks/qnn_simulator.py
 isqlab/vqe/__init__.py
 isqlab/vqe/chem.py
 isqlab/vqe/hamiltonian_measure.py
 isqlab/vqe/kupccgsd.py
+isqlab/vqe/symmetry_preserving.py
 isqlab/vqe/ucc.py
 isqlab/vqe/uccsd.py
```

### Comparing `isqlab-0.3.0/setup.py` & `isqlab-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     # "pyscf",
     # "openfermion",
     # "openfermionpyscf",
 ]
 
 setup(
     name="isqlab",
-    version="0.3.0",
+    version="0.3.1",
     description="application modules for isq",
     platforms="python 3.8+",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Yusheng Yang",
     author_email="yangys@arclightquantum.com",
     packages=find_packages(where="."),
```


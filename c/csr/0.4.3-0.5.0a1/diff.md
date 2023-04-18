# Comparing `tmp/csr-0.4.3.tar.gz` & `tmp/csr-0.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csr-0.4.3.tar", last modified: Mon Aug  1 04:01:15 2022, max compression
+gzip compressed data, was "csr-0.5.0a1.tar", last modified: Tue Apr 18 22:24:18 2023, max compression
```

## Comparing `csr-0.4.3.tar` & `csr-0.5.0a1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      164 2022-08-01 04:00:59.239462 csr-0.4.3/.editorconfig
--rw-r--r--   0        0        0      223 2022-08-01 04:00:59.239462 csr-0.4.3/.gitignore
--rw-r--r--   0        0        0      147 2022-08-01 04:00:59.239462 csr-0.4.3/.readthedocs.yml
--rw-r--r--   0        0        0     1089 2022-08-01 04:00:59.239462 csr-0.4.3/LICENSE
--rw-r--r--   0        0        0      834 2022-08-01 04:00:59.239462 csr-0.4.3/README.md
--rw-r--r--   0        0        0     3358 2022-08-01 04:00:59.239462 csr-0.4.3/Timings.py
--rw-r--r--   0        0        0       48 2022-08-01 04:00:59.239462 csr-0.4.3/codecov.yml
--rw-r--r--   0        0        0     1447 2022-08-01 04:00:59.239462 csr-0.4.3/conftest.py
--rw-r--r--   0        0        0      252 2022-08-01 04:00:59.239462 csr-0.4.3/csr/__init__.py
--rw-r--r--   0        0        0     1490 2022-08-01 04:00:59.239462 csr-0.4.3/csr/_rows.py
--rw-r--r--   0        0        0     1027 2022-08-01 04:00:59.239462 csr-0.4.3/csr/_struct.py
--rw-r--r--   0        0        0      519 2022-08-01 04:00:59.239462 csr-0.4.3/csr/_util.py
--rw-r--r--   0        0        0     2554 2022-08-01 04:00:59.239462 csr-0.4.3/csr/_wiring.py
--rw-r--r--   0        0        0     1778 2022-08-01 04:00:59.239462 csr-0.4.3/csr/constructors.py
--rw-r--r--   0        0        0    21775 2022-08-01 04:00:59.239462 csr-0.4.3/csr/csr.py
--rw-r--r--   0        0        0      363 2022-08-01 04:00:59.243462 csr-0.4.3/csr/kernel.py
--rw-r--r--   0        0        0     2887 2022-08-01 04:00:59.243462 csr-0.4.3/csr/kernels/__init__.py
--rw-r--r--   0        0        0      173 2022-08-01 04:00:59.243462 csr-0.4.3/csr/kernels/mkl/__init__.py
--rw-r--r--   0        0        0      497 2022-08-01 04:00:59.243462 csr-0.4.3/csr/kernels/mkl/_api.py
--rw-r--r--   0        0        0     3269 2022-08-01 04:00:59.243462 csr-0.4.3/csr/kernels/mkl/handle.py
--rw-r--r--   0        0        0     5567 2022-08-01 04:00:59.243462 csr-0.4.3/csr/kernels/mkl/mkl_ops.c
--rw-r--r--   0        0        0     1060 2022-08-01 04:00:59.243462 csr-0.4.3/csr/kernels/mkl/mkl_ops.h
--rw-r--r--   0        0        0      733 2022-08-01 04:00:59.243462 csr-0.4.3/csr/kernels/mkl/multiply.py
--rw-r--r--   0        0        0     1145 2022-08-01 04:00:59.243462 csr-0.4.3/csr/kernels/numba/__init__.py
--rw-r--r--   0        0        0     3235 2022-08-01 04:00:59.243462 csr-0.4.3/csr/kernels/numba/multiply.py
--rw-r--r--   0        0        0      804 2022-08-01 04:00:59.243462 csr-0.4.3/csr/kernels/scipy.py
--rw-r--r--   0        0        0     6566 2022-08-01 04:00:59.243462 csr-0.4.3/csr/structure.py
--rw-r--r--   0        0        0     2601 2022-08-01 04:00:59.243462 csr-0.4.3/csr/test_utils.py
--rw-r--r--   0        0        0      886 2022-08-01 04:00:59.243462 csr-0.4.3/csr/transform.py
--rw-r--r--   0        0        0     1089 2022-08-01 04:00:59.243462 csr-0.4.3/docs/conf.py
--rw-r--r--   0        0        0     1644 2022-08-01 04:00:59.243462 csr-0.4.3/docs/csr.rst
--rw-r--r--   0        0        0     1170 2022-08-01 04:00:59.243462 csr-0.4.3/docs/index.rst
--rw-r--r--   0        0        0     3859 2022-08-01 04:00:59.243462 csr-0.4.3/docs/kernels.rst
--rw-r--r--   0        0        0       70 2022-08-01 04:00:59.243462 csr-0.4.3/jupytext.toml
--rw-r--r--   0        0        0      155 2022-08-01 04:00:59.243462 csr-0.4.3/min-constraints.txt
--rw-r--r--   0        0        0       72 2022-08-01 04:00:59.243462 csr-0.4.3/mkl-devel.yml
--rw-r--r--   0        0        0     1097 2022-08-01 04:00:59.243462 csr-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      466 2022-08-01 04:00:59.243462 csr-0.4.3/pytest.ini
--rw-r--r--   0        0        0      198 2022-08-01 04:00:59.243462 csr-0.4.3/setup.cfg
--rw-r--r--   0        0        0     1776 2022-08-01 04:00:59.243462 csr-0.4.3/tasks.py
--rw-r--r--   0        0        0     1020 2022-08-01 04:00:59.243462 csr-0.4.3/tests/test_active_kernel.py
--rw-r--r--   0        0        0     6653 2022-08-01 04:00:59.243462 csr-0.4.3/tests/test_attributes.py
--rw-r--r--   0        0        0      411 2022-08-01 04:00:59.243462 csr-0.4.3/tests/test_bench_mult_vec.py
--rw-r--r--   0        0        0     2105 2022-08-01 04:00:59.243462 csr-0.4.3/tests/test_bench_multiply.py
--rw-r--r--   0        0        0     5111 2022-08-01 04:00:59.243462 csr-0.4.3/tests/test_convert.py
--rw-r--r--   0        0        0      416 2022-08-01 04:00:59.243462 csr-0.4.3/tests/test_handles.py
--rw-r--r--   0        0        0     3045 2022-08-01 04:00:59.243462 csr-0.4.3/tests/test_initialize.py
--rw-r--r--   0        0        0     2766 2022-08-01 04:00:59.243462 csr-0.4.3/tests/test_mkl.py
--rw-r--r--   0        0        0     1184 2022-08-01 04:00:59.243462 csr-0.4.3/tests/test_mult_vec.py
--rw-r--r--   0        0        0     1812 2022-08-01 04:00:59.243462 csr-0.4.3/tests/test_multiply.py
--rw-r--r--   0        0        0     3773 2022-08-01 04:00:59.243462 csr-0.4.3/tests/test_numba.py
--rw-r--r--   0        0        0      846 2022-08-01 04:00:59.243462 csr-0.4.3/tests/test_numba_mult.py
--rw-r--r--   0        0        0     1178 2022-08-01 04:00:59.243462 csr-0.4.3/tests/test_pickle.py
--rw-r--r--   0        0        0     4873 2022-08-01 04:00:59.243462 csr-0.4.3/tests/test_transform.py
--rw-r--r--   0        0        0     2233 2022-08-01 04:00:59.243462 csr-0.4.3/tests/test_transpose.py
--rw-r--r--   0        0        0      509 2022-08-01 04:00:59.243462 csr-0.4.3/tox.ini
--rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 csr-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      164 2022-02-19 17:31:58.226879 csr-0.5.0a1/.editorconfig
+-rw-r--r--   0        0        0      223 2022-02-19 17:31:58.227901 csr-0.5.0a1/.gitignore
+-rw-r--r--   0        0        0      147 2022-02-19 17:31:58.227901 csr-0.5.0a1/.readthedocs.yml
+-rw-r--r--   0        0        0     1089 2022-02-19 17:31:58.236816 csr-0.5.0a1/LICENSE
+-rw-r--r--   0        0        0      834 2022-02-19 17:31:58.245368 csr-0.5.0a1/README.md
+-rw-r--r--   0        0        0     3358 2022-02-19 17:31:58.249963 csr-0.5.0a1/Timings.py
+-rw-r--r--   0        0        0       59 2022-07-30 21:03:37.175923 csr-0.5.0a1/codecov.yml
+-rw-r--r--   0        0        0     1447 2023-04-10 23:45:09.997691 csr-0.5.0a1/conftest.py
+-rw-r--r--   0        0        0      251 2023-04-18 22:23:58.557628 csr-0.5.0a1/csr/__init__.py
+-rw-r--r--   0        0        0     2698 2023-04-18 22:23:12.666863 csr-0.5.0a1/csr/_rows.py
+-rw-r--r--   0        0        0     1610 2022-07-30 21:03:37.178089 csr-0.5.0a1/csr/_struct.py
+-rw-r--r--   0        0        0      519 2022-02-19 17:31:58.229901 csr-0.5.0a1/csr/_util.py
+-rw-r--r--   0        0        0     3287 2023-04-18 22:23:12.666863 csr-0.5.0a1/csr/_wiring.py
+-rw-r--r--   0        0        0     1778 2022-02-19 17:31:58.228901 csr-0.5.0a1/csr/constructors.py
+-rw-r--r--   0        0        0    22794 2023-04-18 22:23:12.667863 csr-0.5.0a1/csr/csr.py
+-rw-r--r--   0        0        0      363 2022-02-19 17:31:58.230402 csr-0.5.0a1/csr/kernel.py
+-rw-r--r--   0        0        0     2887 2022-02-19 17:31:58.231902 csr-0.5.0a1/csr/kernels/__init__.py
+-rw-r--r--   0        0        0      173 2022-02-19 17:31:58.232401 csr-0.5.0a1/csr/kernels/mkl/__init__.py
+-rw-r--r--   0        0        0      497 2022-02-19 17:31:58.232401 csr-0.5.0a1/csr/kernels/mkl/_api.py
+-rw-r--r--   0        0        0     3424 2022-07-30 21:03:37.178089 csr-0.5.0a1/csr/kernels/mkl/handle.py
+-rw-r--r--   0        0        0     5567 2022-02-19 17:31:58.232919 csr-0.5.0a1/csr/kernels/mkl/mkl_ops.c
+-rw-r--r--   0        0        0     1060 2022-02-19 17:31:58.232401 csr-0.5.0a1/csr/kernels/mkl/mkl_ops.h
+-rw-r--r--   0        0        0      733 2022-02-19 17:31:58.232919 csr-0.5.0a1/csr/kernels/mkl/multiply.py
+-rw-r--r--   0        0        0     1265 2022-07-30 21:03:37.179972 csr-0.5.0a1/csr/kernels/numba/__init__.py
+-rw-r--r--   0        0        0     3235 2022-02-19 17:31:58.234175 csr-0.5.0a1/csr/kernels/numba/multiply.py
+-rw-r--r--   0        0        0      804 2022-02-19 17:31:58.234175 csr-0.5.0a1/csr/kernels/scipy.py
+-rw-r--r--   0        0        0     6566 2022-02-19 17:31:58.234110 csr-0.5.0a1/csr/structure.py
+-rw-r--r--   0        0        0     3500 2022-07-30 21:03:37.180469 csr-0.5.0a1/csr/test_utils.py
+-rw-r--r--   0        0        0     2077 2022-07-30 21:03:37.180469 csr-0.5.0a1/csr/transform.py
+-rw-r--r--   0        0        0     1089 2022-02-19 17:31:58.234677 csr-0.5.0a1/docs/conf.py
+-rw-r--r--   0        0        0     1644 2022-02-19 17:31:58.235177 csr-0.5.0a1/docs/csr.rst
+-rw-r--r--   0        0        0     1170 2022-02-19 17:31:58.236320 csr-0.5.0a1/docs/index.rst
+-rw-r--r--   0        0        0     3859 2022-02-19 17:31:58.235705 csr-0.5.0a1/docs/kernels.rst
+-rw-r--r--   0        0        0       70 2022-02-19 17:31:58.236816 csr-0.5.0a1/jupytext.toml
+-rw-r--r--   0        0        0      155 2022-10-25 18:41:00.310046 csr-0.5.0a1/min-constraints.txt
+-rw-r--r--   0        0        0       68 2022-07-30 21:03:37.183531 csr-0.5.0a1/mkl-devel.yml
+-rw-r--r--   0        0        0     1304 2022-10-25 18:44:18.722422 csr-0.5.0a1/pyproject.toml
+-rw-r--r--   0        0        0      541 2022-07-30 21:03:37.184709 csr-0.5.0a1/pytest.ini
+-rw-r--r--   0        0        0      198 2022-02-19 17:31:58.246419 csr-0.5.0a1/setup.cfg
+-rw-r--r--   0        0        0     1776 2022-07-30 21:02:36.314600 csr-0.5.0a1/tasks.py
+-rw-r--r--   0        0        0     1020 2022-02-19 17:31:58.245368 csr-0.5.0a1/tests/test_active_kernel.py
+-rw-r--r--   0        0        0     8841 2023-04-18 22:23:12.668866 csr-0.5.0a1/tests/test_attributes.py
+-rw-r--r--   0        0        0      411 2022-02-19 17:31:58.246419 csr-0.5.0a1/tests/test_bench_mult_vec.py
+-rw-r--r--   0        0        0     2105 2022-02-19 17:31:58.246962 csr-0.5.0a1/tests/test_bench_multiply.py
+-rw-r--r--   0        0        0     4908 2022-07-30 21:03:37.195086 csr-0.5.0a1/tests/test_convert.py
+-rw-r--r--   0        0        0      445 2022-07-30 21:03:37.193995 csr-0.5.0a1/tests/test_handles.py
+-rw-r--r--   0        0        0     3045 2022-02-19 17:31:58.247463 csr-0.5.0a1/tests/test_initialize.py
+-rw-r--r--   0        0        0      598 2022-07-30 21:03:37.199162 csr-0.5.0a1/tests/test_kernel_numba.py
+-rw-r--r--   0        0        0     2856 2022-07-30 21:03:37.197352 csr-0.5.0a1/tests/test_mkl.py
+-rw-r--r--   0        0        0      900 2022-07-30 21:03:37.184709 csr-0.5.0a1/tests/test_mult_vec.py
+-rw-r--r--   0        0        0     1938 2022-07-30 21:03:37.200327 csr-0.5.0a1/tests/test_multiply.py
+-rw-r--r--   0        0        0     5640 2023-04-18 22:23:12.668866 csr-0.5.0a1/tests/test_numba.py
+-rw-r--r--   0        0        0     1178 2022-02-19 17:31:58.248963 csr-0.5.0a1/tests/test_pickle.py
+-rw-r--r--   0        0        0     5878 2022-07-30 21:03:37.198164 csr-0.5.0a1/tests/test_transform.py
+-rw-r--r--   0        0        0     2095 2022-07-30 21:03:37.200828 csr-0.5.0a1/tests/test_transpose.py
+-rw-r--r--   0        0        0      509 2022-02-19 17:31:58.249462 csr-0.5.0a1/tox.ini
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 csr-0.5.0a1/PKG-INFO
```

### Comparing `csr-0.4.3/LICENSE` & `csr-0.5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/README.md` & `csr-0.5.0a1/README.md`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/Timings.py` & `csr-0.5.0a1/Timings.py`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/conftest.py` & `csr-0.5.0a1/conftest.py`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/csr/_util.py` & `csr-0.5.0a1/csr/_util.py`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/csr/_wiring.py` & `csr-0.5.0a1/csr/_wiring.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,51 @@
 """
 Wire together the Numba and Python types.
 """
 
 import numpy as np
+from numba import types
 from numba.extending import overload_method
 from numba.experimental import structref
 
 from ._struct import CSRType
 from .csr import CSR
-from . import _rows, structure
+from . import _rows, _struct, structure
 
 structref.define_proxy(CSR, CSRType, [
     'nrows', 'ncols', 'nnz',
     'rowptrs', 'colinds', 'values'
 ])
 
 
 @overload_method(CSRType, 'row_extent')
 def _csr_row_extent(csr, row):
     return _rows.extent
 
 
 @overload_method(CSRType, 'row')
 def _csr_row(csr, row):
-    if csr.has_values:
-        return _rows._array_vals
-    else:
-        return _rows._array_ones
+    if isinstance(row, types.Integer):
+        if csr.has_values:
+            return _rows._row_array_vals
+        else:
+            return _rows._row_array_ones
+    elif isinstance(row, types.ArrayCompatible):
+        if csr.has_values:
+            return _rows._mr_matrix_vals
+        else:
+            return _rows._mr_matrix_ones
+
+
+@overload_method(CSRType, 'row_mask')
+def _csr_row_mask(csr, row):
+    if isinstance(row, types.Integer):
+        return _rows._row_array_mask
+    elif isinstance(row, types.ArrayCompatible):
+        return _rows._mr_matrix_mask
 
 
 @overload_method(CSRType, 'row_cs')
 def _csr_row_cs(csr, row):
     return _rows.cs
 
 
@@ -84,14 +99,24 @@
 
     if csr.has_values:
         return vals
     else:
         return ones
 
 
+@overload_method(CSRType, '_filter_zeros')
+def _csr_filter_zeros(csr):
+    if csr.has_values:
+        return _struct._filter_zeros
+    else:
+        def noop(csr):
+            pass
+        return noop
+
+
 @overload_method(CSRType, 'multiply')
 def _csr_multiply(csr, other, transpose):
     from . import kernel
 
     def mult(csr, other, transpose):
         ah = kernel.to_handle(csr)
         bh = kernel.to_handle(other)
@@ -102,14 +127,15 @@
 
         kernel.release_handle(bh)
         kernel.release_handle(ah)
 
         result = kernel.from_handle(ch)
         kernel.release_handle(ch)
 
+        result._filter_zeros()
         return result
 
     return mult
 
 
 @overload_method(CSRType, 'mult_vec')
 def _csr_mult_vec(csr, x):
```

### Comparing `csr-0.4.3/csr/constructors.py` & `csr-0.5.0a1/csr/constructors.py`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/csr/csr.py` & `csr-0.5.0a1/csr/csr.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,18 +144,23 @@
         Args:
             rows(array-like): the row indices.
             cols(array-like): the column indices.
             vals(array-like): the data values; can be ``None``.
             shape(tuple): the array shape, or ``None`` to infer from row & column indices.
         """
         from .structure import from_coo
+
+        assert np.min(rows, initial=0) >= 0
+        assert np.min(cols, initial=0) >= 0
+
         if shape is not None:
             nrows, ncols = shape
-            assert np.max(rows, initial=0) < nrows
-            assert np.max(cols, initial=0) < ncols
+            # if rows/cols is 0, that's fine; max must be zero
+            assert np.max(rows, initial=0) < max(nrows, 1)
+            assert np.max(cols, initial=0) < max(ncols, 1)
         else:
             nrows = np.max(rows) + 1
             ncols = np.max(cols) + 1
 
         nnz = len(rows)
         assert len(cols) == nnz
         assert vals is None or len(vals) == nnz
@@ -289,19 +294,14 @@
         elif val_dtype is False:
             vs = None
         else:
             vs = self.values
 
         return CSR(self.nrows, self.ncols, self.nnz, rps, self.colinds, vs, _cast=False)
 
-    @property
-    def R(self):
-        warnings.warn('.R deprecated, use CSR directly', DeprecationWarning)
-        return self
-
     def copy(self, include_values=True, *, copy_structure=True):
         """
         Create a copy of this CSR.
 
         Args:
             include_values(bool): whether to copy the values or only the structure.
             copy_structure(bool):
@@ -368,26 +368,44 @@
         Get the row indices from this array.  Combined with :py:attr:`colinds` and
         :py:attr:`values`, this can form a COO-format sparse matrix.
         """
         return _rows.all_indices(self)
 
     def row(self, row):
         """
-        Return a row of this matrix as a dense ndarray.
+        Return one or more rows of this matrix as a dense ndarray.
 
         Args:
-            row(int): the row index.
+            row(int or numpy.ndarray): the row index or indices.
 
         Returns:
             numpy.ndarray:
                 the row, with 0s in the place of missing values.  If the CSR only
                 stores matrix structure, the returned vector has 1s where the CSR
                 records an entry.
         """
-        return _rows.array(self, row)
+        row = np.asarray(row, dtype='i4')
+        return _rows.row_array(self, row)
+
+    def row_mask(self, row):
+        """
+        Return a dense logical array indicating which columns are set in the row
+        (or rows).
+
+        Args:
+            row(int or numpy.ndarray): the row index or indices.
+
+        Returns:
+            numpy.ndarray:
+                the row, with ``True`` for columns that are set on this row.  If
+                ``row`` is an array or list of length :math:`k`, this is a matrix
+                of shape :math:`k \\times \\mathrm{ncols}`.
+        """
+        row = np.asarray(row, dtype='i4')
+        return _rows.row_mask(self, row)
 
     def row_extent(self, row):
         """
         Get the extent of a row in the underlying column index and value arrays.
 
         Args:
             row(int): the row index.
@@ -530,14 +548,15 @@
                 if transpose:
                     c_h = K.mult_abt(a_h, b_h)
                 else:
                     c_h = K.mult_ab(a_h, b_h)
                 with releasing(c_h, K):
                     crepr = K.from_handle(c_h)
 
+            crepr._filter_zeros()
             return crepr
 
         if self.nnz <= K.max_nnz:
             # Common / fast path - one matrix
             with releasing(K.to_handle(other), K) as b_h:
                 return mul(self, b_h)
         else:
@@ -566,14 +585,21 @@
             shards = self._shard_rows(K.max_nnz)
             svs = []
             for s in shards:
                 with releasing(K.to_handle(s), K) as h:
                     svs.append(K.mult_vec(h, v))
             return np.concatenate(svs)
 
+    def _filter_zeros(self):
+        """
+        Filter out the stored zero values in-place.
+        """
+        if self.values is not None:
+            _struct.filter_zeros(self)
+
     def _shard_rows(self, tgt_nnz):
         """
         Shard a matrix by rows to fit in a target size.
         """
         assert tgt_nnz > 0
 
         rest = self
@@ -653,13 +679,14 @@
 
     def __repr__(self):
         repr = '<CSR {}x{} ({} nnz)'.format(self.nrows, self.ncols, self.nnz)
         repr += ' {\n'
         repr += '  rowptrs={}\n'.format(self.rowptrs)
         repr += '  colinds={}\n'.format(self.colinds)
         repr += '  values={}\n'.format(self.values)
+        repr += '  dtype={}\n'.format(self.values.dtype if self.values is not None else None)
         repr += '}>'
         return repr
 
     def __reduce__(self):
         args = (self.nrows, self.ncols, self.nnz, self.rowptrs, self.colinds, self.values, False)
         return (CSR, args)
```

### Comparing `csr-0.4.3/csr/kernels/__init__.py` & `csr-0.5.0a1/csr/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/csr/kernels/mkl/handle.py` & `csr-0.5.0a1/csr/kernels/mkl/handle.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from numba import njit, config
 from numba.extending import overload
 from numba.core.types import StructRef, intc, float64
 from numba.experimental import structref
 
 from csr import CSR
 from ._api import *  # noqa: F403
+import csr.kernels.mkl as _hpkg
 from csr.constructors import create_empty
 
 __all__ = [
     'mkl_h',
     'to_handle',
     'from_handle',
     'release_handle'
@@ -54,14 +55,17 @@
     return mkl_h(h, csr.nrows, csr.ncols, csr)
 
 
 _make_handle = njit(_make_handle_impl)
 
 
 def to_handle(csr: CSR) -> mkl_h:
+    if csr.nnz > _hpkg.max_nnz:
+        raise ValueError('CSR size {} exceeds max nnz {}'.format(csr.nnz, _hpkg.max_nnz))
+
     if csr.nnz == 0:
         # empty matrices don't really work
         return mkl_h(0, csr.nrows, csr.ncols, None)
 
     norm = csr._normalize(np.float64, np.intc)
     return _make_handle(norm)
```

### Comparing `csr-0.4.3/csr/kernels/mkl/mkl_ops.c` & `csr-0.5.0a1/csr/kernels/mkl/mkl_ops.c`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/csr/kernels/mkl/mkl_ops.h` & `csr-0.5.0a1/csr/kernels/mkl/mkl_ops.h`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/csr/kernels/mkl/multiply.py` & `csr-0.5.0a1/csr/kernels/mkl/multiply.py`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/csr/kernels/numba/__init__.py` & `csr-0.5.0a1/csr/kernels/numba/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 @njit
 def to_handle(csr):
     """
     Convert a native CSR to a handle.  The caller must arrange for the CSR last at
     least as long as the handle.  The handle must be explicitly released.
 
     Handles are opaque as far as callers are concerned.
+
+    Creating a handle **may** copy data; modifying the matrix is not guaranteed to
+    modify handles created from it.
     """
     return csr
 
 
 @njit
 def from_handle(h):
     """
```

### Comparing `csr-0.4.3/csr/kernels/numba/multiply.py` & `csr-0.5.0a1/csr/kernels/numba/multiply.py`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/csr/kernels/scipy.py` & `csr-0.5.0a1/csr/kernels/scipy.py`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/csr/structure.py` & `csr-0.5.0a1/csr/structure.py`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/docs/conf.py` & `csr-0.5.0a1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/docs/csr.rst` & `csr-0.5.0a1/docs/csr.rst`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/docs/index.rst` & `csr-0.5.0a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/docs/kernels.rst` & `csr-0.5.0a1/docs/kernels.rst`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/pyproject.toml` & `csr-0.5.0a1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 [build-system]
-requires = ["flit_core >=2,<4"]
+requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
-[tool.flit.metadata]
-module = "csr"
-author = "Michael Ekstrand <michaelekstrand@boisestate.edu>"
-author-email = "michaelekstrand@boisestate.edu"
-home-page = "https://csr.lenskit.org"
-classifiers = ["License :: OSI Approved :: MIT License"]
-description-file = "README.md"
+[project]
+name = "csr"
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Intended Audience :: Science/Research",
+]
+description = "Compressed Sparse Row matrices for Python, with Numba API."
+readme = "README.md"
+license = { file = "LICENSE" }
+dynamic = ['version']
 requires-python = ">= 3.7"
-requires = [
+dependencies = [
     "numba >=0.51,<0.57",
     "numpy >=1.17",
     "scipy >=1.2,<2"
 ]
 
-[tool.flit.metadata.requires-extra]
+[[project.authors]]
+name = "Michael Ekstrand"
+email = "michaelekstrand@boisestate.edu"
+
+[project.urls]
+home-page = "https://csr.lenskit.org"
+source = "https://github.com/lenskit/csr"
+
+[project.optional-dependencies]
 test = [
-    "pytest >=6",
+    "pytest ==6.*",
     "pytest-doctestplus >=0.9",
     "pytest-benchmark >=3",
     "pytest-cov >=2.12",
     "hypothesis ~=6.30",
     "psutil >=5"
 ]
 dev = [
-    "flit",
+    "flit >=3.2,<4",
     "keyring",
     "flake8",
     "rstcheck",
     "invoke",
     "lenskit-build-helpers >=0.1",
     "sphinx-autobuild >=2021",
 ]
```

### Comparing `csr-0.4.3/tasks.py` & `csr-0.5.0a1/tasks.py`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/tests/test_active_kernel.py` & `csr-0.5.0a1/tests/test_active_kernel.py`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/tests/test_attributes.py` & `csr-0.5.0a1/tests/test_attributes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import logging
 import numpy as np
 import scipy.sparse as sps
 
 from csr import CSR
-from csr.test_utils import csrs, matrices, sparse_matrices
+from csr.test_utils import csr_slow, csrs, matrices
 
 from pytest import raises
-from hypothesis import given, assume, settings, HealthCheck
+from hypothesis import given, assume
 import hypothesis.strategies as st
 import hypothesis.extra.numpy as nph
 
+_log = logging.getLogger(__name__)
+
 
 def test_csr_rowinds():
     rows = np.array([0, 0, 1, 3], dtype=np.int32)
     cols = np.array([1, 2, 0, 1], dtype=np.int32)
     vals = np.arange(4, dtype=np.float_)
     csr = CSR.from_coo(rows, cols, vals)
 
@@ -38,49 +41,100 @@
 
     assert csr.row_extent(0) == (0, 2)
     assert csr.row_extent(1) == (2, 3)
     assert csr.row_extent(2) == (3, 3)
     assert csr.row_extent(3) == (3, 4)
 
 
-@given(sparse_matrices())
-def test_csr_row_extent(smat):
-    csr = CSR.from_scipy(smat)
-
+@csr_slow()
+@given(csrs(st.integers(1, 100), st.integers(1, 100)))
+def test_csr_row_extent(csr):
     for i in range(csr.nrows):
         sp, ep = csr.row_extent(i)
         assert sp == csr.rowptrs[i]
-        assert ep == csr.rowptrs[i+1]
+        assert ep == csr.rowptrs[i + 1]
 
 
 def test_csr_row_fixed():
     rows = np.array([0, 0, 1, 3], dtype=np.int32)
     cols = np.array([1, 2, 0, 1], dtype=np.int32)
     vals = np.arange(4, dtype=np.float_) + 1
 
     csr = CSR.from_coo(rows, cols, vals)
     assert all(csr.row(0) == np.array([0, 1, 2], dtype=np.float_))
     assert all(csr.row(1) == np.array([3, 0, 0], dtype=np.float_))
     assert all(csr.row(2) == np.array([0, 0, 0], dtype=np.float_))
     assert all(csr.row(3) == np.array([0, 4, 0], dtype=np.float_))
 
 
-@given(sparse_matrices())
-def test_csr_row(smat):
-    csr = CSR.from_scipy(smat)
+@csr_slow()
+@given(csrs(st.integers(1, 100), st.integers(1, 100)))
+def test_csr_row(csr):
+    smat = csr.to_scipy()
 
     for i in range(csr.nrows):
         other = smat[i, :].toarray().ravel()
         row = csr.row(i)
 
         assert row.size == other.size
 
         assert all(row == other)
 
 
+@csr_slow()
+@given(st.data(), csrs(st.integers(1, 100), st.integers(1, 100)))
+def test_csr_multi_rows(data, csr):
+    smat = csr.to_scipy()
+
+    rows = data.draw(st.lists(st.integers(0, csr.nrows - 1), max_size=csr.nrows, unique=True))
+    row_arrs = csr.row(rows)
+    other = smat[rows, :].toarray()
+    assert np.all(row_arrs == other)
+
+
+@csr_slow()
+@given(st.data())
+def test_csr_rows(data):
+    "Test the row() method - row and multi_rows in one test (to demonstrate feasibility)"
+    csr = data.draw(csrs(st.integers(1, 100), st.integers(1, 100)))
+    smat = csr.to_scipy()
+
+    row_id = st.integers(0, csr.nrows - 1)
+    row_list = st.lists(row_id, max_size=csr.nrows, unique=True)
+    rows = data.draw(st.one_of(row_id, row_list))
+
+    row_arrs = csr.row(rows)
+    other = smat[rows, :].toarray()
+    assert np.all(row_arrs == other)
+
+
+@csr_slow()
+@given(st.data())
+def test_csr_row_mask(data):
+    csr = data.draw(csrs(st.integers(1, 100), st.integers(1, 100)))
+
+    row_id = st.integers(0, csr.nrows - 1)
+    row_list = st.lists(row_id, max_size=csr.nrows, unique=True)
+    rows = data.draw(st.one_of(row_id, row_list))
+
+    row_arrs = csr.row_mask(rows)
+    assert row_arrs.dtype == np.bool_
+    if isinstance(rows, list):
+        assert row_arrs.shape == (len(rows), csr.ncols)
+        for i, row in enumerate(rows):
+            sp, ep = csr.row_extent(row)
+            assert np.all(row_arrs[i, csr.row_cs(row)])
+            assert np.sum(row_arrs[i, :]) == ep - sp
+    else:
+        assert row_arrs.shape == (csr.ncols,)
+        sp, ep = csr.row_extent(rows)
+        assert np.all(row_arrs[csr.row_cs(rows)])
+        assert np.sum(row_arrs) == ep - sp
+
+
 def test_csr_sparse_row():
     rows = np.array([0, 0, 1, 3], dtype=np.int32)
     cols = np.array([1, 2, 0, 1], dtype=np.int32)
     vals = np.arange(4, dtype=np.float_)
 
     csr = CSR.from_coo(rows, cols, vals)
     assert all(csr.row_cs(0) == np.array([1, 2], dtype=np.int32))
@@ -90,61 +144,67 @@
 
     assert all(csr.row_vs(0) == np.array([0, 1], dtype=np.float_))
     assert all(csr.row_vs(1) == np.array([2], dtype=np.float_))
     assert all(csr.row_vs(2) == np.array([], dtype=np.float_))
     assert all(csr.row_vs(3) == np.array([3], dtype=np.float_))
 
 
-@given(csrs())
+@csr_slow()
+@given(csrs(st.integers(1, 100), st.integers(1, 100), values=True))
 def test_drop_values(csr):
     csr.drop_values()
     assert csr.values is None
 
 
-@given(csrs(), st.floats(allow_infinity=False, allow_nan=False))
-def test_fill_values(csr, x):
+@csr_slow()
+@given(st.data(), csrs())
+def test_fill_values(data, csr):
+    dtype = np.dtype('f8')
+    if csr.values is not None:
+        dtype = csr.values.dtype
+    x = data.draw(nph.from_dtype(dtype, allow_infinity=False, allow_nan=False))
     csr.fill_values(x)
     assert all(csr.values == x)
 
 
 def test_csr_set_values():
     rows = np.array([0, 0, 1, 3], dtype=np.int32)
     cols = np.array([1, 2, 0, 1], dtype=np.int32)
     vals = np.arange(4, dtype=np.float_)
 
     csr = CSR.from_coo(rows, cols, vals)
 
-    v2 = np.random.randn(4)
+    v2 = 10 - vals
     csr.values = v2
 
     assert all(csr.values == v2)
 
 
 def test_csr_set_values_oversize():
     rows = np.array([0, 0, 1, 3], dtype=np.int32)
     cols = np.array([1, 2, 0, 1], dtype=np.int32)
     vals = np.arange(4, dtype=np.float_)
 
     csr = CSR.from_coo(rows, cols, vals)
 
-    v2 = np.random.randn(6)
+    v2 = np.arange(6, dtype=np.float_) + 10
     csr.values = v2
 
     assert csr.values is not None
     assert all(csr.values == v2[:4])
 
 
 def test_csr_set_values_undersize():
     rows = np.array([0, 0, 1, 3], dtype=np.int32)
     cols = np.array([1, 2, 0, 1], dtype=np.int32)
     vals = np.arange(4, dtype=np.float_)
 
     csr = CSR.from_coo(rows, cols, vals)
 
-    v2 = np.random.randn(3)
+    v2 = np.arange(3, dtype=np.float_) + 5
 
     with raises(ValueError):
         csr.values = v2
 
     assert all(csr.values == vals)
 
 
@@ -158,14 +218,15 @@
 
     assert csr.values is None
     assert all(csr.row(0) == [0, 1, 1])
     assert all(csr.row(1) == [1, 0, 0])
     assert all(csr.row(3) == [0, 1, 0])
 
 
+@csr_slow()
 @given(matrices())
 def test_csr_row_nnzs(mat):
     nrows, ncols = mat.shape
 
     # sparsify the matrix
     mat[mat <= 0] = 0
     smat = sps.csr_matrix(mat)
@@ -176,62 +237,69 @@
     nnzs = csr.row_nnzs()
     assert nnzs.sum() == csr.nnz
     for i in range(nrows):
         row = mat[i, :]
         assert nnzs[i] == np.sum(row > 0)
 
 
-@given(sparse_matrices())
-def test_copy(mat):
+@csr_slow()
+@given(csrs(st.integers(1, 100), st.integers(1, 100)))
+def test_copy(csr):
     "Test copying a CSR"
-    csr = CSR.from_scipy(mat)
     c2 = csr.copy()
 
     assert c2.nrows == csr.nrows
     assert c2.ncols == csr.ncols
     assert c2.nnz == csr.nnz
     assert c2.rowptrs is not csr.rowptrs
     assert all(c2.rowptrs == csr.rowptrs)
     assert c2.colinds is not csr.colinds
     assert all(c2.colinds == csr.colinds)
-    assert c2.values is not csr.values
-    assert all(c2.values == csr.values)
+    if csr.values is not None:
+        assert c2.values is not csr.values
+        assert all(c2.values == csr.values)
+    else:
+        assert c2.values is None
 
 
-@given(sparse_matrices())
-def test_copy_share(mat):
+@csr_slow()
+@given(csrs(st.integers(1, 100), st.integers(1, 100)))
+def test_copy_share(csr):
     "Test copying a CSR and sharing structure"
-    csr = CSR.from_scipy(mat)
     c2 = csr.copy(copy_structure=False)
 
     assert c2.nrows == csr.nrows
     assert c2.ncols == csr.ncols
     assert c2.nnz == csr.nnz
     assert c2.rowptrs is csr.rowptrs
     assert c2.colinds is csr.colinds
-    assert c2.values is not csr.values
-    assert all(c2.values == csr.values)
+    if csr.values is not None:
+        assert c2.values is not csr.values
+        assert all(c2.values == csr.values)
+    else:
+        assert c2.values is None
 
 
-@given(sparse_matrices())
-def test_copy_structure_only(mat):
+@csr_slow()
+@given(csrs(st.integers(1, 100), st.integers(1, 100)))
+def test_copy_structure_only(csr):
     "Test copying only the structure of a CSV."
-    csr = CSR.from_scipy(mat)
     c2 = csr.copy(False)
 
     assert c2.nrows == csr.nrows
     assert c2.ncols == csr.ncols
     assert c2.nnz == csr.nnz
     assert c2.rowptrs is not csr.rowptrs
     assert all(c2.rowptrs == csr.rowptrs)
     assert c2.colinds is not csr.colinds
     assert all(c2.colinds == csr.colinds)
     assert c2.values is None
 
 
+@csr_slow()
 @given(csrs(values=False), st.booleans())
 def test_copy_csrnv(csr, inc):
     "Test copying a CSR with no values."
     c2 = csr.copy(inc)
 
     assert c2.nrows == csr.nrows
     assert c2.ncols == csr.ncols
```

### Comparing `csr-0.4.3/tests/test_bench_multiply.py` & `csr-0.5.0a1/tests/test_bench_multiply.py`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/tests/test_convert.py` & `csr-0.5.0a1/tests/test_convert.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,20 @@
+import logging
 import numpy as np
 import scipy.sparse as sps
 
 from csr import CSR
 from csr.test_utils import csrs, csr_slow, sparse_matrices
 
 from pytest import mark, approx, raises
 from hypothesis import given, assume, settings, HealthCheck
 import hypothesis.strategies as st
 import hypothesis.extra.numpy as nph
 
-
-@mark.parametrize('copy', [True, False])
-def test_csr_from_sps(copy):
-    "Test creating a CSR from a SciPy matrix"
-    # initialize sparse matrix
-    mat = np.random.randn(10, 5)
-    mat[mat <= 0] = 0
-    smat = sps.csr_matrix(mat)
-    # make sure it's sparse
-    assert smat.nnz == np.sum(mat > 0)
-
-    csr = CSR.from_scipy(smat, copy=copy)
-    assert csr.nnz == smat.nnz
-    assert csr.nrows == smat.shape[0]
-    assert csr.ncols == smat.shape[1]
-
-    assert all(csr.rowptrs == smat.indptr)
-    assert all(csr.colinds == smat.indices)
-    assert all(csr.values == smat.data)
-    assert isinstance(csr.rowptrs, np.ndarray)
-    assert isinstance(csr.colinds, np.ndarray)
-    assert isinstance(csr.values, np.ndarray)
+_log = logging.getLogger(__name__)
 
 
 @given(sparse_matrices(format='csr'), st.booleans())
 def test_csr_from_sps_csr(smat, copy):
     "Test creating a CSR from a SciPy CSR matrix"
     csr = CSR.from_scipy(smat, copy=copy)
     assert csr.nnz == smat.nnz
@@ -46,113 +26,124 @@
     assert all(csr.values == smat.data)
     assert isinstance(csr.rowptrs, np.ndarray)
     assert isinstance(csr.colinds, np.ndarray)
     if csr.nnz > 0:
         assert isinstance(csr.values, np.ndarray)
 
 
-def test_csr_is_numpy_compatible():
-    # initialize sparse matrix
-    mat = np.random.randn(10, 5)
-    mat[mat <= 0] = 0
-    smat = sps.csr_matrix(mat)
-    # make sure it's sparse
-    assert smat.nnz == np.sum(mat > 0)
-
-    csr = CSR.from_scipy(smat)
-
-    d2 = csr.values * 10
-    assert d2 == approx(smat.data * 10)
-
-
-def test_csr_from_coo():
+def test_csr_from_coo_fixed():
     "Make a CSR from COO data"
     rows = np.array([0, 0, 1, 3], dtype=np.int32)
     cols = np.array([1, 2, 0, 1], dtype=np.int32)
     vals = np.arange(4, dtype=np.float_)
 
     csr = CSR.from_coo(rows, cols, vals)
     assert csr.nrows == 4
     assert csr.ncols == 3
     assert csr.nnz == 4
     assert csr.values == approx(vals)
 
 
-def test_csr_from_coo_rand():
-    for i in range(100):
-        coords = np.random.choice(np.arange(50 * 100, dtype=np.int32), 1000, False)
-        rows = np.mod(coords, 100, dtype=np.int32)
-        cols = np.floor_divide(coords, 100, dtype=np.int32)
-        vals = np.random.randn(1000)
-
-        csr = CSR.from_coo(rows, cols, vals, (100, 50))
-        rowinds = csr.rowinds()
-        assert csr.nrows == 100
-        assert csr.ncols == 50
-        assert csr.nnz == 1000
-
-        for i in range(100):
-            sp = csr.rowptrs[i]
-            ep = csr.rowptrs[i+1]
-            assert ep - sp == np.sum(rows == i)
-            points, = np.nonzero(rows == i)
-            assert len(points) == ep - sp
-            po = np.argsort(cols[points])
-            points = points[po]
-            assert all(np.sort(csr.colinds[sp:ep]) == cols[points])
-            assert all(np.sort(csr.row_cs(i)) == cols[points])
-            assert all(csr.values[np.argsort(csr.colinds[sp:ep]) + sp] == vals[points])
-            assert all(rowinds[sp:ep] == i)
-
-            row = np.zeros(50)
-            row[cols[points]] = vals[points]
-            assert np.sum(csr.row(i)) == approx(np.sum(vals[points]))
-            assert all(csr.row(i) == row)
-
-
-def test_csr_from_coo_novals():
-    for i in range(50):
-        coords = np.random.choice(np.arange(50 * 100, dtype=np.int32), 1000, False)
-        rows = np.mod(coords, 100, dtype=np.int32)
-        cols = np.floor_divide(coords, 100, dtype=np.int32)
-
-        csr = CSR.from_coo(rows, cols, None, (100, 50))
-        assert csr.nrows == 100
-        assert csr.ncols == 50
-        assert csr.nnz == 1000
-
-        for i in range(100):
-            sp = csr.rowptrs[i]
-            ep = csr.rowptrs[i+1]
-            assert ep - sp == np.sum(rows == i)
-            points, = np.nonzero(rows == i)
-            po = np.argsort(cols[points])
-            points = points[po]
-            assert all(np.sort(csr.colinds[sp:ep]) == cols[points])
-            assert np.sum(csr.row(i)) == len(points)
-
-
-def test_csr_to_sps():
-    # initialize sparse matrix
-    mat = np.random.randn(10, 5)
-    mat[mat <= 0] = 0
-    # get COO
-    smat = sps.coo_matrix(mat)
-    # make sure it's sparse
-    assert smat.nnz == np.sum(mat > 0)
-
-    csr = CSR.from_coo(smat.row, smat.col, smat.data, shape=smat.shape)
-    assert csr.nnz == smat.nnz
-    assert csr.nrows == smat.shape[0]
-    assert csr.ncols == smat.shape[1]
-
-    smat2 = csr.to_scipy()
-    assert sps.isspmatrix(smat2)
-    assert sps.isspmatrix_csr(smat2)
+@given(st.data(), st.integers(0, 100), st.integers(0, 100),
+       st.sampled_from(['f4', 'f8']))
+def test_csr_from_coo(data, nrows, ncols, dtype):
+    dtype = np.dtype(dtype)
+    n = nrows * ncols
+    nnz = data.draw(st.integers(0, int(n * 0.75)))
+    _log.debug('testing %d×%d (%d nnz) of type %s', nrows, ncols, nnz, dtype)
+
+    coords = st.integers(0, max(n - 1, 0))
+    coords = data.draw(nph.arrays(np.int32, nnz, elements=coords, unique=True))
+    rows = np.mod(coords, nrows, dtype=np.int32)
+    cols = np.floor_divide(coords, nrows, dtype=np.int32)
+
+    finite = nph.from_dtype(dtype, allow_infinity=False, allow_nan=False)
+    vals = data.draw(nph.arrays(dtype, nnz, elements=finite))
+
+    csr = CSR.from_coo(rows, cols, vals, (nrows, ncols))
+
+    rowinds = csr.rowinds()
+    assert csr.nrows == nrows
+    assert csr.ncols == ncols
+    assert csr.nnz == nnz
+
+    for i in range(nrows):
+        sp = csr.rowptrs[i]
+        ep = csr.rowptrs[i + 1]
+        assert ep - sp == np.sum(rows == i)
+        points, = np.nonzero(rows == i)
+        assert len(points) == ep - sp
+        po = np.argsort(cols[points])
+        points = points[po]
+        assert all(np.sort(csr.colinds[sp:ep]) == cols[points])
+        assert all(np.sort(csr.row_cs(i)) == cols[points])
+        assert all(csr.values[np.argsort(csr.colinds[sp:ep]) + sp] == vals[points])
+        assert all(rowinds[sp:ep] == i)
+
+        row = np.zeros(ncols, dtype)
+        row[cols[points]] = vals[points]
+        assert all(csr.row(i) == row)
+
+
+@given(st.data(), st.integers(0, 100), st.integers(0, 100))
+def test_csr_from_coo_novals(data, nrows, ncols):
+    n = nrows * ncols
+    nnz = data.draw(st.integers(0, int(n * 0.75)))
+    _log.debug('testing %d×%d (%d nnz) with no values', nrows, ncols, nnz)
+
+    coords = st.integers(0, max(n - 1, 0))
+    coords = data.draw(nph.arrays(np.int32, nnz, elements=coords, unique=True))
+    rows = np.mod(coords, nrows, dtype=np.int32)
+    cols = np.floor_divide(coords, nrows, dtype=np.int32)
+
+    csr = CSR.from_coo(rows, cols, None, (nrows, ncols))
+
+    rowinds = csr.rowinds()
+    assert csr.nrows == nrows
+    assert csr.ncols == ncols
+    assert csr.nnz == nnz
+
+    for i in range(nrows):
+        sp = csr.rowptrs[i]
+        ep = csr.rowptrs[i + 1]
+        assert ep - sp == np.sum(rows == i)
+        points, = np.nonzero(rows == i)
+        assert len(points) == ep - sp
+        po = np.argsort(cols[points])
+        points = points[po]
+        assert all(np.sort(csr.colinds[sp:ep]) == cols[points])
+        assert all(np.sort(csr.row_cs(i)) == cols[points])
+        assert all(rowinds[sp:ep] == i)
+
+        row = csr.row(i)
+        assert np.sum(row) == ep - sp
+
+
+@given(st.data(), st.sampled_from(['csr', 'coo', 'csc']))
+def test_sps_to_csr(data, format):
+    mat = data.draw(sparse_matrices(format=format))
+    nr, nc = mat.shape
+    sp_csr: sps.csr_matrix = mat.tocsr()
+
+    csr = CSR.from_scipy(mat)
+
+    assert csr.ncols == nc
+    assert csr.nrows == nr
+    assert csr.nnz == mat.nnz
+    assert np.all(csr.rowptrs == sp_csr.indptr)
+    assert np.all(csr.colinds == sp_csr.indices)
+    assert np.all(csr.values == sp_csr.data)
+
+
+@given(csrs(values=True))
+def test_csr_to_sps(csr):
+    smat = csr.to_scipy()
+    assert sps.isspmatrix(smat)
+    assert sps.isspmatrix_csr(smat)
 
     for i in range(csr.nrows):
-        assert smat2.indptr[i] == csr.rowptrs[i]
-        assert smat2.indptr[i+1] == csr.rowptrs[i+1]
-        sp = smat2.indptr[i]
-        ep = smat2.indptr[i+1]
-        assert all(smat2.indices[sp:ep] == csr.colinds[sp:ep])
-        assert all(smat2.data[sp:ep] == csr.values[sp:ep])
+        assert smat.indptr[i] == csr.rowptrs[i]
+        assert smat.indptr[i + 1] == csr.rowptrs[i + 1]
+        sp = smat.indptr[i]
+        ep = smat.indptr[i + 1]
+        assert all(smat.indices[sp:ep] == csr.colinds[sp:ep])
+        assert all(smat.data[sp:ep] == csr.values[sp:ep])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `csr-0.4.3/tests/test_initialize.py` & `csr-0.5.0a1/tests/test_initialize.py`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/tests/test_mkl.py` & `csr-0.5.0a1/tests/test_mkl.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 from contextlib import contextmanager
 from numba import njit, prange
 import numpy as np
 
 from csr import CSR
 from csr.test_utils import csrs, has_memory
+from csr.kernels import use_kernel
 
 from pytest import skip, mark
 from hypothesis import given
 
 import test_multiply as tmm
 import test_mult_vec as tmv
 
@@ -70,27 +71,27 @@
         e = s + dense
         values[s:e] = np.random.randn(e - s)
         colinds[s:e] = np.random.choice(ncols, dense, replace=False)
 
 
 def test_mult_vec_lim():
     "Test matrix-vector multiply with limited kernel capacity"
-    with mkl_lim():
+    with mkl_lim(), use_kernel('mkl'):
         tmv.test_mult_vec(mkl)
 
 
 def test_multiply_lim():
     "Test matrix-matrix multiply with limited kernel capacity"
-    with mkl_lim():
+    with mkl_lim(), use_kernel('mkl'):
         tmm.test_multiply(mkl)
 
 
 def test_multiply_transpose_lim():
-    "Select matrix-matrix transpose multiply with limited kernel capacity"
-    with mkl_lim():
+    "Test matrix-matrix transpose multiply with limited kernel capacity"
+    with mkl_lim(), use_kernel('mkl'):
         tmm.test_multiply_transpose(mkl)
 
 
 @mark.skipif(not has_memory(32), reason='insufficient memory')
 def test_large_mult_vec():
     # 10M * 500 = 2.5B >= INT_MAX
     nrows = 10000000
```

### Comparing `csr-0.4.3/tests/test_mult_vec.py` & `csr-0.5.0a1/tests/test_mult_vec.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,39 @@
 import logging
-import numpy as np
 
-from csr import CSR
-from csr.test_utils import sparse_matrices
+from csr.test_utils import csrs, finite_arrays
 
 from pytest import approx
 from hypothesis import given, settings
 import hypothesis.strategies as st
-import hypothesis.extra.numpy as nph
 
 _log = logging.getLogger(__name__)
 
 
 @settings(deadline=None)
-@given(st.data())
-def test_mult_vec(kernel, data):
-    mat = data.draw(sparse_matrices((100, 100)))
-    md = mat.toarray()
-    csra = CSR.from_scipy(mat)
+@given(st.data(), csrs(values=True))
+def test_mult_vec(kernel, data, csra):
+    md = csra.to_scipy().toarray()
     # TODO make the test work with larger values
-    vals = st.floats(-100, 100)
-    v = data.draw(nph.arrays(np.float64, csra.ncols, elements=vals))
+    v = data.draw(finite_arrays(csra.ncols))
 
     prod = csra.mult_vec(v)
     assert prod.shape == (csra.nrows,)
 
     v2 = md @ v
 
-    assert prod == approx(v2, nan_ok=True, rel=1.0e-5)
+    assert prod == approx(v2, nan_ok=True, rel=1.0e-5, abs=1.0e-10)
 
 
 @settings(deadline=None)
-@given(st.data())
-def test_mult_vec_novalue(kernel, data):
-    mat = data.draw(sparse_matrices())
-    csra = CSR.from_scipy(mat, True)
+@given(st.data(), csrs(values=False))
+def test_mult_vec_novalue(kernel, data, csra):
+    mat = csra.to_scipy()
 
-    csra.drop_values()
-    mat.data[:] = 1.0
-
-    vals = st.floats(-100, 100)
-    v = data.draw(nph.arrays(np.float64, csra.ncols, elements=vals))
+    v = data.draw(finite_arrays(csra.ncols))
 
     prod = csra.mult_vec(v)
     assert prod.shape == (csra.nrows,)
 
     v2 = mat @ v
 
     assert prod == approx(v2, nan_ok=True)
```

### Comparing `csr-0.4.3/tests/test_multiply.py` & `csr-0.5.0a1/tests/test_multiply.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,79 @@
 import logging
+import numpy as np
 
 from csr import CSR
-from csr.test_utils import mm_pairs
+from csr.test_utils import mm_pairs, csr_slow
 
 from pytest import approx
 from hypothesis import given, settings, assume
+from hypothesis import strategies as st
 
 _log = logging.getLogger(__name__)
 
 
-@settings(deadline=None)
-@given(mm_pairs())
-def test_multiply(kernel, pair):
-    A, B = pair
-    csra = CSR.from_scipy(A)
-    csrb = CSR.from_scipy(B)
-    assume(csrb.nnz <= kernel.max_nnz)
+@csr_slow()
+@given(st.data())
+def test_multiply(kernel, data):
+    A, B = data.draw(mm_pairs())
+    assume(B.nnz < kernel.max_nnz)
+    dA = A.to_scipy().toarray()
+    dB = B.to_scipy().toarray()
 
-    prod = csra.multiply(csrb)
+    prod = A.multiply(B)
     assert isinstance(prod, CSR)
-    _log.info('got %r', prod)
-    _log.info('inner: %s', prod.R)
-    assert prod.nrows == csra.nrows
-    assert prod.ncols == csrb.ncols
+    _log.debug('got %r', prod)
+    assert prod.nrows == A.nrows
+    assert prod.ncols == B.ncols
 
-    AB = A @ B
-    abnr, abnc = AB.shape
+    dprod = dA @ dB
+    abnr, abnc = dprod.shape
     assert prod.nrows == abnr
     assert prod.ncols == abnc
 
-    assert prod.nnz == AB.nnz
+    # assert prod.nnz == sp_prod.nnz
     if prod.nnz > 0:
         assert prod.values is not None
-    nrows = csra.nrows
+        assert np.all(prod.values != 0)
+    nrows = A.nrows
 
     for i in range(nrows):
-        r_scipy = AB.getrow(i).toarray().ravel()
+        r_scipy = dprod[i, :]
         r_ours = prod.row(i)
 
         assert len(r_ours) == len(r_scipy)
-        assert r_ours == approx(r_scipy)
+        assert r_ours == approx(r_scipy, rel=1.0e-5, abs=1.0e-10)
 
 
-@settings(deadline=None)
-@given(mm_pairs())
-def test_multiply_transpose(kernel, pair):
-    A, B = pair
-    csra = CSR.from_scipy(A)
-    csrb = CSR.from_scipy(B.T)
-    assume(csrb.nnz <= kernel.max_nnz)
+@csr_slow()
+@given(st.data())
+def test_multiply_transpose(kernel, data):
+    A, B = data.draw(mm_pairs())
+    assume(B.nnz < kernel.max_nnz)
+    B = B.transpose()
 
-    prod = csra.multiply(csrb, transpose=True)
+    dA = A.to_scipy().toarray()
+    dB = B.to_scipy().toarray()
+
+    prod = A.multiply(B, transpose=True)
     assert isinstance(prod, CSR)
-    _log.info('got %r', prod)
-    _log.info('inner: %s', prod.R)
-    assert prod.nrows == csra.nrows
-    assert prod.ncols == csrb.nrows
+    _log.debug('got %r', prod)
+    assert prod.nrows == A.nrows
+    assert prod.ncols == B.nrows
 
-    AB = A @ B
-    abnr, abnc = AB.shape
+    dprod = dA @ dB.T
+    abnr, abnc = dprod.shape
     assert prod.nrows == abnr
     assert prod.ncols == abnc
 
-    assert prod.nnz == AB.nnz
+    # assert prod.nnz == sp_prod.nnz
     if prod.nnz > 0:
         assert prod.values is not None
-    nrows = csra.nrows
+        assert np.all(prod.values != 0)
+    nrows = A.nrows
 
     for i in range(nrows):
-        r_scipy = AB.getrow(i).toarray().ravel()
+        r_scipy = dprod[i, :]
         r_ours = prod.row(i)
 
         assert len(r_ours) == len(r_scipy)
-        assert r_ours == approx(r_scipy)
+        assert r_ours == approx(r_scipy, rel=1.0e-5, abs=1.0e-10)
```

### Comparing `csr-0.4.3/tests/test_numba_mult.py` & `csr-0.5.0a1/tests/test_kernel_numba.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 """
-Internal tests for Numba kernel multiplication code.
+Internal tests for Numba kernel multiplication.
 """
 
 import numpy as np
-import scipy.sparse as sps
 
-from csr import CSR
-from csr.test_utils import csrs, csr_slow, sparse_matrices, mm_pairs
+from csr.test_utils import csr_slow, mm_pairs
 from csr.kernels.numba.multiply import _sym_mm
 
-from pytest import mark, approx, raises
-from hypothesis import given, assume, settings, HealthCheck
-import hypothesis.strategies as st
-import hypothesis.extra.numpy as nph
+from hypothesis import given
 
 
-@settings(deadline=None)
-@given(mm_pairs(max_shape=(50, 1000, 50), as_csr=True))
+@csr_slow()
+@given(mm_pairs(max_shape=(50, 1000, 50)))
 def test_symb(pair):
     A, B = pair
 
     cp = np.zeros_like(A.rowptrs)
 
-    cci = _sym_mm(A.R, B.R, cp)
+    cci = _sym_mm(A, B, cp)
 
     # Is everything in range?
     assert all(cci >= 0)
     assert all(cci < B.ncols)
 
     # Are column pointers nondecreasing?
     assert all(np.diff(cp) >= 0)
```

### Comparing `csr-0.4.3/tests/test_pickle.py` & `csr-0.5.0a1/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `csr-0.4.3/tests/test_transform.py` & `csr-0.5.0a1/tests/test_transform.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import numpy as np
 import scipy.sparse as sps
 
 from csr import CSR
-from csr.test_utils import csrs, csr_slow, sparse_matrices
+from csr.test_utils import csrs, csr_slow
 
-from pytest import mark, approx, raises
-from hypothesis import given, assume, settings, HealthCheck
+from pytest import approx
+from hypothesis import given, assume
 import hypothesis.strategies as st
 import hypothesis.extra.numpy as nph
 
 _log = logging.getLogger(__name__)
 
 
 @csr_slow()
@@ -25,16 +25,16 @@
     spm = sps.random(nrows, ncols, dens, format='csr')
     csr = CSR.from_scipy(spm)
 
     m2 = csr.subset_rows(beg, end)
     assert m2.nrows == end - beg
 
     for i in range(m2.nrows):
-        assert all(m2.row_cs(i) == csr.row_cs(beg+i))
-        assert all(m2.row_vs(i) == csr.row_vs(beg+i))
+        assert all(m2.row_cs(i) == csr.row_cs(beg + i))
+        assert all(m2.row_vs(i) == csr.row_vs(beg + i))
 
 
 @csr_slow()
 @given(st.data())
 def test_pick_rows(data):
     include = data.draw(st.booleans())
     csr = data.draw(csrs())
@@ -74,64 +74,90 @@
     assert x2 == approx(x1)
 
 
 @given(csrs())
 def test_kernel_sort_rows(kernel, csr):
     tv = np.ones(csr.ncols)
     x1 = csr.mult_vec(tv)
-    h = kernel.to_handle(csr.R)
+    h = kernel.to_handle(csr)
     kernel.order_columns(h)
     c2 = kernel.from_handle(h)
     kernel.release_handle(h)
     assert all(all(np.diff(c2.row_cs(i)) > 0) for i in range(csr.nrows))
     x2 = c2.mult_vec(tv)
     assert x2 == approx(x1)
 
 
 @csr_slow()
-@given(sparse_matrices())
-def test_mean_center(spm):
+@given(csrs(values=True))
+def test_mean_center(csr):
     # assume(spm.nnz >= 10)
-    csr = CSR.from_scipy(spm)
+    backup = csr.copy()
+    if csr.values.dtype == np.dtype('f4'):
+        rel_tol = 1.0e-5
+        abs_tol = 1.0e-3
+    else:
+        rel_tol = 1.0e-6
+        abs_tol = 1.0e-10
 
     m2 = csr.normalize_rows('center')
     assert len(m2) == csr.nrows
+    assert m2.dtype == csr.values.dtype
     rnnz = csr.row_nnzs()
 
     for i in range(csr.nrows):
         vs = csr.row_vs(i)
-        spr = spm[i, :].toarray()
-        if rnnz[i] > 0:
-            assert m2[i] == approx(np.sum(spr) / rnnz[i])
-            assert np.mean(vs) == approx(0.0)
-            assert vs + m2[i] == approx(spr[0, csr.row_cs(i)])
+        b_vs = backup.row_vs(i)
+        b_row = backup.row(i)
+
+        try:
+            if rnnz[i] > 0:
+                assert m2[i] == approx(np.mean(b_vs), rel=rel_tol, abs=abs_tol)
+                assert m2[i] == approx(np.sum(b_row) / rnnz[i], rel=rel_tol, abs=abs_tol)
+                assert np.mean(vs) == approx(0.0, rel=rel_tol, abs=abs_tol)
+                assert vs + m2[i] == approx(b_row[csr.row_cs(i)], rel=rel_tol, abs=abs_tol)
+        except Exception as e:
+            _log.error('failure on row %d: %s', i, e)
+            _log.info('row original sum: %e', np.sum(b_vs))
+            _log.info('row original ptp: %e', np.ptp(b_vs))
+            _log.info('row original range: %e, %e', np.min(b_vs), np.max(b_vs))
+            _log.info('row new sum: %e', np.sum(vs))
+            _log.info('row normed mean: %e', m2[i])
+            raise e
 
 
 @csr_slow()
-@given(sparse_matrices())
-def test_unit_norm(spm):
+@given(csrs(values=True))
+def test_unit_norm(csr: CSR):
     # assume(spm.nnz >= 10)
-    csr = CSR.from_scipy(spm)
+    backup = csr.copy()
 
     m2 = csr.normalize_rows('unit')
     assert len(m2) == csr.nrows
+    assert m2.dtype == csr.values.dtype
 
     for i in range(csr.nrows):
         vs = csr.row_vs(i)
+        bvs = backup.row_vs(i)
         if len(vs) > 0:
-            assert np.linalg.norm(vs) == approx(1.0)
-            assert vs * m2[i] == approx(spm.getrow(i).toarray()[0, csr.row_cs(i)])
+            assert m2[i] == approx(np.linalg.norm(bvs))
+            if m2[i] > 0:
+                assert np.linalg.norm(vs) == approx(1.0)
+                assert vs * m2[i] == approx(backup.row_vs(i))
+            else:
+                assert all(np.isnan(vs))
+        else:
+            assert m2[i] == 0.0
 
 
 @csr_slow()
-@given(sparse_matrices())
-def test_filter(mat):
-    assume(mat.nnz > 0)
-    assume(not np.all(mat.data <= 0))  # we have to have at least one to retain
-    csr = CSR.from_scipy(mat)
+@given(csrs(values=True))
+def test_filter(csr):
+    assume(csr.nnz > 0)
+    assume(not np.all(csr.values <= 0))  # we have to have at least one to retain
     csrf = csr.filter_nnzs(csr.values > 0)
     assert all(csrf.values > 0)
     assert csrf.nnz <= csr.nnz
 
     for i in range(csr.nrows):
         spo, epo = csr.row_extent(i)
         spf, epf = csrf.row_extent(i)
@@ -139,19 +165,18 @@
 
     d1 = csr.to_scipy().toarray()
     df = csrf.to_scipy().toarray()
     d1[d1 < 0] = 0
     assert df == approx(d1)
 
 
-# @csr_slow()
-@given(sparse_matrices())
-def test_shard(mat):
+@csr_slow()
+@given(csrs(st.integers(10, 100), st.integers(10, 100), max_density=0.99, values=True))
+def test_shard(csr):
     SHARD_SIZE = 1000
-    csr = CSR.from_scipy(mat)
 
     shards = csr._shard_rows(SHARD_SIZE)
     # we have the whole matrix
     assert sum(s.nnz for s in shards) == csr.nnz
     # everything is in spec
     assert all(s.nnz <= SHARD_SIZE for s in shards)
```

### Comparing `csr-0.4.3/tests/test_transpose.py` & `csr-0.5.0a1/tests/test_transpose.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import numpy as np
 import scipy.sparse as sps
 
 from csr import CSR
-from csr.test_utils import csrs, csr_slow, sparse_matrices
+from csr.test_utils import csrs
 
-from pytest import mark, approx, raises
-from hypothesis import given, assume, settings, HealthCheck
-import hypothesis.strategies as st
-import hypothesis.extra.numpy as nph
+from pytest import approx
+from hypothesis import given
 
 
 def test_csr_transpose():
     rows = np.array([0, 0, 1, 3], dtype=np.int32)
     cols = np.array([1, 2, 0, 1], dtype=np.int32)
     vals = np.arange(4, dtype=np.float_)
 
@@ -45,14 +43,15 @@
 
     for r, c, v in zip(rows, cols, vals):
         row = csc.row(c)
         assert row[r] == 1
 
 
 def test_csr_transpose_erow():
+    "Test transposition with an empty output row"
     nrows = np.random.randint(10, 1000)
     ncols = np.random.randint(10, 500)
     mat = np.random.randn(nrows, ncols)
     mat[mat <= 0] = 0
     mat[:, 0:1] = 0
     smat = sps.csr_matrix(mat)
 
@@ -64,21 +63,19 @@
     s2 = csrt.to_scipy()
     smat = smat.T.tocsr()
     assert all(smat.indptr == csrt.rowptrs)
 
     assert np.all(s2.toarray() == smat.toarray())
 
 
-@given(sparse_matrices())
-def test_csr_transpose_many(smat):
-    nrows, ncols = smat.shape
-    csr = CSR.from_scipy(smat)
+@given(csrs(values=True))
+def test_csr_transpose_many(csr):
     csrt = csr.transpose()
-    assert csrt.nrows == ncols
-    assert csrt.ncols == nrows
+    assert csrt.nrows == csr.ncols
+    assert csrt.ncols == csr.nrows
     assert csrt.nnz == csr.nnz
 
     s2 = csrt.to_scipy()
-    smat = smat.T.tocsr()
+    smat = csr.to_scipy().T.tocsr()
     assert all(smat.indptr == csrt.rowptrs)
 
     assert np.all(s2.toarray() == smat.toarray())
```

### Comparing `csr-0.4.3/PKG-INFO` & `csr-0.5.0a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: csr
-Version: 0.4.3
+Version: 0.5.0a1
 Summary: Compressed Sparse Row matrices for Python, with Numba API.
-Home-page: https://csr.lenskit.org
-Author: Michael Ekstrand <michaelekstrand@boisestate.edu>
-Author-email: michaelekstrand@boisestate.edu
+Author-email: Michael Ekstrand <michaelekstrand@boisestate.edu>
 Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Science/Research
 Requires-Dist: numba >=0.51,<0.57
 Requires-Dist: numpy >=1.17
 Requires-Dist: scipy >=1.2,<2
-Requires-Dist: flit ; extra == "dev"
+Requires-Dist: flit >=3.2,<4 ; extra == "dev"
 Requires-Dist: keyring ; extra == "dev"
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: rstcheck ; extra == "dev"
 Requires-Dist: invoke ; extra == "dev"
 Requires-Dist: lenskit-build-helpers >=0.1 ; extra == "dev"
 Requires-Dist: sphinx-autobuild >=2021 ; extra == "dev"
 Requires-Dist: sphinx >=4 ; extra == "doc"
 Requires-Dist: furo ; extra == "doc"
 Requires-Dist: cffi ; extra == "mkl"
 Requires-Dist: notebook ; extra == "profile"
 Requires-Dist: seaborn ; extra == "profile"
 Requires-Dist: jupytext ; extra == "profile"
 Requires-Dist: pandas >=1.0 ; extra == "profile"
-Requires-Dist: pytest >=6 ; extra == "test"
+Requires-Dist: pytest ==6.* ; extra == "test"
 Requires-Dist: pytest-doctestplus >=0.9 ; extra == "test"
 Requires-Dist: pytest-benchmark >=3 ; extra == "test"
 Requires-Dist: pytest-cov >=2.12 ; extra == "test"
 Requires-Dist: hypothesis ~=6.30 ; extra == "test"
 Requires-Dist: psutil >=5 ; extra == "test"
+Project-URL: home-page, https://csr.lenskit.org
+Project-URL: source, https://github.com/lenskit/csr
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: mkl
 Provides-Extra: profile
 Provides-Extra: test
 
 # CSR Matrices for Python
```


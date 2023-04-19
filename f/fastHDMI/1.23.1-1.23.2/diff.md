# Comparing `tmp/fastHDMI-1.23.1.tar.gz` & `tmp/fastHDMI-1.23.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastHDMI-1.23.1.tar", last modified: Tue Apr 18 05:52:31 2023, max compression
+gzip compressed data, was "fastHDMI-1.23.2.tar", last modified: Wed Apr 19 19:29:19 2023, max compression
```

## Comparing `fastHDMI-1.23.1.tar` & `fastHDMI-1.23.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-18 05:52:31.393534 fastHDMI-1.23.1/
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    34523 2022-11-10 23:21:11.000000 fastHDMI-1.23.1/LICENSE
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      103 2023-04-17 22:35:24.000000 fastHDMI-1.23.1/MANIFEST.in
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    46504 2023-04-18 05:52:31.393534 fastHDMI-1.23.1/PKG-INFO
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     5931 2023-02-19 04:38:00.000000 fastHDMI-1.23.1/README.md
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     1170 2023-04-18 05:39:49.000000 fastHDMI-1.23.1/pyproject.toml
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)       38 2023-04-18 05:52:31.393534 fastHDMI-1.23.1/setup.cfg
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      298 2023-04-16 23:35:56.000000 fastHDMI-1.23.1/setup.py
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-18 05:52:31.389534 fastHDMI-1.23.1/src/
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-18 05:52:31.389534 fastHDMI-1.23.1/src/fastHDMI/
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)   227176 2023-04-18 05:45:38.000000 fastHDMI-1.23.1/src/fastHDMI/__init__.py
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)   900663 2023-04-18 05:52:31.000000 fastHDMI-1.23.1/src/fastHDMI/cython_fun.c
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     1956 2023-04-17 23:03:00.000000 fastHDMI-1.23.1/src/fastHDMI/cython_fun.pyx
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-18 05:52:31.393534 fastHDMI-1.23.1/src/fastHDMI.egg-info/
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    46504 2023-04-18 05:52:31.000000 fastHDMI-1.23.1/src/fastHDMI.egg-info/PKG-INFO
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      325 2023-04-18 05:52:31.000000 fastHDMI-1.23.1/src/fastHDMI.egg-info/SOURCES.txt
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)        1 2023-04-18 05:52:31.000000 fastHDMI-1.23.1/src/fastHDMI.egg-info/dependency_links.txt
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      147 2023-04-18 05:52:31.000000 fastHDMI-1.23.1/src/fastHDMI.egg-info/requires.txt
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)        9 2023-04-18 05:52:31.000000 fastHDMI-1.23.1/src/fastHDMI.egg-info/top_level.txt
-drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-18 05:52:31.393534 fastHDMI-1.23.1/tests/
--rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     4258 2023-04-17 23:06:01.000000 fastHDMI-1.23.1/tests/test.py
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-19 19:29:19.396494 fastHDMI-1.23.2/
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    34523 2022-11-10 23:21:11.000000 fastHDMI-1.23.2/LICENSE
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      103 2023-04-17 22:35:24.000000 fastHDMI-1.23.2/MANIFEST.in
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    46504 2023-04-19 19:29:19.396494 fastHDMI-1.23.2/PKG-INFO
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     5931 2023-02-19 04:38:00.000000 fastHDMI-1.23.2/README.md
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     1170 2023-04-19 19:27:46.000000 fastHDMI-1.23.2/pyproject.toml
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)       38 2023-04-19 19:29:19.396494 fastHDMI-1.23.2/setup.cfg
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      298 2023-04-16 23:35:56.000000 fastHDMI-1.23.2/setup.py
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-19 19:29:19.392495 fastHDMI-1.23.2/src/
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-19 19:29:19.396494 fastHDMI-1.23.2/src/fastHDMI/
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)   227176 2023-04-18 05:45:38.000000 fastHDMI-1.23.2/src/fastHDMI/__init__.py
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)   905624 2023-04-19 19:29:19.000000 fastHDMI-1.23.2/src/fastHDMI/cython_fun.c
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     1958 2023-04-19 19:26:49.000000 fastHDMI-1.23.2/src/fastHDMI/cython_fun.pyx
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-19 19:29:19.396494 fastHDMI-1.23.2/src/fastHDMI.egg-info/
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)    46504 2023-04-19 19:29:19.000000 fastHDMI-1.23.2/src/fastHDMI.egg-info/PKG-INFO
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      325 2023-04-19 19:29:19.000000 fastHDMI-1.23.2/src/fastHDMI.egg-info/SOURCES.txt
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)        1 2023-04-19 19:29:19.000000 fastHDMI-1.23.2/src/fastHDMI.egg-info/dependency_links.txt
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)      147 2023-04-19 19:29:19.000000 fastHDMI-1.23.2/src/fastHDMI.egg-info/requires.txt
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)        9 2023-04-19 19:29:19.000000 fastHDMI-1.23.2/src/fastHDMI.egg-info/top_level.txt
+drwxr-xr-x   0 Snoopy    (1000) kaiseryet  (1000)        0 2023-04-19 19:29:19.396494 fastHDMI-1.23.2/tests/
+-rw-r--r--   0 Snoopy    (1000) kaiseryet  (1000)     4258 2023-04-17 23:06:01.000000 fastHDMI-1.23.2/tests/test.py
```

### Comparing `fastHDMI-1.23.1/LICENSE` & `fastHDMI-1.23.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastHDMI-1.23.1/PKG-INFO` & `fastHDMI-1.23.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastHDMI
-Version: 1.23.1
+Version: 1.23.2
 Summary: Use FFT-based mutual information and accelerated gradient method to screen variables and optimize nonconvex sparse learning problems on large CSV files or large genetic bed/bim/fam files. Multiprocessing is now available.
 Author-email: Kai Yang <kai.yang2@mail.mcgill.ca>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `fastHDMI-1.23.1/README.md` & `fastHDMI-1.23.2/README.md`

 * *Files identical despite different names*

### Comparing `fastHDMI-1.23.1/pyproject.toml` & `fastHDMI-1.23.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel>=0.34.2",
     "Cython>=0.29.21"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastHDMI"
-version = "1.23.1"
+version = "1.23.2"
 authors = [
   { name="Kai Yang", email="kai.yang2@mail.mcgill.ca" },
 ]
 description = "Use FFT-based mutual information and accelerated gradient method to screen variables and optimize nonconvex sparse learning problems on large CSV files or large genetic bed/bim/fam files. Multiprocessing is now available."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `fastHDMI-1.23.1/src/fastHDMI/__init__.py` & `fastHDMI-1.23.2/src/fastHDMI/__init__.py`

 * *Files identical despite different names*

### Comparing `fastHDMI-1.23.1/src/fastHDMI/cython_fun.c` & `fastHDMI-1.23.2/src/fastHDMI/cython_fun.c`

 * *Files 1% similar despite different names*

```diff
@@ -1314,14 +1314,36 @@
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
+/* GetItemInt.proto */
+#define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
+    (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
+               __Pyx_GetItemInt_Generic(o, to_py_func(i))))
+#define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_List_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
+    (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL))
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              int wraparound, int boundscheck);
+#define __Pyx_GetItemInt_Tuple(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_GetItemInt_Tuple_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
+    (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              int wraparound, int boundscheck);
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
+                                                     int is_list, int wraparound, int boundscheck);
+
 /* PyDictContains.proto */
 static CYTHON_INLINE int __Pyx_PyDict_ContainsTF(PyObject* item, PyObject* dict, int eq) {
     int result = PyDict_Contains(dict, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
 /* DictGetItem.proto */
@@ -1497,36 +1519,14 @@
                                                    Py_ssize_t* p_orig_length, int* p_is_dict);
 static CYTHON_INLINE int __Pyx_dict_iter_next(PyObject* dict_or_iter, Py_ssize_t orig_length, Py_ssize_t* ppos,
                                               PyObject** pkey, PyObject** pvalue, PyObject** pitem, int is_dict);
 
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
-/* GetItemInt.proto */
-#define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
-    (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
-               __Pyx_GetItemInt_Generic(o, to_py_func(i))))
-#define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_List_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
-    (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL))
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              int wraparound, int boundscheck);
-#define __Pyx_GetItemInt_Tuple(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
-    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
-    __Pyx_GetItemInt_Tuple_Fast(o, (Py_ssize_t)i, wraparound, boundscheck) :\
-    (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              int wraparound, int boundscheck);
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
-                                                     int is_list, int wraparound, int boundscheck);
-
 /* ListAppend.proto */
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
@@ -1536,14 +1536,17 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* BufferIndexError.proto */
+static void __Pyx_RaiseBufferIndexError(int axis);
+
 /* MemviewSliceInit.proto */
 #define __Pyx_BUF_MAX_NDIMS %(BUF_MAX_NDIMS)d
 #define __Pyx_MEMVIEW_DIRECT   1
 #define __Pyx_MEMVIEW_PTR      2
 #define __Pyx_MEMVIEW_FULL     4
 #define __Pyx_MEMVIEW_CONTIG   8
 #define __Pyx_MEMVIEW_STRIDED  16
@@ -2426,15 +2429,15 @@
 static PyObject *__pyx_tuple__33;
 static PyObject *__pyx_tuple__34;
 static PyObject *__pyx_codeobj__28;
 static PyObject *__pyx_codeobj__35;
 /* Late includes */
 
 /* "fastHDMI/cython_fun.pyx":12
- * @cython.boundscheck(False)
+ * # @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def joint_to_mi_cython(floating_float_double[:, ::1] joint, floating_float_double forward_euler_a=1., floating_float_double forward_euler_b=1.):             # <<<<<<<<<<<<<<
  *     cdef int i, j
  *     cdef int joint_shape0 = joint.shape[0]
  */
 
 /* Python wrapper */
@@ -2601,16 +2604,16 @@
   __pyx_t_5 = PyTuple_GET_SIZE(((PyObject*)__pyx_v_args)); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 12, __pyx_L1_error)
   __pyx_t_2 = ((0 < __pyx_t_5) != 0);
   if (__pyx_t_2) {
     if (unlikely(__pyx_v_args == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
       __PYX_ERR(0, 12, __pyx_L1_error)
     }
-    __pyx_t_1 = PyTuple_GET_ITEM(((PyObject*)__pyx_v_args), 0);
-    __Pyx_INCREF(__pyx_t_1);
+    __pyx_t_1 = __Pyx_GetItemInt_Tuple(((PyObject*)__pyx_v_args), 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __pyx_v_arg = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L6;
   }
   __pyx_t_3 = (__pyx_v_kwargs != Py_None);
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
@@ -2738,15 +2741,15 @@
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 12, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 2) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L16_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 12, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float, long, 1, __Pyx_PyInt_From_long, 1, 0, 1) < 0)) __PYX_ERR(0, 12, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           __pyx_t_2 = (((sizeof(double)) == __pyx_v_itemsize) != 0);
           if (__pyx_t_2) {
           } else {
             __pyx_t_3 = __pyx_t_2;
             goto __pyx_L19_bool_binop_done;
@@ -2755,15 +2758,15 @@
           __Pyx_GOTREF(__pyx_t_6);
           __pyx_t_5 = __Pyx_PyIndex_AsSsize_t(__pyx_t_6); if (unlikely((__pyx_t_5 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 12, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
           __pyx_t_2 = ((((Py_ssize_t)__pyx_t_5) == 2) != 0);
           __pyx_t_3 = __pyx_t_2;
           __pyx_L19_bool_binop_done:;
           if (__pyx_t_3) {
-            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_double, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 12, __pyx_L1_error)
+            if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_double, long, 1, __Pyx_PyInt_From_long, 1, 0, 1) < 0)) __PYX_ERR(0, 12, __pyx_L1_error)
             goto __pyx_L10_break;
           }
           break;
           case 'c':
           break;
           case 'O':
           break;
@@ -2782,15 +2785,15 @@
     __pyx_L22_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_float(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 12, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_float, long, 1, __Pyx_PyInt_From_long, 1, 0, 1) < 0)) __PYX_ERR(0, 12, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
     __pyx_t_2 = ((__pyx_v_itemsize == -1L) != 0);
@@ -2804,22 +2807,22 @@
     __pyx_L26_bool_binop_done:;
     if (__pyx_t_3) {
       __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_d_dc_double(__pyx_v_arg, 0); 
       __pyx_v_memslice = __pyx_t_8;
       __pyx_t_3 = (__pyx_v_memslice.memview != 0);
       if (__pyx_t_3) {
         __PYX_XDEC_MEMVIEW((&__pyx_v_memslice), 1); 
-        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_double, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 12, __pyx_L1_error)
+        if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, __pyx_n_s_double, long, 1, __Pyx_PyInt_From_long, 1, 0, 1) < 0)) __PYX_ERR(0, 12, __pyx_L1_error)
         goto __pyx_L10_break;
       }
       /*else*/ {
         PyErr_Clear(); 
       }
     }
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, Py_None, long, 1, __Pyx_PyInt_From_long, 1, 0, 0) < 0)) __PYX_ERR(0, 12, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_dest_sig, 0, Py_None, long, 1, __Pyx_PyInt_From_long, 1, 0, 1) < 0)) __PYX_ERR(0, 12, __pyx_L1_error)
     goto __pyx_L10_break;
   }
   __pyx_L10_break:;
   __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_v_candidates = ((PyObject*)__pyx_t_6);
   __pyx_t_6 = 0;
@@ -2878,22 +2881,22 @@
     __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
     __Pyx_XDECREF_SET(__pyx_v_src_sig, __pyx_t_1);
     __pyx_t_1 = 0;
     __pyx_t_15 = PyList_GET_SIZE(__pyx_v_dest_sig); if (unlikely(__pyx_t_15 == ((Py_ssize_t)-1))) __PYX_ERR(0, 12, __pyx_L1_error)
     __pyx_t_16 = __pyx_t_15;
     for (__pyx_t_17 = 0; __pyx_t_17 < __pyx_t_16; __pyx_t_17+=1) {
       __pyx_v_i = __pyx_t_17;
-      __pyx_t_1 = PyList_GET_ITEM(__pyx_v_dest_sig, __pyx_v_i);
-      __Pyx_INCREF(__pyx_t_1);
+      __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_dest_sig, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
       __Pyx_XDECREF_SET(__pyx_v_dst_type, __pyx_t_1);
       __pyx_t_1 = 0;
       __pyx_t_3 = (__pyx_v_dst_type != Py_None);
       __pyx_t_2 = (__pyx_t_3 != 0);
       if (__pyx_t_2) {
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_src_sig, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_src_sig, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_t_13 = PyObject_RichCompare(__pyx_t_1, __pyx_v_dst_type, Py_EQ); __Pyx_XGOTREF(__pyx_t_13); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 12, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_13); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 12, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         if (__pyx_t_2) {
           __pyx_v_match_found = 1;
@@ -2933,18 +2936,21 @@
   }
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     if (unlikely(__pyx_v_signatures == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
       __PYX_ERR(0, 12, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_signatures), PyList_GET_ITEM(__pyx_v_candidates, 0)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 12, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_GetItemInt_List(__pyx_v_candidates, 0, long, 1, __Pyx_PyInt_From_long, 1, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 12, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_r = __pyx_t_6;
-    __pyx_t_6 = 0;
+    __pyx_t_13 = __Pyx_PyDict_GetItem(((PyObject*)__pyx_v_signatures), __pyx_t_6); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 12, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_13);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_r = __pyx_t_13;
+    __pyx_t_13 = 0;
     goto __pyx_L0;
   }
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_6);
@@ -3126,20 +3132,21 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_t_7;
   Py_ssize_t __pyx_t_8;
   Py_ssize_t __pyx_t_9;
-  double __pyx_t_10;
-  Py_ssize_t __pyx_t_11;
+  int __pyx_t_10;
+  double __pyx_t_11;
   Py_ssize_t __pyx_t_12;
-  float __pyx_t_13;
-  double __pyx_t_14;
-  PyObject *__pyx_t_15 = NULL;
+  Py_ssize_t __pyx_t_13;
+  float __pyx_t_14;
+  double __pyx_t_15;
+  PyObject *__pyx_t_16 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_0joint_to_mi_cython", 0);
 
   /* "fastHDMI/cython_fun.pyx":14
  * def joint_to_mi_cython(floating_float_double[:, ::1] joint, floating_float_double forward_euler_a=1., floating_float_double forward_euler_b=1.):
@@ -3216,26 +3223,48 @@
  *             log_a_marginal[i] += joint[i, j]             # <<<<<<<<<<<<<<
  *             log_b_marginal[j] += joint[i, j]
  *         temp_sum += log_a_marginal[i]
  */
       __pyx_t_7 = __pyx_v_i;
       __pyx_t_8 = __pyx_v_i;
       __pyx_t_9 = __pyx_v_j;
+      __pyx_t_10 = -1;
+      if (__pyx_t_8 < 0) {
+        __pyx_t_10 = 0;
+      } else if (unlikely(__pyx_t_8 >= __pyx_v_joint.shape[0])) __pyx_t_10 = 0;
+      if (__pyx_t_9 < 0) {
+        __pyx_t_10 = 1;
+      } else if (unlikely(__pyx_t_9 >= __pyx_v_joint.shape[1])) __pyx_t_10 = 1;
+      if (unlikely(__pyx_t_10 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_10);
+        __PYX_ERR(0, 23, __pyx_L1_error)
+      }
       (__pyx_v_log_a_marginal[__pyx_t_7]) = ((__pyx_v_log_a_marginal[__pyx_t_7]) + (*((float *) ( /* dim=1 */ ((char *) (((float *) ( /* dim=0 */ (__pyx_v_joint.data + __pyx_t_8 * __pyx_v_joint.strides[0]) )) + __pyx_t_9)) ))));
 
       /* "fastHDMI/cython_fun.pyx":24
  *         for j in range(joint_shape1):
  *             log_a_marginal[i] += joint[i, j]
  *             log_b_marginal[j] += joint[i, j]             # <<<<<<<<<<<<<<
  *         temp_sum += log_a_marginal[i]
  *     temp_sum *= forward_euler_a * forward_euler_b
  */
       __pyx_t_7 = __pyx_v_j;
       __pyx_t_9 = __pyx_v_i;
       __pyx_t_8 = __pyx_v_j;
+      __pyx_t_10 = -1;
+      if (__pyx_t_9 < 0) {
+        __pyx_t_10 = 0;
+      } else if (unlikely(__pyx_t_9 >= __pyx_v_joint.shape[0])) __pyx_t_10 = 0;
+      if (__pyx_t_8 < 0) {
+        __pyx_t_10 = 1;
+      } else if (unlikely(__pyx_t_8 >= __pyx_v_joint.shape[1])) __pyx_t_10 = 1;
+      if (unlikely(__pyx_t_10 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_10);
+        __PYX_ERR(0, 24, __pyx_L1_error)
+      }
       (__pyx_v_log_b_marginal[__pyx_t_7]) = ((__pyx_v_log_b_marginal[__pyx_t_7]) + (*((float *) ( /* dim=1 */ ((char *) (((float *) ( /* dim=0 */ (__pyx_v_joint.data + __pyx_t_9 * __pyx_v_joint.strides[0]) )) + __pyx_t_8)) ))));
     }
 
     /* "fastHDMI/cython_fun.pyx":25
  *             log_a_marginal[i] += joint[i, j]
  *             log_b_marginal[j] += joint[i, j]
  *         temp_sum += log_a_marginal[i]             # <<<<<<<<<<<<<<
@@ -3297,19 +3326,19 @@
  * 
  *     for i in range(joint_shape0):
  *         log_a_marginal[i] = log(log_a_marginal[i]) + log_forward_euler_b if isfinite(log(log_a_marginal[i])) else 0.0             # <<<<<<<<<<<<<<
  *     for j in range(joint_shape1):
  *         log_b_marginal[j] = log(log_b_marginal[j]) + log_forward_euler_a if isfinite(log(log_b_marginal[j])) else 0.0
  */
     if ((isfinite(log((__pyx_v_log_a_marginal[__pyx_v_i]))) != 0)) {
-      __pyx_t_10 = (log((__pyx_v_log_a_marginal[__pyx_v_i])) + __pyx_v_log_forward_euler_b);
+      __pyx_t_11 = (log((__pyx_v_log_a_marginal[__pyx_v_i])) + __pyx_v_log_forward_euler_b);
     } else {
-      __pyx_t_10 = 0.0;
+      __pyx_t_11 = 0.0;
     }
-    (__pyx_v_log_a_marginal[__pyx_v_i]) = __pyx_t_10;
+    (__pyx_v_log_a_marginal[__pyx_v_i]) = __pyx_t_11;
   }
 
   /* "fastHDMI/cython_fun.pyx":33
  *     for i in range(joint_shape0):
  *         log_a_marginal[i] = log(log_a_marginal[i]) + log_forward_euler_b if isfinite(log(log_a_marginal[i])) else 0.0
  *     for j in range(joint_shape1):             # <<<<<<<<<<<<<<
  *         log_b_marginal[j] = log(log_b_marginal[j]) + log_forward_euler_a if isfinite(log(log_b_marginal[j])) else 0.0
@@ -3324,19 +3353,19 @@
  *         log_a_marginal[i] = log(log_a_marginal[i]) + log_forward_euler_b if isfinite(log(log_a_marginal[i])) else 0.0
  *     for j in range(joint_shape1):
  *         log_b_marginal[j] = log(log_b_marginal[j]) + log_forward_euler_a if isfinite(log(log_b_marginal[j])) else 0.0             # <<<<<<<<<<<<<<
  * 
  *     output = 0.0
  */
     if ((isfinite(log((__pyx_v_log_b_marginal[__pyx_v_j]))) != 0)) {
-      __pyx_t_10 = (log((__pyx_v_log_b_marginal[__pyx_v_j])) + __pyx_v_log_forward_euler_a);
+      __pyx_t_11 = (log((__pyx_v_log_b_marginal[__pyx_v_j])) + __pyx_v_log_forward_euler_a);
     } else {
-      __pyx_t_10 = 0.0;
+      __pyx_t_11 = 0.0;
     }
-    (__pyx_v_log_b_marginal[__pyx_v_j]) = __pyx_t_10;
+    (__pyx_v_log_b_marginal[__pyx_v_j]) = __pyx_t_11;
   }
 
   /* "fastHDMI/cython_fun.pyx":36
  *         log_b_marginal[j] = log(log_b_marginal[j]) + log_forward_euler_a if isfinite(log(log_b_marginal[j])) else 0.0
  * 
  *     output = 0.0             # <<<<<<<<<<<<<<
  *     for i in range(joint_shape0):
@@ -3373,51 +3402,84 @@
  *         for j in range(joint_shape1):
  *             log_joint = log(joint[i, j]) if isfinite(log(joint[i, j])) else 0.0             # <<<<<<<<<<<<<<
  *             output += joint[i, j] * (log_joint - log_a_marginal[i] - log_b_marginal[j]) * forward_euler_a * forward_euler_b
  * 
  */
       __pyx_t_8 = __pyx_v_i;
       __pyx_t_9 = __pyx_v_j;
+      __pyx_t_7 = -1;
+      if (__pyx_t_8 < 0) {
+        __pyx_t_7 = 0;
+      } else if (unlikely(__pyx_t_8 >= __pyx_v_joint.shape[0])) __pyx_t_7 = 0;
+      if (__pyx_t_9 < 0) {
+        __pyx_t_7 = 1;
+      } else if (unlikely(__pyx_t_9 >= __pyx_v_joint.shape[1])) __pyx_t_7 = 1;
+      if (unlikely(__pyx_t_7 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_7);
+        __PYX_ERR(0, 39, __pyx_L1_error)
+      }
       if ((isfinite(log((*((float *) ( /* dim=1 */ ((char *) (((float *) ( /* dim=0 */ (__pyx_v_joint.data + __pyx_t_8 * __pyx_v_joint.strides[0]) )) + __pyx_t_9)) ))))) != 0)) {
-        __pyx_t_11 = __pyx_v_i;
-        __pyx_t_12 = __pyx_v_j;
-        __pyx_t_10 = log((*((float *) ( /* dim=1 */ ((char *) (((float *) ( /* dim=0 */ (__pyx_v_joint.data + __pyx_t_11 * __pyx_v_joint.strides[0]) )) + __pyx_t_12)) ))));
+        __pyx_t_12 = __pyx_v_i;
+        __pyx_t_13 = __pyx_v_j;
+        __pyx_t_7 = -1;
+        if (__pyx_t_12 < 0) {
+          __pyx_t_7 = 0;
+        } else if (unlikely(__pyx_t_12 >= __pyx_v_joint.shape[0])) __pyx_t_7 = 0;
+        if (__pyx_t_13 < 0) {
+          __pyx_t_7 = 1;
+        } else if (unlikely(__pyx_t_13 >= __pyx_v_joint.shape[1])) __pyx_t_7 = 1;
+        if (unlikely(__pyx_t_7 != -1)) {
+          __Pyx_RaiseBufferIndexError(__pyx_t_7);
+          __PYX_ERR(0, 39, __pyx_L1_error)
+        }
+        __pyx_t_11 = log((*((float *) ( /* dim=1 */ ((char *) (((float *) ( /* dim=0 */ (__pyx_v_joint.data + __pyx_t_12 * __pyx_v_joint.strides[0]) )) + __pyx_t_13)) ))));
       } else {
-        __pyx_t_10 = 0.0;
+        __pyx_t_11 = 0.0;
       }
-      __pyx_v_log_joint = __pyx_t_10;
+      __pyx_v_log_joint = __pyx_t_11;
 
       /* "fastHDMI/cython_fun.pyx":40
  *         for j in range(joint_shape1):
  *             log_joint = log(joint[i, j]) if isfinite(log(joint[i, j])) else 0.0
  *             output += joint[i, j] * (log_joint - log_a_marginal[i] - log_b_marginal[j]) * forward_euler_a * forward_euler_b             # <<<<<<<<<<<<<<
  * 
  *     output = max(output, 0.0)
  */
       __pyx_t_9 = __pyx_v_i;
       __pyx_t_8 = __pyx_v_j;
+      __pyx_t_7 = -1;
+      if (__pyx_t_9 < 0) {
+        __pyx_t_7 = 0;
+      } else if (unlikely(__pyx_t_9 >= __pyx_v_joint.shape[0])) __pyx_t_7 = 0;
+      if (__pyx_t_8 < 0) {
+        __pyx_t_7 = 1;
+      } else if (unlikely(__pyx_t_8 >= __pyx_v_joint.shape[1])) __pyx_t_7 = 1;
+      if (unlikely(__pyx_t_7 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_7);
+        __PYX_ERR(0, 40, __pyx_L1_error)
+      }
       __pyx_v_output = (__pyx_v_output + ((((*((float *) ( /* dim=1 */ ((char *) (((float *) ( /* dim=0 */ (__pyx_v_joint.data + __pyx_t_9 * __pyx_v_joint.strides[0]) )) + __pyx_t_8)) ))) * ((__pyx_v_log_joint - (__pyx_v_log_a_marginal[__pyx_v_i])) - (__pyx_v_log_b_marginal[__pyx_v_j]))) * __pyx_v_forward_euler_a) * __pyx_v_forward_euler_b));
     }
   }
 
   /* "fastHDMI/cython_fun.pyx":42
  *             output += joint[i, j] * (log_joint - log_a_marginal[i] - log_b_marginal[j]) * forward_euler_a * forward_euler_b
  * 
  *     output = max(output, 0.0)             # <<<<<<<<<<<<<<
  * 
  *     free(log_a_marginal)
  */
-  __pyx_t_10 = 0.0;
-  __pyx_t_13 = __pyx_v_output;
-  if (((__pyx_t_10 > __pyx_t_13) != 0)) {
-    __pyx_t_14 = __pyx_t_10;
+  __pyx_t_11 = 0.0;
+  __pyx_t_14 = __pyx_v_output;
+  if (((__pyx_t_11 > __pyx_t_14) != 0)) {
+    __pyx_t_15 = __pyx_t_11;
   } else {
-    __pyx_t_14 = __pyx_t_13;
+    __pyx_t_15 = __pyx_t_14;
   }
-  __pyx_v_output = __pyx_t_14;
+  __pyx_v_output = __pyx_t_15;
 
   /* "fastHDMI/cython_fun.pyx":44
  *     output = max(output, 0.0)
  * 
  *     free(log_a_marginal)             # <<<<<<<<<<<<<<
  *     free(log_b_marginal)
  * 
@@ -3435,31 +3497,31 @@
 
   /* "fastHDMI/cython_fun.pyx":47
  *     free(log_b_marginal)
  * 
  *     return output             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_15 = PyFloat_FromDouble(__pyx_v_output); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 47, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_15);
-  __pyx_r = __pyx_t_15;
-  __pyx_t_15 = 0;
+  __pyx_t_16 = PyFloat_FromDouble(__pyx_v_output); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_16);
+  __pyx_r = __pyx_t_16;
+  __pyx_t_16 = 0;
   goto __pyx_L0;
 
   /* "fastHDMI/cython_fun.pyx":12
- * @cython.boundscheck(False)
+ * # @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def joint_to_mi_cython(floating_float_double[:, ::1] joint, floating_float_double forward_euler_a=1., floating_float_double forward_euler_b=1.):             # <<<<<<<<<<<<<<
  *     cdef int i, j
  *     cdef int joint_shape0 = joint.shape[0]
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_15);
+  __Pyx_XDECREF(__pyx_t_16);
   __Pyx_AddTraceback("fastHDMI.cython_fun.joint_to_mi_cython", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_joint, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -3622,20 +3684,21 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_t_7;
   Py_ssize_t __pyx_t_8;
   Py_ssize_t __pyx_t_9;
-  double __pyx_t_10;
-  Py_ssize_t __pyx_t_11;
+  int __pyx_t_10;
+  double __pyx_t_11;
   Py_ssize_t __pyx_t_12;
-  double __pyx_t_13;
+  Py_ssize_t __pyx_t_13;
   double __pyx_t_14;
-  PyObject *__pyx_t_15 = NULL;
+  double __pyx_t_15;
+  PyObject *__pyx_t_16 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_fuse_1joint_to_mi_cython", 0);
 
   /* "fastHDMI/cython_fun.pyx":14
  * def joint_to_mi_cython(floating_float_double[:, ::1] joint, floating_float_double forward_euler_a=1., floating_float_double forward_euler_b=1.):
@@ -3712,26 +3775,48 @@
  *             log_a_marginal[i] += joint[i, j]             # <<<<<<<<<<<<<<
  *             log_b_marginal[j] += joint[i, j]
  *         temp_sum += log_a_marginal[i]
  */
       __pyx_t_7 = __pyx_v_i;
       __pyx_t_8 = __pyx_v_i;
       __pyx_t_9 = __pyx_v_j;
+      __pyx_t_10 = -1;
+      if (__pyx_t_8 < 0) {
+        __pyx_t_10 = 0;
+      } else if (unlikely(__pyx_t_8 >= __pyx_v_joint.shape[0])) __pyx_t_10 = 0;
+      if (__pyx_t_9 < 0) {
+        __pyx_t_10 = 1;
+      } else if (unlikely(__pyx_t_9 >= __pyx_v_joint.shape[1])) __pyx_t_10 = 1;
+      if (unlikely(__pyx_t_10 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_10);
+        __PYX_ERR(0, 23, __pyx_L1_error)
+      }
       (__pyx_v_log_a_marginal[__pyx_t_7]) = ((__pyx_v_log_a_marginal[__pyx_t_7]) + (*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_joint.data + __pyx_t_8 * __pyx_v_joint.strides[0]) )) + __pyx_t_9)) ))));
 
       /* "fastHDMI/cython_fun.pyx":24
  *         for j in range(joint_shape1):
  *             log_a_marginal[i] += joint[i, j]
  *             log_b_marginal[j] += joint[i, j]             # <<<<<<<<<<<<<<
  *         temp_sum += log_a_marginal[i]
  *     temp_sum *= forward_euler_a * forward_euler_b
  */
       __pyx_t_7 = __pyx_v_j;
       __pyx_t_9 = __pyx_v_i;
       __pyx_t_8 = __pyx_v_j;
+      __pyx_t_10 = -1;
+      if (__pyx_t_9 < 0) {
+        __pyx_t_10 = 0;
+      } else if (unlikely(__pyx_t_9 >= __pyx_v_joint.shape[0])) __pyx_t_10 = 0;
+      if (__pyx_t_8 < 0) {
+        __pyx_t_10 = 1;
+      } else if (unlikely(__pyx_t_8 >= __pyx_v_joint.shape[1])) __pyx_t_10 = 1;
+      if (unlikely(__pyx_t_10 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_10);
+        __PYX_ERR(0, 24, __pyx_L1_error)
+      }
       (__pyx_v_log_b_marginal[__pyx_t_7]) = ((__pyx_v_log_b_marginal[__pyx_t_7]) + (*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_joint.data + __pyx_t_9 * __pyx_v_joint.strides[0]) )) + __pyx_t_8)) ))));
     }
 
     /* "fastHDMI/cython_fun.pyx":25
  *             log_a_marginal[i] += joint[i, j]
  *             log_b_marginal[j] += joint[i, j]
  *         temp_sum += log_a_marginal[i]             # <<<<<<<<<<<<<<
@@ -3793,19 +3878,19 @@
  * 
  *     for i in range(joint_shape0):
  *         log_a_marginal[i] = log(log_a_marginal[i]) + log_forward_euler_b if isfinite(log(log_a_marginal[i])) else 0.0             # <<<<<<<<<<<<<<
  *     for j in range(joint_shape1):
  *         log_b_marginal[j] = log(log_b_marginal[j]) + log_forward_euler_a if isfinite(log(log_b_marginal[j])) else 0.0
  */
     if ((isfinite(log((__pyx_v_log_a_marginal[__pyx_v_i]))) != 0)) {
-      __pyx_t_10 = (log((__pyx_v_log_a_marginal[__pyx_v_i])) + __pyx_v_log_forward_euler_b);
+      __pyx_t_11 = (log((__pyx_v_log_a_marginal[__pyx_v_i])) + __pyx_v_log_forward_euler_b);
     } else {
-      __pyx_t_10 = 0.0;
+      __pyx_t_11 = 0.0;
     }
-    (__pyx_v_log_a_marginal[__pyx_v_i]) = __pyx_t_10;
+    (__pyx_v_log_a_marginal[__pyx_v_i]) = __pyx_t_11;
   }
 
   /* "fastHDMI/cython_fun.pyx":33
  *     for i in range(joint_shape0):
  *         log_a_marginal[i] = log(log_a_marginal[i]) + log_forward_euler_b if isfinite(log(log_a_marginal[i])) else 0.0
  *     for j in range(joint_shape1):             # <<<<<<<<<<<<<<
  *         log_b_marginal[j] = log(log_b_marginal[j]) + log_forward_euler_a if isfinite(log(log_b_marginal[j])) else 0.0
@@ -3820,19 +3905,19 @@
  *         log_a_marginal[i] = log(log_a_marginal[i]) + log_forward_euler_b if isfinite(log(log_a_marginal[i])) else 0.0
  *     for j in range(joint_shape1):
  *         log_b_marginal[j] = log(log_b_marginal[j]) + log_forward_euler_a if isfinite(log(log_b_marginal[j])) else 0.0             # <<<<<<<<<<<<<<
  * 
  *     output = 0.0
  */
     if ((isfinite(log((__pyx_v_log_b_marginal[__pyx_v_j]))) != 0)) {
-      __pyx_t_10 = (log((__pyx_v_log_b_marginal[__pyx_v_j])) + __pyx_v_log_forward_euler_a);
+      __pyx_t_11 = (log((__pyx_v_log_b_marginal[__pyx_v_j])) + __pyx_v_log_forward_euler_a);
     } else {
-      __pyx_t_10 = 0.0;
+      __pyx_t_11 = 0.0;
     }
-    (__pyx_v_log_b_marginal[__pyx_v_j]) = __pyx_t_10;
+    (__pyx_v_log_b_marginal[__pyx_v_j]) = __pyx_t_11;
   }
 
   /* "fastHDMI/cython_fun.pyx":36
  *         log_b_marginal[j] = log(log_b_marginal[j]) + log_forward_euler_a if isfinite(log(log_b_marginal[j])) else 0.0
  * 
  *     output = 0.0             # <<<<<<<<<<<<<<
  *     for i in range(joint_shape0):
@@ -3869,51 +3954,84 @@
  *         for j in range(joint_shape1):
  *             log_joint = log(joint[i, j]) if isfinite(log(joint[i, j])) else 0.0             # <<<<<<<<<<<<<<
  *             output += joint[i, j] * (log_joint - log_a_marginal[i] - log_b_marginal[j]) * forward_euler_a * forward_euler_b
  * 
  */
       __pyx_t_8 = __pyx_v_i;
       __pyx_t_9 = __pyx_v_j;
+      __pyx_t_7 = -1;
+      if (__pyx_t_8 < 0) {
+        __pyx_t_7 = 0;
+      } else if (unlikely(__pyx_t_8 >= __pyx_v_joint.shape[0])) __pyx_t_7 = 0;
+      if (__pyx_t_9 < 0) {
+        __pyx_t_7 = 1;
+      } else if (unlikely(__pyx_t_9 >= __pyx_v_joint.shape[1])) __pyx_t_7 = 1;
+      if (unlikely(__pyx_t_7 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_7);
+        __PYX_ERR(0, 39, __pyx_L1_error)
+      }
       if ((isfinite(log((*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_joint.data + __pyx_t_8 * __pyx_v_joint.strides[0]) )) + __pyx_t_9)) ))))) != 0)) {
-        __pyx_t_11 = __pyx_v_i;
-        __pyx_t_12 = __pyx_v_j;
-        __pyx_t_10 = log((*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_joint.data + __pyx_t_11 * __pyx_v_joint.strides[0]) )) + __pyx_t_12)) ))));
+        __pyx_t_12 = __pyx_v_i;
+        __pyx_t_13 = __pyx_v_j;
+        __pyx_t_7 = -1;
+        if (__pyx_t_12 < 0) {
+          __pyx_t_7 = 0;
+        } else if (unlikely(__pyx_t_12 >= __pyx_v_joint.shape[0])) __pyx_t_7 = 0;
+        if (__pyx_t_13 < 0) {
+          __pyx_t_7 = 1;
+        } else if (unlikely(__pyx_t_13 >= __pyx_v_joint.shape[1])) __pyx_t_7 = 1;
+        if (unlikely(__pyx_t_7 != -1)) {
+          __Pyx_RaiseBufferIndexError(__pyx_t_7);
+          __PYX_ERR(0, 39, __pyx_L1_error)
+        }
+        __pyx_t_11 = log((*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_joint.data + __pyx_t_12 * __pyx_v_joint.strides[0]) )) + __pyx_t_13)) ))));
       } else {
-        __pyx_t_10 = 0.0;
+        __pyx_t_11 = 0.0;
       }
-      __pyx_v_log_joint = __pyx_t_10;
+      __pyx_v_log_joint = __pyx_t_11;
 
       /* "fastHDMI/cython_fun.pyx":40
  *         for j in range(joint_shape1):
  *             log_joint = log(joint[i, j]) if isfinite(log(joint[i, j])) else 0.0
  *             output += joint[i, j] * (log_joint - log_a_marginal[i] - log_b_marginal[j]) * forward_euler_a * forward_euler_b             # <<<<<<<<<<<<<<
  * 
  *     output = max(output, 0.0)
  */
       __pyx_t_9 = __pyx_v_i;
       __pyx_t_8 = __pyx_v_j;
+      __pyx_t_7 = -1;
+      if (__pyx_t_9 < 0) {
+        __pyx_t_7 = 0;
+      } else if (unlikely(__pyx_t_9 >= __pyx_v_joint.shape[0])) __pyx_t_7 = 0;
+      if (__pyx_t_8 < 0) {
+        __pyx_t_7 = 1;
+      } else if (unlikely(__pyx_t_8 >= __pyx_v_joint.shape[1])) __pyx_t_7 = 1;
+      if (unlikely(__pyx_t_7 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_7);
+        __PYX_ERR(0, 40, __pyx_L1_error)
+      }
       __pyx_v_output = (__pyx_v_output + ((((*((double *) ( /* dim=1 */ ((char *) (((double *) ( /* dim=0 */ (__pyx_v_joint.data + __pyx_t_9 * __pyx_v_joint.strides[0]) )) + __pyx_t_8)) ))) * ((__pyx_v_log_joint - (__pyx_v_log_a_marginal[__pyx_v_i])) - (__pyx_v_log_b_marginal[__pyx_v_j]))) * __pyx_v_forward_euler_a) * __pyx_v_forward_euler_b));
     }
   }
 
   /* "fastHDMI/cython_fun.pyx":42
  *             output += joint[i, j] * (log_joint - log_a_marginal[i] - log_b_marginal[j]) * forward_euler_a * forward_euler_b
  * 
  *     output = max(output, 0.0)             # <<<<<<<<<<<<<<
  * 
  *     free(log_a_marginal)
  */
-  __pyx_t_10 = 0.0;
-  __pyx_t_13 = __pyx_v_output;
-  if (((__pyx_t_10 > __pyx_t_13) != 0)) {
-    __pyx_t_14 = __pyx_t_10;
+  __pyx_t_11 = 0.0;
+  __pyx_t_14 = __pyx_v_output;
+  if (((__pyx_t_11 > __pyx_t_14) != 0)) {
+    __pyx_t_15 = __pyx_t_11;
   } else {
-    __pyx_t_14 = __pyx_t_13;
+    __pyx_t_15 = __pyx_t_14;
   }
-  __pyx_v_output = __pyx_t_14;
+  __pyx_v_output = __pyx_t_15;
 
   /* "fastHDMI/cython_fun.pyx":44
  *     output = max(output, 0.0)
  * 
  *     free(log_a_marginal)             # <<<<<<<<<<<<<<
  *     free(log_b_marginal)
  * 
@@ -3931,31 +4049,31 @@
 
   /* "fastHDMI/cython_fun.pyx":47
  *     free(log_b_marginal)
  * 
  *     return output             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_15 = PyFloat_FromDouble(__pyx_v_output); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 47, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_15);
-  __pyx_r = __pyx_t_15;
-  __pyx_t_15 = 0;
+  __pyx_t_16 = PyFloat_FromDouble(__pyx_v_output); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_16);
+  __pyx_r = __pyx_t_16;
+  __pyx_t_16 = 0;
   goto __pyx_L0;
 
   /* "fastHDMI/cython_fun.pyx":12
- * @cython.boundscheck(False)
+ * # @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def joint_to_mi_cython(floating_float_double[:, ::1] joint, floating_float_double forward_euler_a=1., floating_float_double forward_euler_b=1.):             # <<<<<<<<<<<<<<
  *     cdef int i, j
  *     cdef int joint_shape0 = joint.shape[0]
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_15);
+  __Pyx_XDECREF(__pyx_t_16);
   __Pyx_AddTraceback("fastHDMI.cython_fun.joint_to_mi_cython", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_joint, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -17913,15 +18031,15 @@
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
   /* "fastHDMI/cython_fun.pyx":12
- * @cython.boundscheck(False)
+ * # @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def joint_to_mi_cython(floating_float_double[:, ::1] joint, floating_float_double forward_euler_a=1., floating_float_double forward_euler_b=1.):             # <<<<<<<<<<<<<<
  *     cdef int i, j
  *     cdef int joint_shape0 = joint.shape[0]
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_No_matching_signature_found); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
@@ -18122,15 +18240,15 @@
   __Pyx_GOTREF(__pyx_tuple__25);
   __Pyx_GIVEREF(__pyx_tuple__25);
   __pyx_tuple__26 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
 
   /* "fastHDMI/cython_fun.pyx":12
- * @cython.boundscheck(False)
+ * # @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def joint_to_mi_cython(floating_float_double[:, ::1] joint, floating_float_double forward_euler_a=1., floating_float_double forward_euler_b=1.):             # <<<<<<<<<<<<<<
  *     cdef int i, j
  *     cdef int joint_shape0 = joint.shape[0]
  */
   __pyx_tuple__27 = PyTuple_Pack(15, __pyx_n_s_joint, __pyx_n_s_forward_euler_a, __pyx_n_s_forward_euler_b, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_joint_shape0, __pyx_n_s_joint_shape1, __pyx_n_s_log_a_marginal, __pyx_n_s_log_b_marginal, __pyx_n_s_temp_sum, __pyx_n_s_log_temp_sum, __pyx_n_s_log_forward_euler_a, __pyx_n_s_log_forward_euler_b, __pyx_n_s_log_joint, __pyx_n_s_output); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
@@ -18547,15 +18665,15 @@
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "fastHDMI/cython_fun.pyx":12
- * @cython.boundscheck(False)
+ * # @cython.boundscheck(False)
  * @cython.wraparound(False)
  * def joint_to_mi_cython(floating_float_double[:, ::1] joint, floating_float_double forward_euler_a=1., floating_float_double forward_euler_b=1.):             # <<<<<<<<<<<<<<
  *     cdef int i, j
  *     cdef int joint_shape0 = joint.shape[0]
  */
   __pyx_t_1 = PyFloat_FromDouble(1.); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
@@ -18982,14 +19100,101 @@
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
+/* GetItemInt */
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
+    PyObject *r;
+    if (!j) return NULL;
+    r = PyObject_GetItem(o, j);
+    Py_DECREF(j);
+    return r;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyList_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
+        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyTuple_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
+        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
+                                                     CYTHON_NCP_UNUSED int wraparound,
+                                                     CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
+    if (is_list || PyList_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
+        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
+            PyObject *r = PyList_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    }
+    else if (PyTuple_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
+        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
+            PyObject *r = PyTuple_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    } else {
+        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
+        if (likely(m && m->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
+                Py_ssize_t l = m->sq_length(o);
+                if (likely(l >= 0)) {
+                    i += l;
+                } else {
+                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                        return NULL;
+                    PyErr_Clear();
+                }
+            }
+            return m->sq_item(o, i);
+        }
+    }
+#else
+    if (is_list || PySequence_Check(o)) {
+        return PySequence_GetItem(o, i);
+    }
+#endif
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+}
+
 /* DictGetItem */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
     PyObject *value;
     value = PyDict_GetItemWithError(d, key);
     if (unlikely(!value)) {
         if (!PyErr_Occurred()) {
@@ -19922,99 +20127,18 @@
     result = __Pyx_PyObject_Call(function, args, NULL);
     Py_DECREF(args);
     Py_DECREF(function);
 done:
     return result;
 }
 
-/* GetItemInt */
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
-    PyObject *r;
-    if (!j) return NULL;
-    r = PyObject_GetItem(o, j);
-    Py_DECREF(j);
-    return r;
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyList_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
-        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyTuple_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
-        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
-                                                     CYTHON_NCP_UNUSED int wraparound,
-                                                     CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
-    if (is_list || PyList_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
-        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
-            PyObject *r = PyList_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    }
-    else if (PyTuple_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
-        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
-            PyObject *r = PyTuple_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
-                if (likely(l >= 0)) {
-                    i += l;
-                } else {
-                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                        return NULL;
-                    PyErr_Clear();
-                }
-            }
-            return m->sq_item(o, i);
-        }
-    }
-#else
-    if (is_list || PySequence_Check(o)) {
-        return PySequence_GetItem(o, i);
-    }
-#endif
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+/* BufferIndexError */
+static void __Pyx_RaiseBufferIndexError(int axis) {
+  PyErr_Format(PyExc_IndexError,
+     "Out of bounds on buffer access (axis %d)", axis);
 }
 
 /* MemviewSliceInit */
 static int
 __Pyx_init_memviewslice(struct __pyx_memoryview_obj *memview,
                         int ndim,
                         __Pyx_memviewslice *memviewslice,
```

### Comparing `fastHDMI-1.23.1/src/fastHDMI/cython_fun.pyx` & `fastHDMI-1.23.2/src/fastHDMI/cython_fun.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 cimport cython
 from cython cimport floating
 
 ctypedef fused floating_float_double:
     float
     double
 
-@cython.boundscheck(False)
+# @cython.boundscheck(False)
 @cython.wraparound(False)
 def joint_to_mi_cython(floating_float_double[:, ::1] joint, floating_float_double forward_euler_a=1., floating_float_double forward_euler_b=1.):
     cdef int i, j
     cdef int joint_shape0 = joint.shape[0]
     cdef int joint_shape1 = joint.shape[1]
     cdef floating_float_double *log_a_marginal = <floating_float_double*>calloc(joint_shape0, sizeof(floating_float_double))
     cdef floating_float_double *log_b_marginal = <floating_float_double*>calloc(joint_shape1, sizeof(floating_float_double))
```

### Comparing `fastHDMI-1.23.1/src/fastHDMI.egg-info/PKG-INFO` & `fastHDMI-1.23.2/src/fastHDMI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastHDMI
-Version: 1.23.1
+Version: 1.23.2
 Summary: Use FFT-based mutual information and accelerated gradient method to screen variables and optimize nonconvex sparse learning problems on large CSV files or large genetic bed/bim/fam files. Multiprocessing is now available.
 Author-email: Kai Yang <kai.yang2@mail.mcgill.ca>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `fastHDMI-1.23.1/tests/test.py` & `fastHDMI-1.23.2/tests/test.py`

 * *Files identical despite different names*


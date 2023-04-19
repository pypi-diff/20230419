# Comparing `tmp/shooju-ts-0.1.8.tar.gz` & `tmp/shooju-ts-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shooju-ts-0.1.8.tar", last modified: Tue Nov 21 12:26:02 2017, max compression
+gzip compressed data, was "dist/shooju-ts-0.1.9.tar", last modified: Fri Nov 24 10:50:32 2017, max compression
```

## Comparing `shooju-ts-0.1.8.tar` & `shooju-ts-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2017-11-21 12:26:02.000000 shooju-ts-0.1.8/
--rwxrwxrwx   0 root         (0) root         (0)      218 2017-09-01 08:49:17.000000 shooju-ts-0.1.8/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     1844 2017-11-21 12:26:02.000000 shooju-ts-0.1.8/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2017-11-21 12:26:02.000000 shooju-ts-0.1.8/python/
--rwxrwxrwx   0 root         (0) root         (0)    11640 2017-11-21 12:22:59.000000 shooju-ts-0.1.8/python/JSONtoObj.c
--rwxrwxrwx   0 root         (0) root         (0)    35382 2017-11-21 12:22:59.000000 shooju-ts-0.1.8/python/objToJSON.c
--rwxrwxrwx   0 root         (0) root         (0)     2418 2017-09-01 08:49:17.000000 shooju-ts-0.1.8/python/py_defines.h
--rwxrwxrwx   0 root         (0) root         (0)      379 2017-09-01 08:49:17.000000 shooju-ts-0.1.8/python/py_sjts.h
--rwxrwxrwx   0 root         (0) root         (0)     5288 2017-09-01 08:49:17.000000 shooju-ts-0.1.8/python/ujson.c
--rwxrwxrwx   0 root         (0) root         (0)     2039 2017-11-21 12:22:44.000000 shooju-ts-0.1.8/python/version.h
--rwxrwxrwx   0 root         (0) root         (0)     1215 2017-09-01 08:49:17.000000 shooju-ts-0.1.8/README.rst
--rwxrwxrwx   0 root         (0) root         (0)       38 2017-11-21 12:26:02.000000 shooju-ts-0.1.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3443 2017-09-01 08:49:17.000000 shooju-ts-0.1.8/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2017-11-21 12:26:02.000000 shooju-ts-0.1.8/shooju_ts.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)        1 2017-11-21 12:26:02.000000 shooju-ts-0.1.8/shooju_ts.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        2 2017-09-01 09:08:29.000000 shooju-ts-0.1.8/shooju_ts.egg-info/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)     1844 2017-11-21 12:26:02.000000 shooju-ts-0.1.8/shooju_ts.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      571 2017-11-21 12:26:02.000000 shooju-ts-0.1.8/shooju_ts.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2017-11-21 12:26:02.000000 shooju-ts-0.1.8/shooju_ts.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2017-11-21 12:26:02.000000 shooju-ts-0.1.8/sjts/
--rwxrwxrwx   0 root         (0) root         (0)     1529 2017-06-20 07:22:46.000000 shooju-ts-0.1.8/sjts/sjts.h
--rwxrwxrwx   0 root         (0) root         (0)     2199 2017-06-20 07:22:46.000000 shooju-ts-0.1.8/sjts/sjtsdec.c
--rwxrwxrwx   0 root         (0) root         (0)     2791 2017-06-20 07:22:46.000000 shooju-ts-0.1.8/sjts/sjtsenc.c
--rwxrwxrwx   0 root         (0) root         (0)     9893 2017-02-20 13:22:28.000000 shooju-ts-0.1.8/sjts/ultrajson.h
--rwxrwxrwx   0 root         (0) root         (0)    22199 2017-02-20 13:22:28.000000 shooju-ts-0.1.8/sjts/ultrajsondec.c
--rwxrwxrwx   0 root         (0) root         (0)    24937 2017-02-20 13:22:28.000000 shooju-ts-0.1.8/sjts/ultrajsonenc.c
-drwxrwxrwx   0 root         (0) root         (0)        0 2017-11-21 12:26:02.000000 shooju-ts-0.1.8/tests/
--rwxrwxrwx   0 root         (0) root         (0)   687491 2017-09-01 08:49:17.000000 shooju-ts-0.1.8/tests/sample.json
--rwxrwxrwx   0 root         (0) root         (0)     9017 2017-11-21 12:22:44.000000 shooju-ts-0.1.8/tests/tests.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2017-11-24 10:50:32.000000 shooju-ts-0.1.9/
+-rwxrwxrwx   0 root         (0) root         (0)      218 2017-09-01 08:49:17.000000 shooju-ts-0.1.9/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     1844 2017-11-24 10:50:32.000000 shooju-ts-0.1.9/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2017-11-24 10:50:32.000000 shooju-ts-0.1.9/python/
+-rwxrwxrwx   0 root         (0) root         (0)    11640 2017-11-21 12:22:59.000000 shooju-ts-0.1.9/python/JSONtoObj.c
+-rwxrwxrwx   0 root         (0) root         (0)    35844 2017-11-24 10:09:32.000000 shooju-ts-0.1.9/python/objToJSON.c
+-rwxrwxrwx   0 root         (0) root         (0)     2418 2017-09-01 08:49:17.000000 shooju-ts-0.1.9/python/py_defines.h
+-rwxrwxrwx   0 root         (0) root         (0)      379 2017-09-01 08:49:17.000000 shooju-ts-0.1.9/python/py_sjts.h
+-rwxrwxrwx   0 root         (0) root         (0)     5288 2017-09-01 08:49:17.000000 shooju-ts-0.1.9/python/ujson.c
+-rwxrwxrwx   0 root         (0) root         (0)     2039 2017-11-24 10:19:41.000000 shooju-ts-0.1.9/python/version.h
+-rwxrwxrwx   0 root         (0) root         (0)     1215 2017-09-01 08:49:17.000000 shooju-ts-0.1.9/README.rst
+-rwxrwxrwx   0 root         (0) root         (0)       38 2017-11-24 10:50:32.000000 shooju-ts-0.1.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3443 2017-09-01 08:49:17.000000 shooju-ts-0.1.9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2017-11-24 10:50:32.000000 shooju-ts-0.1.9/shooju_ts.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)        1 2017-11-24 10:50:32.000000 shooju-ts-0.1.9/shooju_ts.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        2 2017-09-01 09:08:29.000000 shooju-ts-0.1.9/shooju_ts.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)     1844 2017-11-24 10:50:32.000000 shooju-ts-0.1.9/shooju_ts.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      571 2017-11-24 10:50:32.000000 shooju-ts-0.1.9/shooju_ts.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2017-11-24 10:50:32.000000 shooju-ts-0.1.9/shooju_ts.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2017-11-24 10:50:32.000000 shooju-ts-0.1.9/sjts/
+-rwxrwxrwx   0 root         (0) root         (0)     1529 2017-06-20 07:22:46.000000 shooju-ts-0.1.9/sjts/sjts.h
+-rwxrwxrwx   0 root         (0) root         (0)     2199 2017-06-20 07:22:46.000000 shooju-ts-0.1.9/sjts/sjtsdec.c
+-rwxrwxrwx   0 root         (0) root         (0)     2791 2017-06-20 07:22:46.000000 shooju-ts-0.1.9/sjts/sjtsenc.c
+-rwxrwxrwx   0 root         (0) root         (0)     9893 2017-02-20 13:22:28.000000 shooju-ts-0.1.9/sjts/ultrajson.h
+-rwxrwxrwx   0 root         (0) root         (0)    22199 2017-02-20 13:22:28.000000 shooju-ts-0.1.9/sjts/ultrajsondec.c
+-rwxrwxrwx   0 root         (0) root         (0)    24937 2017-02-20 13:22:28.000000 shooju-ts-0.1.9/sjts/ultrajsonenc.c
+drwxrwxrwx   0 root         (0) root         (0)        0 2017-11-24 10:50:32.000000 shooju-ts-0.1.9/tests/
+-rwxrwxrwx   0 root         (0) root         (0)   687491 2017-09-01 08:49:17.000000 shooju-ts-0.1.9/tests/sample.json
+-rwxrwxrwx   0 root         (0) root         (0)     9017 2017-11-21 12:22:44.000000 shooju-ts-0.1.9/tests/tests.py
```

### Comparing `shooju-ts-0.1.8/PKG-INFO` & `shooju-ts-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: shooju-ts
-Version: 0.1.8
+Version: 0.1.9
 Summary: Shooju Time Series (SJTS) Serializer
 Home-page: http://shooju.com
 Author: Shooju, LLC
 Author-email: support@shooju.com
 License: TBD
 Description-Content-Type: UNKNOWN
 Description: Shooju
```

### Comparing `shooju-ts-0.1.8/python/JSONtoObj.c` & `shooju-ts-0.1.9/python/JSONtoObj.c`

 * *Files identical despite different names*

### Comparing `shooju-ts-0.1.8/python/objToJSON.c` & `shooju-ts-0.1.9/python/objToJSON.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,19 @@
 /*
+ * m bs4 import BeautifulSoup
+ * import json
+ * import ujson
+ * body = BeautifulSoup('<div><b>hello</b></div>')
+ * val = body.find_all('b')[0].string
+ * print('value: {} type: {}'.format(val, type(val)))
+ * print(sjts.dumps({
+ *     'series': [{'series_id': 'test', 'fields': {'test_field': val}}]
+ *     }))
+ *     print(ujson.dumps({'test_field': val}))
+ *     print(json.dumps({'test_field': val}))
 Developed by ESN, an Electronic Arts Inc. studio. 
 Copyright (c) 2014, Electronic Arts Inc.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 * Redistributions of source code must retain the above copyright
@@ -685,15 +696,15 @@
   pc->size = 0;
   pc->un.longValue = 0;
   pc->un.rawJSONValue = NULL;
 
   pc->sjCtx = (SJContext*)enc->prv;
   pc->level = enc->level;
 
-  if (PyIter_Check(obj))
+  if (PyIter_Check(obj) && !PyUnicode_Check(obj) && !PyString_Check(obj))
   {
     PRINTMARK();
     goto ISITERABLE;
   }
 
   if (PyBool_Check(obj))
   {
```

### Comparing `shooju-ts-0.1.8/python/py_defines.h` & `shooju-ts-0.1.9/python/py_defines.h`

 * *Files identical despite different names*

### Comparing `shooju-ts-0.1.8/python/ujson.c` & `shooju-ts-0.1.9/python/ujson.c`

 * *Files identical despite different names*

### Comparing `shooju-ts-0.1.8/python/version.h` & `shooju-ts-0.1.9/python/version.h`

 * *Files 1% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 
 Numeric decoder derived from from TCL library
 http://www.opensource.apple.com/source/tcl/tcl-14/tcl/license.terms
  * Copyright (c) 1988-1993 The Regents of the University of California.
  * Copyright (c) 1994 Sun Microsystems, Inc.
 */
 
-#define UJSON_VERSION "0.1.8"
+#define UJSON_VERSION "0.1.9"
```

### Comparing `shooju-ts-0.1.8/README.rst` & `shooju-ts-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `shooju-ts-0.1.8/setup.py` & `shooju-ts-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `shooju-ts-0.1.8/shooju_ts.egg-info/PKG-INFO` & `shooju-ts-0.1.9/shooju_ts.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: shooju-ts
-Version: 0.1.8
+Version: 0.1.9
 Summary: Shooju Time Series (SJTS) Serializer
 Home-page: http://shooju.com
 Author: Shooju, LLC
 Author-email: support@shooju.com
 License: TBD
 Description-Content-Type: UNKNOWN
 Description: Shooju
```

### Comparing `shooju-ts-0.1.8/shooju_ts.egg-info/SOURCES.txt` & `shooju-ts-0.1.9/shooju_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shooju-ts-0.1.8/sjts/sjts.h` & `shooju-ts-0.1.9/sjts/sjts.h`

 * *Files identical despite different names*

### Comparing `shooju-ts-0.1.8/sjts/sjtsdec.c` & `shooju-ts-0.1.9/sjts/sjtsdec.c`

 * *Files identical despite different names*

### Comparing `shooju-ts-0.1.8/sjts/sjtsenc.c` & `shooju-ts-0.1.9/sjts/sjtsenc.c`

 * *Files identical despite different names*

### Comparing `shooju-ts-0.1.8/sjts/ultrajson.h` & `shooju-ts-0.1.9/sjts/ultrajson.h`

 * *Files identical despite different names*

### Comparing `shooju-ts-0.1.8/sjts/ultrajsondec.c` & `shooju-ts-0.1.9/sjts/ultrajsondec.c`

 * *Files identical despite different names*

### Comparing `shooju-ts-0.1.8/sjts/ultrajsonenc.c` & `shooju-ts-0.1.9/sjts/ultrajsonenc.c`

 * *Files identical despite different names*

### Comparing `shooju-ts-0.1.8/tests/sample.json` & `shooju-ts-0.1.9/tests/sample.json`

 * *Files identical despite different names*

### Comparing `shooju-ts-0.1.8/tests/tests.py` & `shooju-ts-0.1.9/tests/tests.py`

 * *Files identical despite different names*


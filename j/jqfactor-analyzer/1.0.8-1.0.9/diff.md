# Comparing `tmp/jqfactor_analyzer-1.0.8.tar.gz` & `tmp/jqfactor_analyzer-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jqfactor_analyzer-1.0.8.tar", last modified: Mon Feb 13 03:32:42 2023, max compression
+gzip compressed data, was "jqfactor_analyzer-1.0.9.tar", last modified: Mon Feb 13 04:08:29 2023, max compression
```

## Comparing `jqfactor_analyzer-1.0.8.tar` & `jqfactor_analyzer-1.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-02-13 03:32:42.314986 jqfactor_analyzer-1.0.8/
--rw-rw-rw-   0        0        0     1066 2019-10-09 02:35:28.000000 jqfactor_analyzer-1.0.8/LICENSE
--rw-rw-rw-   0        0        0       74 2019-11-25 04:59:25.000000 jqfactor_analyzer-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     6931 2023-02-13 03:32:42.315850 jqfactor_analyzer-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5956 2023-02-13 03:29:57.000000 jqfactor_analyzer-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-13 03:32:42.214084 jqfactor_analyzer-1.0.8/jqfactor_analyzer/
--rw-rw-rw-   0        0        0     1664 2023-02-13 03:27:45.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer/__init__.py
--rw-rw-rw-   0        0        0    64837 2023-02-13 03:29:57.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer/analyze.py
--rw-rw-rw-   0        0        0     1613 2020-04-09 05:46:20.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer/compat.py
--rw-rw-rw-   0        0        0    11210 2023-02-13 03:27:45.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer/data.py
--rw-rw-rw-   0        0        0     1198 2020-04-09 05:46:22.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer/exceptions.py
--rw-rw-rw-   0        0        0    17872 2023-02-13 03:27:45.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer/performance.py
--rw-rw-rw-   0        0        0     8401 2023-02-13 03:27:45.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer/plot_utils.py
--rw-rw-rw-   0        0        0    22809 2023-02-13 03:27:45.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer/plotting.py
--rw-rw-rw-   0        0        0    18659 2023-02-13 03:27:45.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer/prepare.py
--rw-rw-rw-   0        0        0      412 2020-04-09 05:46:22.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer/sample.py
-drwxrwxrwx   0        0        0        0 2023-02-13 03:32:42.310594 jqfactor_analyzer-1.0.8/jqfactor_analyzer/sample_data/
--rw-rw-rw-   0        0        0   564822 2020-04-09 05:46:22.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer/sample_data/VOL5.csv
--rw-rw-rw-   0        0        0     1113 2023-02-13 03:27:45.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer/utils.py
--rw-rw-rw-   0        0        0       48 2023-02-13 03:29:57.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer/version.py
--rw-rw-rw-   0        0        0      314 2023-02-13 03:27:45.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer/when.py
-drwxrwxrwx   0        0        0        0 2023-02-13 03:32:42.276176 jqfactor_analyzer-1.0.8/jqfactor_analyzer.egg-info/
--rw-rw-rw-   0        0        0     6931 2023-02-13 03:32:41.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      727 2023-02-13 03:32:41.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-13 03:32:41.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-03-21 04:09:24.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      137 2023-02-13 03:32:41.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-02-13 03:32:41.000000 jqfactor_analyzer-1.0.8/jqfactor_analyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      137 2019-03-01 03:09:03.000000 jqfactor_analyzer-1.0.8/requirements.txt
--rw-rw-rw-   0        0        0       74 2023-02-13 03:32:42.319962 jqfactor_analyzer-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2299 2022-03-11 03:07:30.000000 jqfactor_analyzer-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-13 04:08:29.451591 jqfactor_analyzer-1.0.9/
+-rw-rw-rw-   0        0        0     1066 2019-10-09 02:35:28.000000 jqfactor_analyzer-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0       74 2019-11-25 04:59:25.000000 jqfactor_analyzer-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6931 2023-02-13 04:08:29.453493 jqfactor_analyzer-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5956 2023-02-13 03:29:57.000000 jqfactor_analyzer-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-13 04:08:29.385144 jqfactor_analyzer-1.0.9/jqfactor_analyzer/
+-rw-rw-rw-   0        0        0     1664 2023-02-13 03:46:17.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer/__init__.py
+-rw-rw-rw-   0        0        0    64907 2023-02-13 03:48:02.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer/analyze.py
+-rw-rw-rw-   0        0        0     1613 2020-04-09 05:46:20.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer/compat.py
+-rw-rw-rw-   0        0        0    11210 2023-02-13 03:46:17.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer/data.py
+-rw-rw-rw-   0        0        0     1198 2020-04-09 05:46:22.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer/exceptions.py
+-rw-rw-rw-   0        0        0    17872 2023-02-13 03:46:17.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer/performance.py
+-rw-rw-rw-   0        0        0     8401 2023-02-13 03:46:17.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer/plot_utils.py
+-rw-rw-rw-   0        0        0    22809 2023-02-13 03:46:17.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer/plotting.py
+-rw-rw-rw-   0        0        0    18659 2023-02-13 03:46:17.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer/prepare.py
+-rw-rw-rw-   0        0        0      412 2020-04-09 05:46:22.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer/sample.py
+drwxrwxrwx   0        0        0        0 2023-02-13 04:08:29.443023 jqfactor_analyzer-1.0.9/jqfactor_analyzer/sample_data/
+-rw-rw-rw-   0        0        0   564822 2020-04-09 05:46:22.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer/sample_data/VOL5.csv
+-rw-rw-rw-   0        0        0     1183 2023-02-13 03:48:22.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer/utils.py
+-rw-rw-rw-   0        0        0       48 2023-02-13 03:53:26.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer/version.py
+-rw-rw-rw-   0        0        0      314 2023-02-13 03:46:17.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer/when.py
+drwxrwxrwx   0        0        0        0 2023-02-13 04:08:29.436957 jqfactor_analyzer-1.0.9/jqfactor_analyzer.egg-info/
+-rw-rw-rw-   0        0        0     6931 2023-02-13 04:08:28.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2023-02-13 04:08:29.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-13 04:08:28.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-03-21 04:09:24.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      137 2023-02-13 04:08:28.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-02-13 04:08:28.000000 jqfactor_analyzer-1.0.9/jqfactor_analyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      137 2019-03-01 03:09:03.000000 jqfactor_analyzer-1.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       74 2023-02-13 04:08:29.475108 jqfactor_analyzer-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2299 2022-03-11 03:07:30.000000 jqfactor_analyzer-1.0.9/setup.py
```

### Comparing `jqfactor_analyzer-1.0.8/LICENSE` & `jqfactor_analyzer-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jqfactor_analyzer-1.0.8/PKG-INFO` & `jqfactor_analyzer-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jqfactor_analyzer
-Version: 1.0.8
+Version: 1.0.9
 Summary: JoinQuant single factor analyzer
 Home-page: https://www.joinquant.com
 Author: JoinQuant
 Author-email: xlx@joinquant.com
 Maintainer: 
 Maintainer-email: 
 License: Apache License v2
```

### Comparing `jqfactor_analyzer-1.0.8/README.md` & `jqfactor_analyzer-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `jqfactor_analyzer-1.0.8/jqfactor_analyzer/__init__.py` & `jqfactor_analyzer-1.0.9/jqfactor_analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `jqfactor_analyzer-1.0.8/jqfactor_analyzer/analyze.py` & `jqfactor_analyzer-1.0.9/jqfactor_analyzer/analyze.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from __future__ import division, print_function
 
-from collections import Iterable
+try:
+    from collections import Iterable
+except ImportError:
+    from collections.abc import Iterable
 
 import numpy as np
 import pandas as pd
 from fastcache import lru_cache
 from cached_property import cached_property
 from scipy.stats import spearmanr, pearsonr
 from scipy import stats
```

### Comparing `jqfactor_analyzer-1.0.8/jqfactor_analyzer/compat.py` & `jqfactor_analyzer-1.0.9/jqfactor_analyzer/compat.py`

 * *Files identical despite different names*

### Comparing `jqfactor_analyzer-1.0.8/jqfactor_analyzer/data.py` & `jqfactor_analyzer-1.0.9/jqfactor_analyzer/data.py`

 * *Files identical despite different names*

### Comparing `jqfactor_analyzer-1.0.8/jqfactor_analyzer/exceptions.py` & `jqfactor_analyzer-1.0.9/jqfactor_analyzer/exceptions.py`

 * *Files identical despite different names*

### Comparing `jqfactor_analyzer-1.0.8/jqfactor_analyzer/performance.py` & `jqfactor_analyzer-1.0.9/jqfactor_analyzer/performance.py`

 * *Files identical despite different names*

### Comparing `jqfactor_analyzer-1.0.8/jqfactor_analyzer/plot_utils.py` & `jqfactor_analyzer-1.0.9/jqfactor_analyzer/plot_utils.py`

 * *Files identical despite different names*

### Comparing `jqfactor_analyzer-1.0.8/jqfactor_analyzer/plotting.py` & `jqfactor_analyzer-1.0.9/jqfactor_analyzer/plotting.py`

 * *Files identical despite different names*

### Comparing `jqfactor_analyzer-1.0.8/jqfactor_analyzer/prepare.py` & `jqfactor_analyzer-1.0.9/jqfactor_analyzer/prepare.py`

 * *Files identical despite different names*

### Comparing `jqfactor_analyzer-1.0.8/jqfactor_analyzer/sample_data/VOL5.csv` & `jqfactor_analyzer-1.0.9/jqfactor_analyzer/sample_data/VOL5.csv`

 * *Files identical despite different names*

### Comparing `jqfactor_analyzer-1.0.8/jqfactor_analyzer/utils.py` & `jqfactor_analyzer-1.0.9/jqfactor_analyzer/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # -*- coding: utf-8 -*-
 
 
 import re
 import six
 import warnings
 from functools import wraps
-from collections import Iterable
+try:
+    from collections import Iterable
+except ImportError:
+    from collections.abc import Iterable
 
 import pandas as pd
 
 
 def get_forward_returns_columns(columns):
     syntax = re.compile("^period_\\d+$")
     return columns[columns.astype('str').str.contains(syntax, regex=True)]
```

### Comparing `jqfactor_analyzer-1.0.8/jqfactor_analyzer.egg-info/PKG-INFO` & `jqfactor_analyzer-1.0.9/jqfactor_analyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jqfactor-analyzer
-Version: 1.0.8
+Version: 1.0.9
 Summary: JoinQuant single factor analyzer
 Home-page: https://www.joinquant.com
 Author: JoinQuant
 Author-email: xlx@joinquant.com
 Maintainer: 
 Maintainer-email: 
 License: Apache License v2
```

### Comparing `jqfactor_analyzer-1.0.8/jqfactor_analyzer.egg-info/SOURCES.txt` & `jqfactor_analyzer-1.0.9/jqfactor_analyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jqfactor_analyzer-1.0.8/setup.py` & `jqfactor_analyzer-1.0.9/setup.py`

 * *Files identical despite different names*


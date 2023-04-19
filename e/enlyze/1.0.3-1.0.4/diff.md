# Comparing `tmp/enlyze-1.0.3.tar.gz` & `tmp/enlyze-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enlyze-1.0.3.tar", last modified: Fri Mar 31 07:39:14 2023, max compression
+gzip compressed data, was "enlyze-1.0.4.tar", last modified: Wed Apr 19 12:41:21 2023, max compression
```

## Comparing `enlyze-1.0.3.tar` & `enlyze-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:39:14.638861 enlyze-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-31 07:37:40.000000 enlyze-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-31 07:39:14.638861 enlyze-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-31 07:37:40.000000 enlyze-1.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-31 07:37:40.000000 enlyze-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-31 07:39:14.638861 enlyze-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:39:14.638861 enlyze-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:39:14.638861 enlyze-1.0.3/src/enlyze/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-31 07:37:40.000000 enlyze-1.0.3/src/enlyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-31 07:37:51.000000 enlyze-1.0.3/src/enlyze/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-31 07:37:40.000000 enlyze-1.0.3/src/enlyze/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-03-31 07:37:40.000000 enlyze-1.0.3/src/enlyze/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-31 07:37:40.000000 enlyze-1.0.3/src/enlyze/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-31 07:37:40.000000 enlyze-1.0.3/src/enlyze/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-03-31 07:37:40.000000 enlyze-1.0.3/src/enlyze/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 07:37:40.000000 enlyze-1.0.3/src/enlyze/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:39:14.638861 enlyze-1.0.3/src/enlyze/timeseries_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 07:37:40.000000 enlyze-1.0.3/src/enlyze/timeseries_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-03-31 07:37:40.000000 enlyze-1.0.3/src/enlyze/timeseries_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-03-31 07:37:40.000000 enlyze-1.0.3/src/enlyze/timeseries_api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 07:39:14.638861 enlyze-1.0.3/src/enlyze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-31 07:39:14.000000 enlyze-1.0.3/src/enlyze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-31 07:39:14.000000 enlyze-1.0.3/src/enlyze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 07:39:14.000000 enlyze-1.0.3/src/enlyze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-31 07:39:14.000000 enlyze-1.0.3/src/enlyze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 07:39:14.000000 enlyze-1.0.3/src/enlyze.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:41:21.777475 enlyze-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-19 12:38:56.000000 enlyze-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-19 12:41:21.777475 enlyze-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-19 12:38:56.000000 enlyze-1.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-19 12:38:56.000000 enlyze-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-19 12:41:21.777475 enlyze-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:41:21.761475 enlyze-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:41:21.769475 enlyze-1.0.4/src/enlyze/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-19 12:38:56.000000 enlyze-1.0.4/src/enlyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 12:39:12.000000 enlyze-1.0.4/src/enlyze/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-19 12:38:56.000000 enlyze-1.0.4/src/enlyze/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-04-19 12:38:56.000000 enlyze-1.0.4/src/enlyze/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-19 12:38:56.000000 enlyze-1.0.4/src/enlyze/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-19 12:38:56.000000 enlyze-1.0.4/src/enlyze/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-04-19 12:38:56.000000 enlyze-1.0.4/src/enlyze/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 12:38:56.000000 enlyze-1.0.4/src/enlyze/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:41:21.777475 enlyze-1.0.4/src/enlyze/timeseries_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 12:38:56.000000 enlyze-1.0.4/src/enlyze/timeseries_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-04-19 12:38:56.000000 enlyze-1.0.4/src/enlyze/timeseries_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-19 12:38:56.000000 enlyze-1.0.4/src/enlyze/timeseries_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-19 12:38:56.000000 enlyze-1.0.4/src/enlyze/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:41:21.773475 enlyze-1.0.4/src/enlyze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-19 12:41:21.000000 enlyze-1.0.4/src/enlyze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-19 12:41:21.000000 enlyze-1.0.4/src/enlyze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:41:21.000000 enlyze-1.0.4/src/enlyze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-19 12:41:21.000000 enlyze-1.0.4/src/enlyze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 12:41:21.000000 enlyze-1.0.4/src/enlyze.egg-info/top_level.txt
```

### Comparing `enlyze-1.0.3/LICENSE` & `enlyze-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `enlyze-1.0.3/PKG-INFO` & `enlyze-1.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enlyze
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python SDK for interacting with the ENLYZE platform https://www.enlyze.com
 Author-email: ENLYZE GmbH <hello@enlyze.com>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: lint
@@ -54,7 +54,26 @@
 
 Running `mypy`
 ~~~~~~~~~~~~~~
 
 .. code-block:: console
 
     $ tox -e mypy
+
+Generating the documentation
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: console
+
+    $ tox -e docs
+
+Note that this requires the `Enchant C library
+<https://pyenchant.github.io/pyenchant/install.html>` to be installed.
+
+*Note for M1 users, the* ``Enchant`` *library doesn't work out of the box and the
+workaround in the official docs is brittle, I suggest installing the library from*
+``homebrew`` *and setting the environment variable* ``PYENCHANT_LIBRARY_PATH`` *like
+so:*
+
+.. code-block:: console
+
+    $ export PYENCHANT_LIBRARY_PATH=/opt/homebrew/lib/libenchant-2.dylib
```

### Comparing `enlyze-1.0.3/pyproject.toml` & `enlyze-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 authors = [{name = "ENLYZE GmbH", email = "hello@enlyze.com"},]
 requires-python = ">=3.10"
 dynamic = [
   'version',
 ]
 dependencies = [
   "httpx",
-  "pandas",
+  "pandas>=2",
   "pydantic",
 ]
 [project.optional-dependencies]
 docs = [
   "sphinx",
   "sphinx-rtd-theme",
   "sphinx-tabs",
```

### Comparing `enlyze-1.0.3/src/enlyze/auth.py` & `enlyze-1.0.4/src/enlyze/auth.py`

 * *Files identical despite different names*

### Comparing `enlyze-1.0.3/src/enlyze/models.py` & `enlyze-1.0.4/src/enlyze/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from datetime import date, datetime, timezone
 from enum import Enum
 from itertools import chain
-from typing import Any, Iterator, Optional
+from typing import Any, Iterator, Optional, Sequence
 from uuid import UUID
 
 import pandas
 
 
 @dataclass(frozen=True)
 class Site:
@@ -62,14 +62,27 @@
     STRING = "STRING"
     ARRAY_INTEGER = "ARRAY_INTEGER"
     ARRAY_FLOAT = "ARRAY_FLOAT"
     ARRAY_BOOLEAN = "ARRAY_BOOLEAN"
     ARRAY_STRING = "ARRAY_STRING"
 
 
+class ResamplingMethod(str, Enum):
+    """Resampling method to be used when resampling timeseries data."""
+
+    FIRST = "first"
+    LAST = "last"
+    MAX = "max"
+    MIN = "min"
+    COUNT = "count"
+    SUM = "sum"
+    AVG = "avg"
+    MEDIAN = "median"
+
+
 @dataclass(frozen=True)
 class Variable:
     """Representation of a :ref:`variable <variable>` in the ENLYZE platform.
 
     Contains details about the variable, but no timeseries data.
 
     """
@@ -97,15 +110,15 @@
     #: Beginning of the requested time frame.
     start: datetime
 
     #: End of the requested time frame.
     end: datetime
 
     #: The variables for which timeseries data has been requested.
-    variables: list[Variable]
+    variables: Sequence[Variable]
 
     _columns: list[str]
     _records: list[Any]
 
     def __len__(self) -> int:
         """Returns the number of resulting rows"""
         return len(self._records)
@@ -178,9 +191,9 @@
             variable_columns = self._display_names_as_column_names(variable_columns)
 
         df = pandas.DataFrame.from_records(
             self._records,
             columns=[time_column] + variable_columns,
             index="time",
         )
-        df.index = pandas.to_datetime(df.index, utc=True)
+        df.index = pandas.to_datetime(df.index, utc=True, format="ISO8601")
         return df
```

### Comparing `enlyze-1.0.3/src/enlyze/timeseries_api/client.py` & `enlyze-1.0.4/src/enlyze/timeseries_api/client.py`

 * *Files identical despite different names*

### Comparing `enlyze-1.0.3/src/enlyze/timeseries_api/models.py` & `enlyze-1.0.4/src/enlyze/timeseries_api/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import date, datetime
-from typing import Any, Optional
+from typing import Any, Optional, Sequence
 from uuid import UUID
 
 from pydantic import BaseModel
 
 import enlyze.models as user_models
 
 
@@ -73,15 +73,18 @@
     records: list[Any]
 
     def extend(self, other: "TimeseriesData") -> None:
         """Add records from ``other`` after the existing records."""
         self.records.extend(other.records)
 
     def to_user_model(
-        self, start: datetime, end: datetime, variables: list[user_models.Variable]
+        self,
+        start: datetime,
+        end: datetime,
+        variables: Sequence[user_models.Variable],
     ) -> user_models.TimeseriesData:
         return user_models.TimeseriesData(
             start=start,
             end=end,
             variables=variables,
             _columns=self.columns,
             _records=self.records,
```

### Comparing `enlyze-1.0.3/src/enlyze.egg-info/PKG-INFO` & `enlyze-1.0.4/src/enlyze.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enlyze
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python SDK for interacting with the ENLYZE platform https://www.enlyze.com
 Author-email: ENLYZE GmbH <hello@enlyze.com>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: lint
@@ -54,7 +54,26 @@
 
 Running `mypy`
 ~~~~~~~~~~~~~~
 
 .. code-block:: console
 
     $ tox -e mypy
+
+Generating the documentation
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: console
+
+    $ tox -e docs
+
+Note that this requires the `Enchant C library
+<https://pyenchant.github.io/pyenchant/install.html>` to be installed.
+
+*Note for M1 users, the* ``Enchant`` *library doesn't work out of the box and the
+workaround in the official docs is brittle, I suggest installing the library from*
+``homebrew`` *and setting the environment variable* ``PYENCHANT_LIBRARY_PATH`` *like
+so:*
+
+.. code-block:: console
+
+    $ export PYENCHANT_LIBRARY_PATH=/opt/homebrew/lib/libenchant-2.dylib
```


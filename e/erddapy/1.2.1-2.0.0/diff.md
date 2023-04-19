# Comparing `tmp/erddapy-1.2.1.tar.gz` & `tmp/erddapy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erddapy-1.2.1.tar", last modified: Wed Mar 16 13:46:22 2022, max compression
+gzip compressed data, was "erddapy-2.0.0.tar", last modified: Wed Apr 19 11:42:56 2023, max compression
```

## Comparing `erddapy-1.2.1.tar` & `erddapy-2.0.0.tar`

### file list

```diff
@@ -1,29 +1,26 @@
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-03-16 13:46:22.393390 erddapy-1.2.1/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      144 2022-03-14 18:23:01.000000 erddapy-1.2.1/.coveragerc
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-03-16 13:46:22.393390 erddapy-1.2.1/.github/
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-03-16 13:46:22.393390 erddapy-1.2.1/.github/workflows/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1696 2022-03-15 17:13:22.000000 erddapy-1.2.1/.github/workflows/deploy-docs.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1033 2022-03-16 13:44:40.000000 erddapy-1.2.1/.github/workflows/publish.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1047 2022-03-15 16:28:42.000000 erddapy-1.2.1/.github/workflows/tests.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     3118 2021-06-29 17:24:50.000000 erddapy-1.2.1/CHANGES.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1477 2021-06-29 17:24:50.000000 erddapy-1.2.1/LICENSE.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      254 2021-06-29 17:24:50.000000 erddapy-1.2.1/MANIFEST.in
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     5098 2022-03-16 13:46:22.393390 erddapy-1.2.1/PKG-INFO
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     4107 2021-07-08 22:49:02.000000 erddapy-1.2.1/README.md
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      817 2021-06-29 17:24:50.000000 erddapy-1.2.1/code-of-conduct.md
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-03-16 13:46:22.393390 erddapy-1.2.1/erddapy/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      237 2022-03-15 18:57:40.000000 erddapy-1.2.1/erddapy/__init__.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      194 2022-03-15 18:57:40.000000 erddapy-1.2.1/erddapy/doc_helpers.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     8023 2021-06-29 17:24:50.000000 erddapy-1.2.1/erddapy/erddaps.json
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    25209 2022-03-15 19:21:54.000000 erddapy-1.2.1/erddapy/erddapy.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     4732 2022-03-15 18:57:40.000000 erddapy-1.2.1/erddapy/multiple_server_search.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1129 2022-03-15 18:57:40.000000 erddapy-1.2.1/erddapy/netcdf_handling.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      950 2022-03-15 18:57:40.000000 erddapy-1.2.1/erddapy/servers.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     2007 2022-03-15 18:57:40.000000 erddapy-1.2.1/erddapy/url_handling.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2022-03-16 13:46:22.393390 erddapy-1.2.1/erddapy.egg-info/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      427 2022-03-16 13:46:22.000000 erddapy-1.2.1/erddapy.egg-info/SOURCES.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      375 2021-06-29 17:24:50.000000 erddapy-1.2.1/pyproject.toml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      368 2022-03-15 16:28:42.000000 erddapy-1.2.1/requirements-dev.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       29 2021-06-29 17:24:50.000000 erddapy-1.2.1/requirements.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1361 2022-03-16 13:46:22.393390 erddapy-1.2.1/setup.cfg
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      417 2022-03-15 18:57:40.000000 erddapy-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:42:56.054047 erddapy-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-19 11:42:42.000000 erddapy-2.0.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-19 11:42:42.000000 erddapy-2.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-19 11:42:42.000000 erddapy-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-19 11:42:56.054047 erddapy-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-19 11:42:42.000000 erddapy-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:42:56.050047 erddapy-2.0.0/erddapy/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:42:56.054047 erddapy-2.0.0/erddapy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/core/griddap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/core/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/core/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14312 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/core/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16215 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/erddapy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/multiple_server_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:42:56.054047 erddapy-2.0.0/erddapy/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/servers/erddaps.json
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-19 11:42:42.000000 erddapy-2.0.0/erddapy/servers/servers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:42:56.054047 erddapy-2.0.0/erddapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-19 11:42:56.000000 erddapy-2.0.0/erddapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-19 11:42:42.000000 erddapy-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-19 11:42:42.000000 erddapy-2.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-19 11:42:42.000000 erddapy-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 11:42:56.054047 erddapy-2.0.0/setup.cfg
```

### Comparing `erddapy-1.2.1/CHANGES.txt` & `erddapy-2.0.0/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `erddapy-1.2.1/LICENSE.txt` & `erddapy-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `erddapy-1.2.1/PKG-INFO` & `erddapy-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,45 @@
 Metadata-Version: 2.1
 Name: erddapy
-Version: 1.2.1
+Version: 2.0.0
 Summary: Python interface for ERDDAP
-Home-page: https://github.com/ioos/erddapy
-Author: Filipe Fernandes
-Author-email: ocefpaf@gmail.com
-License: BSD-3-Clause
-Project-URL: Documentation, https://ioos.github.io/erddapy
-Project-URL: Bug Tracker, https://github.com/ioos/erddapy/issues
-Project-URL: Source Code, https://github.com/ioos/erddapy
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
+Author-email: Filipe Fernandes <ocefpaf+erddapy@gmail.com>
+License: Copyright 2017 Filipe Fernandes
+        
+        
+        Redistribution and use in source and binary forms,
+        with or without modification,
+        are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice,
+           this list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its contributors
+           may be used to endorse or promote products derived from this software
+           without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
+        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+        ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+        LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+        (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+        LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
+        HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
+        STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY
+        WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: documentation, https://ioos.github.io/erddapy
+Project-URL: homepage, https://github.com/ioos/erddapy
+Project-URL: repository, https://github.com/ioos/erddapy
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <h1 align="center" style="margin:1em;">
   <a href="https://ioos.github.io/erddapy/">erddapy</a>
 </h1>
 
@@ -102,15 +117,15 @@
 ```shell
 conda install --channel conda-forge erddapy
 ```
 
 or, if you are a `pip` users
 
 ```shell
-pip install erddapy
+python -m pip install erddapy
 ```
 
 Note that, if you are installing the `requirements-dev.txt`, the `iris` package
 is named `scitools-iris` on PyPI so `pip` users must rename that before installing.
 
 ### Example
 
@@ -166,9 +181,7 @@
 - [erddap-python](https://github.com/hmedrano/erddap-python) 99% of the same functionality as erddapy but with a JavaScript-like API.
 
 ## License and copyright
 
 Erddapy is licensed under BSD 3-Clause "New" or "Revised" License (BSD-3-Clause).
 
 Development occurs on GitHub at <https://github.com/ioos/erddapy>.
-
-
```

#### html2text {}

```diff
@@ -1,20 +1,32 @@
-Metadata-Version: 2.1 Name: erddapy Version: 1.2.1 Summary: Python interface
-for ERDDAP Home-page: https://github.com/ioos/erddapy Author: Filipe Fernandes
-Author-email: ocefpaf@gmail.com License: BSD-3-Clause Project-URL:
-Documentation, https://ioos.github.io/erddapy Project-URL: Bug Tracker, https:/
-/github.com/ioos/erddapy/issues Project-URL: Source Code, https://github.com/
-ioos/erddapy Platform: UNKNOWN Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
-Operating System :: OS Independent Classifier: License :: OSI Approved :: BSD
-License Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Topic :: Scientific/Engineering Requires-
-Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE.txt
+Metadata-Version: 2.1 Name: erddapy Version: 2.0.0 Summary: Python interface
+for ERDDAP Author-email: Filipe Fernandes
+erddapy@gmail.com> License: Copyright 2017 Filipe Fernandes Redistribution and
+use in source and binary forms, with or without modification, are permitted
+provided that the following conditions are met: 1. Redistributions of source
+code must retain the above copyright notice, this list of conditions and the
+following disclaimer. 2. Redistributions in binary form must reproduce the
+above copyright notice, this list of conditions and the following disclaimer in
+the documentation and/or other materials provided with the distribution. 3.
+Neither the name of the copyright holder nor the names of its contributors may
+be used to endorse or promote products derived from this software without
+specific prior written permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT
+HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
+INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
+FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
+COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
+INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
+LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
+PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
+OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
+ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. Project-URL: documentation, https://
+ioos.github.io/erddapy Project-URL: homepage, https://github.com/ioos/erddapy
+Project-URL: repository, https://github.com/ioos/erddapy Requires-Python: >=3.8
+Description-Content-Type: text/markdown License-File: LICENSE.txt
                              ****** erddapy ******
                        *** erddapy: ERDDAP + Python. ***
    [conda-forge_downloads] [Latest_version] [Commits_since_last_release] [#
       contributors] [zenodo] [zenodo] [pre-commit.ci_status] [GHA-tests]
 
 # Table of contents  - [Overview](#overview) - [Example](#example) - [Get in
 touch](#get-in-touch) - [License and copyright](#license-and-copyright)  ##
@@ -25,15 +37,15 @@
 to get the data in multiple the formats. For more information on ERDDAP servers
 please see [https://coastwatch.pfeg.noaa.gov/erddap/index.html](https://
 coastwatch.pfeg.noaa.gov/erddap/index.html). ### Documentation and code The
 documentation is hosted at
 ioos.github.io/erddapy>. The code is hosted at
 github.com/ioos/erddapy>. ### Installation For `conda` users you can ```shell
 conda install --channel conda-forge erddapy ``` or, if you are a `pip` users
-```shell pip install erddapy ``` Note that, if you are installing the
+```shell python -m pip install erddapy ``` Note that, if you are installing the
 `requirements-dev.txt`, the `iris` package is named `scitools-iris` on PyPI so
 `pip` users must rename that before installing. ### Example ```python from
 erddapy import ERDDAP e = ERDDAP( server="https://gliders.ioos.us/erddap",
 protocol="tabledap", ) e.response = "csv" e.dataset_id = "whoi_406-
 20160902T1700" e.constraints = { "time>=": "2016-07-10T00:00:00Z", "time<=":
 "2017-02-10T00:00:00Z", "latitude>=": 38.0, "latitude<=": 41.0, "longitude>=":
 -72.0, "longitude<=": -69.0, } e.variables = [ "depth", "latitude",
```

### Comparing `erddapy-1.2.1/README.md` & `erddapy-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 ```shell
 conda install --channel conda-forge erddapy
 ```
 
 or, if you are a `pip` users
 
 ```shell
-pip install erddapy
+python -m pip install erddapy
 ```
 
 Note that, if you are installing the `requirements-dev.txt`, the `iris` package
 is named `scitools-iris` on PyPI so `pip` users must rename that before installing.
 
 ### Example
```

#### html2text {}

```diff
@@ -12,15 +12,15 @@
 to get the data in multiple the formats. For more information on ERDDAP servers
 please see [https://coastwatch.pfeg.noaa.gov/erddap/index.html](https://
 coastwatch.pfeg.noaa.gov/erddap/index.html). ### Documentation and code The
 documentation is hosted at
 ioos.github.io/erddapy>. The code is hosted at
 github.com/ioos/erddapy>. ### Installation For `conda` users you can ```shell
 conda install --channel conda-forge erddapy ``` or, if you are a `pip` users
-```shell pip install erddapy ``` Note that, if you are installing the
+```shell python -m pip install erddapy ``` Note that, if you are installing the
 `requirements-dev.txt`, the `iris` package is named `scitools-iris` on PyPI so
 `pip` users must rename that before installing. ### Example ```python from
 erddapy import ERDDAP e = ERDDAP( server="https://gliders.ioos.us/erddap",
 protocol="tabledap", ) e.response = "csv" e.dataset_id = "whoi_406-
 20160902T1700" e.constraints = { "time>=": "2016-07-10T00:00:00Z", "time<=":
 "2017-02-10T00:00:00Z", "latitude>=": 38.0, "latitude<=": 41.0, "longitude>=":
 -72.0, "longitude<=": -69.0, } e.variables = [ "depth", "latitude",
```

### Comparing `erddapy-1.2.1/erddapy/erddaps.json` & `erddapy-2.0.0/erddapy/servers/erddaps.json`

 * *Files identical despite different names*

### Comparing `erddapy-1.2.1/erddapy/multiple_server_search.py` & `erddapy-2.0.0/erddapy/multiple_server_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,35 @@
 """Multiple Server Search."""
 
 import multiprocessing
 from typing import Dict
-from typing.io import BinaryIO
 
 import pandas as pd
-import requests
 
 try:
     joblib = True
     from joblib import Parallel, delayed
 except ImportError:
     joblib = False
 
-from erddapy.erddapy import _search_url
-from erddapy.servers import servers
-from erddapy.url_handling import urlopen
-
-
-def _format_search_string(server: str, query: str) -> str:
-    """Generate a search string for an erddap server with user defined query."""
-    return f'{server}search/index.csv?page=1&itemsPerPage=100000&searchFor="{query}"'
+from erddapy.core.url import (
+    _format_search_string,
+    _multi_urlopen,
+    get_search_url,
+)
+from erddapy.servers.servers import servers
 
 
 def _format_results(dfs: Dict[str, pd.DataFrame]) -> pd.DataFrame:
+    """Format dictionary of results into a Pandas dataframe."""
     # we return None for bad server, so we need to filter them here
     df_all = pd.concat([list(df.values())[0] for df in dfs if df is not None])
     return df_all.reset_index(drop=True)
 
 
-def _multi_urlopen(url: str) -> BinaryIO:
-    """Simpler url open to work with multiprocessing."""
-    try:
-        data = urlopen(url)
-    except (requests.exceptions.HTTPError, requests.exceptions.ConnectionError):
-        return None
-    return data
-
-
 def fetch_results(
     url: str,
     key: str,
     protocol,
 ) -> Dict[str, pd.DataFrame]:
     """
     Fetch search results from multiple servers.
@@ -124,20 +112,20 @@
     if protocol not in ["tabledap", "griddap"]:
         raise ValueError(
             f"Protocol must be tabledap or griddap, got {protocol}",
         )
     response = "csv"
     if servers_list:
         urls = {
-            server: _search_url(server, response=response, **kwargs)
+            server: get_search_url(server, response=response, **kwargs)
             for server in servers_list
         }
     else:
         urls = {
-            key: _search_url(server.url, response=response, **kwargs)
+            key: get_search_url(server.url, response=response, **kwargs)
             for key, server in servers.items()
         }
 
     if parallel:
         num_cores = multiprocessing.cpu_count()
         if not joblib:
             raise ImportError(
```

### Comparing `erddapy-1.2.1/erddapy/netcdf_handling.py` & `erddapy-2.0.0/erddapy/core/netcdf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Handles netCDF responses."""
 
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Dict, Generator
-from typing.io import BinaryIO
+from typing import BinaryIO, Dict, Generator, Optional
 from urllib.parse import urlparse
 
-from erddapy.url_handling import urlopen
+from erddapy.core.url import urlopen
 
 
-def _nc_dataset(url, auth, **requests_kwargs: Dict):
+def _nc_dataset(url, requests_kwargs: Optional[Dict] = None):
     """Return a netCDF4-python Dataset from memory and fallbacks to disk if that fails."""
     from netCDF4 import Dataset
 
-    data = urlopen(url=url, auth=auth, **requests_kwargs)
+    data = urlopen(url, requests_kwargs)
     try:
         return Dataset(Path(urlparse(url).path).name, memory=data.read())
     except OSError:
         # if libnetcdf is not compiled with in-memory support fallback to a local tmp file
+        data.seek(0)
         with _tempnc(data) as _nc:
             return Dataset(_nc)
 
 
 @contextmanager
 def _tempnc(data: BinaryIO) -> Generator[str, None, None]:
     """Create a temporary netcdf file."""
```

### Comparing `erddapy-1.2.1/erddapy/servers.py` & `erddapy-2.0.0/erddapy/servers/servers.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import functools
 from collections import namedtuple
 
 import pandas as pd
 
 
-@functools.lru_cache(maxsize=None)
+@functools.lru_cache(maxsize=128)
 def servers_list():
     """
     Download a new server list from awesome-erddap.
 
     If loading the latest one fails it falls back to the default one shipped with the package.
 
     """
```


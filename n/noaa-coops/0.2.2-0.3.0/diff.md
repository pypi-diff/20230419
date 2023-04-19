# Comparing `tmp/noaa_coops-0.2.2.tar.gz` & `tmp/noaa_coops-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noaa_coops-0.2.2.tar", max compression
+gzip compressed data, was "noaa_coops-0.3.0.tar", max compression
```

## Comparing `noaa_coops-0.2.2.tar` & `noaa_coops-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35141 2023-02-05 16:17:34.880061 noaa_coops-0.2.2/LICENSE
--rw-r--r--   0        0        0     5499 2023-02-07 01:49:14.952908 noaa_coops-0.2.2/README.md
--rw-r--r--   0        0        0      101 2023-04-17 06:04:01.773060 noaa_coops-0.2.2/noaa_coops/__init__.py
--rw-r--r--   0        0        0    35861 2023-04-17 06:04:01.773911 noaa_coops-0.2.2/noaa_coops/station.py
--rw-r--r--   0        0        0     1564 2023-04-17 06:04:01.774618 noaa_coops-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6504 1970-01-01 00:00:00.000000 noaa_coops-0.2.2/setup.py
--rw-r--r--   0        0        0     6385 1970-01-01 00:00:00.000000 noaa_coops-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11345 2023-04-19 16:48:21.778836 noaa_coops-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5654 2023-04-19 16:48:21.780187 noaa_coops-0.3.0/README.md
+-rw-r--r--   0        0        0      101 2023-04-19 16:48:21.781179 noaa_coops-0.3.0/noaa_coops/__init__.py
+-rw-r--r--   0        0        0    30171 2023-04-19 16:48:21.782340 noaa_coops-0.3.0/noaa_coops/station.py
+-rw-r--r--   0        0        0     1567 2023-04-19 16:48:21.783609 noaa_coops-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6650 1970-01-01 00:00:00.000000 noaa_coops-0.3.0/setup.py
+-rw-r--r--   0        0        0     6557 1970-01-01 00:00:00.000000 noaa_coops-0.3.0/PKG-INFO
```

### Comparing `noaa_coops-0.2.2/README.md` & `noaa_coops-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,42 +16,42 @@
 Data is accessed via `Station` class objects. Each station is uniquely identified by an `id`. To initialize a `Station` object, run:
 
 ```python
 >>> from noaa_coops import Station
 >>> seattle = Station(id="9447130")  # Create Station object for Seattle (ID = 9447130)
 ```
 
-Stations can be found with the Tides & Currents [mapping interface](https://tidesandcurrents.noaa.gov/) or the `get_stations_from_bbox` function, which searches a bounding box for stations and returns their IDs (if found).
+Stations and their IDs can be found using the Tides & Currents [mapping interface](https://tidesandcurrents.noaa.gov/). Alternatively, you can search for stations in a bounding box using the `get_stations_from_bbox` function, which will return a list of stations found in the box (if any).
 ```python
 >>> from pprint import pprint
 >>> from noaa_coops import Station, get_stations_from_bbox
 >>> stations = get_stations_from_bbox(lat_coords=[40.389, 40.9397], lon_coords=[-74.4751, -73.7432])
 >>> pprint(stations)
 ['8516945', '8518750', '8519483', '8531680']
 >>> station_one = Station(id="8516945")
 >>> pprint(station_one.name)
 'Kings Point'
 ```
 
-#### Metadata
+### Metadata
 Station metadata is stored in the `.metadata` attribute of a `Station` object. Additionally, the keys of the metadata attribute dictionary are also assigned as attributes of the station object itself.
 
 ```python
 >>> from pprint import pprint
 >>> from noaa_coops import Station
 >>> seattle = Station(id="9447130")
 >>> pprint(list(seattle.metadata.items())[:5])                   # Print first 3 items in metadata
 [('tidal', True), ('greatlakes', False), ('shefcode', 'EBSW1')]  # Metadata dictionary can be very long
 >>> pprint(seattle.lat_lon['lat'])                               # Print latitude
 47.601944
 >>> pprint(seattle.lat_lon['lon'])                               # Print longitude
 -122.339167
 ```
 
-#### Data Inventory
+### Data Inventory
 A description of a Station's data products and available dates can be accessed via the `.data_inventory` attribute of a `Station` object.
 
 ```python
 >>> from noaa_coops import Station
 >>> from pprint import pprint
 >>> seattle = Station(id="9447130")
 >>> pprint(seattle.data_inventory)
@@ -70,48 +70,39 @@
  'Verified Monthly Mean Water Level': {'end_date': '2022-12-31 23:54',
                                        'start_date': '1898-12-01 00:00'},
  'Water Temperature': {'end_date': '2019-01-02 18:36',
                        'start_date': '1991-11-09 00:00'},
  'Wind': {'end_date': '2019-01-02 18:36', 'start_date': '1991-11-09 00:00'}}
 ```
 
-#### Data
-Station data can be fetched using the `.get_data` method on a `Station` object. Data is returned as Pandas DataFrames for ease of use and analysis. Available data products can be found in [NOAA CO-OPS Data API](https://tidesandcurrents.noaa.gov/api/#products) docs.
+### Data Retrieval
+Available data products can be found in NOAA CO-OPS Data API docs.
 
-`noaa_coops` currently supports the following data products:
-- Currents
-- Observed water levels
-- Observed daily high and low water levels (use `product="high_low"`)
-- Predicted water levels
-- Predicted high and low water levels
-- Winds
-- Air pressure
-- Air temperature
-- Water temperature
+Station data can be fetched using the `.get_data` method on a `Station` object. Data is returned as a Pandas [DataFrame](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html) for ease of use and analysis. DataFrame columns are named according to the NOAA CO-OPS API [docs](https://api.tidesandcurrents.noaa.gov/api/prod/responseHelp.html), with the `t` column (timestamp) set as the DataFrame index.
 
-The example below fetches water level data from the Seattle station for a 3 month period.
+The example below fetches water level data from the Seattle station (id=9447130) for a 1 month period. The [web output](https://tidesandcurrents.noaa.gov/waterlevels.html?id=9447130&units=metric&bdate=20150101&edate=20150131&timezone=GMT&datum=MLLW) is shown below the code as a reference.
 
 ```python
 >>> from noaa_coops import Station
 >>> seattle = Station(id="9447130")
 >>> df_water_levels = seattle.get_data(
 ...     begin_date="20150101",
-...     end_date="20150331",
+...     end_date="20150131",
 ...     product="water_level",
 ...     datum="MLLW",
 ...     units="metric",
 ...     time_zone="gmt")
 >>> df_water_levels.head()
-                     water_level  sigma    flags QC
-date_time
-2015-01-01 00:00:00        1.799  0.023  0,0,0,0  v
-2015-01-01 00:06:00        1.718  0.018  0,0,0,0  v
-2015-01-01 00:12:00        1.639  0.013  0,0,0,0  v
-2015-01-01 00:18:00        1.557  0.012  0,0,0,0  v
-2015-01-01 00:24:00        1.473  0.014  0,0,0,0  v
+                         v      s        f  q
+t
+2015-01-01 00:00:00  1.799  0.023  0,0,0,0  v
+2015-01-01 00:06:00  1.718  0.018  0,0,0,0  v
+2015-01-01 00:12:00  1.639  0.013  0,0,0,0  v
+2015-01-01 00:18:00  1.557  0.012  0,0,0,0  v
+2015-01-01 00:24:00  1.473  0.014  0,0,0,0  v
 
 ```
 
 ## Development
 
 ### Requirements
 This package and its dependencies are managed using [poetry](https://python-poetry.org/). To install the development environment for `noaa_coops`, first install poetry, then run (inside the repo):
```

### Comparing `noaa_coops-0.2.2/pyproject.toml` & `noaa_coops-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "noaa-coops"
-version = "0.2.2"
+version = "0.3.0"
 description = "Python wrapper for NOAA Tides & Currents Data and Metadata."
 authors = ["Greg Clunies <greg.clunies@gmail.com>"]
-license = "GNU GPL"
+license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/GClunies/noaa_coops"
 keywords = ["noaa", "coops", "tides", "currents", "weather", "api"]
 packages = [{include = "noaa_coops"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `noaa_coops-0.2.2/setup.py` & `noaa_coops-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['numpy>=1.24.1,<2.0.0',
  'pandas>=1.5.3,<2.0.0',
  'requests>=2.28.2,<3.0.0',
  'zeep>=4.2.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'noaa-coops',
-    'version': '0.2.2',
+    'version': '0.3.0',
     'description': 'Python wrapper for NOAA Tides & Currents Data and Metadata.',
-    'long_description': '# noaa_coops\n\n[![Build Status](https://travis-ci.org/GClunies/noaa_coops.svg?branch=master)](https://travis-ci.org/GClunies/noaa_coops)\n[![PyPI](https://img.shields.io/pypi/v/noaa_coops.svg)](https://pypi.python.org/pypi/noaa-coops)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/noaa_coops.svg)](https://pypi.python.org/pypi/noaa-coops)\n\nA Python wrapper for the NOAA CO-OPS Tides &amp; Currents [Data](https://tidesandcurrents.noaa.gov/api/)\nand [Metadata](https://tidesandcurrents.noaa.gov/mdapi/latest/) APIs.\n\n## Installation\nThis package is distributed through [pip](https://pypi.org/project/noaa-coops/) and can be installed to an environment via `pip install noaa-coops`.\n\n## Getting Started\n\n### Stations\nData is accessed via `Station` class objects. Each station is uniquely identified by an `id`. To initialize a `Station` object, run:\n\n```python\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")  # Create Station object for Seattle (ID = 9447130)\n```\n\nStations can be found with the Tides & Currents [mapping interface](https://tidesandcurrents.noaa.gov/) or the `get_stations_from_bbox` function, which searches a bounding box for stations and returns their IDs (if found).\n```python\n>>> from pprint import pprint\n>>> from noaa_coops import Station, get_stations_from_bbox\n>>> stations = get_stations_from_bbox(lat_coords=[40.389, 40.9397], lon_coords=[-74.4751, -73.7432])\n>>> pprint(stations)\n[\'8516945\', \'8518750\', \'8519483\', \'8531680\']\n>>> station_one = Station(id="8516945")\n>>> pprint(station_one.name)\n\'Kings Point\'\n```\n\n#### Metadata\nStation metadata is stored in the `.metadata` attribute of a `Station` object. Additionally, the keys of the metadata attribute dictionary are also assigned as attributes of the station object itself.\n\n```python\n>>> from pprint import pprint\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")\n>>> pprint(list(seattle.metadata.items())[:5])                   # Print first 3 items in metadata\n[(\'tidal\', True), (\'greatlakes\', False), (\'shefcode\', \'EBSW1\')]  # Metadata dictionary can be very long\n>>> pprint(seattle.lat_lon[\'lat\'])                               # Print latitude\n47.601944\n>>> pprint(seattle.lat_lon[\'lon\'])                               # Print longitude\n-122.339167\n```\n\n#### Data Inventory\nA description of a Station\'s data products and available dates can be accessed via the `.data_inventory` attribute of a `Station` object.\n\n```python\n>>> from noaa_coops import Station\n>>> from pprint import pprint\n>>> seattle = Station(id="9447130")\n>>> pprint(seattle.data_inventory)\n{\'Air Temperature\': {\'end_date\': \'2019-01-02 18:36\',\n                     \'start_date\': \'1991-11-09 01:00\'},\n \'Barometric Pressure\': {\'end_date\': \'2019-01-02 18:36\',\n                         \'start_date\': \'1991-11-09 00:00\'},\n \'Preliminary 6-Minute Water Level\': {\'end_date\': \'2023-02-05 19:54\',\n                                      \'start_date\': \'2001-01-01 00:00\'},\n \'Verified 6-Minute Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                   \'start_date\': \'1995-06-01 00:00\'},\n \'Verified High/Low Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                   \'start_date\': \'1977-10-18 02:18\'},\n \'Verified Hourly Height Water Level\': {\'end_date\': \'2022-12-31 23:00\',\n                                        \'start_date\': \'1899-01-01 00:00\'},\n \'Verified Monthly Mean Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                       \'start_date\': \'1898-12-01 00:00\'},\n \'Water Temperature\': {\'end_date\': \'2019-01-02 18:36\',\n                       \'start_date\': \'1991-11-09 00:00\'},\n \'Wind\': {\'end_date\': \'2019-01-02 18:36\', \'start_date\': \'1991-11-09 00:00\'}}\n```\n\n#### Data\nStation data can be fetched using the `.get_data` method on a `Station` object. Data is returned as Pandas DataFrames for ease of use and analysis. Available data products can be found in [NOAA CO-OPS Data API](https://tidesandcurrents.noaa.gov/api/#products) docs.\n\n`noaa_coops` currently supports the following data products:\n- Currents\n- Observed water levels\n- Observed daily high and low water levels (use `product="high_low"`)\n- Predicted water levels\n- Predicted high and low water levels\n- Winds\n- Air pressure\n- Air temperature\n- Water temperature\n\nThe example below fetches water level data from the Seattle station for a 3 month period.\n\n```python\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")\n>>> df_water_levels = seattle.get_data(\n...     begin_date="20150101",\n...     end_date="20150331",\n...     product="water_level",\n...     datum="MLLW",\n...     units="metric",\n...     time_zone="gmt")\n>>> df_water_levels.head()\n                     water_level  sigma    flags QC\ndate_time\n2015-01-01 00:00:00        1.799  0.023  0,0,0,0  v\n2015-01-01 00:06:00        1.718  0.018  0,0,0,0  v\n2015-01-01 00:12:00        1.639  0.013  0,0,0,0  v\n2015-01-01 00:18:00        1.557  0.012  0,0,0,0  v\n2015-01-01 00:24:00        1.473  0.014  0,0,0,0  v\n\n```\n\n## Development\n\n### Requirements\nThis package and its dependencies are managed using [poetry](https://python-poetry.org/). To install the development environment for `noaa_coops`, first install poetry, then run (inside the repo):\n\n```bash\npoetry install\n```\n\n### TODO\nClick [here](https://github.com/GClunies/noaa_coops/issues) for a list of existing issues and to submit a new one.\n\n### Contribution\nContributions are welcome, feel free to submit a pull request.\n',
+    'long_description': '# noaa_coops\n\n[![Build Status](https://travis-ci.org/GClunies/noaa_coops.svg?branch=master)](https://travis-ci.org/GClunies/noaa_coops)\n[![PyPI](https://img.shields.io/pypi/v/noaa_coops.svg)](https://pypi.python.org/pypi/noaa-coops)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/noaa_coops.svg)](https://pypi.python.org/pypi/noaa-coops)\n\nA Python wrapper for the NOAA CO-OPS Tides &amp; Currents [Data](https://tidesandcurrents.noaa.gov/api/)\nand [Metadata](https://tidesandcurrents.noaa.gov/mdapi/latest/) APIs.\n\n## Installation\nThis package is distributed through [pip](https://pypi.org/project/noaa-coops/) and can be installed to an environment via `pip install noaa-coops`.\n\n## Getting Started\n\n### Stations\nData is accessed via `Station` class objects. Each station is uniquely identified by an `id`. To initialize a `Station` object, run:\n\n```python\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")  # Create Station object for Seattle (ID = 9447130)\n```\n\nStations and their IDs can be found using the Tides & Currents [mapping interface](https://tidesandcurrents.noaa.gov/). Alternatively, you can search for stations in a bounding box using the `get_stations_from_bbox` function, which will return a list of stations found in the box (if any).\n```python\n>>> from pprint import pprint\n>>> from noaa_coops import Station, get_stations_from_bbox\n>>> stations = get_stations_from_bbox(lat_coords=[40.389, 40.9397], lon_coords=[-74.4751, -73.7432])\n>>> pprint(stations)\n[\'8516945\', \'8518750\', \'8519483\', \'8531680\']\n>>> station_one = Station(id="8516945")\n>>> pprint(station_one.name)\n\'Kings Point\'\n```\n\n### Metadata\nStation metadata is stored in the `.metadata` attribute of a `Station` object. Additionally, the keys of the metadata attribute dictionary are also assigned as attributes of the station object itself.\n\n```python\n>>> from pprint import pprint\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")\n>>> pprint(list(seattle.metadata.items())[:5])                   # Print first 3 items in metadata\n[(\'tidal\', True), (\'greatlakes\', False), (\'shefcode\', \'EBSW1\')]  # Metadata dictionary can be very long\n>>> pprint(seattle.lat_lon[\'lat\'])                               # Print latitude\n47.601944\n>>> pprint(seattle.lat_lon[\'lon\'])                               # Print longitude\n-122.339167\n```\n\n### Data Inventory\nA description of a Station\'s data products and available dates can be accessed via the `.data_inventory` attribute of a `Station` object.\n\n```python\n>>> from noaa_coops import Station\n>>> from pprint import pprint\n>>> seattle = Station(id="9447130")\n>>> pprint(seattle.data_inventory)\n{\'Air Temperature\': {\'end_date\': \'2019-01-02 18:36\',\n                     \'start_date\': \'1991-11-09 01:00\'},\n \'Barometric Pressure\': {\'end_date\': \'2019-01-02 18:36\',\n                         \'start_date\': \'1991-11-09 00:00\'},\n \'Preliminary 6-Minute Water Level\': {\'end_date\': \'2023-02-05 19:54\',\n                                      \'start_date\': \'2001-01-01 00:00\'},\n \'Verified 6-Minute Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                   \'start_date\': \'1995-06-01 00:00\'},\n \'Verified High/Low Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                   \'start_date\': \'1977-10-18 02:18\'},\n \'Verified Hourly Height Water Level\': {\'end_date\': \'2022-12-31 23:00\',\n                                        \'start_date\': \'1899-01-01 00:00\'},\n \'Verified Monthly Mean Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                       \'start_date\': \'1898-12-01 00:00\'},\n \'Water Temperature\': {\'end_date\': \'2019-01-02 18:36\',\n                       \'start_date\': \'1991-11-09 00:00\'},\n \'Wind\': {\'end_date\': \'2019-01-02 18:36\', \'start_date\': \'1991-11-09 00:00\'}}\n```\n\n### Data Retrieval\nAvailable data products can be found in NOAA CO-OPS Data API docs.\n\nStation data can be fetched using the `.get_data` method on a `Station` object. Data is returned as a Pandas [DataFrame](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html) for ease of use and analysis. DataFrame columns are named according to the NOAA CO-OPS API [docs](https://api.tidesandcurrents.noaa.gov/api/prod/responseHelp.html), with the `t` column (timestamp) set as the DataFrame index.\n\nThe example below fetches water level data from the Seattle station (id=9447130) for a 1 month period. The [web output](https://tidesandcurrents.noaa.gov/waterlevels.html?id=9447130&units=metric&bdate=20150101&edate=20150131&timezone=GMT&datum=MLLW) is shown below the code as a reference.\n\n```python\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")\n>>> df_water_levels = seattle.get_data(\n...     begin_date="20150101",\n...     end_date="20150131",\n...     product="water_level",\n...     datum="MLLW",\n...     units="metric",\n...     time_zone="gmt")\n>>> df_water_levels.head()\n                         v      s        f  q\nt\n2015-01-01 00:00:00  1.799  0.023  0,0,0,0  v\n2015-01-01 00:06:00  1.718  0.018  0,0,0,0  v\n2015-01-01 00:12:00  1.639  0.013  0,0,0,0  v\n2015-01-01 00:18:00  1.557  0.012  0,0,0,0  v\n2015-01-01 00:24:00  1.473  0.014  0,0,0,0  v\n\n```\n\n## Development\n\n### Requirements\nThis package and its dependencies are managed using [poetry](https://python-poetry.org/). To install the development environment for `noaa_coops`, first install poetry, then run (inside the repo):\n\n```bash\npoetry install\n```\n\n### TODO\nClick [here](https://github.com/GClunies/noaa_coops/issues) for a list of existing issues and to submit a new one.\n\n### Contribution\nContributions are welcome, feel free to submit a pull request.\n',
     'author': 'Greg Clunies',
     'author_email': 'greg.clunies@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/GClunies/noaa_coops',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `noaa_coops-0.2.2/PKG-INFO` & `noaa_coops-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: noaa-coops
-Version: 0.2.2
+Version: 0.3.0
 Summary: Python wrapper for NOAA Tides & Currents Data and Metadata.
 Home-page: https://github.com/GClunies/noaa_coops
-License: GNU GPL
+License: Apache-2.0
 Keywords: noaa,coops,tides,currents,weather,api
 Author: Greg Clunies
 Author-email: greg.clunies@gmail.com
 Requires-Python: >=3.8,<4.0
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
@@ -39,42 +39,42 @@
 Data is accessed via `Station` class objects. Each station is uniquely identified by an `id`. To initialize a `Station` object, run:
 
 ```python
 >>> from noaa_coops import Station
 >>> seattle = Station(id="9447130")  # Create Station object for Seattle (ID = 9447130)
 ```
 
-Stations can be found with the Tides & Currents [mapping interface](https://tidesandcurrents.noaa.gov/) or the `get_stations_from_bbox` function, which searches a bounding box for stations and returns their IDs (if found).
+Stations and their IDs can be found using the Tides & Currents [mapping interface](https://tidesandcurrents.noaa.gov/). Alternatively, you can search for stations in a bounding box using the `get_stations_from_bbox` function, which will return a list of stations found in the box (if any).
 ```python
 >>> from pprint import pprint
 >>> from noaa_coops import Station, get_stations_from_bbox
 >>> stations = get_stations_from_bbox(lat_coords=[40.389, 40.9397], lon_coords=[-74.4751, -73.7432])
 >>> pprint(stations)
 ['8516945', '8518750', '8519483', '8531680']
 >>> station_one = Station(id="8516945")
 >>> pprint(station_one.name)
 'Kings Point'
 ```
 
-#### Metadata
+### Metadata
 Station metadata is stored in the `.metadata` attribute of a `Station` object. Additionally, the keys of the metadata attribute dictionary are also assigned as attributes of the station object itself.
 
 ```python
 >>> from pprint import pprint
 >>> from noaa_coops import Station
 >>> seattle = Station(id="9447130")
 >>> pprint(list(seattle.metadata.items())[:5])                   # Print first 3 items in metadata
 [('tidal', True), ('greatlakes', False), ('shefcode', 'EBSW1')]  # Metadata dictionary can be very long
 >>> pprint(seattle.lat_lon['lat'])                               # Print latitude
 47.601944
 >>> pprint(seattle.lat_lon['lon'])                               # Print longitude
 -122.339167
 ```
 
-#### Data Inventory
+### Data Inventory
 A description of a Station's data products and available dates can be accessed via the `.data_inventory` attribute of a `Station` object.
 
 ```python
 >>> from noaa_coops import Station
 >>> from pprint import pprint
 >>> seattle = Station(id="9447130")
 >>> pprint(seattle.data_inventory)
@@ -93,48 +93,39 @@
  'Verified Monthly Mean Water Level': {'end_date': '2022-12-31 23:54',
                                        'start_date': '1898-12-01 00:00'},
  'Water Temperature': {'end_date': '2019-01-02 18:36',
                        'start_date': '1991-11-09 00:00'},
  'Wind': {'end_date': '2019-01-02 18:36', 'start_date': '1991-11-09 00:00'}}
 ```
 
-#### Data
-Station data can be fetched using the `.get_data` method on a `Station` object. Data is returned as Pandas DataFrames for ease of use and analysis. Available data products can be found in [NOAA CO-OPS Data API](https://tidesandcurrents.noaa.gov/api/#products) docs.
+### Data Retrieval
+Available data products can be found in NOAA CO-OPS Data API docs.
 
-`noaa_coops` currently supports the following data products:
-- Currents
-- Observed water levels
-- Observed daily high and low water levels (use `product="high_low"`)
-- Predicted water levels
-- Predicted high and low water levels
-- Winds
-- Air pressure
-- Air temperature
-- Water temperature
+Station data can be fetched using the `.get_data` method on a `Station` object. Data is returned as a Pandas [DataFrame](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html) for ease of use and analysis. DataFrame columns are named according to the NOAA CO-OPS API [docs](https://api.tidesandcurrents.noaa.gov/api/prod/responseHelp.html), with the `t` column (timestamp) set as the DataFrame index.
 
-The example below fetches water level data from the Seattle station for a 3 month period.
+The example below fetches water level data from the Seattle station (id=9447130) for a 1 month period. The [web output](https://tidesandcurrents.noaa.gov/waterlevels.html?id=9447130&units=metric&bdate=20150101&edate=20150131&timezone=GMT&datum=MLLW) is shown below the code as a reference.
 
 ```python
 >>> from noaa_coops import Station
 >>> seattle = Station(id="9447130")
 >>> df_water_levels = seattle.get_data(
 ...     begin_date="20150101",
-...     end_date="20150331",
+...     end_date="20150131",
 ...     product="water_level",
 ...     datum="MLLW",
 ...     units="metric",
 ...     time_zone="gmt")
 >>> df_water_levels.head()
-                     water_level  sigma    flags QC
-date_time
-2015-01-01 00:00:00        1.799  0.023  0,0,0,0  v
-2015-01-01 00:06:00        1.718  0.018  0,0,0,0  v
-2015-01-01 00:12:00        1.639  0.013  0,0,0,0  v
-2015-01-01 00:18:00        1.557  0.012  0,0,0,0  v
-2015-01-01 00:24:00        1.473  0.014  0,0,0,0  v
+                         v      s        f  q
+t
+2015-01-01 00:00:00  1.799  0.023  0,0,0,0  v
+2015-01-01 00:06:00  1.718  0.018  0,0,0,0  v
+2015-01-01 00:12:00  1.639  0.013  0,0,0,0  v
+2015-01-01 00:18:00  1.557  0.012  0,0,0,0  v
+2015-01-01 00:24:00  1.473  0.014  0,0,0,0  v
 
 ```
 
 ## Development
 
 ### Requirements
 This package and its dependencies are managed using [poetry](https://python-poetry.org/). To install the development environment for `noaa_coops`, first install poetry, then run (inside the repo):
```


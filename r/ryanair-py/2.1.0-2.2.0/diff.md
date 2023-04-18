# Comparing `tmp/ryanair-py-2.1.0.tar.gz` & `tmp/ryanair-py-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryanair-py-2.1.0.tar", last modified: Sun Mar 12 20:55:42 2023, max compression
+gzip compressed data, was "ryanair-py-2.2.0.tar", last modified: Tue Apr 18 22:32:10 2023, max compression
```

## Comparing `ryanair-py-2.1.0.tar` & `ryanair-py-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ciaran    (1000) ciaran    (1000)        0 2023-03-12 20:55:42.360718 ryanair-py-2.1.0/
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     1097 2023-03-11 14:18:49.000000 ryanair-py-2.1.0/LICENSE.md
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     4827 2023-03-12 20:55:42.360718 ryanair-py-2.1.0/PKG-INFO
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     4414 2023-03-12 20:54:14.000000 ryanair-py-2.1.0/README.md
-drwxrwxr-x   0 ciaran    (1000) ciaran    (1000)        0 2023-03-12 20:55:42.360718 ryanair-py-2.1.0/ryanair/
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)       37 2023-03-11 14:18:49.000000 ryanair-py-2.1.0/ryanair/__init__.py
--rw-r--r--   0 ciaran    (1000) ciaran    (1000)     1516 2022-09-17 10:38:33.000000 ryanair-py-2.1.0/ryanair/airport_utils.py
--rw-r--r--   0 ciaran    (1000) ciaran    (1000)  9857193 2022-09-17 10:38:33.000000 ryanair-py-2.1.0/ryanair/airports.csv
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     9961 2023-03-12 20:54:14.000000 ryanair-py-2.1.0/ryanair/ryanair.py
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)      269 2023-03-11 14:18:49.000000 ryanair-py-2.1.0/ryanair/types.py
-drwxrwxr-x   0 ciaran    (1000) ciaran    (1000)        0 2023-03-12 20:55:42.360718 ryanair-py-2.1.0/ryanair_py.egg-info/
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     4827 2023-03-12 20:55:42.000000 ryanair-py-2.1.0/ryanair_py.egg-info/PKG-INFO
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)      300 2023-03-12 20:55:42.000000 ryanair-py-2.1.0/ryanair_py.egg-info/SOURCES.txt
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)        1 2023-03-12 20:55:42.000000 ryanair-py-2.1.0/ryanair_py.egg-info/dependency_links.txt
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)       28 2023-03-12 20:55:42.000000 ryanair-py-2.1.0/ryanair_py.egg-info/requires.txt
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)        8 2023-03-12 20:55:42.000000 ryanair-py-2.1.0/ryanair_py.egg-info/top_level.txt
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)       38 2023-03-12 20:55:42.360718 ryanair-py-2.1.0/setup.cfg
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     1009 2023-03-12 20:54:30.000000 ryanair-py-2.1.0/setup.py
+drwxrwxr-x   0 ciaran    (1000) ciaran    (1000)        0 2023-04-18 22:32:10.991868 ryanair-py-2.2.0/
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     1097 2023-03-11 14:18:49.000000 ryanair-py-2.2.0/LICENSE.md
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     5463 2023-04-18 22:32:10.987868 ryanair-py-2.2.0/PKG-INFO
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     5056 2023-04-18 22:28:28.000000 ryanair-py-2.2.0/README.md
+drwxrwxr-x   0 ciaran    (1000) ciaran    (1000)        0 2023-04-18 22:32:10.987868 ryanair-py-2.2.0/ryanair/
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)       37 2023-03-11 14:18:49.000000 ryanair-py-2.2.0/ryanair/__init__.py
+-rw-r--r--   0 ciaran    (1000) ciaran    (1000)     1516 2022-09-17 10:38:33.000000 ryanair-py-2.2.0/ryanair/airport_utils.py
+-rw-r--r--   0 ciaran    (1000) ciaran    (1000)  9857193 2022-09-17 10:38:33.000000 ryanair-py-2.2.0/ryanair/airports.csv
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)    11141 2023-04-18 22:28:28.000000 ryanair-py-2.2.0/ryanair/ryanair.py
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)      281 2023-04-18 22:28:28.000000 ryanair-py-2.2.0/ryanair/types.py
+drwxrwxr-x   0 ciaran    (1000) ciaran    (1000)        0 2023-04-18 22:32:10.987868 ryanair-py-2.2.0/ryanair_py.egg-info/
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     5463 2023-04-18 22:32:10.000000 ryanair-py-2.2.0/ryanair_py.egg-info/PKG-INFO
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)      300 2023-04-18 22:32:10.000000 ryanair-py-2.2.0/ryanair_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)        1 2023-04-18 22:32:10.000000 ryanair-py-2.2.0/ryanair_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)       28 2023-04-18 22:32:10.000000 ryanair-py-2.2.0/ryanair_py.egg-info/requires.txt
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)        8 2023-04-18 22:32:10.000000 ryanair-py-2.2.0/ryanair_py.egg-info/top_level.txt
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)       38 2023-04-18 22:32:10.991868 ryanair-py-2.2.0/setup.cfg
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     1009 2023-04-18 22:29:05.000000 ryanair-py-2.2.0/setup.py
```

### Comparing `ryanair-py-2.1.0/LICENSE.md` & `ryanair-py-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ryanair-py-2.1.0/PKG-INFO` & `ryanair-py-2.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryanair-py
-Version: 2.1.0
+Version: 2.2.0
 Summary: A module which allows you to retrieve data about the cheapest one-way and return flights in a date range, or all available flights on a given day for a given route.
 Home-page: https://github.com/cohaolain/ryanair-py
 Author: Ciarán Ó hAoláin
 Author-email: ciaran@cohaolain.ie
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -23,79 +23,85 @@
 ```
 pip install ryanair-py
 ```
 ## Usage
 To create an instance:
 ```python
 from ryanair import Ryanair
-api = Ryanair("EUR")  # Euro currency, so could also be GBP etc. also
+
+# You can set a currency at the API instance level, so could also be GBP etc. also.
+# Note that this may not *always* be respected by the API, so always check the currency returned matches
+# your expectation. For example, the underlying API for get_all_flights does not support this.
+api = Ryanair("EUR")
 ```
 ### Get the cheapest one-way flights
 Get the cheapest flights from a given origin airport (returns at most 1 flight to each destination).
 ```python
 from datetime import datetime, timedelta
 from ryanair import Ryanair
 from ryanair.types import Flight
 
-api = Ryanair("EUR")  # Euro currency, so could also be GBP etc. also
+api = Ryanair(currency="EUR")  # Euro currency, so could also be GBP etc. also
 tomorrow = datetime.today().date() + timedelta(days=1)
 
 flights = api.get_cheapest_flights("DUB", tomorrow, tomorrow + timedelta(days=1))
 
 # Returns a list of Flight namedtuples
 flight: Flight = flights[0]
-print(flight)  # Flight(departureTime=datetime.datetime(2023, 3, 12, 17, 0), flightNumber='FR9717', price=31.99, origin='DUB', originFull='Dublin, Ireland', destination='GOA', destinationFull='Genoa, Italy')
+print(flight)  # Flight(departureTime=datetime.datetime(2023, 3, 12, 17, 0), flightNumber='FR9717', price=31.99, currency='EUR' origin='DUB', originFull='Dublin, Ireland', destination='GOA', destinationFull='Genoa, Italy')
 print(flight.price)  # 9.78
 ```
 ### Get the cheapest return trips (outbound and inbound)
 ```python
 from datetime import datetime, timedelta
 from ryanair import Ryanair
 
-api = Ryanair("EUR")  # Euro currency, so could also be GBP etc. also
+api = Ryanair(currency="EUR")  # Euro currency, so could also be GBP etc. also
 tomorrow = datetime.today().date() + timedelta(days=1)
 tomorrow_1 = tomorrow + timedelta(days=1)
 
 trips = api.get_cheapest_return_flights("DUB", tomorrow, tomorrow, tomorrow_1, tomorrow_1)
-print(trips[0])  # Trip(totalPrice=85.31, outbound=Flight(departureTime=datetime.datetime(2023, 3, 12, 7, 30), flightNumber='FR5437', price=49.84, origin='DUB', originFull='Dublin, Ireland', destination='EMA', destinationFull='East Midlands, United Kingdom'), inbound=Flight(departureTime=datetime.datetime(2023, 3, 13, 7, 45), flightNumber='FR5438', price=35.47, origin='EMA', originFull='East Midlands, United Kingdom', destination='DUB', destinationFull='Dublin, Ireland'))
+print(trips[0])  # Trip(totalPrice=85.31, outbound=Flight(departureTime=datetime.datetime(2023, 3, 12, 7, 30), flightNumber='FR5437', price=49.84, currency='EUR', origin='DUB', originFull='Dublin, Ireland', destination='EMA', destinationFull='East Midlands, United Kingdom'), inbound=Flight(departureTime=datetime.datetime(2023, 3, 13, 7, 45), flightNumber='FR5438', price=35.47, origin='EMA', originFull='East Midlands, United Kingdom', destination='DUB', destinationFull='Dublin, Ireland'))
 ```
 
 ### Get all available flights between two airports
 E.g. get all available flights from Dublin to London Gatwick, or London, tomorrow:
 ```python
 from datetime import datetime, timedelta
 
 from ryanair import Ryanair
 from tabulate import tabulate
 
-api = Ryanair("EUR")
+# We don't need to specify a currency if we're only using `get_all_flights`, as this API doesn't support currency 
+# conversion. It will always return dares denominated in the currency of the departure country.  
+api = Ryanair()
 tomorrow = datetime.today().date() + timedelta(days=1)
 
 flights = api.get_all_flights("DUB", tomorrow, "LGW")
 print(tabulate(flights, headers="keys", tablefmt="github"))
 
 # We can even expand it to include all vaguely-London airports:
 flights = api.get_all_flights("DUB", tomorrow, "LON", destination_is_mac=True)
 print(tabulate(flights, headers="keys", tablefmt="github"))
 ```
 
 This prints the following:
 
-| departureTime       | flightNumber   |   price | origin   | originFull   | destination   | destinationFull   |
-|---------------------|----------------|---------|----------|--------------|---------------|-------------------|
-| 2023-03-12 06:25:00 | FR 114         |   61.99 | DUB      | Dublin       | LGW           | London (Gatwick)  |
-| 2023-03-12 09:20:00 | FR 112         |   88.12 | DUB      | Dublin       | LGW           | London (Gatwick)  |
-| 2023-03-12 11:30:00 | FR 122         |  120.37 | DUB      | Dublin       | LGW           | London (Gatwick)  |
-| ...                 |                |         |          |              |               |                   |
+| departureTime       | flightNumber   |   price | currency | origin   | originFull   | destination   | destinationFull   |
+|---------------------|----------------|---------|----------|----------|--------------|---------------|-------------------|
+| 2023-03-12 06:25:00 | FR 114         |   61.99 | EUR      | DUB      | Dublin       | LGW           | London (Gatwick)  |
+| 2023-03-12 09:20:00 | FR 112         |   88.12 | EUR      | DUB      | Dublin       | LGW           | London (Gatwick)  |
+| 2023-03-12 11:30:00 | FR 122         |  120.37 | EUR      | DUB      | Dublin       | LGW           | London (Gatwick)  |
+| ...                 |                |         | EUR      |          |              |               |                   |
 
 
 and
 
-| departureTime       | flightNumber   |   price | origin   | originFull   | destination   | destinationFull   |
-|---------------------|----------------|---------|----------|--------------|---------------|-------------------|
-| 2023-03-12 06:25:00 | FR 114         |   61.99 | DUB      | Dublin       | LGW           | LON               |
-| 2023-03-12 06:35:00 | FR 202         |   65.09 | DUB      | Dublin       | STN           | LON               |
-| 2023-03-12 07:10:00 | FR 342         |   65.09 | DUB      | Dublin       | LTN           | LON               |
-| 2023-03-12 08:20:00 | FR 206         |  102.09 | DUB      | Dublin       | STN           | LON               |
-| ...                 |                |         |          |              |               |                   |
+| departureTime       | flightNumber   |   price | currency | origin   | originFull   | destination   | destinationFull   |
+|---------------------|----------------|---------|----------|----------|--------------|---------------|-------------------|
+| 2023-03-12 06:25:00 | FR 114         |   61.99 | EUR      | DUB      | Dublin       | LGW           | LON               |
+| 2023-03-12 06:35:00 | FR 202         |   65.09 | EUR      | DUB      | Dublin       | STN           | LON               |
+| 2023-03-12 07:10:00 | FR 342         |   65.09 | EUR      | DUB      | Dublin       | LTN           | LON               |
+| 2023-03-12 08:20:00 | FR 206         |  102.09 | EUR      | DUB      | Dublin       | STN           | LON               |
+| ...                 |                |         |          |          |              |               |                   |
```

### Comparing `ryanair-py-2.1.0/README.md` & `ryanair-py-2.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -11,79 +11,85 @@
 ```
 pip install ryanair-py
 ```
 ## Usage
 To create an instance:
 ```python
 from ryanair import Ryanair
-api = Ryanair("EUR")  # Euro currency, so could also be GBP etc. also
+
+# You can set a currency at the API instance level, so could also be GBP etc. also.
+# Note that this may not *always* be respected by the API, so always check the currency returned matches
+# your expectation. For example, the underlying API for get_all_flights does not support this.
+api = Ryanair("EUR")
 ```
 ### Get the cheapest one-way flights
 Get the cheapest flights from a given origin airport (returns at most 1 flight to each destination).
 ```python
 from datetime import datetime, timedelta
 from ryanair import Ryanair
 from ryanair.types import Flight
 
-api = Ryanair("EUR")  # Euro currency, so could also be GBP etc. also
+api = Ryanair(currency="EUR")  # Euro currency, so could also be GBP etc. also
 tomorrow = datetime.today().date() + timedelta(days=1)
 
 flights = api.get_cheapest_flights("DUB", tomorrow, tomorrow + timedelta(days=1))
 
 # Returns a list of Flight namedtuples
 flight: Flight = flights[0]
-print(flight)  # Flight(departureTime=datetime.datetime(2023, 3, 12, 17, 0), flightNumber='FR9717', price=31.99, origin='DUB', originFull='Dublin, Ireland', destination='GOA', destinationFull='Genoa, Italy')
+print(flight)  # Flight(departureTime=datetime.datetime(2023, 3, 12, 17, 0), flightNumber='FR9717', price=31.99, currency='EUR' origin='DUB', originFull='Dublin, Ireland', destination='GOA', destinationFull='Genoa, Italy')
 print(flight.price)  # 9.78
 ```
 ### Get the cheapest return trips (outbound and inbound)
 ```python
 from datetime import datetime, timedelta
 from ryanair import Ryanair
 
-api = Ryanair("EUR")  # Euro currency, so could also be GBP etc. also
+api = Ryanair(currency="EUR")  # Euro currency, so could also be GBP etc. also
 tomorrow = datetime.today().date() + timedelta(days=1)
 tomorrow_1 = tomorrow + timedelta(days=1)
 
 trips = api.get_cheapest_return_flights("DUB", tomorrow, tomorrow, tomorrow_1, tomorrow_1)
-print(trips[0])  # Trip(totalPrice=85.31, outbound=Flight(departureTime=datetime.datetime(2023, 3, 12, 7, 30), flightNumber='FR5437', price=49.84, origin='DUB', originFull='Dublin, Ireland', destination='EMA', destinationFull='East Midlands, United Kingdom'), inbound=Flight(departureTime=datetime.datetime(2023, 3, 13, 7, 45), flightNumber='FR5438', price=35.47, origin='EMA', originFull='East Midlands, United Kingdom', destination='DUB', destinationFull='Dublin, Ireland'))
+print(trips[0])  # Trip(totalPrice=85.31, outbound=Flight(departureTime=datetime.datetime(2023, 3, 12, 7, 30), flightNumber='FR5437', price=49.84, currency='EUR', origin='DUB', originFull='Dublin, Ireland', destination='EMA', destinationFull='East Midlands, United Kingdom'), inbound=Flight(departureTime=datetime.datetime(2023, 3, 13, 7, 45), flightNumber='FR5438', price=35.47, origin='EMA', originFull='East Midlands, United Kingdom', destination='DUB', destinationFull='Dublin, Ireland'))
 ```
 
 ### Get all available flights between two airports
 E.g. get all available flights from Dublin to London Gatwick, or London, tomorrow:
 ```python
 from datetime import datetime, timedelta
 
 from ryanair import Ryanair
 from tabulate import tabulate
 
-api = Ryanair("EUR")
+# We don't need to specify a currency if we're only using `get_all_flights`, as this API doesn't support currency 
+# conversion. It will always return dares denominated in the currency of the departure country.  
+api = Ryanair()
 tomorrow = datetime.today().date() + timedelta(days=1)
 
 flights = api.get_all_flights("DUB", tomorrow, "LGW")
 print(tabulate(flights, headers="keys", tablefmt="github"))
 
 # We can even expand it to include all vaguely-London airports:
 flights = api.get_all_flights("DUB", tomorrow, "LON", destination_is_mac=True)
 print(tabulate(flights, headers="keys", tablefmt="github"))
 ```
 
 This prints the following:
 
-| departureTime       | flightNumber   |   price | origin   | originFull   | destination   | destinationFull   |
-|---------------------|----------------|---------|----------|--------------|---------------|-------------------|
-| 2023-03-12 06:25:00 | FR 114         |   61.99 | DUB      | Dublin       | LGW           | London (Gatwick)  |
-| 2023-03-12 09:20:00 | FR 112         |   88.12 | DUB      | Dublin       | LGW           | London (Gatwick)  |
-| 2023-03-12 11:30:00 | FR 122         |  120.37 | DUB      | Dublin       | LGW           | London (Gatwick)  |
-| ...                 |                |         |          |              |               |                   |
+| departureTime       | flightNumber   |   price | currency | origin   | originFull   | destination   | destinationFull   |
+|---------------------|----------------|---------|----------|----------|--------------|---------------|-------------------|
+| 2023-03-12 06:25:00 | FR 114         |   61.99 | EUR      | DUB      | Dublin       | LGW           | London (Gatwick)  |
+| 2023-03-12 09:20:00 | FR 112         |   88.12 | EUR      | DUB      | Dublin       | LGW           | London (Gatwick)  |
+| 2023-03-12 11:30:00 | FR 122         |  120.37 | EUR      | DUB      | Dublin       | LGW           | London (Gatwick)  |
+| ...                 |                |         | EUR      |          |              |               |                   |
 
 
 and
 
-| departureTime       | flightNumber   |   price | origin   | originFull   | destination   | destinationFull   |
-|---------------------|----------------|---------|----------|--------------|---------------|-------------------|
-| 2023-03-12 06:25:00 | FR 114         |   61.99 | DUB      | Dublin       | LGW           | LON               |
-| 2023-03-12 06:35:00 | FR 202         |   65.09 | DUB      | Dublin       | STN           | LON               |
-| 2023-03-12 07:10:00 | FR 342         |   65.09 | DUB      | Dublin       | LTN           | LON               |
-| 2023-03-12 08:20:00 | FR 206         |  102.09 | DUB      | Dublin       | STN           | LON               |
-| ...                 |                |         |          |              |               |                   |
+| departureTime       | flightNumber   |   price | currency | origin   | originFull   | destination   | destinationFull   |
+|---------------------|----------------|---------|----------|----------|--------------|---------------|-------------------|
+| 2023-03-12 06:25:00 | FR 114         |   61.99 | EUR      | DUB      | Dublin       | LGW           | LON               |
+| 2023-03-12 06:35:00 | FR 202         |   65.09 | EUR      | DUB      | Dublin       | STN           | LON               |
+| 2023-03-12 07:10:00 | FR 342         |   65.09 | EUR      | DUB      | Dublin       | LTN           | LON               |
+| 2023-03-12 08:20:00 | FR 206         |  102.09 | EUR      | DUB      | Dublin       | STN           | LON               |
+| ...                 |                |         |          |          |              |               |                   |
```

### Comparing `ryanair-py-2.1.0/ryanair/airport_utils.py` & `ryanair-py-2.2.0/ryanair/airport_utils.py`

 * *Files identical despite different names*

### Comparing `ryanair-py-2.1.0/ryanair/airports.csv` & `ryanair-py-2.2.0/ryanair/airports.csv`

 * *Files identical despite different names*

### Comparing `ryanair-py-2.1.0/ryanair/ryanair.py` & `ryanair-py-2.2.0/ryanair/ryanair.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,35 +2,39 @@
 This module allows you to retrieve either
 1) the cheapest flights, with or without return flights, within a fixed set of dates.
 or
 2) all available flights between two locations, on a given date
 This is done directly through Ryanair's API, and does not require an API key.
 """
 import logging
-from typing import Union
+from datetime import datetime, date, time
+from typing import Union, Optional
 
 import backoff
 import requests
-from datetime import datetime, date, time
-from time import sleep
-
 from deprecated import deprecated
 
 from ryanair.types import Flight, Trip
 
-logging.basicConfig(level=logging.INFO,
-                    format='%(asctime)s.%(msecs)03d %(levelname)s:%(message)s', datefmt="%m/%d/%Y %I:%M:%S")
+logger = logging.getLogger("ryanair")
+logger.setLevel(logging.INFO)
+
+console_handler = logging.StreamHandler()
+formatter = logging.Formatter('%(asctime)s.%(msecs)03d %(levelname)s:%(message)s', datefmt="%Y-%m-%d %I:%M:%S")
+
+console_handler.setFormatter(formatter)
+logger.addHandler(console_handler)
 
 
 # noinspection PyBroadException
 class Ryanair:
     BASE_SERVICES_API_URL = "https://services-api.ryanair.com/farfnd/v4/"
     BASE_AVAILABILITY_API_URL = "https://www.ryanair.com/api/booking/v4/"
 
-    def __init__(self, currency):
+    def __init__(self, currency: Optional[str] = None):
         self.currency = currency
 
         self._num_queries = 0
 
     @deprecated(version="2.0.0", reason="deprecated in favour of get_cheapest_flights", action="once")
     def get_flights(self, airport, date_from, date_to, destination_country=None):
         return self.get_cheapest_flights(airport, date_from, date_to, destination_country)
@@ -42,35 +46,39 @@
         return self.get_cheapest_return_flights(source_airport, date_from, date_to,
                                                 return_date_from, return_date_to, destination_country)
 
     def get_cheapest_flights(self, airport, date_from, date_to, destination_country=None,
                              custom_params=None,
                              departure_time_from: Union[str, time] = "00:00",
                              departure_time_to: Union[str, time] = "23:59",
+                             max_price: int = None
                              ):
         query_url = ''.join((Ryanair.BASE_SERVICES_API_URL,
                              "oneWayFares"))
 
         params = {
             "departureAirportIataCode": airport,
             "outboundDepartureDateFrom": self._format_date_for_api(date_from),
             "outboundDepartureDateTo": self._format_date_for_api(date_to),
-            "currency": self.currency,
             "outboundDepartureTimeFrom": self._format_time_for_api(departure_time_from),
             "outboundDepartureTimeTo": self._format_time_for_api(departure_time_to)
         }
+        if self.currency:
+            params['currency'] = self.currency
         if destination_country:
             params['arrivalCountryCode'] = destination_country
+        if max_price:
+            params['priceValueTo'] = max_price
         if custom_params:
             params.update(custom_params)
 
         try:
             response = self._retryable_query(query_url, params)["fares"]
         except Exception:
-            logging.exception(f"Failed to parse response when querying {query_url}")
+            logger.exception(f"Failed to parse response when querying {query_url}")
             return []
 
         if response:
             return [self._parse_cheapest_flight(flight['outbound']) for flight in response]
 
         return []
 
@@ -78,14 +86,15 @@
                                     return_date_from, return_date_to,
                                     destination_country=None,
                                     custom_params=None,
                                     outbound_departure_time_from: Union[str, time] = "00:00",
                                     outbound_departure_time_to: Union[str, time] = "23:59",
                                     inbound_departure_time_from: Union[str, time] = "00:00",
                                     inbound_departure_time_to: Union[str, time] = "23:59",
+                                    max_price: int = None
                                     ):
         query_url = ''.join((Ryanair.BASE_SERVICES_API_URL,
                              "roundTripFares"))
 
         params = {
             "departureAirportIataCode": source_airport,
             "outboundDepartureDateFrom": self._format_date_for_api(date_from),
@@ -96,21 +105,23 @@
             "outboundDepartureTimeFrom": self._format_time_for_api(outbound_departure_time_from),
             "outboundDepartureTimeTo": self._format_time_for_api(outbound_departure_time_to),
             "inboundDepartureTimeFrom": self._format_time_for_api(inbound_departure_time_from),
             "inboundDepartureTimeTo": self._format_time_for_api(inbound_departure_time_to)
         }
         if destination_country:
             params['arrivalCountryCode'] = destination_country
+        if max_price:
+            params['priceValueTo'] = max_price
         if custom_params:
             params.update(custom_params)
 
         try:
             response = self._retryable_query(query_url, params)["fares"]
         except Exception as e:
-            logging.exception(f"Failed to parse response when querying {query_url}")
+            logger.exception(f"Failed to parse response when querying {query_url}")
             return []
 
         if response:
             return [self._parse_cheapest_return_flights_as_trip(trip["outbound"], trip["inbound"])
                     for trip in response]
         else:
             return []
@@ -149,64 +160,75 @@
             # "RoundTrip": false,
         }
 
         if custom_params:
             params.update(custom_params)
 
         try:
-            response = self._retryable_query(query_url, params)["trips"][0]
-            flights = response['dates'][0]['flights']
+            response = self._retryable_query(query_url, params)
+            currency = response["currency"]
+            trip = response["trips"][0]
+            flights = trip['dates'][0]['flights']
             if flights:
+                if self.currency and self.currency != currency:
+                    logger.warning(f"Configured to fetch fares in {self.currency} but availability API doesn't support"
+                                   f" specifying the currency, so it responded with fares in {currency}")
+
                 return [self._parse_all_flights_availability_result_as_flight(flight,
-                                                                              response['originName'],
-                                                                              response['destinationName'])
+                                                                              trip['originName'],
+                                                                              trip['destinationName'],
+                                                                              currency)
                         for flight in flights]
         except Exception:
-            logging.exception(f"Failed to parse response when querying {query_url}")
+            logger.exception(f"Failed to parse response when querying {query_url}")
             return []
 
     @staticmethod
     def _on_query_error(e):
-        logging.exception(f"Gave up retrying query, last exception was {e}")
+        logger.exception(f"Gave up retrying query, last exception was {e}")
 
-    @backoff.on_exception(backoff.expo, Exception, max_tries=5, logger=logging.getLogger(), on_giveup=_on_query_error,
+    @backoff.on_exception(backoff.expo, Exception, max_tries=5, logger=logger, on_giveup=_on_query_error,
                           raise_on_giveup=False)
     def _retryable_query(self, url, params):
         self._num_queries += 1
 
         return requests.get(url, params=params).json()
 
-    @staticmethod
-    def _parse_cheapest_flight(flight):
+    def _parse_cheapest_flight(self, flight):
+        currency = flight['price']['currencyCode']
+        if self.currency and self.currency != currency:
+            logger.warning(f"Requested cheapest flights in {self.currency} but API responded with fares in {currency}")
         return Flight(
             origin=flight['departureAirport']['iataCode'],
             originFull=', '.join((flight['departureAirport']['name'], flight['departureAirport']['countryName'])),
             destination=flight['arrivalAirport']['iataCode'],
             destinationFull=', '.join((flight['arrivalAirport']['name'], flight['arrivalAirport']['countryName'])),
             departureTime=datetime.fromisoformat(flight['departureDate']),
             flightNumber=f"{flight['flightNumber'][:2]} {flight['flightNumber'][2:]}",
-            price=flight['price']['value']
+            price=flight['price']['value'],
+            currency=currency
         )
 
     def _parse_cheapest_return_flights_as_trip(self, outbound, inbound):
         outbound = self._parse_cheapest_flight(outbound)
         inbound = self._parse_cheapest_flight(inbound)
 
         return Trip(
             outbound=outbound,
             inbound=inbound,
             totalPrice=inbound.price + outbound.price
         )
 
     @staticmethod
-    def _parse_all_flights_availability_result_as_flight(response, origin_full, destination_full):
+    def _parse_all_flights_availability_result_as_flight(response, origin_full, destination_full, currency):
         return Flight(departureTime=datetime.fromisoformat(response['time'][0]),
                       flightNumber=response['flightNumber'],
                       price=response['regularFare']['fares'][0]['amount'] if response['faresLeft'] != 0 else float(
                           'inf'),
+                      currency=currency,
                       origin=response['segments'][0]['origin'],
                       originFull=origin_full,
                       destination=response['segments'][0]['destination'],
                       destinationFull=destination_full
                       )
 
     @staticmethod
```

### Comparing `ryanair-py-2.1.0/ryanair_py.egg-info/PKG-INFO` & `ryanair-py-2.2.0/ryanair_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryanair-py
-Version: 2.1.0
+Version: 2.2.0
 Summary: A module which allows you to retrieve data about the cheapest one-way and return flights in a date range, or all available flights on a given day for a given route.
 Home-page: https://github.com/cohaolain/ryanair-py
 Author: Ciarán Ó hAoláin
 Author-email: ciaran@cohaolain.ie
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -23,79 +23,85 @@
 ```
 pip install ryanair-py
 ```
 ## Usage
 To create an instance:
 ```python
 from ryanair import Ryanair
-api = Ryanair("EUR")  # Euro currency, so could also be GBP etc. also
+
+# You can set a currency at the API instance level, so could also be GBP etc. also.
+# Note that this may not *always* be respected by the API, so always check the currency returned matches
+# your expectation. For example, the underlying API for get_all_flights does not support this.
+api = Ryanair("EUR")
 ```
 ### Get the cheapest one-way flights
 Get the cheapest flights from a given origin airport (returns at most 1 flight to each destination).
 ```python
 from datetime import datetime, timedelta
 from ryanair import Ryanair
 from ryanair.types import Flight
 
-api = Ryanair("EUR")  # Euro currency, so could also be GBP etc. also
+api = Ryanair(currency="EUR")  # Euro currency, so could also be GBP etc. also
 tomorrow = datetime.today().date() + timedelta(days=1)
 
 flights = api.get_cheapest_flights("DUB", tomorrow, tomorrow + timedelta(days=1))
 
 # Returns a list of Flight namedtuples
 flight: Flight = flights[0]
-print(flight)  # Flight(departureTime=datetime.datetime(2023, 3, 12, 17, 0), flightNumber='FR9717', price=31.99, origin='DUB', originFull='Dublin, Ireland', destination='GOA', destinationFull='Genoa, Italy')
+print(flight)  # Flight(departureTime=datetime.datetime(2023, 3, 12, 17, 0), flightNumber='FR9717', price=31.99, currency='EUR' origin='DUB', originFull='Dublin, Ireland', destination='GOA', destinationFull='Genoa, Italy')
 print(flight.price)  # 9.78
 ```
 ### Get the cheapest return trips (outbound and inbound)
 ```python
 from datetime import datetime, timedelta
 from ryanair import Ryanair
 
-api = Ryanair("EUR")  # Euro currency, so could also be GBP etc. also
+api = Ryanair(currency="EUR")  # Euro currency, so could also be GBP etc. also
 tomorrow = datetime.today().date() + timedelta(days=1)
 tomorrow_1 = tomorrow + timedelta(days=1)
 
 trips = api.get_cheapest_return_flights("DUB", tomorrow, tomorrow, tomorrow_1, tomorrow_1)
-print(trips[0])  # Trip(totalPrice=85.31, outbound=Flight(departureTime=datetime.datetime(2023, 3, 12, 7, 30), flightNumber='FR5437', price=49.84, origin='DUB', originFull='Dublin, Ireland', destination='EMA', destinationFull='East Midlands, United Kingdom'), inbound=Flight(departureTime=datetime.datetime(2023, 3, 13, 7, 45), flightNumber='FR5438', price=35.47, origin='EMA', originFull='East Midlands, United Kingdom', destination='DUB', destinationFull='Dublin, Ireland'))
+print(trips[0])  # Trip(totalPrice=85.31, outbound=Flight(departureTime=datetime.datetime(2023, 3, 12, 7, 30), flightNumber='FR5437', price=49.84, currency='EUR', origin='DUB', originFull='Dublin, Ireland', destination='EMA', destinationFull='East Midlands, United Kingdom'), inbound=Flight(departureTime=datetime.datetime(2023, 3, 13, 7, 45), flightNumber='FR5438', price=35.47, origin='EMA', originFull='East Midlands, United Kingdom', destination='DUB', destinationFull='Dublin, Ireland'))
 ```
 
 ### Get all available flights between two airports
 E.g. get all available flights from Dublin to London Gatwick, or London, tomorrow:
 ```python
 from datetime import datetime, timedelta
 
 from ryanair import Ryanair
 from tabulate import tabulate
 
-api = Ryanair("EUR")
+# We don't need to specify a currency if we're only using `get_all_flights`, as this API doesn't support currency 
+# conversion. It will always return dares denominated in the currency of the departure country.  
+api = Ryanair()
 tomorrow = datetime.today().date() + timedelta(days=1)
 
 flights = api.get_all_flights("DUB", tomorrow, "LGW")
 print(tabulate(flights, headers="keys", tablefmt="github"))
 
 # We can even expand it to include all vaguely-London airports:
 flights = api.get_all_flights("DUB", tomorrow, "LON", destination_is_mac=True)
 print(tabulate(flights, headers="keys", tablefmt="github"))
 ```
 
 This prints the following:
 
-| departureTime       | flightNumber   |   price | origin   | originFull   | destination   | destinationFull   |
-|---------------------|----------------|---------|----------|--------------|---------------|-------------------|
-| 2023-03-12 06:25:00 | FR 114         |   61.99 | DUB      | Dublin       | LGW           | London (Gatwick)  |
-| 2023-03-12 09:20:00 | FR 112         |   88.12 | DUB      | Dublin       | LGW           | London (Gatwick)  |
-| 2023-03-12 11:30:00 | FR 122         |  120.37 | DUB      | Dublin       | LGW           | London (Gatwick)  |
-| ...                 |                |         |          |              |               |                   |
+| departureTime       | flightNumber   |   price | currency | origin   | originFull   | destination   | destinationFull   |
+|---------------------|----------------|---------|----------|----------|--------------|---------------|-------------------|
+| 2023-03-12 06:25:00 | FR 114         |   61.99 | EUR      | DUB      | Dublin       | LGW           | London (Gatwick)  |
+| 2023-03-12 09:20:00 | FR 112         |   88.12 | EUR      | DUB      | Dublin       | LGW           | London (Gatwick)  |
+| 2023-03-12 11:30:00 | FR 122         |  120.37 | EUR      | DUB      | Dublin       | LGW           | London (Gatwick)  |
+| ...                 |                |         | EUR      |          |              |               |                   |
 
 
 and
 
-| departureTime       | flightNumber   |   price | origin   | originFull   | destination   | destinationFull   |
-|---------------------|----------------|---------|----------|--------------|---------------|-------------------|
-| 2023-03-12 06:25:00 | FR 114         |   61.99 | DUB      | Dublin       | LGW           | LON               |
-| 2023-03-12 06:35:00 | FR 202         |   65.09 | DUB      | Dublin       | STN           | LON               |
-| 2023-03-12 07:10:00 | FR 342         |   65.09 | DUB      | Dublin       | LTN           | LON               |
-| 2023-03-12 08:20:00 | FR 206         |  102.09 | DUB      | Dublin       | STN           | LON               |
-| ...                 |                |         |          |              |               |                   |
+| departureTime       | flightNumber   |   price | currency | origin   | originFull   | destination   | destinationFull   |
+|---------------------|----------------|---------|----------|----------|--------------|---------------|-------------------|
+| 2023-03-12 06:25:00 | FR 114         |   61.99 | EUR      | DUB      | Dublin       | LGW           | LON               |
+| 2023-03-12 06:35:00 | FR 202         |   65.09 | EUR      | DUB      | Dublin       | STN           | LON               |
+| 2023-03-12 07:10:00 | FR 342         |   65.09 | EUR      | DUB      | Dublin       | LTN           | LON               |
+| 2023-03-12 08:20:00 | FR 206         |  102.09 | EUR      | DUB      | Dublin       | STN           | LON               |
+| ...                 |                |         |          |          |              |               |                   |
```

### Comparing `ryanair-py-2.1.0/setup.py` & `ryanair-py-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='ryanair-py',
-      version='2.1.0',
+      version='2.2.0',
       description='A module which allows you to retrieve data about the cheapest one-way and return flights '
                   'in a date range, or all available flights on a given day for a given route.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Ciarán Ó hAoláin',
       author_email='ciaran@cohaolain.ie',
       url='https://github.com/cohaolain/ryanair-py',
```


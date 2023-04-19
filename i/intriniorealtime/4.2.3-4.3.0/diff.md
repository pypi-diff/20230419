# Comparing `tmp/intriniorealtime-4.2.3.tar.gz` & `tmp/intriniorealtime-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/intriniorealtime-4.2.3.tar", last modified: Tue Jan 31 23:34:33 2023, max compression
+gzip compressed data, was "dist/intriniorealtime-4.3.0.tar", last modified: Wed Apr 19 20:03:10 2023, max compression
```

## Comparing `intriniorealtime-4.2.3.tar` & `intriniorealtime-4.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-01-31 23:34:33.000000 intriniorealtime-4.2.3/
--rw-r--r--   0 shawn      (503) staff       (20)     9073 2023-01-31 23:34:33.000000 intriniorealtime-4.2.3/PKG-INFO
--rw-r--r--   0 shawn      (503) staff       (20)    35141 2022-01-04 22:35:51.000000 intriniorealtime-4.2.3/LICENSE
--rw-r--r--   0 shawn      (503) staff       (20)       65 2022-01-04 22:35:51.000000 intriniorealtime-4.2.3/MANIFEST.in
--rw-r--r--   0 shawn      (503) staff       (20)     6849 2023-01-24 23:23:44.000000 intriniorealtime-4.2.3/README.md
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-01-31 23:34:33.000000 intriniorealtime-4.2.3/intriniorealtime/
--rw-r--r--   0 shawn      (503) staff       (20)    14944 2023-01-31 23:34:15.000000 intriniorealtime-4.2.3/intriniorealtime/client.py
--rw-r--r--   0 shawn      (503) staff       (20)        0 2022-01-04 22:35:51.000000 intriniorealtime-4.2.3/intriniorealtime/__init__.py
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-01-31 23:34:33.000000 intriniorealtime-4.2.3/intriniorealtime.egg-info/
--rw-r--r--   0 shawn      (503) staff       (20)     9073 2023-01-31 23:34:33.000000 intriniorealtime-4.2.3/intriniorealtime.egg-info/PKG-INFO
--rw-r--r--   0 shawn      (503) staff       (20)      303 2023-01-31 23:34:33.000000 intriniorealtime-4.2.3/intriniorealtime.egg-info/SOURCES.txt
--rw-r--r--   0 shawn      (503) staff       (20)       56 2023-01-31 23:34:33.000000 intriniorealtime-4.2.3/intriniorealtime.egg-info/requires.txt
--rw-r--r--   0 shawn      (503) staff       (20)       17 2023-01-31 23:34:33.000000 intriniorealtime-4.2.3/intriniorealtime.egg-info/top_level.txt
--rw-r--r--   0 shawn      (503) staff       (20)        1 2023-01-31 23:34:33.000000 intriniorealtime-4.2.3/intriniorealtime.egg-info/dependency_links.txt
--rw-r--r--   0 shawn      (503) staff       (20)      963 2023-01-31 23:34:15.000000 intriniorealtime-4.2.3/setup.py
--rw-r--r--   0 shawn      (503) staff       (20)       79 2023-01-31 23:34:33.000000 intriniorealtime-4.2.3/setup.cfg
+drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/
+-rw-r--r--   0 shawn      (503) staff       (20)     9401 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/PKG-INFO
+-rw-r--r--   0 shawn      (503) staff       (20)    35141 2022-01-04 22:35:51.000000 intriniorealtime-4.3.0/LICENSE
+-rw-r--r--   0 shawn      (503) staff       (20)       65 2022-01-04 22:35:51.000000 intriniorealtime-4.3.0/MANIFEST.in
+-rw-r--r--   0 shawn      (503) staff       (20)     7113 2023-04-19 19:47:24.000000 intriniorealtime-4.3.0/README.md
+drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/intriniorealtime/
+-rw-r--r--   0 shawn      (503) staff       (20)    15258 2023-04-19 19:54:13.000000 intriniorealtime-4.3.0/intriniorealtime/client.py
+-rw-r--r--   0 shawn      (503) staff       (20)        0 2022-01-04 22:35:51.000000 intriniorealtime-4.3.0/intriniorealtime/__init__.py
+drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/intriniorealtime.egg-info/
+-rw-r--r--   0 shawn      (503) staff       (20)     9401 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/intriniorealtime.egg-info/PKG-INFO
+-rw-r--r--   0 shawn      (503) staff       (20)      303 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/intriniorealtime.egg-info/SOURCES.txt
+-rw-r--r--   0 shawn      (503) staff       (20)       56 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/intriniorealtime.egg-info/requires.txt
+-rw-r--r--   0 shawn      (503) staff       (20)       17 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/intriniorealtime.egg-info/top_level.txt
+-rw-r--r--   0 shawn      (503) staff       (20)        1 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/intriniorealtime.egg-info/dependency_links.txt
+-rw-r--r--   0 shawn      (503) staff       (20)      963 2023-04-19 19:41:25.000000 intriniorealtime-4.3.0/setup.py
+-rw-r--r--   0 shawn      (503) staff       (20)       79 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/setup.cfg
```

### Comparing `intriniorealtime-4.2.3/PKG-INFO` & `intriniorealtime-4.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 Metadata-Version: 2.1
 Name: intriniorealtime
-Version: 4.2.3
+Version: 4.3.0
 Summary: Intrinio Python SDK for Real-Time Stock Prices
 Home-page: https://intrinio.com
 Author: Intrinio Python SDK for Real-Time Stock Prices
 Author-email: success@intrinio.com
 License: UNKNOWN
-Download-URL: https://github.com/intrinio/intrinio-realtime-python-sdk/archive/v4.2.3.tar.gz
+Download-URL: https://github.com/intrinio/intrinio-realtime-python-sdk/archive/v4.3.0.tar.gz
 Description: # intrinio realtime python sdk
         SDK for working with Intrinio's realtime Multi-Exchange prices feed.  Intrinio’s Multi-Exchange feed bridges the gap by merging real-time equity pricing from the IEX and MEMX exchanges. Get a comprehensive view with increased market volume and enjoy no exchange fees, no per-user requirements, no permissions or authorizations, and little to no paperwork.
         
         [Intrinio](https://intrinio.com/) provides real-time stock prices via a two-way WebSocket connection. To get started, [subscribe to a real-time data feed](https://intrinio.com/real-time-multi-exchange) and follow the instructions below.
         
         [Documentation for our legacy realtime client](https://github.com/intrinio/intrinio-realtime-python-sdk/tree/2.2.0)
         
         ## Requirements
         
         - Python 3.6
+        - You need https://pypi.org/project/websocket-client/, not https://pypi.org/project/websocket/.
+        
+        ## Docker
+        Add your API key to the example_app.py file, then
+        ```
+        docker compose build
+        docker compose run client
+        ```
         
         ## Features
         
         * Receive streaming, real-time price quotes (last trade, bid, ask)
         * Subscribe to updates from individual securities
         * Subscribe to updates for all securities
-        * Multiple sources of data - REALTIME or DELAYED_SIP
+        * Multiple sources of data - REALTIME or DELAYED_SIP or NASDAQ_BASIC
         
         ## Installation
         ```
         pip install intriniorealtime
         ```
         
         ## Example Usage
@@ -69,15 +77,15 @@
                 global ask_count
                 global backlog_count
                 while not self.stopped.wait(5):
                     print("trades: " + str(trade_count) + "; asks: " + str(ask_count) + "; bids: " + str(bid_count) + "; backlog: " + str(backlog_count))
         
         options = {
             'api_key': 'API_KEY_HERE',
-            'provider': 'REALTIME' # or 'DELAYED_SIP'
+            'provider': 'REALTIME' # or 'DELAYED_SIP' or 'NASDAQ_BASIC'
         }
         
         client = IntrinioRealtimeClient(options, on_trade, on_quote)
         client.join(['AAPL','GE','MSFT'])
         #client.join(['lobby'])
         client.connect()
         stopFlag = Event()
@@ -136,15 +144,15 @@
         
         ## Documentation
         
         ### Methods
         
         `client = IntrinioRealtimeClient(options)` - Creates an Intrinio Realtime client
         * **Parameter** `options.api_key`: Your Intrinio API Key
-        * **Parameter** `options.provider`: The real-time data provider to use ("REALTIME" or "DELAYED_SIP")
+        * **Parameter** `options.provider`: The real-time data provider to use ("REALTIME" or "DELAYED_SIP" or "NASDAQ_BASIC")
         * **Parameter** `options.on_quote(quote, backlog)`: A function that handles received quotes. `backlog` is an integer representing the approximate size of the queue of unhandled quote/trade events.
         * **Parameter** `options.on_trade(quote, backlog)`: A function that handles received trades. `backlog` is an integer representing the approximate size of the queue of unhandled quote/trade events.
         * **Parameter** `options.logger`: (optional) A Python Logger instance to use for logging
         
         ```python
         def on_quote(quote, backlog):
             print("QUOTE: " , quote, "BACKLOG LENGTH: ", backlog)
```

### Comparing `intriniorealtime-4.2.3/LICENSE` & `intriniorealtime-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `intriniorealtime-4.2.3/README.md` & `intriniorealtime-4.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,21 +4,29 @@
 [Intrinio](https://intrinio.com/) provides real-time stock prices via a two-way WebSocket connection. To get started, [subscribe to a real-time data feed](https://intrinio.com/real-time-multi-exchange) and follow the instructions below.
 
 [Documentation for our legacy realtime client](https://github.com/intrinio/intrinio-realtime-python-sdk/tree/2.2.0)
 
 ## Requirements
 
 - Python 3.6
+- You need https://pypi.org/project/websocket-client/, not https://pypi.org/project/websocket/.
+
+## Docker
+Add your API key to the example_app.py file, then
+```
+docker compose build
+docker compose run client
+```
 
 ## Features
 
 * Receive streaming, real-time price quotes (last trade, bid, ask)
 * Subscribe to updates from individual securities
 * Subscribe to updates for all securities
-* Multiple sources of data - REALTIME or DELAYED_SIP
+* Multiple sources of data - REALTIME or DELAYED_SIP or NASDAQ_BASIC
 
 ## Installation
 ```
 pip install intriniorealtime
 ```
 
 ## Example Usage
@@ -60,15 +68,15 @@
         global ask_count
         global backlog_count
         while not self.stopped.wait(5):
             print("trades: " + str(trade_count) + "; asks: " + str(ask_count) + "; bids: " + str(bid_count) + "; backlog: " + str(backlog_count))
 
 options = {
     'api_key': 'API_KEY_HERE',
-    'provider': 'REALTIME' # or 'DELAYED_SIP'
+    'provider': 'REALTIME' # or 'DELAYED_SIP' or 'NASDAQ_BASIC'
 }
 
 client = IntrinioRealtimeClient(options, on_trade, on_quote)
 client.join(['AAPL','GE','MSFT'])
 #client.join(['lobby'])
 client.connect()
 stopFlag = Event()
@@ -127,15 +135,15 @@
 
 ## Documentation
 
 ### Methods
 
 `client = IntrinioRealtimeClient(options)` - Creates an Intrinio Realtime client
 * **Parameter** `options.api_key`: Your Intrinio API Key
-* **Parameter** `options.provider`: The real-time data provider to use ("REALTIME" or "DELAYED_SIP")
+* **Parameter** `options.provider`: The real-time data provider to use ("REALTIME" or "DELAYED_SIP" or "NASDAQ_BASIC")
 * **Parameter** `options.on_quote(quote, backlog)`: A function that handles received quotes. `backlog` is an integer representing the approximate size of the queue of unhandled quote/trade events.
 * **Parameter** `options.on_trade(quote, backlog)`: A function that handles received trades. `backlog` is an integer representing the approximate size of the queue of unhandled quote/trade events.
 * **Parameter** `options.logger`: (optional) A Python Logger instance to use for logging
 
 ```python
 def on_quote(quote, backlog):
     print("QUOTE: " , quote, "BACKLOG LENGTH: ", backlog)
```

### Comparing `intriniorealtime-4.2.3/intriniorealtime/client.py` & `intriniorealtime-4.3.0/intriniorealtime/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 import sys
 import wsaccel
 
 SELF_HEAL_BACKOFFS = [10, 30, 60, 300, 600]
 HEARTBEAT_TIME = 20
 REALTIME = "REALTIME"
 DELAYED_SIP = "DELAYED_SIP"
+NASDAQ_BASIC = "NASDAQ_BASIC"
 MANUAL = "MANUAL"
-PROVIDERS = [REALTIME, MANUAL, DELAYED_SIP]
+PROVIDERS = [REALTIME, MANUAL, DELAYED_SIP, NASDAQ_BASIC]
 MAX_QUEUE_SIZE = 10000
 DEBUGGING = not (sys.gettrace() is None)
 
 
 class Quote:
     def __init__(self, symbol, type, price, size, timestamp):
         self.symbol = symbol
@@ -121,14 +122,16 @@
     def auth_url(self):
         auth_url = ""
 
         if self.provider == REALTIME:
             auth_url = "https://realtime-mx.intrinio.com/auth"
         elif self.provider == DELAYED_SIP:
             auth_url = "https://realtime-delayed-sip.intrinio.com/auth"
+        elif self.provider == NASDAQ_BASIC:
+            auth_url = "https://realtime-nasdaq-basic.intrinio.com/auth"
         elif self.provider == MANUAL:
             auth_url = "http://" + self.ipaddress + "/auth"
 
         if self.api_key:
             auth_url = self.api_auth_url(auth_url)
 
         return auth_url
@@ -142,14 +145,16 @@
         return auth_url + "api_key=" + self.api_key
 
     def websocket_url(self):
         if self.provider == REALTIME:
             return "wss://realtime-mx.intrinio.com/socket/websocket?vsn=1.0.0&token=" + self.token
         elif self.provider == DELAYED_SIP:
             return "wss://realtime-delayed-sip.intrinio.com/socket/websocket?vsn=1.0.0&token=" + self.token
+        elif self.provider == NASDAQ_BASIC:
+            return "wss://realtime-nasdaq-basic.intrinio.com/socket/websocket?vsn=1.0.0&token=" + self.token
         elif self.provider == MANUAL:
             return "ws://" + self.ipaddress + "/socket/websocket?vsn=1.0.0&token=" + self.token
 
     def do_backoff(self):
         self.last_self_heal_backoff += 1
         i = min(self.last_self_heal_backoff, len(SELF_HEAL_BACKOFFS) - 1)
         backoff = SELF_HEAL_BACKOFFS[i]
@@ -179,15 +184,15 @@
         self.joined_channels = set()
 
         if self.ws:
             self.ws.close()
             time.sleep(1)
 
     def refresh_token(self):
-        headers = {'Client-Information': 'IntrinioPythonSDKv4.2.3'}
+        headers = {'Client-Information': 'IntrinioPythonSDKv4.3.0'}
         if self.api_key:
             response = requests.get(self.auth_url(), headers=headers)
         else:
             response = requests.get(self.auth_url(), auth=(self.username, self.password), headers=headers)
 
         if response.status_code != 200:
             raise RuntimeError("Auth failed")
```

### Comparing `intriniorealtime-4.2.3/intriniorealtime.egg-info/PKG-INFO` & `intriniorealtime-4.3.0/intriniorealtime.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 Metadata-Version: 2.1
 Name: intriniorealtime
-Version: 4.2.3
+Version: 4.3.0
 Summary: Intrinio Python SDK for Real-Time Stock Prices
 Home-page: https://intrinio.com
 Author: Intrinio Python SDK for Real-Time Stock Prices
 Author-email: success@intrinio.com
 License: UNKNOWN
-Download-URL: https://github.com/intrinio/intrinio-realtime-python-sdk/archive/v4.2.3.tar.gz
+Download-URL: https://github.com/intrinio/intrinio-realtime-python-sdk/archive/v4.3.0.tar.gz
 Description: # intrinio realtime python sdk
         SDK for working with Intrinio's realtime Multi-Exchange prices feed.  Intrinio’s Multi-Exchange feed bridges the gap by merging real-time equity pricing from the IEX and MEMX exchanges. Get a comprehensive view with increased market volume and enjoy no exchange fees, no per-user requirements, no permissions or authorizations, and little to no paperwork.
         
         [Intrinio](https://intrinio.com/) provides real-time stock prices via a two-way WebSocket connection. To get started, [subscribe to a real-time data feed](https://intrinio.com/real-time-multi-exchange) and follow the instructions below.
         
         [Documentation for our legacy realtime client](https://github.com/intrinio/intrinio-realtime-python-sdk/tree/2.2.0)
         
         ## Requirements
         
         - Python 3.6
+        - You need https://pypi.org/project/websocket-client/, not https://pypi.org/project/websocket/.
+        
+        ## Docker
+        Add your API key to the example_app.py file, then
+        ```
+        docker compose build
+        docker compose run client
+        ```
         
         ## Features
         
         * Receive streaming, real-time price quotes (last trade, bid, ask)
         * Subscribe to updates from individual securities
         * Subscribe to updates for all securities
-        * Multiple sources of data - REALTIME or DELAYED_SIP
+        * Multiple sources of data - REALTIME or DELAYED_SIP or NASDAQ_BASIC
         
         ## Installation
         ```
         pip install intriniorealtime
         ```
         
         ## Example Usage
@@ -69,15 +77,15 @@
                 global ask_count
                 global backlog_count
                 while not self.stopped.wait(5):
                     print("trades: " + str(trade_count) + "; asks: " + str(ask_count) + "; bids: " + str(bid_count) + "; backlog: " + str(backlog_count))
         
         options = {
             'api_key': 'API_KEY_HERE',
-            'provider': 'REALTIME' # or 'DELAYED_SIP'
+            'provider': 'REALTIME' # or 'DELAYED_SIP' or 'NASDAQ_BASIC'
         }
         
         client = IntrinioRealtimeClient(options, on_trade, on_quote)
         client.join(['AAPL','GE','MSFT'])
         #client.join(['lobby'])
         client.connect()
         stopFlag = Event()
@@ -136,15 +144,15 @@
         
         ## Documentation
         
         ### Methods
         
         `client = IntrinioRealtimeClient(options)` - Creates an Intrinio Realtime client
         * **Parameter** `options.api_key`: Your Intrinio API Key
-        * **Parameter** `options.provider`: The real-time data provider to use ("REALTIME" or "DELAYED_SIP")
+        * **Parameter** `options.provider`: The real-time data provider to use ("REALTIME" or "DELAYED_SIP" or "NASDAQ_BASIC")
         * **Parameter** `options.on_quote(quote, backlog)`: A function that handles received quotes. `backlog` is an integer representing the approximate size of the queue of unhandled quote/trade events.
         * **Parameter** `options.on_trade(quote, backlog)`: A function that handles received trades. `backlog` is an integer representing the approximate size of the queue of unhandled quote/trade events.
         * **Parameter** `options.logger`: (optional) A Python Logger instance to use for logging
         
         ```python
         def on_quote(quote, backlog):
             print("QUOTE: " , quote, "BACKLOG LENGTH: ", backlog)
```

### Comparing `intriniorealtime-4.2.3/setup.py` & `intriniorealtime-4.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
     name = 'intriniorealtime',
     packages = ['intriniorealtime'],
-    version = '4.2.3',
+    version = '4.3.0',
     author = 'Intrinio Python SDK for Real-Time Stock Prices',
     author_email = 'success@intrinio.com',
     url = 'https://intrinio.com',
     description = 'Intrinio Python SDK for Real-Time Stock Prices',
     long_description = readme(),
     long_description_content_type = 'text/markdown',
     install_requires = ['requests>=2.26.0','websocket-client>=1.2.1','wsaccel>=0.6.3'],
     python_requires = '~=3.6',
-    download_url = 'https://github.com/intrinio/intrinio-realtime-python-sdk/archive/v4.2.3.tar.gz',
+    download_url = 'https://github.com/intrinio/intrinio-realtime-python-sdk/archive/v4.3.0.tar.gz',
     keywords = ['realtime','stock prices','intrinio','stock market','stock data','financial'],
     classifiers = [
         'Intended Audience :: Financial and Insurance Industry',
         'Topic :: Office/Business :: Financial :: Investment'
     ]
 )
```


# Comparing `tmp/dnptools-0.0.3.tar.gz` & `tmp/dnptools-0.0.4.tar.gz`

## Comparing `dnptools-0.0.3.tar` & `dnptools-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 dnptools-0.0.3/.github/workflows/build_and_test_package.yml
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 dnptools-0.0.3/.github/workflows/publish_conda_package.yml
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 dnptools-0.0.3/.github/workflows/publish_pypi_package.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dnptools-0.0.3/conda/environment.yml
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dnptools-0.0.3/conda/meta.yaml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dnptools-0.0.3/src/dnptools/.gitignore
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 dnptools-0.0.3/src/dnptools/__init__.py
--rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 dnptools-0.0.3/src/dnptools/scoringservice.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 dnptools-0.0.3/test/test_scoringserver.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 dnptools-0.0.3/.gitignore
--rw-r--r--   0        0        0    32386 2020-02-02 00:00:00.000000 dnptools-0.0.3/LICENSE
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 dnptools-0.0.3/README.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 dnptools-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 dnptools-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 dnptools-0.0.4/DEVELOPERS_MANNUAL.md
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 dnptools-0.0.4/.github/workflows/build_and_test_package.yml
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 dnptools-0.0.4/.github/workflows/publish_conda_package.yml
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 dnptools-0.0.4/.github/workflows/publish_pypi_package.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dnptools-0.0.4/conda/environment.yml
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dnptools-0.0.4/conda/meta.yaml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dnptools-0.0.4/src/dnptools/.gitignore
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 dnptools-0.0.4/src/dnptools/__init__.py
+-rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 dnptools-0.0.4/src/dnptools/scoringservice.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 dnptools-0.0.4/test/test_scoringserver.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 dnptools-0.0.4/.gitignore
+-rw-r--r--   0        0        0    32386 2020-02-02 00:00:00.000000 dnptools-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 dnptools-0.0.4/README.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 dnptools-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 dnptools-0.0.4/PKG-INFO
```

### Comparing `dnptools-0.0.3/.github/workflows/build_and_test_package.yml` & `dnptools-0.0.4/.github/workflows/build_and_test_package.yml`

 * *Files identical despite different names*

### Comparing `dnptools-0.0.3/.github/workflows/publish_conda_package.yml` & `dnptools-0.0.4/.github/workflows/publish_conda_package.yml`

 * *Files identical despite different names*

### Comparing `dnptools-0.0.3/.github/workflows/publish_pypi_package.yml` & `dnptools-0.0.4/.github/workflows/publish_pypi_package.yml`

 * *Files identical despite different names*

### Comparing `dnptools-0.0.3/conda/meta.yaml` & `dnptools-0.0.4/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `dnptools-0.0.3/src/dnptools/scoringservice.py` & `dnptools-0.0.4/src/dnptools/scoringservice.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,25 +20,35 @@
 import socket
 import sys
 import json
 import socketserver
 import time
 from threading import Thread
 from typing import Tuple
+import logging
 
 MY_NAME = "scoringservice"
 
 
 # NB: the strings defined here are part of a convention.
 JSON_KEY_SMILES = 'SMILES'
 JSON_KEY_SCORE = 'SCORE'
 JSON_KEY_ERROR = 'ERROR'
 
 SERVER_START_MAX_TIME = 5  # seconds
 
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.WARNING)
+log_stream_handler = logging.StreamHandler(sys.stdout)
+log_stream_handler.setLevel(logging.DEBUG)
+log_formatter = logging.Formatter(
+    "%(name)s %(asctime)s %(levelname)s %(message)s")
+log_stream_handler.setFormatter(log_formatter)
+logger.addHandler(log_stream_handler)
+
 
 class ScoreError(Exception):
     """Formats and exception as a JSON object adhering to DENOPTIM's convention.
 
     The JSON format is used to communicate any result to the client waiting for
     an answer, i.e., waiting for a score. If an exception occurs, we must
     communicate that the score cannot be produced and why. This method creates
@@ -79,45 +89,52 @@
     port : int
         the port number where the server should accept requests. By default,
         i.e., with a value of 0, we search for an available port.
     """
     # Find available port: we assume it stays available for as long as it takes
     # to start the server.
     if port == 0:
+        logger.debug('Searching for an available port')
         sock = socket.socket()
         sock.bind((host, 0))
         port = sock.getsockname()[1]
+        logger.debug(f'Port {port} is available')
         sock.close()
 
     # Try to start the server in another thread
     serverThread = Thread(target=__run_server, args=[scoring_function,
                                                      host, port])
+
+    logger.debug('Starting server thread')
     serverThread.start()
 
     # Verify the server is up before returning
     sock2 = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     door_is_closed = True
     start_time = time.time()
     waited_time = 0
     while door_is_closed and (waited_time < SERVER_START_MAX_TIME):
         response = sock2.connect_ex((host, port))
+        logger.debug(f"Verifying that server is up and running:"
+                     f" waited {waited_time}")
         if response == 0:
             door_is_closed = False
         else:
             time.sleep(1)
             waited_time = time.time() - start_time
 
     if door_is_closed:
         # noinspection PyBroadException
         try:
             stop((host, port))
         except Exception:
             pass
         raise Exception('Max time for server startup reached. Abandoning.')
 
+    logger.debug(f"Server started at {host}:{port}")
     return host, port
 
 
 def __run_server(scoring_function, host: str, port: int):
     """Start the server and keeps it running forever.
 
     Parameters
@@ -146,32 +163,38 @@
     ----------
     scoring_function :
         The function the handler should use to calculate the score for a given
         request."""
     class ScoreRequestHandler(socketserver.StreamRequestHandler):
         def handle(self):
             message = self.rfile.read().decode('utf8')
+            logger.debug(f"Handling request {message}")
             if 'shutdown' in message:
+                logger.debug(f"Shutting down server upon JSON request")
                 self.server.shutdown()
                 return
+            if '' == message:
+                logger.debug("Received empty request")
+                return
             try:
                 json_msg = json.loads(message)
             except json.decoder.JSONDecodeError as e:
-                return
-                raise ScoreError(f"Invalid JSON: {e}")
+                raise ScoreError(f"Invalid JSON '{message}': {e}")
             answer = ''
             try:
                 score = scoring_function(json_msg)
+                logger.debug(f"Score is {score}")
                 answer = json.dumps({
                     JSON_KEY_SCORE: score,
                 })
             except ScoreError as e:
                 print('Error:', e, file=sys.stderr)
                 answer = json.dumps(e.json_errmsg)
             finally:
+                logger.debug(f"Sending response  {answer}")
                 answer += '\n'
                 self.wfile.write(answer.encode('utf8'))
     return ScoreRequestHandler
 
 
 def stop(address: Tuple[str, int]):
     """Sends a shutdown request to the server to close it for good.
@@ -184,9 +207,7 @@
         number as an integer.
     """
     try:
         socket_connection = socket.create_connection(address)
         socket_connection.send('shutdown'.encode('utf8'))
     except Exception as e:
         raise Exception('Could not communicate with socket server.', e)
-
-
```

### Comparing `dnptools-0.0.3/test/test_scoringserver.py` & `dnptools-0.0.4/test/test_scoringserver.py`

 * *Files identical despite different names*

### Comparing `dnptools-0.0.3/LICENSE` & `dnptools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dnptools-0.0.3/README.md` & `dnptools-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 scoringservice.start(scoring_function, 'localhost', 3863)
 ```
 Note that `localhost` and port number 3863 are just parameters that can be choosen freely, but should be consistent with the settings of any client that wants to communicate with such server. The server is a threading server that can deal with multiple clients, like parallel threads running a fitness providing task each.
 When you do not need the scoring service any more, use the following to stop the server:
 ```
 scoringservice.stop('localhost',3863)
 ```
+Logging can be controlled as follows:
+```
+scoringservice.logger.setLevel(logging.DEBUG)
+```
 
 ## Install
 The package is available on <a href="https://pypi.org/project/dnptools/">pypi</a> and <a href="https://anaconda.org/denoptim-project/dnptools">anaconda</a>, so install it with 
 ```
 pip install dnptools
 ```
 or
```

### Comparing `dnptools-0.0.3/PKG-INFO` & `dnptools-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnptools
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python utilities for working with DENOPTIM (https://github.com/denoptim-project/DENOPTIM)
 Author: David Grellscheid, Marco Foscato, Marcello Costamagna
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -30,14 +30,18 @@
 scoringservice.start(scoring_function, 'localhost', 3863)
 ```
 Note that `localhost` and port number 3863 are just parameters that can be choosen freely, but should be consistent with the settings of any client that wants to communicate with such server. The server is a threading server that can deal with multiple clients, like parallel threads running a fitness providing task each.
 When you do not need the scoring service any more, use the following to stop the server:
 ```
 scoringservice.stop('localhost',3863)
 ```
+Logging can be controlled as follows:
+```
+scoringservice.logger.setLevel(logging.DEBUG)
+```
 
 ## Install
 The package is available on <a href="https://pypi.org/project/dnptools/">pypi</a> and <a href="https://anaconda.org/denoptim-project/dnptools">anaconda</a>, so install it with 
 ```
 pip install dnptools
 ```
 or
```


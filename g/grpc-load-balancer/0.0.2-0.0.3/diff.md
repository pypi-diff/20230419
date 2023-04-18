# Comparing `tmp/grpc_load_balancer-0.0.2.tar.gz` & `tmp/grpc_load_balancer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpc_load_balancer-0.0.2.tar", last modified: Mon Apr 10 08:03:13 2023, max compression
+gzip compressed data, was "grpc_load_balancer-0.0.3.tar", last modified: Tue Apr 18 22:34:55 2023, max compression
```

## Comparing `grpc_load_balancer-0.0.2.tar` & `grpc_load_balancer-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:03:13.452857 grpc_load_balancer-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-10 08:03:13.452857 grpc_load_balancer-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:03:13.448857 grpc_load_balancer-0.0.2/grpc_load_balancer/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/grpc_load_balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/grpc_load_balancer/connection_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/grpc_load_balancer/env_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/grpc_load_balancer/grpc_connection_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/grpc_load_balancer/lock_with_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/grpc_load_balancer/metrics_based_server_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:03:13.452857 grpc_load_balancer-0.0.2/grpc_load_balancer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-10 08:03:13.000000 grpc_load_balancer-0.0.2/grpc_load_balancer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-10 08:03:13.000000 grpc_load_balancer-0.0.2/grpc_load_balancer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:03:13.000000 grpc_load_balancer-0.0.2/grpc_load_balancer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 08:03:13.000000 grpc_load_balancer-0.0.2/grpc_load_balancer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 08:03:13.000000 grpc_load_balancer-0.0.2/grpc_load_balancer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:03:13.452857 grpc_load_balancer-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:03:13.452857 grpc_load_balancer-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-10 08:02:47.000000 grpc_load_balancer-0.0.2/tests/test_grpc_load_balancer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:55.907007 grpc_load_balancer-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-18 22:34:39.000000 grpc_load_balancer-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-18 22:34:55.907007 grpc_load_balancer-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-18 22:34:39.000000 grpc_load_balancer-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:55.907007 grpc_load_balancer-0.0.3/grpc_load_balancer/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-18 22:34:39.000000 grpc_load_balancer-0.0.3/grpc_load_balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-18 22:34:39.000000 grpc_load_balancer-0.0.3/grpc_load_balancer/connection_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-18 22:34:39.000000 grpc_load_balancer-0.0.3/grpc_load_balancer/env_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-18 22:34:39.000000 grpc_load_balancer-0.0.3/grpc_load_balancer/grpc_connection_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 22:34:39.000000 grpc_load_balancer-0.0.3/grpc_load_balancer/lock_with_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-18 22:34:39.000000 grpc_load_balancer-0.0.3/grpc_load_balancer/metrics_based_server_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:55.907007 grpc_load_balancer-0.0.3/grpc_load_balancer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-18 22:34:55.000000 grpc_load_balancer-0.0.3/grpc_load_balancer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-18 22:34:55.000000 grpc_load_balancer-0.0.3/grpc_load_balancer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:34:55.000000 grpc_load_balancer-0.0.3/grpc_load_balancer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 22:34:55.000000 grpc_load_balancer-0.0.3/grpc_load_balancer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 22:34:55.000000 grpc_load_balancer-0.0.3/grpc_load_balancer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 22:34:55.907007 grpc_load_balancer-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-18 22:34:39.000000 grpc_load_balancer-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:34:55.907007 grpc_load_balancer-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-18 22:34:39.000000 grpc_load_balancer-0.0.3/tests/test_grpc_load_balancer.py
```

### Comparing `grpc_load_balancer-0.0.2/LICENSE` & `grpc_load_balancer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `grpc_load_balancer-0.0.2/PKG-INFO` & `grpc_load_balancer-0.0.3/grpc_load_balancer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: grpc_load_balancer
-Version: 0.0.2
+Name: grpc-load-balancer
+Version: 0.0.3
 Summary: A small toolset to implement load balancing for gRPC services
 Home-page: https://github.com/flagman/grpc-load-balancer
 Author: Pavel Malay
 Author-email: flagmansupport@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 License-File: LICENSE
 
 # gRPC Load Balancer
 
 `grpc_load_balancer` is a Python package that allows you to easily configure and manage separate gRPC server and client instances using a metrics-based load balancing approach. This is useful when you have multiple services running and want to distribute the load efficiently among them. The package includes a connection forwarder, a metrics-based server finder, and a configuration loader.
 It implemetns the following design:
 
-<img src="imgs/design.jpg" width="50%" height="50%">
+<img src="https://github.com/flagman/grpc-load-balancer/blob/main/imgs/design.jpg?raw=true" width="50%" height="50%">
 
 
 
 ## Features
 
 - Forward connections from clients to gRPC servers.
 - Use Prometheus metrics to select the best server to handle a request.
@@ -39,29 +39,28 @@
 ```bash
 pip install prometheus-client
 ```
 
 ## Usage 
 ## Configuring and running a gRPC server
 
-Here's a simple example of how to use grpc_connection_forwarder with a gRPC server and prometeus-client:
+Here's a simple example of how to use grpc_load_balancer with a gRPC server and prometeus-client:
 
 # Import the required modules:
 ```python 
 import grpc
-from grpc_connection_forwarder import GrpcConnnectionForwarder
+from grpc_load_balancer import GrpcConnnectionForwarder
 from prometheus_client import start_http_server, Gauge
 ```
 
 
 # Initialize your gRPC server(s)
 ```python
     grpc_server = create_example_grpc_server() # implement this function yourself
-    connection_counter = Gauge(
-        f'connections_num', 'Number of connections forwarded')
+    connection_counter = Gauge('connections_num', 'Number of connections forwarded')
     forwarder = GrpcConnnectionForwarder(
         grpc_server, callback=lambda value: connection_counter.set(value)
     )
     start_http_server(prometheus_port)
     # forwarder_port - port to listen connections from gRPC clients
 
     # Note this call is blocking
@@ -71,15 +70,15 @@
     
 ```
 
 ## Configuring and running a gRPC client
 # Import the required modules:    
 ```python
 import grpc
-from grpc_connection_forwarder import EnvConfigLoader, MetricsBasedServerFinder
+from grpc_load_balancer import EnvConfigLoader, MetricsBasedServerFinder
 ```
 
 
 
 # Initialize the configuration loader
 ```python
 # This is example how your environment variables can look like
@@ -105,12 +104,13 @@
 
 ## Troubleshooting
 
 If you have any problems with `grpc_load_balancer`, please open an issue on GitHub.
 Also, you can check [tests/test_grpc_load_balancer.py](tests/test_grpc_load_balancer.py) for more information.
 
 ## Contributing
+
 We welcome contributions to `grpc_load_balancer`. If you find a bug or want to propose a new feature, please open a GitHub issue or submit a pull request.
 
 ## License
 
 This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
```

### Comparing `grpc_load_balancer-0.0.2/README.md` & `grpc_load_balancer-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # gRPC Load Balancer
 
 `grpc_load_balancer` is a Python package that allows you to easily configure and manage separate gRPC server and client instances using a metrics-based load balancing approach. This is useful when you have multiple services running and want to distribute the load efficiently among them. The package includes a connection forwarder, a metrics-based server finder, and a configuration loader.
 It implemetns the following design:
 
-<img src="imgs/design.jpg" width="50%" height="50%">
+<img src="https://github.com/flagman/grpc-load-balancer/blob/main/imgs/design.jpg?raw=true" width="50%" height="50%">
 
 
 
 ## Features
 
 - Forward connections from clients to gRPC servers.
 - Use Prometheus metrics to select the best server to handle a request.
@@ -26,29 +26,28 @@
 ```bash
 pip install prometheus-client
 ```
 
 ## Usage 
 ## Configuring and running a gRPC server
 
-Here's a simple example of how to use grpc_connection_forwarder with a gRPC server and prometeus-client:
+Here's a simple example of how to use grpc_load_balancer with a gRPC server and prometeus-client:
 
 # Import the required modules:
 ```python 
 import grpc
-from grpc_connection_forwarder import GrpcConnnectionForwarder
+from grpc_load_balancer import GrpcConnnectionForwarder
 from prometheus_client import start_http_server, Gauge
 ```
 
 
 # Initialize your gRPC server(s)
 ```python
     grpc_server = create_example_grpc_server() # implement this function yourself
-    connection_counter = Gauge(
-        f'connections_num', 'Number of connections forwarded')
+    connection_counter = Gauge('connections_num', 'Number of connections forwarded')
     forwarder = GrpcConnnectionForwarder(
         grpc_server, callback=lambda value: connection_counter.set(value)
     )
     start_http_server(prometheus_port)
     # forwarder_port - port to listen connections from gRPC clients
 
     # Note this call is blocking
@@ -58,15 +57,15 @@
     
 ```
 
 ## Configuring and running a gRPC client
 # Import the required modules:    
 ```python
 import grpc
-from grpc_connection_forwarder import EnvConfigLoader, MetricsBasedServerFinder
+from grpc_load_balancer import EnvConfigLoader, MetricsBasedServerFinder
 ```
 
 
 
 # Initialize the configuration loader
 ```python
 # This is example how your environment variables can look like
@@ -92,12 +91,13 @@
 
 ## Troubleshooting
 
 If you have any problems with `grpc_load_balancer`, please open an issue on GitHub.
 Also, you can check [tests/test_grpc_load_balancer.py](tests/test_grpc_load_balancer.py) for more information.
 
 ## Contributing
+
 We welcome contributions to `grpc_load_balancer`. If you find a bug or want to propose a new feature, please open a GitHub issue or submit a pull request.
 
 ## License
 
 This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
```

### Comparing `grpc_load_balancer-0.0.2/grpc_load_balancer/connection_counter.py` & `grpc_load_balancer-0.0.3/grpc_load_balancer/connection_counter.py`

 * *Files identical despite different names*

### Comparing `grpc_load_balancer-0.0.2/grpc_load_balancer/env_config_loader.py` & `grpc_load_balancer-0.0.3/grpc_load_balancer/env_config_loader.py`

 * *Files identical despite different names*

### Comparing `grpc_load_balancer-0.0.2/grpc_load_balancer/grpc_connection_forwarder.py` & `grpc_load_balancer-0.0.3/grpc_load_balancer/grpc_connection_forwarder.py`

 * *Files identical despite different names*

### Comparing `grpc_load_balancer-0.0.2/grpc_load_balancer/metrics_based_server_finder.py` & `grpc_load_balancer-0.0.3/grpc_load_balancer/metrics_based_server_finder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import re
 import requests
+
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 
 class MetricsBasedServerFinder:
     def __init__(
         self,
         hosts_config: List[Dict[str, Optional[Union[str, int]]]],
@@ -42,11 +44,11 @@
             return self._parse_prometheus_metrics(response.text)
         except requests.exceptions.RequestException as e:
             print(
                 f"Warning: Couldn't fetch metrics from {metrics_url}, skipping. Reason: {e}")
             return None
 
     def _parse_prometheus_metrics(self, response_text: str) -> Optional[float]:
-        for line in response_text.split("\n"):
-            if line.startswith(self.metrics_name):
-                return float(line[len(self.metrics_name):].strip().split(" ")[0])
-        return None
+        pattern = rf"{self.metrics_name}(?:\s*{{[^}}]*}})?\s+(\d+\.\d+)"
+        match = re.search(pattern, response_text)
+
+        return float(match.group(1)) if match else None
```

### Comparing `grpc_load_balancer-0.0.2/grpc_load_balancer.egg-info/PKG-INFO` & `grpc_load_balancer-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: grpc-load-balancer
-Version: 0.0.2
+Name: grpc_load_balancer
+Version: 0.0.3
 Summary: A small toolset to implement load balancing for gRPC services
 Home-page: https://github.com/flagman/grpc-load-balancer
 Author: Pavel Malay
 Author-email: flagmansupport@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 License-File: LICENSE
 
 # gRPC Load Balancer
 
 `grpc_load_balancer` is a Python package that allows you to easily configure and manage separate gRPC server and client instances using a metrics-based load balancing approach. This is useful when you have multiple services running and want to distribute the load efficiently among them. The package includes a connection forwarder, a metrics-based server finder, and a configuration loader.
 It implemetns the following design:
 
-<img src="imgs/design.jpg" width="50%" height="50%">
+<img src="https://github.com/flagman/grpc-load-balancer/blob/main/imgs/design.jpg?raw=true" width="50%" height="50%">
 
 
 
 ## Features
 
 - Forward connections from clients to gRPC servers.
 - Use Prometheus metrics to select the best server to handle a request.
@@ -39,29 +39,28 @@
 ```bash
 pip install prometheus-client
 ```
 
 ## Usage 
 ## Configuring and running a gRPC server
 
-Here's a simple example of how to use grpc_connection_forwarder with a gRPC server and prometeus-client:
+Here's a simple example of how to use grpc_load_balancer with a gRPC server and prometeus-client:
 
 # Import the required modules:
 ```python 
 import grpc
-from grpc_connection_forwarder import GrpcConnnectionForwarder
+from grpc_load_balancer import GrpcConnnectionForwarder
 from prometheus_client import start_http_server, Gauge
 ```
 
 
 # Initialize your gRPC server(s)
 ```python
     grpc_server = create_example_grpc_server() # implement this function yourself
-    connection_counter = Gauge(
-        f'connections_num', 'Number of connections forwarded')
+    connection_counter = Gauge('connections_num', 'Number of connections forwarded')
     forwarder = GrpcConnnectionForwarder(
         grpc_server, callback=lambda value: connection_counter.set(value)
     )
     start_http_server(prometheus_port)
     # forwarder_port - port to listen connections from gRPC clients
 
     # Note this call is blocking
@@ -71,15 +70,15 @@
     
 ```
 
 ## Configuring and running a gRPC client
 # Import the required modules:    
 ```python
 import grpc
-from grpc_connection_forwarder import EnvConfigLoader, MetricsBasedServerFinder
+from grpc_load_balancer import EnvConfigLoader, MetricsBasedServerFinder
 ```
 
 
 
 # Initialize the configuration loader
 ```python
 # This is example how your environment variables can look like
@@ -105,12 +104,13 @@
 
 ## Troubleshooting
 
 If you have any problems with `grpc_load_balancer`, please open an issue on GitHub.
 Also, you can check [tests/test_grpc_load_balancer.py](tests/test_grpc_load_balancer.py) for more information.
 
 ## Contributing
+
 We welcome contributions to `grpc_load_balancer`. If you find a bug or want to propose a new feature, please open a GitHub issue or submit a pull request.
 
 ## License
 
 This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
```

### Comparing `grpc_load_balancer-0.0.2/grpc_load_balancer.egg-info/SOURCES.txt` & `grpc_load_balancer-0.0.3/grpc_load_balancer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grpc_load_balancer-0.0.2/setup.py` & `grpc_load_balancer-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="grpc_load_balancer",
-    version="0.0.2",
+    version="0.0.3",
     author="Pavel Malay",
     author_email="flagmansupport@gmail.com",
     description="A small toolset to implement load balancing for gRPC services",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flagman/grpc-load-balancer",
     packages=find_packages(exclude=["tests"]),
```

### Comparing `grpc_load_balancer-0.0.2/tests/test_grpc_load_balancer.py` & `grpc_load_balancer-0.0.3/tests/test_grpc_load_balancer.py`

 * *Files identical despite different names*


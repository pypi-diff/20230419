# Comparing `tmp/netpackAIO-0.0.2.tar.gz` & `tmp/netpackAIO-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netpackAIO-0.0.2.tar", last modified: Sat Apr 15 00:51:03 2023, max compression
+gzip compressed data, was "netpackAIO-0.0.3.tar", last modified: Wed Apr 19 06:27:27 2023, max compression
```

## Comparing `netpackAIO-0.0.2.tar` & `netpackAIO-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 00:51:03.643650 netpackAIO-0.0.2/
--rw-rw-rw-   0        0        0     1089 2023-04-14 20:36:26.000000 netpackAIO-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2172 2023-04-15 00:51:03.643650 netpackAIO-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1661 2023-04-14 23:20:11.000000 netpackAIO-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 00:51:03.607649 netpackAIO-0.0.2/netpack/
--rw-rw-rw-   0        0        0        0 2023-04-12 17:33:48.000000 netpackAIO-0.0.2/netpack/__init__.py
--rw-rw-rw-   0        0        0     3034 2023-04-14 21:45:51.000000 netpackAIO-0.0.2/netpack/func.py
--rw-rw-rw-   0        0        0      100 2023-04-14 20:40:41.000000 netpackAIO-0.0.2/netpack/test.py
-drwxrwxrwx   0        0        0        0 2023-04-15 00:51:03.641612 netpackAIO-0.0.2/netpackAIO.egg-info/
--rw-rw-rw-   0        0        0     2172 2023-04-15 00:51:03.000000 netpackAIO-0.0.2/netpackAIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-04-15 00:51:03.000000 netpackAIO-0.0.2/netpackAIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 00:51:03.000000 netpackAIO-0.0.2/netpackAIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-15 00:51:03.000000 netpackAIO-0.0.2/netpackAIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-15 00:51:03.000000 netpackAIO-0.0.2/netpackAIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-04-15 00:51:03.650613 netpackAIO-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-04-15 00:50:45.000000 netpackAIO-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:27:27.029025 netpackAIO-0.0.3/
+-rw-rw-rw-   0        0        0     1089 2023-04-14 20:36:26.000000 netpackAIO-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3389 2023-04-19 06:27:27.030026 netpackAIO-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2878 2023-04-19 06:22:56.000000 netpackAIO-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 06:27:26.987029 netpackAIO-0.0.3/netpack/
+-rw-rw-rw-   0        0        0        0 2023-04-12 17:33:48.000000 netpackAIO-0.0.3/netpack/__init__.py
+-rw-rw-rw-   0        0        0    10478 2023-04-19 05:40:57.000000 netpackAIO-0.0.3/netpack/func.py
+-rw-rw-rw-   0        0        0      158 2023-04-19 05:57:47.000000 netpackAIO-0.0.3/netpack/test.py
+drwxrwxrwx   0        0        0        0 2023-04-19 06:27:27.027025 netpackAIO-0.0.3/netpackAIO.egg-info/
+-rw-rw-rw-   0        0        0     3389 2023-04-19 06:27:26.000000 netpackAIO-0.0.3/netpackAIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-04-19 06:27:26.000000 netpackAIO-0.0.3/netpackAIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 06:27:26.000000 netpackAIO-0.0.3/netpackAIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-19 06:27:26.000000 netpackAIO-0.0.3/netpackAIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 06:27:26.000000 netpackAIO-0.0.3/netpackAIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-19 06:27:27.036025 netpackAIO-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-04-19 06:24:40.000000 netpackAIO-0.0.3/setup.py
```

### Comparing `netpackAIO-0.0.2/LICENSE` & `netpackAIO-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netpackAIO-0.0.2/PKG-INFO` & `netpackAIO-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netpackAIO
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for performing network-related tasks
 Home-page: https://github.com/crusaderay/netpack
 Author: Dongjie Zhang
 Author-email: crusade.ray@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -31,15 +31,14 @@
 
 ### Classes and Methods
 The NetPack package contains the following classes and methods:
 
 
 #### NetPack.inr(server: str, ipv4v6: str, query_flags: str = None) -> str
 * This is a static method that takes the following parameters, and return the check result from the INR whois server:
-
     * server: The whois server address
       * ##### Pre-set NetPack.ServerLocation
           * AFRINIC: The AFRINIC whois server address
           * ARIN: The ARIN whois server address
           * APNIC: The APNIC whois server address
           * LACNIC: The LACNIC whois server address
           * RIPE_NCC: The RIPE NCC whois server address
@@ -48,7 +47,22 @@
     * ipv4v6: The IP address or CIDR range
     * query_flags: Optional parameter that specifies query flags for certain whois servers
     * (The method returns the response received from the whois server as a string.)
 
 #### NetPack.radb(ip: str) -> str
 * This is a static method that takes an IPv4 address as an input and return the result from RADB
 
+#### ping(host, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5) -> tuple
+* The ping() method can be used to ping a single host:
+    * Arguments
+        * host: the hostname or IP address of the host to ping.
+        * packet_size: the size of the packets to send (in bytes). Default is 64.
+        * protocol: the protocol to use for the ping test. Must be either "icmp" or "tcp". Default is "icmp".
+        * interval: the time (in seconds) to wait between sending each packet. Default is 0.2.
+        * timeout: the time (in seconds) to wait for a response before considering the packet lost. Default is 1.
+        * packet_num: the number of packets to send. Default is 5.
+
+#### multiple_ping(hosts, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5) -> dict
+* The multiple_ping() method can be used to ping multiple hosts in parallel, This will return a dictionary where each key is a host from the hosts list and each value is a dictionary containing the average latency and success rate of the ping test.
+    * Arguments
+        * The arguments for multiple_ping() are the same as for ping(), except that they are used for all hosts in the hosts list.
+
```

### Comparing `netpackAIO-0.0.2/netpackAIO.egg-info/PKG-INFO` & `netpackAIO-0.0.3/netpackAIO.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netpackAIO
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package for performing network-related tasks
 Home-page: https://github.com/crusaderay/netpack
 Author: Dongjie Zhang
 Author-email: crusade.ray@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -31,15 +31,14 @@
 
 ### Classes and Methods
 The NetPack package contains the following classes and methods:
 
 
 #### NetPack.inr(server: str, ipv4v6: str, query_flags: str = None) -> str
 * This is a static method that takes the following parameters, and return the check result from the INR whois server:
-
     * server: The whois server address
       * ##### Pre-set NetPack.ServerLocation
           * AFRINIC: The AFRINIC whois server address
           * ARIN: The ARIN whois server address
           * APNIC: The APNIC whois server address
           * LACNIC: The LACNIC whois server address
           * RIPE_NCC: The RIPE NCC whois server address
@@ -48,7 +47,22 @@
     * ipv4v6: The IP address or CIDR range
     * query_flags: Optional parameter that specifies query flags for certain whois servers
     * (The method returns the response received from the whois server as a string.)
 
 #### NetPack.radb(ip: str) -> str
 * This is a static method that takes an IPv4 address as an input and return the result from RADB
 
+#### ping(host, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5) -> tuple
+* The ping() method can be used to ping a single host:
+    * Arguments
+        * host: the hostname or IP address of the host to ping.
+        * packet_size: the size of the packets to send (in bytes). Default is 64.
+        * protocol: the protocol to use for the ping test. Must be either "icmp" or "tcp". Default is "icmp".
+        * interval: the time (in seconds) to wait between sending each packet. Default is 0.2.
+        * timeout: the time (in seconds) to wait for a response before considering the packet lost. Default is 1.
+        * packet_num: the number of packets to send. Default is 5.
+
+#### multiple_ping(hosts, packet_size=64, protocol="icmp", interval=0.2, timeout=1, packet_num=5) -> dict
+* The multiple_ping() method can be used to ping multiple hosts in parallel, This will return a dictionary where each key is a host from the hosts list and each value is a dictionary containing the average latency and success rate of the ping test.
+    * Arguments
+        * The arguments for multiple_ping() are the same as for ping(), except that they are used for all hosts in the hosts list.
+
```

### Comparing `netpackAIO-0.0.2/setup.py` & `netpackAIO-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='netpackAIO',
-    version='0.0.2',
+    version='0.0.3',
     description='A Python package for performing network-related tasks',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Dongjie Zhang',
     author_email='crusade.ray@gmail.com',
     url='https://github.com/crusaderay/netpack',
     packages=find_packages(),
```


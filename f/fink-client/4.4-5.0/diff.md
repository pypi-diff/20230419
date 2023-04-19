# Comparing `tmp/fink-client-4.4.tar.gz` & `tmp/fink-client-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fink-client-4.4.tar", last modified: Wed Feb 15 20:45:53 2023, max compression
+gzip compressed data, was "fink-client-5.0.tar", last modified: Wed Apr 19 08:57:34 2023, max compression
```

## Comparing `fink-client-4.4.tar` & `fink-client-5.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-15 20:45:53.281551 fink-client-4.4/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)    11357 2022-08-16 12:31:59.000000 fink-client-4.4/LICENSE
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     5732 2023-02-15 20:45:53.281551 fink-client-4.4/PKG-INFO
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     4951 2023-02-10 20:37:11.000000 fink-client-4.4/README.md
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-15 20:45:53.277551 fink-client-4.4/bin/
--rwxrwxr-x   0 peloton   (1000) peloton   (1000)     1421 2022-08-16 12:31:59.000000 fink-client-4.4/bin/fink_client_test.sh
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-15 20:45:53.281551 fink-client-4.4/fink_client/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)      686 2023-02-15 20:44:17.000000 fink-client-4.4/fink_client/__init__.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)    13513 2023-01-16 15:09:39.000000 fink-client-4.4/fink_client/avroUtils.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     4129 2022-08-16 12:31:59.000000 fink-client-4.4/fink_client/configuration.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)    10041 2023-01-25 12:43:02.000000 fink-client-4.4/fink_client/consumer.py
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-15 20:45:53.281551 fink-client-4.4/fink_client/scripts/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)      606 2022-08-16 12:31:59.000000 fink-client-4.4/fink_client/scripts/__init__.py
--rwxrwxr-x   0 peloton   (1000) peloton   (1000)     3308 2022-08-16 12:31:59.000000 fink-client-4.4/fink_client/scripts/fink_alert_viewer.py
--rwxrwxr-x   0 peloton   (1000) peloton   (1000)     2547 2023-01-16 15:09:39.000000 fink-client-4.4/fink_client/scripts/fink_client_register.py
--rwxrwxr-x   0 peloton   (1000) peloton   (1000)     4167 2023-01-25 12:43:02.000000 fink-client-4.4/fink_client/scripts/fink_consumer.py
--rwxrwxr-x   0 peloton   (1000) peloton   (1000)     7236 2023-02-15 20:44:10.000000 fink-client-4.4/fink_client/scripts/fink_datatransfer.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     1756 2022-08-16 12:31:59.000000 fink-client-4.4/fink_client/tester.py
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     3466 2022-08-16 12:31:59.000000 fink-client-4.4/fink_client/visualisation.py
-drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-02-15 20:45:53.281551 fink-client-4.4/fink_client.egg-info/
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     5732 2023-02-15 20:45:52.000000 fink-client-4.4/fink_client.egg-info/PKG-INFO
--rw-rw-r--   0 peloton   (1000) peloton   (1000)      610 2023-02-15 20:45:53.000000 fink-client-4.4/fink_client.egg-info/SOURCES.txt
--rw-rw-r--   0 peloton   (1000) peloton   (1000)        1 2023-02-15 20:45:52.000000 fink-client-4.4/fink_client.egg-info/dependency_links.txt
--rw-rw-r--   0 peloton   (1000) peloton   (1000)      268 2023-02-15 20:45:53.000000 fink-client-4.4/fink_client.egg-info/entry_points.txt
--rw-rw-r--   0 peloton   (1000) peloton   (1000)      135 2023-02-15 20:45:53.000000 fink-client-4.4/fink_client.egg-info/requires.txt
--rw-rw-r--   0 peloton   (1000) peloton   (1000)       12 2023-02-15 20:45:53.000000 fink-client-4.4/fink_client.egg-info/top_level.txt
--rw-rw-r--   0 peloton   (1000) peloton   (1000)       38 2023-02-15 20:45:53.281551 fink-client-4.4/setup.cfg
--rw-rw-r--   0 peloton   (1000) peloton   (1000)     2169 2023-01-17 15:11:10.000000 fink-client-4.4/setup.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-04-19 08:57:34.257747 fink-client-5.0/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)    11357 2022-08-16 12:31:59.000000 fink-client-5.0/LICENSE
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     6028 2023-04-19 08:57:34.257747 fink-client-5.0/PKG-INFO
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     5247 2023-04-19 08:57:04.000000 fink-client-5.0/README.md
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-04-19 08:57:34.257747 fink-client-5.0/bin/
+-rwxrwxr-x   0 peloton   (1000) peloton   (1000)     1421 2022-08-16 12:31:59.000000 fink-client-5.0/bin/fink_client_test.sh
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-04-19 08:57:34.257747 fink-client-5.0/fink_client/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)      686 2023-04-19 08:57:04.000000 fink-client-5.0/fink_client/__init__.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)    13513 2023-01-16 15:09:39.000000 fink-client-5.0/fink_client/avroUtils.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     4129 2023-03-22 05:19:32.000000 fink-client-5.0/fink_client/configuration.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)    12891 2023-04-19 08:57:04.000000 fink-client-5.0/fink_client/consumer.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-04-19 08:57:34.257747 fink-client-5.0/fink_client/scripts/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)      606 2022-08-16 12:31:59.000000 fink-client-5.0/fink_client/scripts/__init__.py
+-rwxrwxr-x   0 peloton   (1000) peloton   (1000)     3308 2022-08-16 12:31:59.000000 fink-client-5.0/fink_client/scripts/fink_alert_viewer.py
+-rwxrwxr-x   0 peloton   (1000) peloton   (1000)     2547 2023-01-16 15:09:39.000000 fink-client-5.0/fink_client/scripts/fink_client_register.py
+-rwxrwxr-x   0 peloton   (1000) peloton   (1000)     4167 2023-01-25 12:43:02.000000 fink-client-5.0/fink_client/scripts/fink_consumer.py
+-rwxrwxr-x   0 peloton   (1000) peloton   (1000)    12363 2023-04-19 08:57:04.000000 fink-client-5.0/fink_client/scripts/fink_datatransfer.py
+-rwxrwxr-x   0 peloton   (1000) peloton   (1000)     8466 2023-02-27 14:53:47.000000 fink-client-5.0/fink_client/scripts/fink_datatransfer_mpi.py
+-rwxrwxr-x   0 peloton   (1000) peloton   (1000)     9438 2023-03-02 09:51:35.000000 fink-client-5.0/fink_client/scripts/fink_datatransfer_offsets.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     1756 2022-08-16 12:31:59.000000 fink-client-5.0/fink_client/tester.py
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     3466 2022-08-16 12:31:59.000000 fink-client-5.0/fink_client/visualisation.py
+drwxrwxr-x   0 peloton   (1000) peloton   (1000)        0 2023-04-19 08:57:34.257747 fink-client-5.0/fink_client.egg-info/
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     6028 2023-04-19 08:57:33.000000 fink-client-5.0/fink_client.egg-info/PKG-INFO
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)      704 2023-04-19 08:57:34.000000 fink-client-5.0/fink_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)        1 2023-04-19 08:57:33.000000 fink-client-5.0/fink_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)      268 2023-04-19 08:57:34.000000 fink-client-5.0/fink_client.egg-info/entry_points.txt
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)      132 2023-04-19 08:57:34.000000 fink-client-5.0/fink_client.egg-info/requires.txt
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)       12 2023-04-19 08:57:34.000000 fink-client-5.0/fink_client.egg-info/top_level.txt
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)       38 2023-04-19 08:57:34.257747 fink-client-5.0/setup.cfg
+-rw-rw-r--   0 peloton   (1000) peloton   (1000)     2169 2023-01-17 15:11:10.000000 fink-client-5.0/setup.py
```

### Comparing `fink-client-4.4/LICENSE` & `fink-client-5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fink-client-4.4/PKG-INFO` & `fink-client-5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: fink-client
-Version: 4.4
-Summary: Light-weight client to manipulate alerts from Fink
-Home-page: https://fink-broker.readthedocs.io/en/latest/
-Author: AstroLab Software
-Author-email: peloton@lal.in2p3.fr
-License: UNKNOWN
-Project-URL: Documentation, https://fink-broker.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/astrolabsoftware/fink-client
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: Unix
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![pypi](https://img.shields.io/pypi/v/fink-client.svg)](https://pypi.python.org/pypi/fink-client)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fink-client&metric=alert_status)](https://sonarcloud.io/dashboard?id=fink-client)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=fink-client&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=fink-client)
 [![Sentinel](https://github.com/astrolabsoftware/fink-client/workflows/Sentinel/badge.svg)](https://github.com/astrolabsoftware/fink-client/actions?query=workflow%3ASentinel)
 [![codecov](https://codecov.io/gh/astrolabsoftware/fink-client/branch/master/graph/badge.svg)](https://codecov.io/gh/astrolabsoftware/fink-client)
 [![Documentation Status](https://readthedocs.org/projects/fink-broker/badge/?version=latest)](https://fink-broker.readthedocs.io/en/latest/?badge=latest)
 
@@ -29,34 +9,36 @@
 
 `fink-client` is a light package to manipulate catalogs and alerts issued from the [fink broker](https://github.com/astrolabsoftware/fink-broker) programmatically. It is used in the context of 2 major Fink services: Livestream and Data Transfer.
 
 ## Installation
 
 `fink_client` requires a version of Python 3.9+.
 
-### install with pip
+### Install with pip
 
 ```bash
 pip install fink-client --upgrade
 ```
 
-### install within a conda environment
+### Use or develop in a controlled environment
 
 ```bash
 git clone https://github.com/astrolabsoftware/fink-client.git
 cd fink-client
 conda env create -f environment.yml
-# install the latest release
-pip install fink-client
+conda activate fink-client
+```
+
+and then install it locally:
+
+```bash
 # install for development
 pip install -e .
 ```
 
-Learn how to connect and use it by checking the [documentation](docs/).
-
 ## Registration
 
 In order to connect and poll alerts from Fink, you need to get your credentials:
 
 1. Subscribe to one or more Fink streams by filling this [form](https://forms.gle/2td4jysT4e9pkf889).
 2. After filling the form, we will send your credentials. Register them on your laptop by simply running:
   ```
@@ -99,37 +81,37 @@
 Display cutouts and lightcurve from a ZTF alert
 
 optional arguments:
   -h, --help          show this help message and exit
   -filename FILENAME  Path to an alert data file (avro format)
 ```
 
-More information at [docs/livestream](docs/livestream_manual.md).
+More information at [docs/livestream](https://fink-broker.readthedocs.io/en/latest/services/livestream).
 
 ## Data Transfer usage
 
 If you requested data using the [Data Transfer service](https://fink-portal.org/download), you can easily poll your stream using:
 
 ```bash
-fink_datatransfer -h
-usage: fink_datatransfer [-h] [-topic TOPIC] [-limit LIMIT] [-outdir OUTDIR] [-partitionby PARTITIONBY] [-batchsize BATCHSIZE] [--restart_from_beginning]
-                            [--verbose]
+usage: fink_datatransfer [-h] [-topic TOPIC] [-limit LIMIT] [-outdir OUTDIR] [-partitionby PARTITIONBY] [-batchsize BATCHSIZE] [-nconsumers NCONSUMERS] [-maxtimeout MAXTIMEOUT] [--restart_from_beginning] [--verbose]
 
 Kafka consumer to listen and archive Fink streams from the data transfer service
 
 optional arguments:
   -h, --help            show this help message and exit
   -topic TOPIC          Topic name for the stream that contains the data.
   -limit LIMIT          If specified, download only `limit` alerts from the stream. Default is None, that is download all alerts.
   -outdir OUTDIR        Folder to store incoming alerts. It will be created if it does not exist.
   -partitionby PARTITIONBY
-                        Partition data by `time` (year=YYYY/month=MM/day=DD), or `finkclass` (finkclass=CLASS), or `tnsclass` (tnsclass=CLASS). Default is
-                        time.
+                        Partition data by `time` (year=YYYY/month=MM/day=DD), or `finkclass` (finkclass=CLASS), or `tnsclass` (tnsclass=CLASS). `classId` is also available for ELASTiCC data. Default is time.
   -batchsize BATCHSIZE  Maximum number of alert within the `maxtimeout` (see conf). Default is 1000 alerts.
+  -nconsumers NCONSUMERS
+                        Number of parallel consumer to use. Default is 1.
+  -maxtimeout MAXTIMEOUT
+                        Overwrite the default timeout (in seconds) from user configuration. Default is None.
   --restart_from_beginning
                         If specified, restart downloading from the 1st alert in the stream. Default is False.
   --verbose             If specified, print on screen information about the consuming.
 
 ```
 
-More information at [docs/datatransfer](docs/datatransfer.md).
-
+More information at [docs/datatransfer](https://fink-broker.readthedocs.io/en/latest/services/data_transfer/).
```

### Comparing `fink-client-4.4/README.md` & `fink-client-5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: fink-client
+Version: 5.0
+Summary: Light-weight client to manipulate alerts from Fink
+Home-page: https://fink-broker.readthedocs.io/en/latest/
+Author: AstroLab Software
+Author-email: peloton@lal.in2p3.fr
+License: UNKNOWN
+Project-URL: Documentation, https://fink-broker.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/astrolabsoftware/fink-client
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: Unix
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![pypi](https://img.shields.io/pypi/v/fink-client.svg)](https://pypi.python.org/pypi/fink-client)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=fink-client&metric=alert_status)](https://sonarcloud.io/dashboard?id=fink-client)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=fink-client&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=fink-client)
 [![Sentinel](https://github.com/astrolabsoftware/fink-client/workflows/Sentinel/badge.svg)](https://github.com/astrolabsoftware/fink-client/actions?query=workflow%3ASentinel)
 [![codecov](https://codecov.io/gh/astrolabsoftware/fink-client/branch/master/graph/badge.svg)](https://codecov.io/gh/astrolabsoftware/fink-client)
 [![Documentation Status](https://readthedocs.org/projects/fink-broker/badge/?version=latest)](https://fink-broker.readthedocs.io/en/latest/?badge=latest)
 
@@ -9,34 +29,36 @@
 
 `fink-client` is a light package to manipulate catalogs and alerts issued from the [fink broker](https://github.com/astrolabsoftware/fink-broker) programmatically. It is used in the context of 2 major Fink services: Livestream and Data Transfer.
 
 ## Installation
 
 `fink_client` requires a version of Python 3.9+.
 
-### install with pip
+### Install with pip
 
 ```bash
 pip install fink-client --upgrade
 ```
 
-### install within a conda environment
+### Use or develop in a controlled environment
 
 ```bash
 git clone https://github.com/astrolabsoftware/fink-client.git
 cd fink-client
 conda env create -f environment.yml
-# install the latest release
-pip install fink-client
+conda activate fink-client
+```
+
+and then install it locally:
+
+```bash
 # install for development
 pip install -e .
 ```
 
-Learn how to connect and use it by checking the [documentation](docs/).
-
 ## Registration
 
 In order to connect and poll alerts from Fink, you need to get your credentials:
 
 1. Subscribe to one or more Fink streams by filling this [form](https://forms.gle/2td4jysT4e9pkf889).
 2. After filling the form, we will send your credentials. Register them on your laptop by simply running:
   ```
@@ -79,36 +101,38 @@
 Display cutouts and lightcurve from a ZTF alert
 
 optional arguments:
   -h, --help          show this help message and exit
   -filename FILENAME  Path to an alert data file (avro format)
 ```
 
-More information at [docs/livestream](docs/livestream_manual.md).
+More information at [docs/livestream](https://fink-broker.readthedocs.io/en/latest/services/livestream).
 
 ## Data Transfer usage
 
 If you requested data using the [Data Transfer service](https://fink-portal.org/download), you can easily poll your stream using:
 
 ```bash
-fink_datatransfer -h
-usage: fink_datatransfer [-h] [-topic TOPIC] [-limit LIMIT] [-outdir OUTDIR] [-partitionby PARTITIONBY] [-batchsize BATCHSIZE] [--restart_from_beginning]
-                            [--verbose]
+usage: fink_datatransfer [-h] [-topic TOPIC] [-limit LIMIT] [-outdir OUTDIR] [-partitionby PARTITIONBY] [-batchsize BATCHSIZE] [-nconsumers NCONSUMERS] [-maxtimeout MAXTIMEOUT] [--restart_from_beginning] [--verbose]
 
 Kafka consumer to listen and archive Fink streams from the data transfer service
 
 optional arguments:
   -h, --help            show this help message and exit
   -topic TOPIC          Topic name for the stream that contains the data.
   -limit LIMIT          If specified, download only `limit` alerts from the stream. Default is None, that is download all alerts.
   -outdir OUTDIR        Folder to store incoming alerts. It will be created if it does not exist.
   -partitionby PARTITIONBY
-                        Partition data by `time` (year=YYYY/month=MM/day=DD), or `finkclass` (finkclass=CLASS), or `tnsclass` (tnsclass=CLASS). Default is
-                        time.
+                        Partition data by `time` (year=YYYY/month=MM/day=DD), or `finkclass` (finkclass=CLASS), or `tnsclass` (tnsclass=CLASS). `classId` is also available for ELASTiCC data. Default is time.
   -batchsize BATCHSIZE  Maximum number of alert within the `maxtimeout` (see conf). Default is 1000 alerts.
+  -nconsumers NCONSUMERS
+                        Number of parallel consumer to use. Default is 1.
+  -maxtimeout MAXTIMEOUT
+                        Overwrite the default timeout (in seconds) from user configuration. Default is None.
   --restart_from_beginning
                         If specified, restart downloading from the 1st alert in the stream. Default is False.
   --verbose             If specified, print on screen information about the consuming.
 
 ```
 
-More information at [docs/datatransfer](docs/datatransfer.md).
+More information at [docs/datatransfer](https://fink-broker.readthedocs.io/en/latest/services/data_transfer/).
+
```

### Comparing `fink-client-4.4/bin/fink_client_test.sh` & `fink-client-5.0/bin/fink_client_test.sh`

 * *Files identical despite different names*

### Comparing `fink-client-4.4/fink_client/__init__.py` & `fink-client-5.0/fink_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "4.4"
+__version__ = "5.0"
 __schema_version__ = "distribution_schema_fink_ztf_{}.avsc"
```

### Comparing `fink-client-4.4/fink_client/avroUtils.py` & `fink-client-5.0/fink_client/avroUtils.py`

 * *Files identical despite different names*

### Comparing `fink-client-4.4/fink_client/configuration.py` & `fink-client-5.0/fink_client/configuration.py`

 * *Files identical despite different names*

### Comparing `fink-client-4.4/fink_client/consumer.py` & `fink-client-5.0/fink_client/consumer.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import io
 import json
+import time
 import fastavro
 import confluent_kafka
 
 from fink_client.avroUtils import write_alert
 from fink_client.avroUtils import _get_alert_schema
 from fink_client.avroUtils import _decode_avro_alert
 
@@ -263,14 +264,95 @@
         return self._consumer.list_topics().brokers
 
     def close(self):
         """Close connection to Fink broker"""
         self._consumer.close()
 
 
+def return_offsets(consumer, topic, waitfor=1, timeout=10, verbose=False):
+    """ Poll servers to get the total committed offsets, and remaining lag
+
+    Parameters
+    ----------
+    consumer: confluent_kafka.Consumer
+        Kafka consumer
+    topic: str
+        Topic name
+    waitfor: int, optional
+        Time in second to wait before polling. Default is 1 second.
+    timeout: int, optional
+        Timeout in second when polling the servers. Default is 10.
+    verbose: bool, optional
+        If True, prints useful table. Default is False.
+
+    Returns
+    ---------
+    total_offsets: int
+        Total number of messages committed across all partitions
+    total_lag: int
+        Remaining messages in the topic across all partitions.
+    """
+    time.sleep(waitfor)
+    # Get the topic's partitions
+    metadata = consumer.list_topics(topic, timeout=timeout)
+    if metadata.topics[topic].error is not None:
+        raise confluent_kafka.KafkaException(metadata.topics[topic].error)
+
+    # Construct TopicPartition list of partitions to query
+    partitions = [confluent_kafka.TopicPartition(topic, p) for p in metadata.topics[topic].partitions]
+
+    # Query committed offsets for this group and the given partitions
+    try:
+        committed = consumer.committed(partitions, timeout=timeout)
+    except confluent_kafka.KafkaException as exception:
+        kafka_error = exception.args[0]
+        if kafka_error.code() == confluent_kafka.KafkaError._TIMED_OUT:
+            return -1, -1
+        else:
+            return 0, 0
+
+    total_offsets = 0
+    total_lag = 0
+    if verbose:
+        print("%-50s  %9s  %9s" % ("Topic [Partition]", "Committed", "Lag"))
+        print("=" * 72)
+    for partition in committed:
+        # Get the partitions low and high watermark offsets.
+        (lo, hi) = consumer.get_watermark_offsets(partition, timeout=timeout, cached=False)
+
+        if partition.offset == confluent_kafka.OFFSET_INVALID:
+            offset = "-"
+        else:
+            offset = "%d" % (partition.offset)
+
+        if hi < 0:
+            lag = "no hwmark"  # Unlikely
+        elif partition.offset < 0:
+            # No committed offset, show total message count as lag.
+            # The actual message count may be lower due to compaction
+            # and record deletions.
+            lag = "%d" % (hi - lo)
+            partition.offset = 0
+        else:
+            lag = "%d" % (hi - partition.offset)
+
+        total_offsets = partition.offset
+        total_lag = int(lag)
+
+        if verbose:
+            print("%-50s  %9s  %9s" % (
+                "{} [{}]".format(partition.topic, partition.partition), offset, lag))
+    if verbose:
+        print("-" * 72)
+        print("%-50s  %9s  %9s" % (
+            "Total", total_offsets, total_lag))
+        print("-" * 72)
+
+    return total_offsets, total_lag
+
 def _get_kafka_config(config: dict) -> dict:
     """Returns configurations for a consumer instance
 
     Parameters
     ----------
     config: dict
         Dictionary of configurations
```

### Comparing `fink-client-4.4/fink_client/scripts/__init__.py` & `fink-client-5.0/fink_client/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `fink-client-4.4/fink_client/scripts/fink_alert_viewer.py` & `fink-client-5.0/fink_client/scripts/fink_alert_viewer.py`

 * *Files identical despite different names*

### Comparing `fink-client-4.4/fink_client/scripts/fink_client_register.py` & `fink-client-5.0/fink_client/scripts/fink_client_register.py`

 * *Files identical despite different names*

### Comparing `fink-client-4.4/fink_client/scripts/fink_consumer.py` & `fink-client-5.0/fink_client/scripts/fink_consumer.py`

 * *Files identical despite different names*

### Comparing `fink-client-4.4/fink_client/scripts/fink_datatransfer.py` & `fink-client-5.0/fink_client/scripts/fink_datatransfer_offsets.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,16 +26,47 @@
 import pyarrow.parquet as pq
 import fastavro
 import confluent_kafka
 
 import numpy as np
 import pandas as pd
 
+from fink_client.consumer import return_offsets
+
 from fink_client.configuration import load_credentials
 
+def get_schema(kafka_config, topic, maxtimeout):
+    """
+    """
+    # Instantiate a consumer
+    consumer_schema = confluent_kafka.Consumer(kafka_config)
+
+    # Subscribe to schema topic
+    topics = ['{}_schema'.format(topic)]
+    consumer_schema.subscribe(topics)
+
+    # Poll
+    msg = consumer_schema.poll(maxtimeout)
+    if msg is not None:
+        schema = fastavro.schema.parse_schema(json.loads(msg.key()))
+    else:
+        schema = None
+
+    consumer_schema.close()
+
+    return schema
+
+def my_assign(consumer, partitions):
+    """
+    """
+    for p in partitions:
+        p.offset = 0
+    # print('assign', partitions)
+    consumer.assign(partitions)
+
 def main():
     """ """
     parser = argparse.ArgumentParser(description=__doc__)
     parser.add_argument(
         '-topic', type=str, default='.',
         help="Topic name for the stream that contains the data.")
     parser.add_argument(
@@ -50,30 +81,34 @@
     parser.add_argument(
         '-batchsize', type=int, default=1000,
         help="Maximum number of alert within the `maxtimeout` (see conf). Default is 1000 alerts.")
     parser.add_argument(
         '--restart_from_beginning', action='store_true',
         help="If specified, restart downloading from the 1st alert in the stream. Default is False.")
     parser.add_argument(
+        '--list_offsets', action='store_true',
+        help="If specified, list the current offset commited, and the lag (remaining alerts to poll), and exit.")
+    parser.add_argument(
         '--verbose', action='store_true',
         help="If specified, print on screen information about the consuming.")
     args = parser.parse_args(None)
 
     if args.partitionby not in ['time', 'finkclass', 'tnsclass', 'classId']:
         print("{} is an unknown partitioning. `-partitionby` should be in ['time', 'finkclass', 'tnsclass', 'classId']".format(args.partitionby))
         sys.exit()
 
     # load user configuration
     conf = load_credentials()
 
-    if args.restart_from_beginning:
-        # resetting the group ID acts as a new consumer
-        group_id = conf['group_id'] + '_{}'.format(np.random.randint(1e6))
-    else:
-        group_id = conf['group_id']
+    group_id = conf['group_id']
+    # if args.restart_from_beginning:
+    #     # resetting the group ID acts as a new consumer
+    #     group_id = conf['group_id'] + '_{}'.format(np.random.randint(1e6))
+    # else:
+    #     group_id = conf['group_id']
 
     kafka_config = {
         'bootstrap.servers': conf['servers'],
         'group.id': group_id,
         "auto.offset.reset": "earliest"
     }
 
@@ -85,45 +120,51 @@
 
     # Time to wait before polling again if no alerts
     maxtimeout = conf['maxtimeout']
 
     if (args.limit is not None) and (args.limit < args.batchsize):
         args.batchsize = args.limit
 
+    schema = get_schema(kafka_config, args.topic, maxtimeout)
+    if schema is None:
+        #TBD: raise error
+        print('No schema found -- wait a few seconds and relaunch. If the error persists, maybe the queue is empty.')
+
     # Instantiate a consumer
     consumer = confluent_kafka.Consumer(kafka_config)
 
     # Subscribe to schema topic
-    topics = ['{}_schema'.format(args.topic)]
-    consumer.subscribe(topics)
-
-    # Poll
-    msg = consumer.poll(maxtimeout)
-    schema = fastavro.schema.parse_schema(json.loads(msg.key()))
-
-    # Subscribe to schema topic
     topics = ['{}'.format(args.topic)]
-    consumer.subscribe(topics)
+
+    if args.restart_from_beginning:
+        consumer.subscribe(topics, on_assign=my_assign)
+    else:
+        consumer.subscribe(topics)
 
     # infinite loop
     maxpoll = args.limit if args.limit is not None else 1e10
+    parts = []
     try:
         poll_number = 0
         while poll_number < maxpoll:
             msgs = consumer.consume(args.batchsize, maxtimeout)
-
             # Decode the message
             if msgs is not None:
                 pdf = pd.DataFrame.from_records(
                     [fastavro.schemaless_reader(io.BytesIO(msg.value()), schema) for msg in msgs],
                 )
                 if pdf.empty:
+                    print("%-50s  %9s  %9s" % ("Topic [Partition]", "Committed", "Lag"))
+                    print("=" * 72)
+                    initial_offset, lag = return_offsets(consumer, args.topic, waitfor=1, verbose=True)
                     print('No alerts the last {} seconds ({} polled)... Exiting'.format(maxtimeout, poll_number))
                     break
 
+                [parts.append(i.partition()) for i in msgs]
+
                 # known mismatches between partitions
                 # see https://github.com/astrolabsoftware/fink-client/issues/165
                 if 'cats_broad_max_prob' in pdf.columns:
                     pdf['cats_broad_max_prob'] = pdf['cats_broad_max_prob'].astype('float')
 
                 if 'cats_broad_class' in pdf.columns:
                     pdf['cats_broad_class'] = pdf['cats_broad_class'].astype('float')
@@ -165,24 +206,39 @@
                         args.outdir,
                         schema=table_schema_,
                         basename_template='part-{{i}}-{}.parquet'.format(poll_number),
                         partition_cols=partitioning,
                         existing_data_behavior='overwrite_or_ignore'
                     )
 
-                poll_number += len(msgs)
                 if args.verbose:
-                    print('Number of alerts polled: {}'.format(poll_number))
+                    if poll_number == 0:
+                        print("%-50s  %9s  %9s" % ("Topic [Partition]", "Committed", "Lag"))
+                        print("=" * 72)
+                        initial_offset, lag = return_offsets(consumer, args.topic, waitfor=5, verbose=True)
+                    elif lag - poll_number >= 0:
+                        # TBD get the last offset commited, and add it
+                        print("%-50s  %9s  %9s" % (
+                            "", initial_offset + poll_number, lag - poll_number))
+                    else:
+                        print('No more alerts found ({} polled)'.format(initial_offset + lag))
+                        break
+                poll_number += len(msgs)
             else:
+                print("%-50s  %9s  %9s" % ("Topic [Partition]", "Committed", "Lag"))
+                print("=" * 72)
+                initial_offset, lag = return_offsets(consumer, args.topic, waitfor=5, verbose=True)
                 print('No alerts the last {} seconds ({} polled)'.format(maxtimeout, poll_number))
     except KeyboardInterrupt:
         sys.stderr.write('%% Aborted by user\n')
     finally:
         consumer.close()
 
+    print(parts)
+
     # remove empty partition
     list_of_dirs = glob.glob(os.path.join(args.outdir, '*'))
     for d_ in list_of_dirs:
         if '__HIVE_DEFAULT_PARTITION__' in d_:
             print('Removing empty partition: {}'.format(d_))
             shutil.rmtree(d_)
```

### Comparing `fink-client-4.4/fink_client/tester.py` & `fink-client-5.0/fink_client/tester.py`

 * *Files identical despite different names*

### Comparing `fink-client-4.4/fink_client/visualisation.py` & `fink-client-5.0/fink_client/visualisation.py`

 * *Files identical despite different names*

### Comparing `fink-client-4.4/fink_client.egg-info/PKG-INFO` & `fink-client-5.0/fink_client.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fink-client
-Version: 4.4
+Version: 5.0
 Summary: Light-weight client to manipulate alerts from Fink
 Home-page: https://fink-broker.readthedocs.io/en/latest/
 Author: AstroLab Software
 Author-email: peloton@lal.in2p3.fr
 License: UNKNOWN
 Project-URL: Documentation, https://fink-broker.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/astrolabsoftware/fink-client
@@ -29,34 +29,36 @@
 
 `fink-client` is a light package to manipulate catalogs and alerts issued from the [fink broker](https://github.com/astrolabsoftware/fink-broker) programmatically. It is used in the context of 2 major Fink services: Livestream and Data Transfer.
 
 ## Installation
 
 `fink_client` requires a version of Python 3.9+.
 
-### install with pip
+### Install with pip
 
 ```bash
 pip install fink-client --upgrade
 ```
 
-### install within a conda environment
+### Use or develop in a controlled environment
 
 ```bash
 git clone https://github.com/astrolabsoftware/fink-client.git
 cd fink-client
 conda env create -f environment.yml
-# install the latest release
-pip install fink-client
+conda activate fink-client
+```
+
+and then install it locally:
+
+```bash
 # install for development
 pip install -e .
 ```
 
-Learn how to connect and use it by checking the [documentation](docs/).
-
 ## Registration
 
 In order to connect and poll alerts from Fink, you need to get your credentials:
 
 1. Subscribe to one or more Fink streams by filling this [form](https://forms.gle/2td4jysT4e9pkf889).
 2. After filling the form, we will send your credentials. Register them on your laptop by simply running:
   ```
@@ -99,37 +101,38 @@
 Display cutouts and lightcurve from a ZTF alert
 
 optional arguments:
   -h, --help          show this help message and exit
   -filename FILENAME  Path to an alert data file (avro format)
 ```
 
-More information at [docs/livestream](docs/livestream_manual.md).
+More information at [docs/livestream](https://fink-broker.readthedocs.io/en/latest/services/livestream).
 
 ## Data Transfer usage
 
 If you requested data using the [Data Transfer service](https://fink-portal.org/download), you can easily poll your stream using:
 
 ```bash
-fink_datatransfer -h
-usage: fink_datatransfer [-h] [-topic TOPIC] [-limit LIMIT] [-outdir OUTDIR] [-partitionby PARTITIONBY] [-batchsize BATCHSIZE] [--restart_from_beginning]
-                            [--verbose]
+usage: fink_datatransfer [-h] [-topic TOPIC] [-limit LIMIT] [-outdir OUTDIR] [-partitionby PARTITIONBY] [-batchsize BATCHSIZE] [-nconsumers NCONSUMERS] [-maxtimeout MAXTIMEOUT] [--restart_from_beginning] [--verbose]
 
 Kafka consumer to listen and archive Fink streams from the data transfer service
 
 optional arguments:
   -h, --help            show this help message and exit
   -topic TOPIC          Topic name for the stream that contains the data.
   -limit LIMIT          If specified, download only `limit` alerts from the stream. Default is None, that is download all alerts.
   -outdir OUTDIR        Folder to store incoming alerts. It will be created if it does not exist.
   -partitionby PARTITIONBY
-                        Partition data by `time` (year=YYYY/month=MM/day=DD), or `finkclass` (finkclass=CLASS), or `tnsclass` (tnsclass=CLASS). Default is
-                        time.
+                        Partition data by `time` (year=YYYY/month=MM/day=DD), or `finkclass` (finkclass=CLASS), or `tnsclass` (tnsclass=CLASS). `classId` is also available for ELASTiCC data. Default is time.
   -batchsize BATCHSIZE  Maximum number of alert within the `maxtimeout` (see conf). Default is 1000 alerts.
+  -nconsumers NCONSUMERS
+                        Number of parallel consumer to use. Default is 1.
+  -maxtimeout MAXTIMEOUT
+                        Overwrite the default timeout (in seconds) from user configuration. Default is None.
   --restart_from_beginning
                         If specified, restart downloading from the 1st alert in the stream. Default is False.
   --verbose             If specified, print on screen information about the consuming.
 
 ```
 
-More information at [docs/datatransfer](docs/datatransfer.md).
+More information at [docs/datatransfer](https://fink-broker.readthedocs.io/en/latest/services/data_transfer/).
```

### Comparing `fink-client-4.4/fink_client.egg-info/SOURCES.txt` & `fink-client-5.0/fink_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,8 +14,10 @@
 fink_client.egg-info/entry_points.txt
 fink_client.egg-info/requires.txt
 fink_client.egg-info/top_level.txt
 fink_client/scripts/__init__.py
 fink_client/scripts/fink_alert_viewer.py
 fink_client/scripts/fink_client_register.py
 fink_client/scripts/fink_consumer.py
-fink_client/scripts/fink_datatransfer.py
+fink_client/scripts/fink_datatransfer.py
+fink_client/scripts/fink_datatransfer_mpi.py
+fink_client/scripts/fink_datatransfer_offsets.py
```

### Comparing `fink-client-4.4/setup.py` & `fink-client-5.0/setup.py`

 * *Files identical despite different names*


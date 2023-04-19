# Comparing `tmp/spark-submit-1.3.0.tar.gz` & `tmp/spark-submit-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\spark-submit-1.3.0.tar", last modified: Sat Jul 30 13:33:37 2022, max compression
+gzip compressed data, was "spark-submit-1.4.0.tar", last modified: Wed Apr 19 11:15:00 2023, max compression
```

## Comparing `spark-submit-1.3.0.tar` & `spark-submit-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-07-30 13:33:37.292280 spark-submit-1.3.0/
--rw-rw-rw-   0        0        0     7740 2022-07-30 13:33:37.290316 spark-submit-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     5289 2022-07-28 08:59:12.000000 spark-submit-1.3.0/README.md
--rw-rw-rw-   0        0        0       42 2022-07-30 13:33:37.292280 spark-submit-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1641 2022-07-25 10:27:42.000000 spark-submit-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-30 13:33:37.273330 spark-submit-1.3.0/spark_submit/
--rw-rw-rw-   0        0        0      666 2022-07-28 12:05:30.000000 spark-submit-1.3.0/spark_submit/__info__.py
--rw-rw-rw-   0        0        0      318 2022-07-28 14:25:12.000000 spark-submit-1.3.0/spark_submit/__init__.py
--rw-rw-rw-   0        0        0     1385 2022-07-20 17:23:16.000000 spark-submit-1.3.0/spark_submit/_defaults.py
--rw-rw-rw-   0        0        0      211 2022-07-20 17:22:08.000000 spark-submit-1.3.0/spark_submit/exceptions.py
--rw-rw-rw-   0        0        0    11744 2022-07-28 14:02:20.000000 spark-submit-1.3.0/spark_submit/sparkjob.py
--rw-rw-rw-   0        0        0     2211 2022-07-28 14:14:38.000000 spark-submit-1.3.0/spark_submit/system.py
-drwxrwxrwx   0        0        0        0 2022-07-30 13:33:37.288290 spark-submit-1.3.0/spark_submit.egg-info/
--rw-rw-rw-   0        0        0     7740 2022-07-30 13:33:36.000000 spark-submit-1.3.0/spark_submit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2022-07-30 13:33:37.000000 spark-submit-1.3.0/spark_submit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-30 13:33:36.000000 spark-submit-1.3.0/spark_submit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-07-30 13:33:36.000000 spark-submit-1.3.0/spark_submit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-07-30 13:33:36.000000 spark-submit-1.3.0/spark_submit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-07-30 13:33:36.000000 spark-submit-1.3.0/spark_submit.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-19 11:15:00.452158 spark-submit-1.4.0/
+-rw-rw-rw-   0        0        0     1070 2022-12-03 16:16:13.000000 spark-submit-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0     6585 2023-04-19 11:15:00.450954 spark-submit-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5428 2022-12-16 21:32:55.000000 spark-submit-1.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 11:15:00.452158 spark-submit-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2022-12-03 15:27:42.000000 spark-submit-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:15:00.428144 spark-submit-1.4.0/spark_submit/
+-rw-rw-rw-   0        0        0      643 2023-04-19 11:06:06.000000 spark-submit-1.4.0/spark_submit/__info__.py
+-rw-rw-rw-   0        0        0      318 2022-12-03 15:25:19.000000 spark-submit-1.4.0/spark_submit/__init__.py
+-rw-rw-rw-   0        0        0     1380 2022-12-16 21:03:26.000000 spark-submit-1.4.0/spark_submit/_defaults.py
+-rw-rw-rw-   0        0        0      297 2022-12-03 15:30:06.000000 spark-submit-1.4.0/spark_submit/exceptions.py
+-rw-rw-rw-   0        0        0    11591 2022-12-17 13:14:59.000000 spark-submit-1.4.0/spark_submit/sparkjob.py
+-rw-rw-rw-   0        0        0     2321 2023-02-17 18:06:49.000000 spark-submit-1.4.0/spark_submit/system.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:15:00.441355 spark-submit-1.4.0/spark_submit.egg-info/
+-rw-rw-rw-   0        0        0     6585 2023-04-19 11:15:00.000000 spark-submit-1.4.0/spark_submit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2023-04-19 11:15:00.000000 spark-submit-1.4.0/spark_submit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 11:15:00.000000 spark-submit-1.4.0/spark_submit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 11:15:00.000000 spark-submit-1.4.0/spark_submit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-19 11:15:00.000000 spark-submit-1.4.0/spark_submit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-19 11:15:00.000000 spark-submit-1.4.0/spark_submit.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-19 11:15:00.448866 spark-submit-1.4.0/tests/
+-rw-rw-rw-   0        0        0        0 2022-12-03 15:44:18.000000 spark-submit-1.4.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      463 2022-12-03 15:29:44.000000 spark-submit-1.4.0/tests/run_integration_test.py
+-rw-rw-rw-   0        0        0     1497 2023-04-19 11:09:31.000000 spark-submit-1.4.0/tests/test_sparkjob.py
+-rw-rw-rw-   0        0        0      486 2022-12-03 15:53:46.000000 spark-submit-1.4.0/tests/test_system.py
```

### Comparing `spark-submit-1.3.0/PKG-INFO` & `spark-submit-1.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,195 +1,201 @@
 Metadata-Version: 2.1
 Name: spark-submit
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python manager for spark-submit jobs
 Home-page: https://github.com/PApostol/spark-submit
 Author: PApostol
 Author-email: foo@bar.com
 Maintainer: PApostol
 License: MIT
-Description: ## Spark-submit
-        
-        [![PyPI version](https://badge.fury.io/py/spark-submit.svg)](https://badge.fury.io/py/spark-submit)
-        [![Downloads](https://static.pepy.tech/personalized-badge/spark-submit?period=month&units=international_system&left_color=grey&right_color=green&left_text=total%20downloads)](https://pepy.tech/project/spark-submit)
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/spark-submit)](https://pypi.org/project/spark-submit/)
-        [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
-        [![License](https://img.shields.io/badge/License-MIT-blue)](#license "Go to license section")
-        [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/PApostol/spark-submit/issues)
-        
-        #### TL;DR: Python manager for spark-submit jobs
-        
-        ### Description
-        This package allows for submission and management of Spark jobs in Python scripts via [Apache Spark's](https://spark.apache.org/) `spark-submit` functionality.
-        
-        ### Installation
-        The easiest way to install is using `pip`:
-        
-        `pip install spark-submit`
-        
-        To install from source:
-        ```
-        git clone https://github.com/PApostol/spark-submit.git
-        cd spark-submit
-        python setup.py install
-        ```
-        
-        For usage details check `help(spark_submit)`.
-        
-        ### Usage Examples
-        Spark arguments can either be provided as keyword arguments or as an unpacked dictionary.
-        
-        ##### Simple example:
-        ```
-        from spark_submit import SparkJob
-        
-        app = SparkJob('/path/some_file.py', master='local', name='simple-test')
-        app.submit()
-        
-        print(app.get_state())
-        ```
-        ##### Another example:
-        ```
-        from spark_submit import SparkJob
-        
-        spark_args = {
-            'master': 'spark://some.spark.master:6066',
-            'deploy_mode': 'cluster',
-            'name': 'spark-submit-app',
-            'class': 'main.Class',
-            'executor_memory': '2G',
-            'executor_cores': '1',
-            'total_executor_cores': '2',
-            'verbose': True,
-            'conf': ["spark.foo.bar='baz'", "spark.x.y='z'"],
-            'main_file_args': '--foo arg1 --bar arg2'
-            }
-        
-        app = SparkJob('s3a://bucket/path/some_file.jar', **spark_args)
-        print(app.get_submit_cmd(multiline=True))
-        
-        # poll state in the background every x seconds with `poll_time=x`
-        app.submit(use_env_vars=True,
-                   extra_env_vars={'PYTHONPATH': '/some/path/'},
-                   poll_time=10
-                   )
-        
-        print(app.get_state()) # 'SUBMITTED'
-        
-        while not app.concluded:
-            # do other stuff...
-            print(app.get_state()) # 'RUNNING'
-        
-        print(app.get_state()) # 'FINISHED'
-        ```
-        
-        #### Examples of `spark-submit` to `spark_args` dictionary:
-        ##### A `client` example:
-        ```
-        ~/spark_home/bin/spark-submit \
-        --master spark://some.spark.master:7077 \
-        --name spark-submit-job \
-        --total-executor-cores 8 \
-        --executor-cores 4 \
-        --executor-memory 4G \
-        --driver-memory 2G \
-        --py-files /some/utils.zip \
-        --files /some/file.json \
-        /path/to/pyspark/file.py --data /path/to/data.csv
-        ```
-        ##### becomes
-        ```
-        spark_args = {
-            'master': 'spark://some.spark.master:7077',
-            'name': 'spark_job_client',
-            'total_executor_cores: '8',
-            'executor_cores': '4',
-            'executor_memory': '4G',
-            'driver_memory': '2G',
-            'py_files': '/some/utils.zip',
-            'files': '/some/file.json',
-            'main_file_args': '--data /path/to/data.csv'
-            }
-        main_file = '/path/to/pyspark/file.py'
-        app = SparkJob(main_file, **spark_args)
-        ```
-        ##### A `cluster` example:
-        ```
-        ~/spark_home/bin/spark-submit \
-        --master spark://some.spark.master:6066 \
-        --deploy-mode cluster \
-        --name spark_job_cluster \
-        --jars "s3a://mybucket/some/file.jar" \
-        --conf "spark.some.conf=foo" \
-        --conf "spark.some.other.conf=bar" \
-        --total-executor-cores 16 \
-        --executor-cores 4 \
-        --executor-memory 4G \
-        --driver-memory 2G \
-        --class my.main.Class \
-        --verbose \
-        s3a://mybucket/file.jar "positional_arg1" "positional_arg2"
-        ```
-        ##### becomes
-        ```
-        spark_args = {
-            'master': 'spark://some.spark.master:6066',
-            'deploy_mode': 'cluster',
-            'name': 'spark_job_cluster',
-            'jars': 's3a://mybucket/some/file.jar',
-            'conf': ["spark.some.conf='foo'", "spark.some.other.conf='bar'"], # note the use of quotes
-            'total_executor_cores: '16',
-            'executor_cores': '4',
-            'executor_memory': '4G',
-            'driver_memory': '2G',
-            'class': 'my.main.Class',
-            'verbose': True,
-            'main_file_args': '"positional_arg1" "positional_arg2"'
-            }
-        main_file = 's3a://mybucket/file.jar'
-        app = SparkJob(main_file, **spark_args)
-        ```
-        
-        #### Testing
-        
-        You can do some simple testing with local mode Spark after cloning the repo:
-        
-        `python tests/run_test.py`
-        
-        Note any additional requirements for running the tests: `pip install -r tests/requirements.txt`
-        
-        #### Additional methods
-        
-        `spark_submit.system_info()`: Collects Spark related system information, such as versions of spark-submit, Scala, Java, PySpark, Python and OS
-        
-        `spark_submit.SparkJob.kill()`: Kills the running Spark job (cluster mode only)
-        
-        `spark_submit.SparkJob.get_code()`: Gets the spark-submit return code
-        
-        `spark_submit.SparkJob.get_output()`: Gets the spark-submit stdout
-        
-        `spark_submit.SparkJob.get_id()`: Gets the spark-submit submission ID
-        
-        
-        ### License
-        
-        Released under [MIT](/LICENSE) by [@PApostol](https://github.com/PApostol).
-        
-        - You can freely modify and reuse.
-        - The original license must be included with copies of this software.
-        - Please link back to this repo if you use a significant portion the source code.
-        
 Keywords: apache,spark,submit
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## Spark-submit
+
+[![PyPI version](https://badge.fury.io/py/spark-submit.svg)](https://badge.fury.io/py/spark-submit)
+[![Downloads](https://static.pepy.tech/personalized-badge/spark-submit?period=month&units=international_system&left_color=grey&right_color=green&left_text=total%20downloads)](https://pepy.tech/project/spark-submit)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/spark-submit)](https://pypi.org/project/spark-submit/)
+[![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
+[![Code style: blue](https://img.shields.io/badge/code%20style-blue-blue.svg)](https://blue.readthedocs.io/)
+[![License](https://img.shields.io/badge/License-MIT-blue)](#license "Go to license section")
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/PApostol/spark-submit/issues)
+
+#### TL;DR: Python manager for spark-submit jobs
+
+### Description
+This package allows for submission and management of Spark jobs in Python scripts via [Apache Spark's](https://spark.apache.org/) `spark-submit` functionality.
+
+### Installation
+The easiest way to install is using `pip`:
+
+`pip install spark-submit`
+
+To install from source:
+```
+git clone https://github.com/PApostol/spark-submit.git
+cd spark-submit
+python setup.py install
+```
+
+For usage details check `help(spark_submit)`.
+
+### Usage Examples
+Spark arguments can either be provided as keyword arguments or as an unpacked dictionary.
+
+##### Simple example:
+```
+from spark_submit import SparkJob
+
+app = SparkJob('/path/some_file.py', master='local', name='simple-test')
+app.submit()
+
+print(app.get_state())
+```
+##### Another example:
+```
+from spark_submit import SparkJob
+
+spark_args = {
+    'master': 'spark://some.spark.master:6066',
+    'deploy_mode': 'cluster',
+    'name': 'spark-submit-app',
+    'class': 'main.Class',
+    'executor_memory': '2G',
+    'executor_cores': '1',
+    'total_executor_cores': '2',
+    'verbose': True,
+    'conf': ["spark.foo.bar='baz'", "spark.x.y='z'"],
+    'main_file_args': '--foo arg1 --bar arg2'
+    }
+
+app = SparkJob('s3a://bucket/path/some_file.jar', **spark_args)
+print(app.get_submit_cmd(multiline=True))
+
+# poll state in the background every x seconds with `poll_time=x`
+app.submit(use_env_vars=True,
+           extra_env_vars={'PYTHONPATH': '/some/path/'},
+           poll_time=10
+           )
+
+print(app.get_state()) # 'SUBMITTED'
+
+while not app.concluded:
+    # do other stuff...
+    print(app.get_state()) # 'RUNNING'
+
+print(app.get_state()) # 'FINISHED'
+```
+
+#### Examples of `spark-submit` to `spark_args` dictionary:
+##### A `client` example:
+```
+~/spark_home/bin/spark-submit \
+--master spark://some.spark.master:7077 \
+--name spark-submit-job \
+--total-executor-cores 8 \
+--executor-cores 4 \
+--executor-memory 4G \
+--driver-memory 2G \
+--py-files /some/utils.zip \
+--files /some/file.json \
+/path/to/pyspark/file.py --data /path/to/data.csv
+```
+##### becomes
+```
+spark_args = {
+    'master': 'spark://some.spark.master:7077',
+    'name': 'spark_job_client',
+    'total_executor_cores: '8',
+    'executor_cores': '4',
+    'executor_memory': '4G',
+    'driver_memory': '2G',
+    'py_files': '/some/utils.zip',
+    'files': '/some/file.json',
+    'main_file_args': '--data /path/to/data.csv'
+    }
+main_file = '/path/to/pyspark/file.py'
+app = SparkJob(main_file, **spark_args)
+```
+##### A `cluster` example:
+```
+~/spark_home/bin/spark-submit \
+--master spark://some.spark.master:6066 \
+--deploy-mode cluster \
+--name spark_job_cluster \
+--jars "s3a://mybucket/some/file.jar" \
+--conf "spark.some.conf=foo" \
+--conf "spark.some.other.conf=bar" \
+--total-executor-cores 16 \
+--executor-cores 4 \
+--executor-memory 4G \
+--driver-memory 2G \
+--class my.main.Class \
+--verbose \
+s3a://mybucket/file.jar "positional_arg1" "positional_arg2"
+```
+##### becomes
+```
+spark_args = {
+    'master': 'spark://some.spark.master:6066',
+    'deploy_mode': 'cluster',
+    'name': 'spark_job_cluster',
+    'jars': 's3a://mybucket/some/file.jar',
+    'conf': ["spark.some.conf='foo'", "spark.some.other.conf='bar'"], # note the use of quotes
+    'total_executor_cores: '16',
+    'executor_cores': '4',
+    'executor_memory': '4G',
+    'driver_memory': '2G',
+    'class': 'my.main.Class',
+    'verbose': True,
+    'main_file_args': '"positional_arg1" "positional_arg2"'
+    }
+main_file = 's3a://mybucket/file.jar'
+app = SparkJob(main_file, **spark_args)
+```
+
+#### Testing
+
+You can do some simple testing with local mode Spark after cloning the repo.
+
+Note any additional requirements for running the tests: `pip install -r tests/requirements.txt`
+
+`pytest tests/`
+
+`python tests/run_integration_test.py`
+
+
+#### Additional methods
+
+`spark_submit.system_info()`: Collects Spark related system information, such as versions of spark-submit, Scala, Java, PySpark, Python and OS
+
+`spark_submit.SparkJob.kill()`: Kills the running Spark job (cluster mode only)
+
+`spark_submit.SparkJob.get_code()`: Gets the spark-submit return code
+
+`spark_submit.SparkJob.get_output()`: Gets the spark-submit stdout
+
+`spark_submit.SparkJob.get_id()`: Gets the spark-submit submission ID
+
+
+### License
+
+Released under [MIT](/LICENSE) by [@PApostol](https://github.com/PApostol).
+
+- You can freely modify and reuse.
+- The original license must be included with copies of this software.
+- Please link back to this repo if you use a significant portion the source code.
```

### Comparing `spark-submit-1.3.0/README.md` & `spark-submit-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ## Spark-submit
 
 [![PyPI version](https://badge.fury.io/py/spark-submit.svg)](https://badge.fury.io/py/spark-submit)
 [![Downloads](https://static.pepy.tech/personalized-badge/spark-submit?period=month&units=international_system&left_color=grey&right_color=green&left_text=total%20downloads)](https://pepy.tech/project/spark-submit)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/spark-submit)](https://pypi.org/project/spark-submit/)
 [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
+[![Code style: blue](https://img.shields.io/badge/code%20style-blue-blue.svg)](https://blue.readthedocs.io/)
 [![License](https://img.shields.io/badge/License-MIT-blue)](#license "Go to license section")
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/PApostol/spark-submit/issues)
 
 #### TL;DR: Python manager for spark-submit jobs
 
 ### Description
 This package allows for submission and management of Spark jobs in Python scripts via [Apache Spark's](https://spark.apache.org/) `spark-submit` functionality.
@@ -138,20 +139,23 @@
     }
 main_file = 's3a://mybucket/file.jar'
 app = SparkJob(main_file, **spark_args)
 ```
 
 #### Testing
 
-You can do some simple testing with local mode Spark after cloning the repo:
-
-`python tests/run_test.py`
+You can do some simple testing with local mode Spark after cloning the repo.
 
 Note any additional requirements for running the tests: `pip install -r tests/requirements.txt`
 
+`pytest tests/`
+
+`python tests/run_integration_test.py`
+
+
 #### Additional methods
 
 `spark_submit.system_info()`: Collects Spark related system information, such as versions of spark-submit, Scala, Java, PySpark, Python and OS
 
 `spark_submit.SparkJob.kill()`: Kills the running Spark job (cluster mode only)
 
 `spark_submit.SparkJob.get_code()`: Gets the spark-submit return code
```

### Comparing `spark-submit-1.3.0/setup.py` & `spark-submit-1.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """spark-submit module installation script"""
 import os
 from typing import Dict
 
 from setuptools import find_packages, setup
 
-info_location = os.path.join(os.path.abspath(os.path.dirname(__file__)),
-                             'spark_submit',
-                             '__info__.py'
-                             )
+info_location = os.path.join(os.path.abspath(os.path.dirname(__file__)), 'spark_submit', '__info__.py')
 about: Dict[str, str] = {}
 
 with open(info_location, 'r', encoding='utf-8') as f:
     exec(f.read(), about)
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
@@ -36,14 +33,15 @@
         'License :: OSI Approved :: MIT License',
         'Topic :: Software Development :: Libraries',
         'Topic :: Utilities',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Operating System :: OS Independent',
     ],
     zip_safe=True,
     platforms=['any'],
     python_requires='~=3.7',
     keywords=['apache', 'spark', 'submit'],
```

### Comparing `spark-submit-1.3.0/spark_submit/__info__.py` & `spark-submit-1.4.0/spark_submit/__info__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-r"""                       __                    __              _ __
+r"""__                    __              _ __
    _________  ____ ______/ /__      _______  __/ /_  ____ ___  (_) /_
   / ___/ __ \/ __ `/ ___/ //_/_____/ ___/ / / / __ \/ __ `__ \/ / __/
  (__  ) /_/ / /_/ / /  / ,< /_____(__  ) /_/ / /_/ / / / / / / / /_
 /____/ .___/\__,_/_/  /_/|_|     /____/\__,_/_.___/_/ /_/ /_/_/\__/
     /_/
 """
 
 __title__ = 'spark-submit'
 __author__ = 'PApostol'
 __author_email__ = 'foo@bar.com'
 __maintainer__ = 'PApostol'
 __license__ = 'MIT'
-__version__ = '1.3.0'
+__version__ = '1.4.0'
 __description__ = 'Python manager for spark-submit jobs'
 __url__ = f'https://github.com/{__author__}/{__title__}'
 __bugtrack_url__ = f'{__url__}/issues'
```

### Comparing `spark-submit-1.3.0/spark_submit/_defaults.py` & `spark-submit-1.4.0/spark_submit/_defaults.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Some basic default spark-submit arguments and driver end states"""
 import os
 from typing import Any, Dict, Set
 
 __defaults__: Dict[str, Any] = {
-    'spark_home': os.environ.get('SPARK_HOME', os.path.expanduser('~/spark_home')),
+    'spark_home': os.getenv('SPARK_HOME', os.path.expanduser('~/spark_home')),
     'master': 'local[*]',
     'name': 'spark-submit-task',
     'deploy_mode': 'client',
     'driver_memory': '1g',
     'executor_memory': '1g',
     'executor_cores': '1',
     'total_executor_cores': '2',
```

### Comparing `spark-submit-1.3.0/spark_submit/sparkjob.py` & `spark-submit-1.4.0/spark_submit/sparkjob.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             raise FileNotFoundError(
                 f'bin/spark-submit was not found in "{spark_home}". '
                 f'Please add SPARK_HOME to path or provide it as a keyword argument: spark_home'
             )
 
         self.env_vars = os.environ.copy()
         if 'JAVA_HOME' not in self.env_vars:
-            logging.warning('"JAVA_HOME" is not defined in environment variables.')
+            logging.warning('JAVA_HOME is not defined in environment variables.')
 
         self.is_yarn = 'yarn' in self.spark_args['master']
         self.is_k8s = 'k8s' in self.spark_args['master']
 
         self.submit_cmd = self._get_submit_cmd()
         self.submit_response: Dict[str, Any] = {
             'output': '',
@@ -74,32 +74,22 @@
 
         args = [
             f"--{arg.replace('_', '-')} {val}"
             for arg, val in self.spark_args.items()
             if arg not in exclude and val is not None
         ]
         confs = [f'--conf {c}' for c in self.spark_args['conf']]
+        boolean_args = [f"--{arg.replace('_', '-')}" for arg in booleans if self.spark_args[arg]]
 
-        booleans_str = ''
-        for arg in booleans:
-            if self.spark_args[arg]:
-                booleans_str += '--' + arg.replace('_', '-')
-
-        cmd = (
-            self.spark_bin
-            + ' '.join(args)
-            + booleans_str
-            + ' '.join(confs)
-            + ' '
-            + self.spark_args['main_file']
-            + ' '
-            + str(self.spark_args['main_file_args'])
-        )
+        args_str = ' '.join(args)
+        bool_str = ' '.join(boolean_args)
+        conf_str = ' '.join(confs)
 
-        return cmd.replace('--', ' --').replace('  ', ' ').strip()
+        cmd = f"{self.spark_bin} {args_str} {bool_str} {conf_str} {self.spark_args['main_file']} {self.spark_args['main_file_args']}"
+        return cmd
 
     def _get_api_url(self, endpoint: str) -> str:
         return f"{self.spark_args['master'].replace('spark://', 'http://')}/v1/submissions/{endpoint}/{self.get_id()}"
 
     def _get_status_response(self) -> str:
         if self.is_yarn:
             status_cmd = f'yarn application -status {self.get_id()}'
@@ -147,20 +137,22 @@
             kill_cmd = f"{self.spark_bin} --master {self.spark_args['master']} --kill {self.get_id()}"
             return _execute_cmd(kill_cmd)
 
         kill_url = self._get_api_url('kill')
         resp = requests.get(kill_url)
         return resp.text, resp.status_code
 
-    def submit(self, *,
-               use_env_vars: bool = False,
-               extra_env_vars: Optional[Dict[str, str]] = None,
-               poll_time: int = 0,
-               timeout: Optional[int] = None
-               ) -> None:
+    def submit(
+        self,
+        *,
+        use_env_vars: bool = False,
+        extra_env_vars: Optional[Dict[str, str]] = None,
+        poll_time: int = 0,
+        timeout: Optional[int] = None,
+    ) -> None:
         """Submits the current Spark job to Spark master.
            If `use_env_vars=True`, the host environment variables in `os.environ` will be used
            with the spark-submit shell.
            Additional environment variables can be supplied with the dictionary `extra_env_vars`
            as key-value pairs (if `use_env_vars=True`, any common keys between `os.environ` and
            `extra_env_vars` will be overwritten by the latter).
            The state of the Spark job can be  polled and updated in the background if a positive
```

### Comparing `spark-submit-1.3.0/spark_submit/system.py` & `spark-submit-1.4.0/spark_submit/system.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,18 +33,19 @@
     Returns:
         str: system information
     """
 
     def _quote_spaces(text: str) -> str:
         return f'"{text}"' if ' ' in text else text
 
-    spark_home = os.environ.get('SPARK_HOME', os.path.expanduser('~/spark_home')).replace(os.path.sep, '/')
-    info_cmd = f'{_quote_spaces(spark_home)}/bin/spark-submit --version'
+    spark_home = os.getenv('SPARK_HOME', os.path.expanduser('~/spark_home')).replace(os.path.sep, '/')
+    spark_bin = _quote_spaces(f'{spark_home}/bin/spark-submit')
+    info_cmd = f'{spark_bin} --version'
 
-    java_home = os.environ.get('JAVA_HOME', '').replace(os.path.sep, '/')
+    java_home = os.getenv('JAVA_HOME', '').replace(os.path.sep, '/')
     if java_home:
         java_bin = f'{java_home}/bin/java'
         info_cmd += f' ; {_quote_spaces(java_bin)} -version'
     else:
         info_cmd += ' ; java -version'
 
     info_cmd += f' ; {_quote_spaces(sys.executable)} -m pip show pyspark'
@@ -57,14 +58,16 @@
         'Scala version': 'scala version (.+?),',
         'Java version': 'version "(.+)"',
         'PySpark version': 'Version: (.+)',
     }
 
     sys_info: Dict[str, str] = {}
     for key, val in info_re.items():
-        i = re.findall(val, info_stdout, re.IGNORECASE)
-        if i:
-            sys_info[key] = i[0].strip()
+        match = re.findall(val, info_stdout, re.IGNORECASE)
+        if match:
+            sys_info[key] = match[0].strip()
+        else:
+            sys_info[key] = key.split(' ')[0] + ' not detected!'
 
     sys_info['Python version'] = sys.version.split(' ', maxsplit=1)[0]
     sys_info['OS'] = platform.platform()
-    return '\n'.join([f'{key}: {val}' for key, val in sys_info.items()])
+    return '\n'.join(f'{key}: {val}' for key, val in sys_info.items())
```

### Comparing `spark-submit-1.3.0/spark_submit.egg-info/PKG-INFO` & `spark-submit-1.4.0/spark_submit.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,195 +1,201 @@
 Metadata-Version: 2.1
 Name: spark-submit
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python manager for spark-submit jobs
 Home-page: https://github.com/PApostol/spark-submit
 Author: PApostol
 Author-email: foo@bar.com
 Maintainer: PApostol
 License: MIT
-Description: ## Spark-submit
-        
-        [![PyPI version](https://badge.fury.io/py/spark-submit.svg)](https://badge.fury.io/py/spark-submit)
-        [![Downloads](https://static.pepy.tech/personalized-badge/spark-submit?period=month&units=international_system&left_color=grey&right_color=green&left_text=total%20downloads)](https://pepy.tech/project/spark-submit)
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/spark-submit)](https://pypi.org/project/spark-submit/)
-        [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
-        [![License](https://img.shields.io/badge/License-MIT-blue)](#license "Go to license section")
-        [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/PApostol/spark-submit/issues)
-        
-        #### TL;DR: Python manager for spark-submit jobs
-        
-        ### Description
-        This package allows for submission and management of Spark jobs in Python scripts via [Apache Spark's](https://spark.apache.org/) `spark-submit` functionality.
-        
-        ### Installation
-        The easiest way to install is using `pip`:
-        
-        `pip install spark-submit`
-        
-        To install from source:
-        ```
-        git clone https://github.com/PApostol/spark-submit.git
-        cd spark-submit
-        python setup.py install
-        ```
-        
-        For usage details check `help(spark_submit)`.
-        
-        ### Usage Examples
-        Spark arguments can either be provided as keyword arguments or as an unpacked dictionary.
-        
-        ##### Simple example:
-        ```
-        from spark_submit import SparkJob
-        
-        app = SparkJob('/path/some_file.py', master='local', name='simple-test')
-        app.submit()
-        
-        print(app.get_state())
-        ```
-        ##### Another example:
-        ```
-        from spark_submit import SparkJob
-        
-        spark_args = {
-            'master': 'spark://some.spark.master:6066',
-            'deploy_mode': 'cluster',
-            'name': 'spark-submit-app',
-            'class': 'main.Class',
-            'executor_memory': '2G',
-            'executor_cores': '1',
-            'total_executor_cores': '2',
-            'verbose': True,
-            'conf': ["spark.foo.bar='baz'", "spark.x.y='z'"],
-            'main_file_args': '--foo arg1 --bar arg2'
-            }
-        
-        app = SparkJob('s3a://bucket/path/some_file.jar', **spark_args)
-        print(app.get_submit_cmd(multiline=True))
-        
-        # poll state in the background every x seconds with `poll_time=x`
-        app.submit(use_env_vars=True,
-                   extra_env_vars={'PYTHONPATH': '/some/path/'},
-                   poll_time=10
-                   )
-        
-        print(app.get_state()) # 'SUBMITTED'
-        
-        while not app.concluded:
-            # do other stuff...
-            print(app.get_state()) # 'RUNNING'
-        
-        print(app.get_state()) # 'FINISHED'
-        ```
-        
-        #### Examples of `spark-submit` to `spark_args` dictionary:
-        ##### A `client` example:
-        ```
-        ~/spark_home/bin/spark-submit \
-        --master spark://some.spark.master:7077 \
-        --name spark-submit-job \
-        --total-executor-cores 8 \
-        --executor-cores 4 \
-        --executor-memory 4G \
-        --driver-memory 2G \
-        --py-files /some/utils.zip \
-        --files /some/file.json \
-        /path/to/pyspark/file.py --data /path/to/data.csv
-        ```
-        ##### becomes
-        ```
-        spark_args = {
-            'master': 'spark://some.spark.master:7077',
-            'name': 'spark_job_client',
-            'total_executor_cores: '8',
-            'executor_cores': '4',
-            'executor_memory': '4G',
-            'driver_memory': '2G',
-            'py_files': '/some/utils.zip',
-            'files': '/some/file.json',
-            'main_file_args': '--data /path/to/data.csv'
-            }
-        main_file = '/path/to/pyspark/file.py'
-        app = SparkJob(main_file, **spark_args)
-        ```
-        ##### A `cluster` example:
-        ```
-        ~/spark_home/bin/spark-submit \
-        --master spark://some.spark.master:6066 \
-        --deploy-mode cluster \
-        --name spark_job_cluster \
-        --jars "s3a://mybucket/some/file.jar" \
-        --conf "spark.some.conf=foo" \
-        --conf "spark.some.other.conf=bar" \
-        --total-executor-cores 16 \
-        --executor-cores 4 \
-        --executor-memory 4G \
-        --driver-memory 2G \
-        --class my.main.Class \
-        --verbose \
-        s3a://mybucket/file.jar "positional_arg1" "positional_arg2"
-        ```
-        ##### becomes
-        ```
-        spark_args = {
-            'master': 'spark://some.spark.master:6066',
-            'deploy_mode': 'cluster',
-            'name': 'spark_job_cluster',
-            'jars': 's3a://mybucket/some/file.jar',
-            'conf': ["spark.some.conf='foo'", "spark.some.other.conf='bar'"], # note the use of quotes
-            'total_executor_cores: '16',
-            'executor_cores': '4',
-            'executor_memory': '4G',
-            'driver_memory': '2G',
-            'class': 'my.main.Class',
-            'verbose': True,
-            'main_file_args': '"positional_arg1" "positional_arg2"'
-            }
-        main_file = 's3a://mybucket/file.jar'
-        app = SparkJob(main_file, **spark_args)
-        ```
-        
-        #### Testing
-        
-        You can do some simple testing with local mode Spark after cloning the repo:
-        
-        `python tests/run_test.py`
-        
-        Note any additional requirements for running the tests: `pip install -r tests/requirements.txt`
-        
-        #### Additional methods
-        
-        `spark_submit.system_info()`: Collects Spark related system information, such as versions of spark-submit, Scala, Java, PySpark, Python and OS
-        
-        `spark_submit.SparkJob.kill()`: Kills the running Spark job (cluster mode only)
-        
-        `spark_submit.SparkJob.get_code()`: Gets the spark-submit return code
-        
-        `spark_submit.SparkJob.get_output()`: Gets the spark-submit stdout
-        
-        `spark_submit.SparkJob.get_id()`: Gets the spark-submit submission ID
-        
-        
-        ### License
-        
-        Released under [MIT](/LICENSE) by [@PApostol](https://github.com/PApostol).
-        
-        - You can freely modify and reuse.
-        - The original license must be included with copies of this software.
-        - Please link back to this repo if you use a significant portion the source code.
-        
 Keywords: apache,spark,submit
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## Spark-submit
+
+[![PyPI version](https://badge.fury.io/py/spark-submit.svg)](https://badge.fury.io/py/spark-submit)
+[![Downloads](https://static.pepy.tech/personalized-badge/spark-submit?period=month&units=international_system&left_color=grey&right_color=green&left_text=total%20downloads)](https://pepy.tech/project/spark-submit)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/spark-submit)](https://pypi.org/project/spark-submit/)
+[![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
+[![Code style: blue](https://img.shields.io/badge/code%20style-blue-blue.svg)](https://blue.readthedocs.io/)
+[![License](https://img.shields.io/badge/License-MIT-blue)](#license "Go to license section")
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/PApostol/spark-submit/issues)
+
+#### TL;DR: Python manager for spark-submit jobs
+
+### Description
+This package allows for submission and management of Spark jobs in Python scripts via [Apache Spark's](https://spark.apache.org/) `spark-submit` functionality.
+
+### Installation
+The easiest way to install is using `pip`:
+
+`pip install spark-submit`
+
+To install from source:
+```
+git clone https://github.com/PApostol/spark-submit.git
+cd spark-submit
+python setup.py install
+```
+
+For usage details check `help(spark_submit)`.
+
+### Usage Examples
+Spark arguments can either be provided as keyword arguments or as an unpacked dictionary.
+
+##### Simple example:
+```
+from spark_submit import SparkJob
+
+app = SparkJob('/path/some_file.py', master='local', name='simple-test')
+app.submit()
+
+print(app.get_state())
+```
+##### Another example:
+```
+from spark_submit import SparkJob
+
+spark_args = {
+    'master': 'spark://some.spark.master:6066',
+    'deploy_mode': 'cluster',
+    'name': 'spark-submit-app',
+    'class': 'main.Class',
+    'executor_memory': '2G',
+    'executor_cores': '1',
+    'total_executor_cores': '2',
+    'verbose': True,
+    'conf': ["spark.foo.bar='baz'", "spark.x.y='z'"],
+    'main_file_args': '--foo arg1 --bar arg2'
+    }
+
+app = SparkJob('s3a://bucket/path/some_file.jar', **spark_args)
+print(app.get_submit_cmd(multiline=True))
+
+# poll state in the background every x seconds with `poll_time=x`
+app.submit(use_env_vars=True,
+           extra_env_vars={'PYTHONPATH': '/some/path/'},
+           poll_time=10
+           )
+
+print(app.get_state()) # 'SUBMITTED'
+
+while not app.concluded:
+    # do other stuff...
+    print(app.get_state()) # 'RUNNING'
+
+print(app.get_state()) # 'FINISHED'
+```
+
+#### Examples of `spark-submit` to `spark_args` dictionary:
+##### A `client` example:
+```
+~/spark_home/bin/spark-submit \
+--master spark://some.spark.master:7077 \
+--name spark-submit-job \
+--total-executor-cores 8 \
+--executor-cores 4 \
+--executor-memory 4G \
+--driver-memory 2G \
+--py-files /some/utils.zip \
+--files /some/file.json \
+/path/to/pyspark/file.py --data /path/to/data.csv
+```
+##### becomes
+```
+spark_args = {
+    'master': 'spark://some.spark.master:7077',
+    'name': 'spark_job_client',
+    'total_executor_cores: '8',
+    'executor_cores': '4',
+    'executor_memory': '4G',
+    'driver_memory': '2G',
+    'py_files': '/some/utils.zip',
+    'files': '/some/file.json',
+    'main_file_args': '--data /path/to/data.csv'
+    }
+main_file = '/path/to/pyspark/file.py'
+app = SparkJob(main_file, **spark_args)
+```
+##### A `cluster` example:
+```
+~/spark_home/bin/spark-submit \
+--master spark://some.spark.master:6066 \
+--deploy-mode cluster \
+--name spark_job_cluster \
+--jars "s3a://mybucket/some/file.jar" \
+--conf "spark.some.conf=foo" \
+--conf "spark.some.other.conf=bar" \
+--total-executor-cores 16 \
+--executor-cores 4 \
+--executor-memory 4G \
+--driver-memory 2G \
+--class my.main.Class \
+--verbose \
+s3a://mybucket/file.jar "positional_arg1" "positional_arg2"
+```
+##### becomes
+```
+spark_args = {
+    'master': 'spark://some.spark.master:6066',
+    'deploy_mode': 'cluster',
+    'name': 'spark_job_cluster',
+    'jars': 's3a://mybucket/some/file.jar',
+    'conf': ["spark.some.conf='foo'", "spark.some.other.conf='bar'"], # note the use of quotes
+    'total_executor_cores: '16',
+    'executor_cores': '4',
+    'executor_memory': '4G',
+    'driver_memory': '2G',
+    'class': 'my.main.Class',
+    'verbose': True,
+    'main_file_args': '"positional_arg1" "positional_arg2"'
+    }
+main_file = 's3a://mybucket/file.jar'
+app = SparkJob(main_file, **spark_args)
+```
+
+#### Testing
+
+You can do some simple testing with local mode Spark after cloning the repo.
+
+Note any additional requirements for running the tests: `pip install -r tests/requirements.txt`
+
+`pytest tests/`
+
+`python tests/run_integration_test.py`
+
+
+#### Additional methods
+
+`spark_submit.system_info()`: Collects Spark related system information, such as versions of spark-submit, Scala, Java, PySpark, Python and OS
+
+`spark_submit.SparkJob.kill()`: Kills the running Spark job (cluster mode only)
+
+`spark_submit.SparkJob.get_code()`: Gets the spark-submit return code
+
+`spark_submit.SparkJob.get_output()`: Gets the spark-submit stdout
+
+`spark_submit.SparkJob.get_id()`: Gets the spark-submit submission ID
+
+
+### License
+
+Released under [MIT](/LICENSE) by [@PApostol](https://github.com/PApostol).
+
+- You can freely modify and reuse.
+- The original license must be included with copies of this software.
+- Please link back to this repo if you use a significant portion the source code.
```


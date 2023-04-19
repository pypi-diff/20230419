# Comparing `tmp/avro-helper-devlibx-0.2.2.tar.gz` & `tmp/avro-helper-devlibx-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avro-helper-devlibx-0.2.2.tar", last modified: Fri Mar 31 12:45:52 2023, max compression
+gzip compressed data, was "avro-helper-devlibx-0.2.3.tar", last modified: Wed Apr 19 07:06:35 2023, max compression
```

## Comparing `avro-helper-devlibx-0.2.2.tar` & `avro-helper-devlibx-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:45:52.471136 avro-helper-devlibx-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-03-31 12:45:52.471136 avro-helper-devlibx-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13570 2023-03-31 12:45:40.000000 avro-helper-devlibx-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:45:52.467136 avro-helper-devlibx-0.2.2/avro_helper_devlibx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-03-31 12:45:52.000000 avro-helper-devlibx-0.2.2/avro_helper_devlibx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-31 12:45:52.000000 avro-helper-devlibx-0.2.2/avro_helper_devlibx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 12:45:52.000000 avro-helper-devlibx-0.2.2/avro_helper_devlibx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-31 12:45:52.000000 avro-helper-devlibx-0.2.2/avro_helper_devlibx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-31 12:45:52.000000 avro-helper-devlibx-0.2.2/avro_helper_devlibx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 12:45:52.467136 avro-helper-devlibx-0.2.2/devlibx_avro_helper/
--rw-r--r--   0 runner    (1001) docker     (123)    19146 2023-03-31 12:45:40.000000 avro-helper-devlibx-0.2.2/devlibx_avro_helper/month_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-03-31 12:45:40.000000 avro-helper-devlibx-0.2.2/devlibx_avro_helper/month_data_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23972 2023-03-31 12:45:40.000000 avro-helper-devlibx-0.2.2/devlibx_avro_helper/test_month_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-03-31 12:45:40.000000 avro-helper-devlibx-0.2.2/devlibx_avro_helper/test_month_data_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-31 12:45:40.000000 avro-helper-devlibx-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 12:45:52.471136 avro-helper-devlibx-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-31 12:45:40.000000 avro-helper-devlibx-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:06:35.261871 avro-helper-devlibx-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-04-19 07:06:35.261871 avro-helper-devlibx-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13570 2023-04-19 07:06:24.000000 avro-helper-devlibx-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:06:35.257871 avro-helper-devlibx-0.2.3/avro_helper_devlibx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-04-19 07:06:35.000000 avro-helper-devlibx-0.2.3/avro_helper_devlibx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-19 07:06:35.000000 avro-helper-devlibx-0.2.3/avro_helper_devlibx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 07:06:35.000000 avro-helper-devlibx-0.2.3/avro_helper_devlibx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 07:06:35.000000 avro-helper-devlibx-0.2.3/avro_helper_devlibx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-19 07:06:35.000000 avro-helper-devlibx-0.2.3/avro_helper_devlibx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:06:35.257871 avro-helper-devlibx-0.2.3/devlibx_avro_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)    19146 2023-04-19 07:06:24.000000 avro-helper-devlibx-0.2.3/devlibx_avro_helper/month_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-04-19 07:06:24.000000 avro-helper-devlibx-0.2.3/devlibx_avro_helper/month_data_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23972 2023-04-19 07:06:24.000000 avro-helper-devlibx-0.2.3/devlibx_avro_helper/test_month_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-04-19 07:06:24.000000 avro-helper-devlibx-0.2.3/devlibx_avro_helper/test_month_data_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 07:06:24.000000 avro-helper-devlibx-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 07:06:35.261871 avro-helper-devlibx-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-19 07:06:24.000000 avro-helper-devlibx-0.2.3/setup.py
```

### Comparing `avro-helper-devlibx-0.2.2/PKG-INFO` & `avro-helper-devlibx-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro-helper-devlibx
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python DSL for setting up Flask app CDC
 Home-page: https://github.com/devlibx/avro-helper-py
 Author: devlibx
 Author-email: devlibxgithub@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `avro-helper-devlibx-0.2.2/README.md` & `avro-helper-devlibx-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `avro-helper-devlibx-0.2.2/avro_helper_devlibx.egg-info/PKG-INFO` & `avro-helper-devlibx-0.2.3/avro_helper_devlibx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro-helper-devlibx
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python DSL for setting up Flask app CDC
 Home-page: https://github.com/devlibx/avro-helper-py
 Author: devlibx
 Author-email: devlibxgithub@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `avro-helper-devlibx-0.2.2/devlibx_avro_helper/month_data.py` & `avro-helper-devlibx-0.2.3/devlibx_avro_helper/month_data.py`

 * *Files identical despite different names*

### Comparing `avro-helper-devlibx-0.2.2/devlibx_avro_helper/month_data_v1.py` & `avro-helper-devlibx-0.2.3/devlibx_avro_helper/month_data_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import json
 from datetime import datetime
 from datetime import timedelta
 
 
-def get_keys_for_current_week_for_day_aggregation_from_given_time(time):
+def get_keys_for_current_week_for_day_aggregation_from_given_time(time, week_start):
     """
     Give key week given by time - which are then used to aggregate data
     :param time: week to use
     :return: array containing keys for this week (including given time)
     """
     result = []
     end = time
-    start = time.replace(minute=0, hour=0, second=0, microsecond=0) - timedelta(days=time.weekday())
+    d_diff = time.weekday()
+    d_diff = d_diff + (7 - week_start) if d_diff < week_start else d_diff - week_start
+    start = time.replace(minute=0, hour=0, second=0, microsecond=0)-timedelta(days=d_diff)
     while start <= end:
         result.append("{}-{}".format(start.month, start.day))
         start = start + timedelta(days=1)
     return result
 
 
 def get_keys_for_current_two_week_for_day_aggregation_from_given_time(time):
@@ -121,26 +123,27 @@
 
         if len(self.minutes) > 0:
             print("Minutes Aggregations")
             print(self.minutes)
 
         print("-------------------------------------- End: Data ----------------------------------------------------")
 
-    def get_current_week_numeric_aggregation_from_given_time(self, time, aggregate=True, aggregation_key="days"):
+    def get_current_week_numeric_aggregation_from_given_time(self, time, week_start=0, aggregate=True, aggregation_key="days"):
         """
         This method will give you data for current week.
 
         :param aggregation_key:  days, days_hour [currently only days is supported]
         :param time: from [start of this week <--> the time given]
         :param aggregate: aggregation or raw values
+        :param week_start: day considered to be the start of the week, default 0 (Monday), range [0, 6]
         :return: if aggregate=True, then single numeric value of the total, otherwise array of values
         """
 
         # Find the keys
-        keys = get_keys_for_current_week_for_day_aggregation_from_given_time(time)
+        keys = get_keys_for_current_week_for_day_aggregation_from_given_time(time, week_start)
 
         # Find data with all keys
         result = []
         for day in keys:
             try:
                 if aggregation_key == "days":
                     result.append(self.days[day])
@@ -152,24 +155,24 @@
             return result
         else:
             sum = 0
             for i in result:
                 sum = sum + i
             return sum
 
-    def get_current_week_numeric_aggregation_from_now(self, aggregate=True, aggregation_key="days"):
+    def get_current_week_numeric_aggregation_from_now(self, week_start=0, aggregate=True, aggregation_key="days"):
         """
         This method will give you data for current week.
 
         :param aggregation_key:  days, days_hour [currently only days is supported]
         :param aggregate: aggregation or raw values
         :return: if aggregate=True, then single numeric value of the total, otherwise array of values
         """
 
-        return self.get_current_week_numeric_aggregation_from_given_time(datetime.now(), aggregate, aggregation_key)
+        return self.get_current_week_numeric_aggregation_from_given_time(datetime.now(), week_start, aggregate, aggregation_key)
 
     def get_current_two_week_numeric_aggregation_from_given_time(self, time, aggregate=True, aggregation_key="days"):
         """
         This method will give you data for current week plus the last week.
 
         :param aggregation_key:  days, days_hour [currently only days is supported]
         :param time: from [start of last week <--> the time given]
```

### Comparing `avro-helper-devlibx-0.2.2/devlibx_avro_helper/test_month_data.py` & `avro-helper-devlibx-0.2.3/devlibx_avro_helper/test_month_data.py`

 * *Files identical despite different names*

### Comparing `avro-helper-devlibx-0.2.2/devlibx_avro_helper/test_month_data_v1.py` & `avro-helper-devlibx-0.2.3/devlibx_avro_helper/test_month_data_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         # This is the data you will get from DB or some other place
         inputDataFromDB = '''
                       {"updated_at":1663665518937,"days":{"9-5":3,"9-6":1,"9-10":2,"9-11":1,"9-13":1}}
                       '''
         helper = MonthDataAvroHelperV1(inputDataFromDB)
 
         # Check with aggregate=False
-        result = helper.get_current_month_numeric_aggregation_from_given_time(
+        result = helper.get_current_week_numeric_aggregation_from_given_time(
             date_time_obj_for_this_test,
             aggregate=False
         )
         self.assertEqual(3, result[0])
         print(result)
 
         # Check with aggregate=True
```

### Comparing `avro-helper-devlibx-0.2.2/setup.py` & `avro-helper-devlibx-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 """
 
 description = 'Python DSL for setting up Flask app CDC'
 
 setuptools.setup(
     name='avro-helper-devlibx',
-    version="0.2.2",
+    version="0.2.3",
     description='{0}\n\n{1}'.format(description, history),
     long_description_content_type="text/markdown",
     long_description=open("README.md").read(),
     author='devlibx',
     author_email='devlibxgithub@gmail.com',
     url='https://github.com/devlibx/avro-helper-py',
     packages=['devlibx_avro_helper'],
```


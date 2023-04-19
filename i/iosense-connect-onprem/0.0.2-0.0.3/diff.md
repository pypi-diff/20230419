# Comparing `tmp/iosense_connect_onprem-0.0.2.tar.gz` & `tmp/iosense_connect_onprem-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect_onprem-0.0.2.tar", last modified: Tue Apr 18 05:58:17 2023, max compression
+gzip compressed data, was "dist\iosense_connect_onprem-0.0.3.tar", last modified: Wed Apr 19 09:15:36 2023, max compression
```

## Comparing `iosense_connect_onprem-0.0.2.tar` & `iosense_connect_onprem-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 05:58:17.606824 iosense_connect_onprem-0.0.2/
--rw-rw-rw-   0        0        0     1087 2023-04-18 04:21:30.000000 iosense_connect_onprem-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1062 2023-04-18 05:58:17.604821 iosense_connect_onprem-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      683 2023-04-18 04:44:54.000000 iosense_connect_onprem-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 05:58:17.517831 iosense_connect_onprem-0.0.2/iosense_connect_onprem/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect_onprem-0.0.2/iosense_connect_onprem/__init__.py
--rw-rw-rw-   0        0        0    19470 2023-04-18 05:58:11.000000 iosense_connect_onprem-0.0.2/iosense_connect_onprem/data_access.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:58:17.601824 iosense_connect_onprem-0.0.2/iosense_connect_onprem.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-04-18 05:58:17.000000 iosense_connect_onprem-0.0.2/iosense_connect_onprem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-04-18 05:58:17.000000 iosense_connect_onprem-0.0.2/iosense_connect_onprem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 05:58:17.000000 iosense_connect_onprem-0.0.2/iosense_connect_onprem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-18 05:58:17.000000 iosense_connect_onprem-0.0.2/iosense_connect_onprem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 05:58:17.606824 iosense_connect_onprem-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      626 2023-04-18 05:58:11.000000 iosense_connect_onprem-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 09:15:36.600631 iosense_connect_onprem-0.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-04-18 04:21:30.000000 iosense_connect_onprem-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-04-19 09:15:36.520853 iosense_connect_onprem-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      683 2023-04-18 04:44:54.000000 iosense_connect_onprem-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 09:15:36.378030 iosense_connect_onprem-0.0.3/iosense_connect_onprem/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect_onprem-0.0.3/iosense_connect_onprem/__init__.py
+-rw-rw-rw-   0        0        0    19478 2023-04-19 09:13:04.000000 iosense_connect_onprem-0.0.3/iosense_connect_onprem/data_access.py
+drwxrwxrwx   0        0        0        0 2023-04-19 09:15:36.515374 iosense_connect_onprem-0.0.3/iosense_connect_onprem.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-04-19 09:15:35.000000 iosense_connect_onprem-0.0.3/iosense_connect_onprem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-04-19 09:15:35.000000 iosense_connect_onprem-0.0.3/iosense_connect_onprem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 09:15:35.000000 iosense_connect_onprem-0.0.3/iosense_connect_onprem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-19 09:15:35.000000 iosense_connect_onprem-0.0.3/iosense_connect_onprem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 09:15:36.601637 iosense_connect_onprem-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      626 2023-04-19 09:15:16.000000 iosense_connect_onprem-0.0.3/setup.py
```

### Comparing `iosense_connect_onprem-0.0.2/LICENSE.txt` & `iosense_connect_onprem-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect_onprem-0.0.2/PKG-INFO` & `iosense_connect_onprem-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense_connect_onprem
-Version: 0.0.2
+Version: 0.0.3
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect_onprem-0.0.2/README.md` & `iosense_connect_onprem-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect_onprem-0.0.2/iosense_connect_onprem/data_access.py` & `iosense_connect_onprem-0.0.3/iosense_connect_onprem/data_access.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         """
         try:
             url = "http://" + self.url + "/api/metaData/device/" + device_id
             header = {'userID': self.userID}
             payload = {}
             response = requests.request('GET', url, headers=header, data=payload, verify=False)
-            print(response.text)
+            # print(response.text)
             if response.status_code != 200:
                 raw = json.loads(response.text)
                 raise ValueError(raw['error'])
             else:
                 raw_data = json.loads(response.text)['data']
                 return raw_data
 
@@ -54,19 +54,19 @@
 
         Maps sensor_alias/ sensor name with corresponding sensor ID
         replaces column names with sensor_alias_sensor_id
 
         """
 
         list1 = list(df['sensor'].unique())
-        print(raw_metadata)
+        # print(raw_metadata)
         if len(raw_metadata) == 0:
             raw_metadata = DataAccess.get_device_metadata(self, device_id)
-            print(raw_metadata)
-        print(raw_metadata)
+            # print(raw_metadata)
+        # print(raw_metadata)
         sensor_spec = 'sensors'
         sensor_param_df = pd.DataFrame(raw_metadata[sensor_spec])
 
         for i in list1:
             sensor_param_df1 = sensor_param_df[sensor_param_df['sensorId'] == i]
             if len(sensor_param_df1) != 0:
                 # print('sensor_param_df',sensor_param_df1)
```

### Comparing `iosense_connect_onprem-0.0.2/iosense_connect_onprem.egg-info/PKG-INFO` & `iosense_connect_onprem-0.0.3/iosense_connect_onprem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense-connect-onprem
-Version: 0.0.2
+Version: 0.0.3
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect_onprem-0.0.2/setup.py` & `iosense_connect_onprem-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect_onprem",
-    version = "0.0.2",
+    version = "0.0.3",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect_onprem"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     classifiers = [
```


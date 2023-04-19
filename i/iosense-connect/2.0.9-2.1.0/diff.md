# Comparing `tmp/iosense_connect-2.0.9.tar.gz` & `tmp/iosense_connect-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-2.0.9.tar", last modified: Tue Apr 18 06:13:30 2023, max compression
+gzip compressed data, was "dist\iosense_connect-2.1.0.tar", last modified: Wed Apr 19 09:43:56 2023, max compression
```

## Comparing `iosense_connect-2.0.9.tar` & `iosense_connect-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 06:13:30.822833 iosense_connect-2.0.9/
--rw-rw-rw-   0        0        0     1087 2023-04-18 04:21:30.000000 iosense_connect-2.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0     1046 2023-04-18 06:13:30.822833 iosense_connect-2.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      674 2023-04-15 12:45:17.000000 iosense_connect-2.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 06:13:30.775959 iosense_connect-2.0.9/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.0.9/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    19328 2023-04-18 06:12:50.000000 iosense_connect-2.0.9/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:13:30.807213 iosense_connect-2.0.9/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0     1046 2023-04-18 06:13:30.000000 iosense_connect-2.0.9/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-04-18 06:13:30.000000 iosense_connect-2.0.9/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 06:13:30.000000 iosense_connect-2.0.9/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-18 06:13:30.000000 iosense_connect-2.0.9/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 06:13:30.822833 iosense_connect-2.0.9/setup.cfg
--rw-rw-rw-   0        0        0      612 2023-04-18 06:13:28.000000 iosense_connect-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 09:43:56.005913 iosense_connect-2.1.0/
+-rw-rw-rw-   0        0        0     1087 2023-04-18 04:21:30.000000 iosense_connect-2.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1046 2023-04-19 09:43:56.003913 iosense_connect-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      674 2023-04-15 12:45:17.000000 iosense_connect-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 09:43:55.936887 iosense_connect-2.1.0/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.0/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    19815 2023-04-19 09:43:47.000000 iosense_connect-2.1.0/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-04-19 09:43:55.991814 iosense_connect-2.1.0/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1046 2023-04-19 09:43:55.000000 iosense_connect-2.1.0/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-04-19 09:43:55.000000 iosense_connect-2.1.0/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 09:43:55.000000 iosense_connect-2.1.0/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-19 09:43:55.000000 iosense_connect-2.1.0/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 09:43:56.006916 iosense_connect-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      612 2023-04-19 09:43:47.000000 iosense_connect-2.1.0/setup.py
```

### Comparing `iosense_connect-2.0.9/LICENSE.txt` & `iosense_connect-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.0.9/PKG-INFO` & `iosense_connect-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense_connect
-Version: 2.0.9
+Version: 2.1.0
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-2.0.9/README.md` & `iosense_connect-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.0.9/iosense_connect/data_access.py` & `iosense_connect-2.1.0/iosense_connect/data_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 raw_data = json.loads(response.text)['data']
                 return raw_data
 
         except Exception as e:
             print('Failed to fetch device Metadata')
             print(e)
 
-    def get_sensor_alias(self, device_id, df,raw_metadata):
+    def get_sensor_alias(self, device_id, df, raw_metadata):
         """
 
         :param raw_metadata: json of device metadata
         :param device_id: string
         :param df: Dataframe
         :return: dataframe with columns having sensor alias
 
@@ -56,28 +56,28 @@
 
         """
 
         list1 = list(df['sensor'].unique())
 
         if len(raw_metadata) == 0:
             raw_metadata = DataAccess.get_device_metadata(self, device_id)
-            print(raw_metadata)
+
         sensor_spec = 'sensors'
         sensor_param_df = pd.DataFrame(raw_metadata[sensor_spec])
 
         for i in list1:
             sensor_param_df1 = sensor_param_df[sensor_param_df['sensorId'] == i]
             if len(sensor_param_df1) != 0:
                 # print('sensor_param_df',sensor_param_df1)
                 sensor_name = sensor_param_df1.iloc[0]['sensorName']
                 sensor_name = sensor_name + " (" + i + ")"
                 df['sensor'] = df['sensor'].replace(i, sensor_name)
-        return df,raw_metadata
+        return df, raw_metadata
 
-    def get_caliberation(self,device_id,metadata,df):
+    def get_caliberation(self, device_id, metadata, df):
         """
 
         :param df_raw: Dataframe
         :param device_id: string
         :return: Calibrated dataframe
 
         Perform cal on original data
@@ -87,15 +87,15 @@
 
         """
         sensor_name_list = list(df.columns)
         sensor_name_list.remove('time')
         # print(sensor_name_list)
         sensor_id_list = [s[s.rfind("(") + 1:s.rfind(")")] for s in sensor_name_list]
         if len(metadata) == 0:
-            metadata = DataAccess.get_device_metadata(self,device_id)
+            metadata = DataAccess.get_device_metadata(self, device_id)
         data = metadata['params']
 
         for (value1, value2) in zip(sensor_id_list, sensor_name_list):
             # print(value1, value2)
             # print(data[str(value1)])
             df_meta = pd.DataFrame(data[str(value1)])
             # print(df_meta)
@@ -104,15 +104,16 @@
             if 'm' in df_meta.columns and 'c' in df_meta.columns:
                 # print(df_meta.iloc[0]['m'],type(df_meta.iloc[0]['m']))
                 m = float(df_meta.iloc[0]['m'])
                 # print('M value',m)
                 c = int(df_meta.iloc[0]['c'])
                 # print(m, type(c))
                 # print(df[str(value2)])
-                df[str(value2)] =  df[str(value2)].replace('BAD 255', '-99999').replace('-','99999').replace('BAD undefined', '-99999').replace('BAD 0', '-99999')
+                df[str(value2)] = df[str(value2)].replace('BAD 255', '-99999').replace('-', '99999').replace(
+                    'BAD undefined', '-99999').replace('BAD 0', '-99999')
                 df[str(value2)] = df[str(value2)].astype('float')
                 # print('==',df[str(value2)])
                 df[str(value2)] = (df[str(value2)] * m) + c
                 if 'min' in df_meta.columns:
                     min = int(df_meta.iloc[0]['min'])
                     df[str(value2)] = np.where(df[str(value2)] <= min, min, df[str(value2)])
                 if 'max' in df_meta.columns:
@@ -219,14 +220,18 @@
         :param IST: bool (default: True)
         :return: Dataframe with values
 
         Get Data Point fetches data containing values of last n data points of given sensor at given time.
 
         """
         try:
+            df_devices = DataAccess.get_device_details(self)
+            device_list = df_devices['devID'].tolist()
+            if device_id not in device_list:
+                raise Exception('Message: Device not added')
             metadata = {}
             end_time = pd.to_datetime(end_time)
             if IST:
                 end_time = end_time - timedelta(hours=5, minutes=30)
             end_time = int(round(end_time.timestamp()))
             if type(sensors) == list:
                 len_sensors = len(sensors)
@@ -274,16 +279,21 @@
             df = DataAccess.get_cleaned_table(self, df)
             if str(cal).lower() == 'true':
                 df = DataAccess.get_caliberation(self, device_id, metadata, df)
             return df
         except Exception as e:
             print(e)
 
-    def data_query(self, device_id, start_time, end_time=datetime.now(), sensors=None, cal=True, bands=None, IST=True ,echo=True):
+    def data_query(self, device_id, start_time, end_time=datetime.now(), sensors=None, cal=True, bands=None, IST=True,
+                   echo=True):
         # df = pd.DataFrame()
+        df_devices = DataAccess.get_device_details(self)
+        device_list = df_devices['devID'].tolist()
+        if device_id not in device_list:
+            raise Exception('Message: Device not added')
         metadata = {}
         if sensors == None:
             metadata = DataAccess.get_device_metadata(self, device_id)
             data_sensor = metadata['sensors']
             df_sensor = pd.DataFrame(data_sensor)
             sensor_id_list = list(df_sensor['sensorId'])
             sensors = sensor_id_list
@@ -311,52 +321,54 @@
                 for record in range(counter):
                     sys.stdout.write('\r')
                     sys.stdout.write("Approx Records Fetched %d" % (10000 * record))
                     sys.stdout.flush()
             if sensors is None:
                 url_api = "https://" + self.url + "/api/apiLayer/getDataByStEt?device="
                 if counter == 0:
-                    temp = url_api + device_id + "&sTime=" + str(st_time) + "&eTime=" + str(en_time) + "&cursor=true&limit=50000"
+                    temp = url_api + device_id + "&sTime=" + str(st_time) + "&eTime=" + str(
+                        en_time) + "&cursor=true&limit=50000"
                 else:
                     temp = url_api + device_id + "&sTime=" + str(cursor['start']) + "&eTime=" + str(
                         cursor['end']) + "&cursor=true&limit=50000"
             if sensors is not None:
                 url_api = "https://" + self.url + "/api/apiLayer/getAllData?device="
                 if counter == 0:
                     str1 = ","
                     sensor_values = str1.join(sensors)
-                    temp = url_api + device_id + "&sensor=" + sensor_values + "&sTime=" + str(st_time) + "&eTime=" + str(
+                    temp = url_api + device_id + "&sensor=" + sensor_values + "&sTime=" + str(
+                        st_time) + "&eTime=" + str(
                         en_time) + "&cursor=true&limit=50000"
                 else:
                     str1 = ","
                     sensor_values = str1.join(sensors)
                     temp = url_api + device_id + "&sensor=" + sensor_values + "&sTime=" + str(
                         cursor['start']) + "&eTime=" + str(cursor['end']) + "&cursor=true&limit=50000"
 
             response = requests.request("GET", temp, headers=header, data=payload)
             raw = json.loads(response.text)
             # print(raw)
             if response.status_code != 200:
-                raise ValueError(raw['error'])
+                raise ValueError(raw)
             if 'success' in raw:
-                raise ValueError(raw['error'])
+                raise ValueError(raw)
 
             else:
                 raw_data = json.loads(response.text)['data']
                 # print('====================',raw_data)
                 cursor = json.loads(response.text)['cursor']
-                if len(raw_data) !=0:
+                if len(raw_data) != 0:
                     rawdata_res = rawdata_res + raw_data
                 counter = counter + 1
             if cursor['start'] is None or cursor['end'] is None:
                 break
         # print(rawdata_res)
         df_raw = pd.DataFrame(rawdata_res)
 
-        if len(df_raw) != 0 :
+        if len(df_raw) != 0:
             if IST:
                 df_raw['time'] = pd.to_datetime(df_raw['time'], utc=False)
                 df_raw['time'] = df_raw['time'].dt.tz_convert('Asia/Kolkata').dt.tz_localize(None)
             if len(df_raw.columns) == 2:
                 df_raw['sensor'] = sensors[0]
             df, metadata = DataAccess.get_sensor_alias(self, device_id, df_raw, metadata)
             df = DataAccess.get_cleaned_table(self, df)
```

### Comparing `iosense_connect-2.0.9/iosense_connect.egg-info/PKG-INFO` & `iosense_connect-2.1.0/iosense_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense-connect
-Version: 2.0.9
+Version: 2.1.0
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-2.0.9/setup.py` & `iosense_connect-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect",
-    version = "2.0.9",
+    version = "2.1.0",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     classifiers = [
```


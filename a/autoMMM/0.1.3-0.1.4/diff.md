# Comparing `tmp/autoMMM-0.1.3.tar.gz` & `tmp/autoMMM-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoMMM-0.1.3.tar", last modified: Wed Apr 19 20:31:14 2023, max compression
+gzip compressed data, was "autoMMM-0.1.4.tar", last modified: Wed Apr 19 20:58:27 2023, max compression
```

## Comparing `autoMMM-0.1.3.tar` & `autoMMM-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 20:31:14.390209 autoMMM-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-04-19 20:31:14.374582 autoMMM-0.1.3/AutoMMM/
--rw-rw-rw-   0        0        0        0 2023-04-08 15:41:28.000000 autoMMM-0.1.3/AutoMMM/__init__.py
--rw-rw-rw-   0        0        0     2581 2023-04-19 20:24:50.000000 autoMMM-0.1.3/AutoMMM/autoholidays.py
--rw-rw-rw-   0        0        0    11953 2023-04-18 11:17:07.000000 autoMMM-0.1.3/AutoMMM/automodeller.py
--rw-rw-rw-   0        0        0    10898 2023-04-19 20:31:14.390209 autoMMM-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    10132 2023-04-12 09:34:42.000000 autoMMM-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 20:31:14.390209 autoMMM-0.1.3/autoMMM.egg-info/
--rw-rw-rw-   0        0        0    10898 2023-04-19 20:31:14.000000 autoMMM-0.1.3/autoMMM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-19 20:31:14.000000 autoMMM-0.1.3/autoMMM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 20:31:14.000000 autoMMM-0.1.3/autoMMM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-19 20:31:14.000000 autoMMM-0.1.3/autoMMM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 20:31:14.000000 autoMMM-0.1.3/autoMMM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 20:31:14.390209 autoMMM-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      995 2023-04-19 20:28:17.000000 autoMMM-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:58:27.659669 autoMMM-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-04-19 20:58:27.643959 autoMMM-0.1.4/AutoMMM/
+-rw-rw-rw-   0        0        0        0 2023-04-08 15:41:28.000000 autoMMM-0.1.4/AutoMMM/__init__.py
+-rw-rw-rw-   0        0        0     2849 2023-04-19 20:57:48.000000 autoMMM-0.1.4/AutoMMM/autoholidays.py
+-rw-rw-rw-   0        0        0    11953 2023-04-18 11:17:07.000000 autoMMM-0.1.4/AutoMMM/automodeller.py
+-rw-rw-rw-   0        0        0    10898 2023-04-19 20:58:27.659669 autoMMM-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10132 2023-04-12 09:34:42.000000 autoMMM-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 20:58:27.659669 autoMMM-0.1.4/autoMMM.egg-info/
+-rw-rw-rw-   0        0        0    10898 2023-04-19 20:58:27.000000 autoMMM-0.1.4/autoMMM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-19 20:58:27.000000 autoMMM-0.1.4/autoMMM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 20:58:27.000000 autoMMM-0.1.4/autoMMM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-19 20:58:27.000000 autoMMM-0.1.4/autoMMM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 20:58:27.000000 autoMMM-0.1.4/autoMMM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 20:58:27.659669 autoMMM-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      995 2023-04-19 20:58:05.000000 autoMMM-0.1.4/setup.py
```

### Comparing `autoMMM-0.1.3/AutoMMM/autoholidays.py` & `autoMMM-0.1.4/AutoMMM/autoholidays.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,31 +12,38 @@
     def get_holidays_by_nation(self):
         holiday_dict = {}
         start_year, end_year = self.start_date.year, self.end_date.year
         for year in range(start_year, end_year + 1):
             for date, name in sorted(holidays.CountryHoliday(self.country, years=year).items()):
                 holiday_dict[date] = name
         return holiday_dict
+    
+    def week_start_to_int(self, week_start):
+        days = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
+        return days.index(week_start)
+
 
     def get_holidays_by_region(self, region):
         regional_holiday_dict = {}
         start_year, end_year = self.start_date.year, self.end_date.year
         for year in range(start_year, end_year + 1):
             for date, name in sorted(holidays.CountryHoliday(self.country, prov=region, years=year).items()):
                 regional_holiday_dict[date] = name
         return regional_holiday_dict
 
     def generate_timeseries(self, holiday_dict=None, week_start='Monday', custom_holiday_list=None):
         if holiday_dict is None:
             holiday_dict = self.holiday_dict
 
+        week_start_int = self.week_start_to_int(week_start)
+
         date_range = pd.date_range(self.start_date, self.end_date, freq='D')
         timeseries_df = pd.DataFrame(date_range, columns=['Date'])
 
-        timeseries_df['Week Commencing'] = timeseries_df['Date'] - pd.to_timedelta(timeseries_df['Date'].dt.weekday, unit='d')
+        timeseries_df['Week Commencing'] = timeseries_df['Date'] - pd.to_timedelta((timeseries_df['Date'].dt.weekday - week_start_int) % 7, unit='d')
         timeseries_df['Holiday'] = timeseries_df['Date'].map(holiday_dict)
         timeseries_df['Is Holiday'] = (timeseries_df['Holiday'].notna()).astype(int)
 
         if custom_holiday_list is not None:
             timeseries_df['Custom Holiday'] = timeseries_df['Holiday'].isin(custom_holiday_list).astype(int)
 
         weekly_timeseries_df = timeseries_df.groupby('Week Commencing').agg({'Is Holiday': 'sum', 'Custom Holiday': 'max'}).reset_index()
@@ -47,8 +54,8 @@
         for index, row in weekly_timeseries_df.iterrows():
             if row['Is Holiday'] > 0:
                 if last_holiday_week is not None:
                     weeks_since_last_holiday = (row['Week Commencing'] - last_holiday_week).days // 7
                     weekly_timeseries_df.at[index, 'Weeks Since Last Holiday'] = weeks_since_last_holiday
                 last_holiday_week = row['Week Commencing']
 
-        return weekly_timeseries_df
+        return weekly_timeseries_df
```

### Comparing `autoMMM-0.1.3/AutoMMM/automodeller.py` & `autoMMM-0.1.4/AutoMMM/automodeller.py`

 * *Files identical despite different names*

### Comparing `autoMMM-0.1.3/PKG-INFO` & `autoMMM-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoMMM
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `autoMMM-0.1.3/README.md` & `autoMMM-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `autoMMM-0.1.3/autoMMM.egg-info/PKG-INFO` & `autoMMM-0.1.4/autoMMM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoMMM
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `autoMMM-0.1.3/setup.py` & `autoMMM-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="autoMMM",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "scikit-learn",
         "statsmodels",
         "matplotlib",
```


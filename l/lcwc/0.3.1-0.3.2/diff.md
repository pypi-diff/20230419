# Comparing `tmp/lcwc-0.3.1.tar.gz` & `tmp/lcwc-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcwc-0.3.1.tar", last modified: Sat Apr 15 18:22:15 2023, max compression
+gzip compressed data, was "lcwc-0.3.2.tar", last modified: Wed Apr 19 14:05:55 2023, max compression
```

## Comparing `lcwc-0.3.1.tar` & `lcwc-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 18:22:15.280538 lcwc-0.3.1/
--rw-rw-rw-   0        0        0     1058 2023-01-16 14:14:04.000000 lcwc-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     1766 2023-04-15 18:22:15.279538 lcwc-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1110 2023-04-15 17:56:28.000000 lcwc-0.3.1/README.md
--rw-rw-rw-   0        0        0      791 2023-04-15 18:19:52.000000 lcwc-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 18:22:15.280538 lcwc-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 18:22:15.251539 lcwc-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:22:15.270538 lcwc-0.3.1/src/lcwc/
--rw-rw-rw-   0        0        0      172 2023-02-04 13:19:54.000000 lcwc-0.3.1/src/lcwc/__init__.py
--rw-rw-rw-   0        0        0      324 2023-01-28 13:09:14.000000 lcwc-0.3.1/src/lcwc/category.py
--rw-rw-rw-   0        0        0      915 2023-04-08 10:55:17.000000 lcwc-0.3.1/src/lcwc/client.py
--rw-rw-rw-   0        0        0     6241 2023-04-15 18:20:57.000000 lcwc-0.3.1/src/lcwc/feedclient.py
--rw-rw-rw-   0        0        0     2314 2023-04-15 17:45:56.000000 lcwc-0.3.1/src/lcwc/incident.py
--rw-rw-rw-   0        0        0     3609 2023-04-15 17:56:04.000000 lcwc-0.3.1/src/lcwc/webclient.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:22:15.278540 lcwc-0.3.1/src/lcwc.egg-info/
--rw-rw-rw-   0        0        0     1766 2023-04-15 18:22:15.000000 lcwc-0.3.1/src/lcwc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-04-15 18:22:15.000000 lcwc-0.3.1/src/lcwc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 18:22:15.000000 lcwc-0.3.1/src/lcwc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-15 18:22:15.000000 lcwc-0.3.1/src/lcwc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-15 18:22:15.000000 lcwc-0.3.1/src/lcwc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:55.324644 lcwc-0.3.2/
+-rw-rw-rw-   0        0        0     1058 2023-01-16 14:14:04.000000 lcwc-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     1766 2023-04-19 14:05:55.324644 lcwc-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1110 2023-04-15 17:56:28.000000 lcwc-0.3.2/README.md
+-rw-rw-rw-   0        0        0      791 2023-04-19 14:05:40.000000 lcwc-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 14:05:55.325645 lcwc-0.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:55.303643 lcwc-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:55.316644 lcwc-0.3.2/src/lcwc/
+-rw-rw-rw-   0        0        0        0 2023-04-19 14:03:09.000000 lcwc-0.3.2/src/lcwc/__init__.py
+-rw-rw-rw-   0        0        0      324 2023-01-28 13:09:14.000000 lcwc-0.3.2/src/lcwc/category.py
+-rw-rw-rw-   0        0        0      915 2023-04-08 10:55:17.000000 lcwc-0.3.2/src/lcwc/client.py
+-rw-rw-rw-   0        0        0     6859 2023-04-19 14:02:08.000000 lcwc-0.3.2/src/lcwc/feedclient.py
+-rw-rw-rw-   0        0        0     2314 2023-04-15 17:45:56.000000 lcwc-0.3.2/src/lcwc/incident.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:55.323644 lcwc-0.3.2/src/lcwc/utils/
+-rw-rw-rw-   0        0        0        8 2023-04-19 14:03:46.000000 lcwc-0.3.2/src/lcwc/utils/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-19 14:03:00.000000 lcwc-0.3.2/src/lcwc/utils.py
+-rw-rw-rw-   0        0        0     3609 2023-04-15 17:56:04.000000 lcwc-0.3.2/src/lcwc/webclient.py
+drwxrwxrwx   0        0        0        0 2023-04-19 14:05:55.322643 lcwc-0.3.2/src/lcwc.egg-info/
+-rw-rw-rw-   0        0        0     1766 2023-04-19 14:05:55.000000 lcwc-0.3.2/src/lcwc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2023-04-19 14:05:55.000000 lcwc-0.3.2/src/lcwc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 14:05:55.000000 lcwc-0.3.2/src/lcwc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-19 14:05:55.000000 lcwc-0.3.2/src/lcwc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-19 14:05:55.000000 lcwc-0.3.2/src/lcwc.egg-info/top_level.txt
```

### Comparing `lcwc-0.3.1/LICENSE` & `lcwc-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lcwc-0.3.1/PKG-INFO` & `lcwc-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcwc
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python library for fetching the Lancaster County-Wide Communications live incident list.
 Author-email: Nate Shoffner <nate.shoffner@gmail.com>
 Project-URL: Homepage, https://github.com/NateShoffner/python-lcwc
 Project-URL: Bug Tracker, https://github.com/NateShoffner/python-lcwc/issues
 Keywords: lcwc,lancaster,police,fire,ems,dispatch,911,incident
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lcwc-0.3.1/README.md` & `lcwc-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `lcwc-0.3.1/pyproject.toml` & `lcwc-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lcwc"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Nate Shoffner", email="nate.shoffner@gmail.com" },
 ]
 description = "Python library for fetching the Lancaster County-Wide Communications live incident list."
 keywords = ["lcwc", "lancaster", "police", "fire", "ems", "dispatch", "911", "incident"]
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `lcwc-0.3.1/src/lcwc/client.py` & `lcwc-0.3.2/src/lcwc/client.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.3.1/src/lcwc/feedclient.py` & `lcwc-0.3.2/src/lcwc/feedclient.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         return self._guid
 
 class IncidentFeedClient(Client):
 
     URL = 'https://webcad.lcwc911.us/Pages/Public/LiveIncidentsFeed.aspx'
     """ The URL of the live incident feed """
 
-    FIRE_UNIT_NAMES = ['BRUSH', 'CHIEF', 'DEPUTY', 'DUTY OFFICER', 'ENGINE', 'FIRE POLICE', 'RESCUE', 'SQUAD', 'TRUCK', 'UTV']
+    FIRE_UNIT_NAMES = ['BRUSH', 'CHIEF', 'DEPUTY', 'DUTY OFFICER', 'ENGINE', 'FIRE POLICE', 'RESCUE', 'SQUAD', 'TAC', 'TRUCK', 'UTILITY', 'UTV']
     MEDICAL_UNIT_NAMES = ['AMB', 'EMS', 'INT', 'MEDIC', 'QRS']
 
     LOCATION_NAMES = ['ALY', 'AVE', 'CIR', 'CT', 'DR', 'LN', 'PL', 'PIKE', 'RAMP', 'RD', 'ROUTE', 'ST']
 
     MEDICAL_DESCRIPTION_KEYWORDS = ['MEDICAL']
     FIRE_DESCRIPTION_KEYWORDS = ['FIRE']
     TRAFFIC_DESCRIPTION_KEYWORDS = ['TRAFFIC', 'VEHICLE']
@@ -69,62 +69,78 @@
         :return: A list of incidents
         :rtype: list[Incident]
         """
         incidents = []
 
         d = feedparser.parse(contents)
 
+        def has_intersection(details_segment: str) -> bool:
+            return any(k in details_segment for k in self.LOCATION_NAMES)
+            
+        def has_unit_names(details_segment: str) -> bool:
+            return any(k in details_segment for k in self.FIRE_UNIT_NAMES + self.MEDICAL_UNIT_NAMES)S
+
         for entry in d.entries:
 
+            guid = entry.guid
+            date = datetime.datetime.fromtimestamp( email.utils.mktime_tz(email.utils.parsedate_tz(entry.published)))
+            description = entry.title
+
+            # Possible formats:
             # [township];[intersection];[units assigned]
+            # [township];[intersection]
+            # [township];[units assigned]
+            # [township]
             details_split = entry['description'].strip().split(';', maxsplit=3)
 
             # first item is always the township
             township = details_split[0].strip()
 
             intersection = None
             units = []
 
-            def split_units(units_data: str) -> list[str]:
-                units_data = units_data.strip()
-                if units_data == '':
-                    return []
-                return [u.strip() for u in units_data.strip().split('<br />')]
-
-            # intersection is not always present, so we need to check for it before splitting the units
-            has_unit_names = any(k in details_split[1] for k in self.FIRE_UNIT_NAMES + self.MEDICAL_UNIT_NAMES)
-            has_intersection = any(k in details_split[1] for k in self.LOCATION_NAMES)
-
-            if has_unit_names and not has_intersection:
-                units = split_units(details_split[1])
-            else:
-                intersection = details_split[1].strip()
-                units = split_units(details_split[2])
+            # skip if only township is present
+            if len(details_split >= 2):
+                if has_unit_names(details_split[1]):
+                    units = self.__extract_units(details_split[1])
+                else:
+                    if has_intersection(details_split[1]):
+                        intersection = details_split[1].strip()
+                    if len(details_split) > 2 and has_unit_names(details_split[2]):
+                        units = self.__extract_units(details_split[2])
 
-            date = datetime.datetime.fromtimestamp( email.utils.mktime_tz(email.utils.parsedate_tz(entry.published)))
+            category = self.__determine_category(description, units)
 
-            guid = entry.guid
-
-            description = entry.title
-            cat = self.__determine_category(description, units)
-            incidents.append(FeedIncident(cat, date, description, township, intersection, units, guid))
+            incidents.append(FeedIncident(category, date, description, township, intersection, units, guid))
 
         return incidents
 
     async def fetch_and_parse(self, session: aiohttp.ClientSession, timeout: int = 10) -> list[FeedIncident]:
         """ Gets the live incident feed and returns a list of incidents
 
         :param session: The aiohttp session to use
         :param timeout: The timeout for the request
         :return: A list of incidents
         :rtype: list[Incident]
         """
         result = await self.fetch(session, timeout)
         active_incidents = self.parse(result)
         return active_incidents
+    
+    def __extract_units(self, units_data: str) -> list[str]:
+        """ Extracts the units from the data string
+
+        :param units_data: The data string containing the units
+        :return: A list of units
+        :rtype: list[str]
+        """
+        units_data = units_data.strip()
+        if units_data == '':
+            return []
+        return [u.strip() for u in units_data.strip().split('<br />')]
 
     def __determine_category(self, description: str, units: list[str]) -> IncidentCategory:
         """ Determines the category of an incident based on the description and units assigned 
         
         :param description: The description of the incident
         :param units: The units assigned to the incident
         :return: The category of the incident
```

### Comparing `lcwc-0.3.1/src/lcwc/incident.py` & `lcwc-0.3.2/src/lcwc/incident.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.3.1/src/lcwc/webclient.py` & `lcwc-0.3.2/src/lcwc/webclient.py`

 * *Files identical despite different names*

### Comparing `lcwc-0.3.1/src/lcwc.egg-info/PKG-INFO` & `lcwc-0.3.2/src/lcwc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcwc
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python library for fetching the Lancaster County-Wide Communications live incident list.
 Author-email: Nate Shoffner <nate.shoffner@gmail.com>
 Project-URL: Homepage, https://github.com/NateShoffner/python-lcwc
 Project-URL: Bug Tracker, https://github.com/NateShoffner/python-lcwc/issues
 Keywords: lcwc,lancaster,police,fire,ems,dispatch,911,incident
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```


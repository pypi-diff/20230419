# Comparing `tmp/seven2one-4.0.0.tar.gz` & `tmp/seven2one-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seven2one-4.0.0.tar", last modified: Thu Mar  9 10:45:46 2023, max compression
+gzip compressed data, was "seven2one-4.1.0.tar", last modified: Wed Apr 19 07:44:18 2023, max compression
```

## Comparing `seven2one-4.0.0.tar` & `seven2one-4.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-03-09 10:45:46.522852 seven2one-4.0.0/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1105 2022-11-02 13:56:37.000000 seven2one-4.0.0/LICENSE
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2022-11-02 13:56:37.000000 seven2one-4.0.0/MANIFEST.in
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2224 2023-03-09 10:45:46.522852 seven2one-4.0.0/PKG-INFO
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1771 2023-01-12 09:56:35.000000 seven2one-4.0.0/README.md
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       38 2023-03-09 10:45:46.522852 seven2one-4.0.0/setup.cfg
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1381 2023-01-11 13:22:28.000000 seven2one-4.0.0/setup.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-03-09 10:45:46.522852 seven2one-4.0.0/seven2one/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       51 2023-03-09 10:45:40.000000 seven2one-4.0.0/seven2one/__init__.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    14931 2023-01-31 14:07:00.000000 seven2one-4.0.0/seven2one/authorization.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    10848 2023-01-31 14:07:00.000000 seven2one-4.0.0/seven2one/automation.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    63376 2023-01-31 14:07:00.000000 seven2one-4.0.0/seven2one/core.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3769 2023-01-04 09:37:30.000000 seven2one-4.0.0/seven2one/email.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1549 2022-11-02 13:56:37.000000 seven2one-4.0.0/seven2one/fileImportService.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    53999 2023-01-12 09:56:35.000000 seven2one-4.0.0/seven2one/fileimport.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-03-09 10:45:46.522852 seven2one-4.0.0/seven2one/logging_loki/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      189 2023-01-04 09:37:30.000000 seven2one-4.0.0/seven2one/logging_loki/__init__.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      756 2023-01-04 09:37:30.000000 seven2one-4.0.0/seven2one/logging_loki/const.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5177 2023-01-04 09:37:30.000000 seven2one-4.0.0/seven2one/logging_loki/emitter.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2929 2023-01-04 09:37:30.000000 seven2one-4.0.0/seven2one/logging_loki/handlers.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15392 2023-01-31 14:07:00.000000 seven2one-4.0.0/seven2one/programming.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     9486 2023-03-09 10:39:10.000000 seven2one-4.0.0/seven2one/schedule.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    57800 2023-01-31 14:07:00.000000 seven2one-4.0.0/seven2one/timeseries.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-03-09 10:45:46.522852 seven2one-4.0.0/seven2one/utils/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       21 2023-03-09 10:45:40.000000 seven2one-4.0.0/seven2one/utils/__init__.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    35320 2023-01-31 14:07:00.000000 seven2one-4.0.0/seven2one/utils/ut.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1832 2022-11-02 13:56:37.000000 seven2one-4.0.0/seven2one/utils/ut_autprog.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    26023 2022-12-07 10:15:15.000000 seven2one-4.0.0/seven2one/utils/ut_fileimport.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5856 2022-11-02 13:56:37.000000 seven2one-4.0.0/seven2one/utils/ut_init.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1000 2023-01-30 08:36:11.000000 seven2one-4.0.0/seven2one/utils/ut_log.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     4229 2022-11-02 13:56:37.000000 seven2one-4.0.0/seven2one/utils/ut_meta.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3435 2022-11-02 13:56:37.000000 seven2one-4.0.0/seven2one/utils/ut_time.py
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     6584 2022-11-02 13:56:37.000000 seven2one-4.0.0/seven2one/utils/ut_timeseries.py
-drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-03-09 10:45:46.522852 seven2one-4.0.0/seven2one.egg-info/
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2224 2023-03-09 10:45:46.000000 seven2one-4.0.0/seven2one.egg-info/PKG-INFO
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      859 2023-03-09 10:45:46.000000 seven2one-4.0.0/seven2one.egg-info/SOURCES.txt
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-03-09 10:45:46.000000 seven2one-4.0.0/seven2one.egg-info/dependency_links.txt
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-03-09 10:45:46.000000 seven2one-4.0.0/seven2one.egg-info/not-zip-safe
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       90 2023-03-09 10:45:46.000000 seven2one-4.0.0/seven2one.egg-info/requires.txt
--rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       10 2023-03-09 10:45:46.000000 seven2one-4.0.0/seven2one.egg-info/top_level.txt
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-19 07:44:18.064157 seven2one-4.1.0/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1105 2023-04-14 08:32:42.000000 seven2one-4.1.0/LICENSE
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-14 08:32:42.000000 seven2one-4.1.0/MANIFEST.in
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2224 2023-04-19 07:44:18.064157 seven2one-4.1.0/PKG-INFO
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1771 2023-04-14 08:32:42.000000 seven2one-4.1.0/README.md
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       38 2023-04-19 07:44:18.064157 seven2one-4.1.0/setup.cfg
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1381 2023-04-19 07:30:12.000000 seven2one-4.1.0/setup.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-19 07:44:18.060157 seven2one-4.1.0/seven2one/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       51 2023-04-19 07:44:13.000000 seven2one-4.1.0/seven2one/__init__.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15405 2023-04-19 07:30:12.000000 seven2one-4.1.0/seven2one/authorization.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    10848 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/automation.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    63376 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/core.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3769 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/email.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1549 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/fileImportService.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    53999 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/fileimport.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-19 07:44:18.060157 seven2one-4.1.0/seven2one/logging_loki/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      189 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/logging_loki/__init__.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      756 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/logging_loki/const.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5177 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/logging_loki/emitter.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2929 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/logging_loki/handlers.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    15392 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/programming.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     9486 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/schedule.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    61487 2023-04-19 07:30:12.000000 seven2one-4.1.0/seven2one/timeseries.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-19 07:44:18.064157 seven2one-4.1.0/seven2one/utils/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       21 2023-04-19 07:44:13.000000 seven2one-4.1.0/seven2one/utils/__init__.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    35310 2023-04-19 07:30:12.000000 seven2one-4.1.0/seven2one/utils/ut.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     1832 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/utils/ut_autprog.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)    26023 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/utils/ut_fileimport.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     5856 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/utils/ut_init.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      989 2023-04-19 07:30:12.000000 seven2one-4.1.0/seven2one/utils/ut_log.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     4229 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/utils/ut_meta.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     3435 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/utils/ut_time.py
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     6584 2023-04-14 08:32:42.000000 seven2one-4.1.0/seven2one/utils/ut_timeseries.py
+drwxr-xr-x   0 az_devops_agent  (1000) az_devops_agent  (1000)        0 2023-04-19 07:44:18.060157 seven2one-4.1.0/seven2one.egg-info/
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)     2224 2023-04-19 07:44:18.000000 seven2one-4.1.0/seven2one.egg-info/PKG-INFO
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)      859 2023-04-19 07:44:18.000000 seven2one-4.1.0/seven2one.egg-info/SOURCES.txt
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-04-19 07:44:18.000000 seven2one-4.1.0/seven2one.egg-info/dependency_links.txt
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)        1 2023-04-19 07:44:17.000000 seven2one-4.1.0/seven2one.egg-info/not-zip-safe
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       90 2023-04-19 07:44:18.000000 seven2one-4.1.0/seven2one.egg-info/requires.txt
+-rw-r--r--   0 az_devops_agent  (1000) az_devops_agent  (1000)       10 2023-04-19 07:44:18.000000 seven2one-4.1.0/seven2one.egg-info/top_level.txt
```

### Comparing `seven2one-4.0.0/LICENSE` & `seven2one-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/PKG-INFO` & `seven2one-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven2one
-Version: 4.0.0
+Version: 4.1.0
 Summary: Functions to interact with the Seven2one TechStack
 Home-page: http://www.seven2one.de
 Author: Seven2one Informationssysteme GmbH
 Author-email: info@seven2one.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `seven2one-4.0.0/README.md` & `seven2one-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/setup.py` & `seven2one-4.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one/authorization.py` & `seven2one-4.1.0/seven2one/authorization.py`

 * *Files 6% similar despite different names*

```diff
@@ -239,30 +239,31 @@
         roleName:str,
         userGroups:list=None, 
         objectPermissions:list=['Create', 'Delete'], 
         propertiesPermissions:list=['Read', 'Update']
         ) -> None:
 
         """
-        Creates a role and sets all rights to all propertes except references
+        Creates a role and sets all rights to all properties
 
         Parameters:
         ----------
         inventoryName : str
             The name of the inventory for which the new role authorizes rights.
         roleName : str
             Name of the new role.
         userGroup : list = None
             List of user group names. If None, the role will be created without attaching user groups.
         objectPermissions : list = ['Create', 'Delete']
             Default is 'Create' and 'Delete' to allow creating and deleting items of the specified inventory.
             Other entries are not allowed.
         propertiesPermissions : list = ['Read', 'Update']
-            Default is 'Read' and 'Update'. All properties except references will receive 
-            the here specified rights. Other entries are not allowed.     
+            Default is 'Read' and 'Update'. All properties will receive 
+            the specified rights. Other entries are not allowed.
+            Permissions are not extended on referenced inventories!
         """
 
         correlationId = str(uuid4())
         with logger.contextualize(correlation_id=correlationId):
 
             # Parameter validation
             try:
@@ -295,39 +296,45 @@
                     return
 
             # Create role
             properties = dyno_client.structure[inventoryName]['properties']
 
             ppstring = '[' + ','.join(map(str.upper, propertiesPermissions)) + ']'
             props = '[\n'
+            refProps = '[\n'
             for _, value in properties.items():
-                props += f'{{ propertyId: {Utils._toGraphQL(value["propertyId"])}\n permissions: {ppstring} }}\n'
+                if value["type"] == 'scalar':
+                    props += f'{{ propertyId: {Utils._toGraphQL(value["propertyId"])}\n permissions: {ppstring} }}\n'
+                elif value["type"] == 'reference':
+                    refProps += f'{{ propertyId: {Utils._toGraphQL(value["propertyId"])}\n inventoryId: {Utils._toGraphQL(value["inventoryId"])}\n propertyPermissions: {ppstring}\n inventoryPermissions: [NONE]\n properties: []\n referencedProperties: []\n }}'
             props += ']'
+            refProps += ']'
+            
             graphQLString= f'''
             mutation AddRole($roleName: String!, $inventoryId: String!, $inventoryPermissions: [ObjectPermission!]!) {{ 
                 addRole (input: {{
                     name: $roleName
                     rootInventoryPermission: {{
                         inventoryId: $inventoryId
                         inventoryPermissions: $inventoryPermissions
                         properties: {props}
-                        referencedProperties: []
+                        referencedProperties: {refProps}
                         }}
                     }})
                     {{
                     id
                 }}
             }}
             '''
             params = {
                 "roleName": roleName,
                 "inventoryId": dyno_client.structure[inventoryName]['inventoryId'],
                 "inventoryPermissions": list(map(str.upper, objectPermissions)),
             }
-
+            
             result = Utils._executeGraphQL(self, graphQLString, correlationId, params=params)
             if result == None: return
 
             # if result['addRole']['errors']:
             #     Utils._listGraphQlErrors(result, 'createInventory')
             #     return
```

### Comparing `seven2one-4.0.0/seven2one/automation.py` & `seven2one-4.1.0/seven2one/automation.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one/core.py` & `seven2one-4.1.0/seven2one/core.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one/email.py` & `seven2one-4.1.0/seven2one/email.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one/fileImportService.py` & `seven2one-4.1.0/seven2one/fileImportService.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one/fileimport.py` & `seven2one-4.1.0/seven2one/fileimport.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one/logging_loki/const.py` & `seven2one-4.1.0/seven2one/logging_loki/const.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one/logging_loki/emitter.py` & `seven2one-4.1.0/seven2one/logging_loki/emitter.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one/logging_loki/handlers.py` & `seven2one-4.1.0/seven2one/logging_loki/handlers.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one/programming.py` & `seven2one-4.1.0/seven2one/programming.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one/schedule.py` & `seven2one-4.1.0/seven2one/schedule.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one/timeseries.py` & `seven2one-4.1.0/seven2one/timeseries.py`

 * *Files 3% similar despite different names*

```diff
@@ -481,151 +481,153 @@
         ---------
         >>> timeSeriesData('meterData', '2020-10-01', '2020-10-01T:05:30:00Z')
         >>> timeSeriesData('meterData', fromTimepoint='2020-06-01',
                 toTimepoint='2020-06-15', fields=['meterId', 'phase']
                 where='measure eq "voltage"')
         """
 
-        if timeZone == None:
-            timeZone = self.defaults.timeZone
-        logger.debug(f"Timezone: {timeZone}")
-
-        _fromTimepoint = TimeUtils._inputTimestamp(fromTimepoint, timeZone)
-        _toTimepoint = TimeUtils._inputTimestamp(toTimepoint, timeZone)
-
-        # where
-        topLevelWhere, resolvedFilterDict = Utils._handleWhere(core, where, inventoryName)
-
-        # fields
-        deleteIdAfterwards = False
-        if fields != None:
-            propertyDict = Utils._properties(self.scheme, inventoryName, recursive=True, 
-                sysProperties=False)
-            if type(fields) != list:
-                fields = [fields]
-            if 'sys_inventoryItemId' not in fields:
-                fields += ['sys_inventoryItemId']
-                deleteIdAfterwards = True
-            _fields = Utils._queryFields(fields, propertyDict['arrayTypeFields'], 50, 
-                filter=resolvedFilterDict, recursive=True)
-            if 'pageSize' in _fields:
-                Utils._error(self, f"Array type fields are not supported in 'fields'-argument ({_fields})")
-                return
-        else:
-            if self.structure[inventoryName]['displayValue'] != None:
-                fields = ['sys_displayValue', 'sys_inventoryItemId']
-                deleteIdAfterwards = True
+        correlationId = str(uuid4())
+        with logger.contextualize(correlation_id=correlationId):
+            if timeZone == None:
+                timeZone = self.defaults.timeZone
+            logger.debug(f"Timezone: {timeZone}")
+
+            _fromTimepoint = TimeUtils._inputTimestamp(fromTimepoint, timeZone)
+            _toTimepoint = TimeUtils._inputTimestamp(toTimepoint, timeZone)
+
+            # where
+            topLevelWhere, resolvedFilterDict = Utils._handleWhere(core, where, inventoryName)
+
+            # fields
+            deleteIdAfterwards = False
+            if fields != None:
+                propertyDict = Utils._properties(self.scheme, inventoryName, recursive=True, 
+                    sysProperties=False)
+                if type(fields) != list:
+                    fields = [fields]
+                if 'sys_inventoryItemId' not in fields:
+                    fields += ['sys_inventoryItemId']
+                    deleteIdAfterwards = True
+                _fields = Utils._queryFields(fields, propertyDict['arrayTypeFields'], 50, 
+                    filter=resolvedFilterDict, recursive=True)
+                if 'pageSize' in _fields:
+                    Utils._error(self, f"Array type fields are not supported in 'fields'-argument ({_fields})")
+                    return
             else:
-                fields = ['sys_inventoryItemId']
-
-            _fields = ''
-            for field in fields:
-                _fields += field + '\n'
+                if self.structure[inventoryName]['displayValue'] != None:
+                    fields = ['sys_displayValue', 'sys_inventoryItemId']
+                    deleteIdAfterwards = True
+                else:
+                    fields = ['sys_inventoryItemId']
 
-        unit = Utils._argNone('unit', unit)
+                _fields = ''
+                for field in fields:
+                    _fields += field + '\n'
+
+            unit = Utils._argNone('unit', unit)
+
+            if timeUnit != None:
+                aggregation = f'''
+                    aggregation: {aggregationRule}
+                    resolution: {{timeUnit: {timeUnit} factor: {factor}}}
+                    '''
+            else:
+                aggregation = ''
 
-        if timeUnit != None:
-            aggregation = f'''
-                aggregation: {aggregationRule}
-                resolution: {{timeUnit: {timeUnit} factor: {factor}}}
-                '''
-        else:
-            aggregation = ''
+            if includeMissing == True:
+                allowedFlags = f'allowedFlags: [MISSING, VALID, NO_VALUE, INTERPOLATED, ESTIMATED, ACCOUNTED, MANUALLY_REPLACED, SCHEDULE, FAULTY]'
+            else:
+                allowedFlags= f'allowedFlags: [VALID, INTERPOLATED, ESTIMATED, ACCOUNTED, MANUALLY_REPLACED, SCHEDULE, FAULTY]'
 
-        if includeMissing == True:
-            allowedFlags = f'allowedFlags: [MISSING, VALID, NO_VALUE, INTERPOLATED, ESTIMATED, ACCOUNTED, MANUALLY_REPLACED, SCHEDULE, FAULTY]'
-        else:
-            allowedFlags= f'allowedFlags: [VALID, INTERPOLATED, ESTIMATED, ACCOUNTED, MANUALLY_REPLACED, SCHEDULE, FAULTY]'
-
-        result = []
-        count = 0
-        countDp = 0
-        lastId = ''
-        pageSize = 1 # Initial page size
-        maxTimePoints = 40000
-
-        key = inventoryName
-        while True:
-            start = time()
-            graphQLString = f'''query timeSeriesData {{
-                {key} (
-                pageSize: {pageSize}
-                {topLevelWhere}
-                {lastId}
-                )
-                {{
-                    {_fields}
-                    _dataPoints (input:{{
-                        from:"{_fromTimepoint}"
-                        to:"{_toTimepoint}"
-                        {unit}                        
-                        {aggregation}
-                        {allowedFlags}
-                        }})
+            result = []
+            count = 0
+            countDp = 0
+            lastId = ''
+            pageSize = 1 # Initial page size
+            maxTimePoints = 40000
+
+            key = inventoryName
+            while True:
+                start = time()
+                graphQLString = f'''query timeSeriesData {{
+                    {key} (
+                    pageSize: {pageSize}
+                    {topLevelWhere}
+                    {lastId}
+                    )
                     {{
-                        timestamp
-                        value
-                        flag
+                        {_fields}
+                        _dataPoints (input:{{
+                            from:"{_fromTimepoint}"
+                            to:"{_toTimepoint}"
+                            {unit}                        
+                            {aggregation}
+                            {allowedFlags}
+                            }})
+                        {{
+                            timestamp
+                            value
+                            flag
+                        }}
                     }}
-                }}
-            }}'''
+                }}'''
 
-            if count == 0:
-                Utils._copyGraphQLString(graphQLString)
+                if count == 0:
+                    Utils._copyGraphQLString(graphQLString)
 
-            _result = Utils._executeGraphQL(self, graphQLString)
+                _result = Utils._executeGraphQL(self, graphQLString)
 
-            ## Automatic paging
-            countDp = 0
-            countTs = len(_result[key])
-            if countTs == 0: break
-            for i in _result[key]:
-                if i['_dataPoints'] == None:
-                    continue
-                else:
-                    countDp += len(i['_dataPoints'])
-            end = round(time()-start, 2)
-            logger.debug(f"Iteration: {count}, timeSeries: {countTs}, dataPoints: {countDp}, pageSize: {pageSize}, time: {end}")
-            try:
-                pageSize = maxTimePoints * pageSize // countDp
-                if pageSize > 2000: pageSize = 2000
-            except ZeroDivisionError:
-                pageSize = 10**(count + 1)
-                if pageSize > 2000: pageSize = 2000
-            pageSize = 1 if pageSize == 0 else pageSize
-
-            if _result[inventoryName]:
-                result += _result[inventoryName]
-                count += 1
-            try:
-                cursor = _result[inventoryName][-1]['sys_inventoryItemId']
-                lastId = f'lastId: "{cursor}"'
-            except Exception as err:
-                Utils._error(self, f"Problem with pagination: {err}")
-                return
+                ## Automatic paging
+                countDp = 0
+                countTs = len(_result[key])
+                if countTs == 0: break
+                for i in _result[key]:
+                    if i['_dataPoints'] == None:
+                        continue
+                    else:
+                        countDp += len(i['_dataPoints'])
+                end = round(time()-start, 2)
+                logger.debug(f"Iteration: {count}, timeSeries: {countTs}, dataPoints: {countDp}, pageSize: {pageSize}, time: {end}")
+                try:
+                    pageSize = maxTimePoints * pageSize // countDp
+                    if pageSize > 2000: pageSize = 2000
+                except ZeroDivisionError:
+                    pageSize = 10**(count + 1)
+                    if pageSize > 2000: pageSize = 2000
+                pageSize = 1 if pageSize == 0 else pageSize
 
-        if deleteIdAfterwards == True:
-            fields.remove('sys_inventoryItemId')
+                if _result[inventoryName]:
+                    result += _result[inventoryName]
+                    count += 1
+                try:
+                    cursor = _result[inventoryName][-1]['sys_inventoryItemId']
+                    lastId = f'lastId: "{cursor}"'
+                except Exception as err:
+                    Utils._error(self, f"Problem with pagination: {err}")
+                    return
 
-        meta = []
-        for field in fields:
-            if field.count('.') == 1:
-                compoundField = field.split('.')
-                meta.append([compoundField[0], compoundField[1]])
-            else:
-                meta.append(field)
+            if deleteIdAfterwards == True:
+                fields.remove('sys_inventoryItemId')
+
+            meta = []
+            for field in fields:
+                if field.count('.') == 1:
+                    compoundField = field.split('.')
+                    meta.append([compoundField[0], compoundField[1]])
+                else:
+                    meta.append(field)
 
-        df = pd.json_normalize(result, record_path = ['_dataPoints'], meta=meta, errors='ignore')
+            df = pd.json_normalize(result, record_path = ['_dataPoints'], meta=meta, errors='ignore')
 
-        if df.empty:
-            logger.info('The query did not produce results.')
-            return df
+            if df.empty:
+                logger.info('The query did not produce results.')
+                return df
 
-        df = UtilsTimeSeries._processDataFrame(core, result, df, fields, timeZone, displayMode, includeMissing)
-        return df
+            df = UtilsTimeSeries._processDataFrame(core, result, df, fields, timeZone, displayMode, includeMissing)
+            return df
 
     def timeSeriesGroupData(
             self, 
             inventoryName:str, 
             fromTimepoint:str, 
             toTimepoint:str, 
             fields:list=None, 
@@ -695,187 +697,189 @@
                 instancePrefix='',
                 where='region in ["DE", "FR", "PL"],
                 whereInstance='issueDate >= '2022-10-01',
                 timeUnit:'DAY'
                 )
         """
 
-        if timeZone == None:
-            timeZone = self.defaults.timeZone 
-        logger.debug(f"Timezone: {timeZone}")        
-
-        _fromTimepoint = TimeUtils._inputTimestamp(fromTimepoint, timeZone)
-        _toTimepoint = TimeUtils._inputTimestamp(toTimepoint, timeZone)
-
-        deleteIdAfterwards = False
-        if fields != None:
-            if type(fields) != list:
-                fields = [fields]
-            if 'sys_inventoryItemId' not in fields:
-                fields += ['sys_inventoryItemId']
-                deleteIdAfterwards = True
-        else:
-            if self.structure[inventoryName]['displayValue'] != None:
-                fields = ['sys_displayValue', 'sys_inventoryItemId']
-                deleteIdAfterwards = True
+        correlationId = str(uuid4())
+        with logger.contextualize(correlation_id=correlationId):
+            if timeZone == None:
+                timeZone = self.defaults.timeZone 
+            logger.debug(f"Timezone: {timeZone}")        
+
+            _fromTimepoint = TimeUtils._inputTimestamp(fromTimepoint, timeZone)
+            _toTimepoint = TimeUtils._inputTimestamp(toTimepoint, timeZone)
+
+            deleteIdAfterwards = False
+            if fields != None:
+                if type(fields) != list:
+                    fields = [fields]
+                if 'sys_inventoryItemId' not in fields:
+                    fields += ['sys_inventoryItemId']
+                    deleteIdAfterwards = True
             else:
-                fields = ['sys_inventoryItemId']
+                if self.structure[inventoryName]['displayValue'] != None:
+                    fields = ['sys_displayValue', 'sys_inventoryItemId']
+                    deleteIdAfterwards = True
+                else:
+                    fields = ['sys_inventoryItemId']
 
-        _groupFields = ''
-        for field in fields:
-            _groupFields += field + '\n'
+            _groupFields = ''
+            for field in fields:
+                _groupFields += field + '\n'
 
-        if instanceFields != None:
-            if type(instanceFields) != list:
-                instanceFields = [instanceFields]
-        else:
-            instanceInventoryName = self.structure[inventoryName]['properties']['timeSeriesInstances']['inventoryName']
-            if self.structure[instanceInventoryName]['displayValue'] != None:
-                instanceFields  = ['sys_displayValue', 'sys_inventoryItemId']
+            if instanceFields != None:
+                if type(instanceFields) != list:
+                    instanceFields = [instanceFields]
             else:
-                instanceFields  = ['sys_inventoryItemId']
-
-        _instanceFields = ''
-        for field in instanceFields:
-            _instanceFields += field + '\n'
+                instanceInventoryName = self.structure[inventoryName]['properties']['timeSeriesInstances']['inventoryName']
+                if self.structure[instanceInventoryName]['displayValue'] != None:
+                    instanceFields  = ['sys_displayValue', 'sys_inventoryItemId']
+                else:
+                    instanceFields  = ['sys_inventoryItemId']
 
-        topLevelWhere, _ = Utils._handleWhere(self, where, inventoryName)
-        instanceWhere, _ = Utils._handleWhere(self, whereInstance, inventoryName)
+            _instanceFields = ''
+            for field in instanceFields:
+                _instanceFields += field + '\n'
 
-        unit = Utils._argNone('unit', unit)
+            topLevelWhere, _ = Utils._handleWhere(self, where, inventoryName)
+            instanceWhere, _ = Utils._handleWhere(self, whereInstance, inventoryName)
 
-        if timeUnit != None:
-            aggregation = f'''
-                aggregation: {aggregationRule}
-                resolution: {{timeUnit: {timeUnit} factor: {factor}}}
-                '''
-        else:
-            aggregation = ''
+            unit = Utils._argNone('unit', unit)
 
-        if includeMissing == True:
-            allowedFlags = f'allowedFlags: [MISSING, VALID, NO_VALUE, INTERPOLATED, ESTIMATED, ACCOUNTED, MANUALLY_REPLACED, SCHEDULE, FAULTY]'
-        else:
-            allowedFlags= f'allowedFlags: [VALID, INTERPOLATED, ESTIMATED, ACCOUNTED, MANUALLY_REPLACED, SCHEDULE, FAULTY]'
-           
-        instanceDataPoints = f'''_dataPoints (input:{{
-                        from:"{_fromTimepoint}"
-                        to:"{_toTimepoint}"
-                        {unit}
-                        {aggregation}
-                        {allowedFlags}
-                        }})
-                    {{
-                        timestamp
-                        value
-                        flag
-                    }}
-        '''
-        
-        key = inventoryName
-
-        result = []
-        count = 0
-        countDp = 0
-        lastId = ''
-        pageSize = 1 # Initial page size
-        maxTimePoints = 40000
+            if timeUnit != None:
+                aggregation = f'''
+                    aggregation: {aggregationRule}
+                    resolution: {{timeUnit: {timeUnit} factor: {factor}}}
+                    '''
+            else:
+                aggregation = ''
 
-        while True:
+            if includeMissing == True:
+                allowedFlags = f'allowedFlags: [MISSING, VALID, NO_VALUE, INTERPOLATED, ESTIMATED, ACCOUNTED, MANUALLY_REPLACED, SCHEDULE, FAULTY]'
+            else:
+                allowedFlags= f'allowedFlags: [VALID, INTERPOLATED, ESTIMATED, ACCOUNTED, MANUALLY_REPLACED, SCHEDULE, FAULTY]'
             
-            start = time()
-            graphQLString = f'''query timeSeriesData {{
-                {key} (
-                pageSize: {pageSize}
-                {topLevelWhere}
-                {lastId}
-                )
-                {{
-                    {_groupFields}
-                    timeSeriesInstances (
-                    pageSize: 5000
-                    {instanceWhere}
-                    ) {{
-                        {_instanceFields}
-                        {instanceDataPoints}
+            instanceDataPoints = f'''_dataPoints (input:{{
+                            from:"{_fromTimepoint}"
+                            to:"{_toTimepoint}"
+                            {unit}
+                            {aggregation}
+                            {allowedFlags}
+                            }})
+                        {{
+                            timestamp
+                            value
+                            flag
+                        }}
+            '''
+            
+            key = inventoryName
+
+            result = []
+            count = 0
+            countDp = 0
+            lastId = ''
+            pageSize = 1 # Initial page size
+            maxTimePoints = 40000
+
+            while True:
+                
+                start = time()
+                graphQLString = f'''query timeSeriesData {{
+                    {key} (
+                    pageSize: {pageSize}
+                    {topLevelWhere}
+                    {lastId}
+                    )
+                    {{
+                        {_groupFields}
+                        timeSeriesInstances (
+                        pageSize: 5000
+                        {instanceWhere}
+                        ) {{
+                            {_instanceFields}
+                            {instanceDataPoints}
+                        }}
                     }}
-                }}
-            }}'''
+                }}'''
 
-            if count == 0:
-                Utils._copyGraphQLString(graphQLString)
+                if count == 0:
+                    Utils._copyGraphQLString(graphQLString)
 
-            _result = Utils._executeGraphQL(self, graphQLString)
-            
-            # Automatic paging
-            try:
-                countDp = 0
-                countInst = 0
-                countGroupTs = len(_result[key])
-                if countGroupTs == 0: break
-                for i in _result[key]:
-                    countInst += len(i['timeSeriesInstances'])
-                    for j in i['timeSeriesInstances']:
-                        countDp += len(j['_dataPoints'])
-                end = round(time()-start, 2)
-                logger.debug(f"Iteration: {count}, groupTimeSeries: {countGroupTs}, instances: {countInst}, dataPoints: {countDp}, pageSize: {pageSize}, time: {end}")
+                _result = Utils._executeGraphQL(self, graphQLString)
+                
+                # Automatic paging
                 try:
-                    pageSize = maxTimePoints * pageSize // countDp
-                    if pageSize > 10000: pageSize = 10000
-                except ZeroDivisionError:
-                    pageSize = 10**(count + 1)
-                    if pageSize > 10000: pageSize = 10000
-                pageSize = 1 if pageSize == 0 else pageSize
-            except Exception as err:
-                Utils._error(self, f"Problem with pagination: {err}")
-                return
+                    countDp = 0
+                    countInst = 0
+                    countGroupTs = len(_result[key])
+                    if countGroupTs == 0: break
+                    for i in _result[key]:
+                        countInst += len(i['timeSeriesInstances'])
+                        for j in i['timeSeriesInstances']:
+                            countDp += len(j['_dataPoints'])
+                    end = round(time()-start, 2)
+                    logger.debug(f"Iteration: {count}, groupTimeSeries: {countGroupTs}, instances: {countInst}, dataPoints: {countDp}, pageSize: {pageSize}, time: {end}")
+                    try:
+                        pageSize = maxTimePoints * pageSize // countDp
+                        if pageSize > 10000: pageSize = 10000
+                    except ZeroDivisionError:
+                        pageSize = 10**(count + 1)
+                        if pageSize > 10000: pageSize = 10000
+                    pageSize = 1 if pageSize == 0 else pageSize
+                except Exception as err:
+                    Utils._error(self, f"Problem with pagination: {err}")
+                    return
+
+                if _result[inventoryName]:
+                    result += _result[inventoryName]
+                    count += 1
+                try:
+                    cursor = _result[inventoryName][-1]['sys_inventoryItemId']
+                    lastId = f'lastId: "{cursor}"'
+                except Exception as err: 
+                    Utils._error(self, f"Problem with pagination: {err}")
+                    return
+
+            if deleteIdAfterwards == True:
+                fields.remove('sys_inventoryItemId')
+            meta = []
+            if type(fields) != list:
+                meta.append(fields)
+            else:
+                for field in fields:
+                    meta.append(field)
+
+            if type(instanceFields) != list:
+                meta.append(['timeSeriesInstances', instanceFields])
+            else:
+                for field in instanceFields:
+                    meta.append(['timeSeriesInstance', field])
 
-            if _result[inventoryName]:
-                result += _result[inventoryName]
-                count += 1
             try:
-                cursor = _result[inventoryName][-1]['sys_inventoryItemId']
-                lastId = f'lastId: "{cursor}"'
-            except Exception as err: 
-                Utils._error(self, f"Problem with pagination: {err}")
+                df = pd.json_normalize(result, record_path = ['timeSeriesInstances', '_dataPoints'],
+                    meta=meta)
+            except KeyError:
+                Utils._error(self, f"There is a problem with the provided fields. Probably one or more fields have no values. ")
                 return
 
-        if deleteIdAfterwards == True:
-            fields.remove('sys_inventoryItemId')
-        meta = []
-        if type(fields) != list:
-            meta.append(fields)
-        else:
-            for field in fields:
-                meta.append(field)
-
-        if type(instanceFields) != list:
-            meta.append(['timeSeriesInstances', instanceFields])
-        else:
-            for field in instanceFields:
-                meta.append(['timeSeriesInstance', field])
-
-        try:
-            df = pd.json_normalize(result, record_path = ['timeSeriesInstances', '_dataPoints'],
-                meta=meta)
-        except KeyError:
-            Utils._error(self, f"There is a problem with the provided fields. Probably one or more fields have no values. ")
-            return
+            # rename columns
+            reColumns = []
+            for col in df.columns:
+                if col.startswith('timeSeriesInstance'):
+                    col = col.replace('timeSeriesInstance.', instancePrefix)
+                reColumns.append(col)
+            df.columns = reColumns  
 
-        # rename columns
-        reColumns = []
-        for col in df.columns:
-            if col.startswith('timeSeriesInstance'):
-                col = col.replace('timeSeriesInstance.', instancePrefix)
-            reColumns.append(col)
-        df.columns = reColumns  
+            pivotColumns = list(df.columns)[3:]
 
-        pivotColumns = list(df.columns)[3:]
-
-        df = UtilsTimeSeries._processDataFrame(core, result, df, pivotColumns, timeZone, displayMode, includeMissing)
-        return df       
+            df = UtilsTimeSeries._processDataFrame(core, result, df, pivotColumns, timeZone, displayMode, includeMissing)
+            return df       
         
     def timeSeriesGroupDataReduced(
             self, 
             inventoryName:str, 
             fromTimepoint:str, 
             toTimepoint:str, 
             reduceFunction:str='LAST', 
@@ -949,159 +953,161 @@
                 instancePrefix='',
                 where='region in ["DE", "FR", "PL"],
                 whereInstance='issueDate >= '2022-10-01',
                 timeUnit:'DAY'
                 )
         """
 
-        if timeZone == None:
-            timeZone = self.defaults.timeZone 
-        logger.debug(f"Timezone: {timeZone}")            
-
-        _fromTimepoint = TimeUtils._inputTimestamp(fromTimepoint, timeZone)
-        _toTimepoint = TimeUtils._inputTimestamp(toTimepoint, timeZone)
-
-        if type(fields) != list:
-            _groupFields = fields
-            if 'sys_inventoryItemId' not in _groupFields:
-                _groupFields += ['sys_inventoryItemId']
-        else:
-            _groupFields = ''
-            for field in fields:
-                _groupFields += field + '\n'
-            _groupFields += 'sys_inventoryItemId\n'
-        if type(instanceFields) != list:
-            _instanceFields = instanceFields
-        else:
-            _instanceFields = ''
-            for field in instanceFields:
-                _instanceFields += field + '\n'
+        correlationId = str(uuid4())
+        with logger.contextualize(correlation_id=correlationId):
+            if timeZone == None:
+                timeZone = self.defaults.timeZone 
+            logger.debug(f"Timezone: {timeZone}")            
 
-        resolvedFilter = ''
-        if where != None: 
-            resolvedFilter = Utils._resolveWhereString(self, where)
-
-        resolvedInstanceFilter = ''
-        if whereInstance != None: 
-            resolvedInstanceFilter = Utils._resolveWhereString(self, whereInstance)
-
-        unit = Utils._argNone('unit', unit)
-
-        if timeUnit != None:
-            aggregation = f'''
-                resolution: {{timeUnit: {timeUnit} factor: {factor}}}
-                '''
-        else:
-            aggregation = ''
+            _fromTimepoint = TimeUtils._inputTimestamp(fromTimepoint, timeZone)
+            _toTimepoint = TimeUtils._inputTimestamp(toTimepoint, timeZone)
 
-        if resolvedInstanceFilter == '':
-            instanceInput = ''
-        else:
-            instanceInput = f'''({resolvedInstanceFilter})'''
-           
-        groupInput = f'''input:{{
-                        from:"{_fromTimepoint}"
-                        to:"{_toTimepoint}"
-                        {unit}
-                        {aggregation}
-                        reducer: {reduceFunction}
-                        showMissing: true
-                        }}
-        '''
-        
-        key = inventoryName
-        graphQLString = f'''query timeSeriesData {{
-                {key} (
-                pageSize: 500 
-                {resolvedFilter}
-                {groupInput}
-                )
-                {{
-                    {_groupFields}
-                    _dataPoints {{
-                        timestamp
-                        value
-                        flag
-                        }}
-                    timeSeriesInstances {instanceInput} {{
-                        sys_inventoryItemId
-                    }}
-                }}
-            }}'''
-
-        result = []
-        count = 0
-        countDp = 0
-        lastId = ''
-        pageSize = 1 # Initial page size
-        maxTimePoints = 40000
+            if type(fields) != list:
+                _groupFields = fields
+                if 'sys_inventoryItemId' not in _groupFields:
+                    _groupFields += ['sys_inventoryItemId']
+            else:
+                _groupFields = ''
+                for field in fields:
+                    _groupFields += field + '\n'
+                _groupFields += 'sys_inventoryItemId\n'
+            if type(instanceFields) != list:
+                _instanceFields = instanceFields
+            else:
+                _instanceFields = ''
+                for field in instanceFields:
+                    _instanceFields += field + '\n'
+
+            resolvedFilter = ''
+            if where != None: 
+                resolvedFilter = Utils._resolveWhereString(self, where)
+
+            resolvedInstanceFilter = ''
+            if whereInstance != None: 
+                resolvedInstanceFilter = Utils._resolveWhereString(self, whereInstance)
+
+            unit = Utils._argNone('unit', unit)
+
+            if timeUnit != None:
+                aggregation = f'''
+                    resolution: {{timeUnit: {timeUnit} factor: {factor}}}
+                    '''
+            else:
+                aggregation = ''
 
-        while True:
+            if resolvedInstanceFilter == '':
+                instanceInput = ''
+            else:
+                instanceInput = f'''({resolvedInstanceFilter})'''
             
-            start = time()
+            groupInput = f'''input:{{
+                            from:"{_fromTimepoint}"
+                            to:"{_toTimepoint}"
+                            {unit}
+                            {aggregation}
+                            reducer: {reduceFunction}
+                            showMissing: true
+                            }}
+            '''
+            
+            key = inventoryName
             graphQLString = f'''query timeSeriesData {{
-                {key} (
-                pageSize: {pageSize}
-                {resolvedFilter}
-                {lastId}
-                {groupInput}
-                )
-                {{
-                    {_groupFields}
-                    _dataPoints {{
-                        timestamp
-                        value
-                        flag
+                    {key} (
+                    pageSize: 500 
+                    {resolvedFilter}
+                    {groupInput}
+                    )
+                    {{
+                        {_groupFields}
+                        _dataPoints {{
+                            timestamp
+                            value
+                            flag
+                            }}
+                        timeSeriesInstances {instanceInput} {{
+                            sys_inventoryItemId
                         }}
-                    timeSeriesInstances {instanceInput} {{
-                        sys_inventoryItemId
                     }}
-                }}
-            }}'''
-
-            if count == 0:
-                Utils._copyGraphQLString(graphQLString)
+                }}'''
 
-            _result = Utils._executeGraphQL(self, graphQLString)
-            
-            # Automatic paging
+            result = []
+            count = 0
             countDp = 0
-            countTs = len(_result[key])
-            if countTs == 0: break
-            for i in _result[key]:
-                countDp += len(i['_dataPoints'])
-            end = round(time()-start, 2)
-            logger.debug(f"Iteration: {count}, groupTimeSeries: {countTs}, dataPoints: {countDp}, pageSize: {pageSize}, time: {end}")
-            try:
-                pageSize = maxTimePoints * pageSize // countDp
-            except ZeroDivisionError:
-                pageSize = 10**(count + 1)
-                if count == 5: count = 1 # To prevent too large pageSize
-            pageSize = 1 if pageSize == 0 else pageSize
-
-            if _result[inventoryName]:
-                result += _result[inventoryName]
-                count += 1
+            lastId = ''
+            pageSize = 1 # Initial page size
+            maxTimePoints = 40000
+
+            while True:
+                
+                start = time()
+                graphQLString = f'''query timeSeriesData {{
+                    {key} (
+                    pageSize: {pageSize}
+                    {resolvedFilter}
+                    {lastId}
+                    {groupInput}
+                    )
+                    {{
+                        {_groupFields}
+                        _dataPoints {{
+                            timestamp
+                            value
+                            flag
+                            }}
+                        timeSeriesInstances {instanceInput} {{
+                            sys_inventoryItemId
+                        }}
+                    }}
+                }}'''
+
+                if count == 0:
+                    Utils._copyGraphQLString(graphQLString)
+
+                _result = Utils._executeGraphQL(self, graphQLString)
+                
+                # Automatic paging
+                countDp = 0
+                countTs = len(_result[key])
+                if countTs == 0: break
+                for i in _result[key]:
+                    countDp += len(i['_dataPoints'])
+                end = round(time()-start, 2)
+                logger.debug(f"Iteration: {count}, groupTimeSeries: {countTs}, dataPoints: {countDp}, pageSize: {pageSize}, time: {end}")
+                try:
+                    pageSize = maxTimePoints * pageSize // countDp
+                except ZeroDivisionError:
+                    pageSize = 10**(count + 1)
+                    if count == 5: count = 1 # To prevent too large pageSize
+                pageSize = 1 if pageSize == 0 else pageSize
+
+                if _result[inventoryName]:
+                    result += _result[inventoryName]
+                    count += 1
+                try:
+                    cursor = _result[inventoryName][-1]['sys_inventoryItemId']
+                    lastId = f'lastId: "{cursor}"'
+                except Exception as err: 
+                    Utils._error(self, f"Problem with pagination: {err}")
+                    return
+
             try:
-                cursor = _result[inventoryName][-1]['sys_inventoryItemId']
-                lastId = f'lastId: "{cursor}"'
-            except Exception as err: 
-                Utils._error(self, f"Problem with pagination: {err}")
+                df = pd.json_normalize(result, ['_dataPoints'], fields)
+            except KeyError:
+                Utils._error(self, f"There is a problem with the provided fields. Probably one or more fields have no values. ")
                 return
+                
+            pivotColumns = list(df.columns)[3:]
 
-        try:
-            df = pd.json_normalize(result, ['_dataPoints'], fields)
-        except KeyError:
-            Utils._error(self, f"There is a problem with the provided fields. Probably one or more fields have no values. ")
-            return
-            
-        pivotColumns = list(df.columns)[3:]
-
-        df = UtilsTimeSeries._processDataFrame(core, result, df, pivotColumns, timeZone, displayMode, includeMissing)
-        return df  
+            df = UtilsTimeSeries._processDataFrame(core, result, df, pivotColumns, timeZone, displayMode, includeMissing)
+            return df  
        
     def deleteTimeSeriesData(
             self,
             inventoryName:str, 
             fromTimepoint:str,
             toTimepoint:str, 
             inventoryItemIds:list=None, 
@@ -1129,100 +1135,102 @@
         timeZone: str = None
             A time zone provided in IANA or isoformat (e.g. 'Europe/Berlin' or 'CET'). Defaults
             to the local time zone or to a previously set default time zone.
         force: bool = False
             Use True to ignore confirmation.
         """
 
-        def createDataPoints(fromTimepoint, toTimepoint, timeUnit, factor) -> list:
-            unitMapping = {
-                'MILLISECOND':'ms',
-                'SECOND':'S',
-                'MINUTE':'min',
-                'HOUR':'H',
-                'DAY':'D',
-                'WEEK':'W',
-                'MONTH':'M',
-                'YEAR':'YS'
-            }
-            freq = f'{factor}{unitMapping[timeUnit]}'
-            index = pd.date_range(fromTimepoint, toTimepoint, freq=freq)
-            logger.debug(f"DateTimeIndex: {index}")
-
-            dataPoints = []
-            for timepoint in index:
-                data = {
-                    'timestamp': timepoint,
-                    'value': 0,
-                    'flag':'MISSING'
+        correlationId = str(uuid4())
+        with logger.contextualize(correlation_id=correlationId):
+            def createDataPoints(fromTimepoint, toTimepoint, timeUnit, factor) -> list:
+                unitMapping = {
+                    'MILLISECOND':'ms',
+                    'SECOND':'S',
+                    'MINUTE':'min',
+                    'HOUR':'H',
+                    'DAY':'D',
+                    'WEEK':'W',
+                    'MONTH':'M',
+                    'YEAR':'YS'
                 }
-                dataPoints.append(data)
-            
-            return dataPoints
+                freq = f'{factor}{unitMapping[timeUnit]}'
+                index = pd.date_range(fromTimepoint, toTimepoint, freq=freq)
+                logger.debug(f"DateTimeIndex: {index}")
+
+                dataPoints = []
+                for timepoint in index:
+                    data = {
+                        'timestamp': timepoint,
+                        'value': 0,
+                        'flag':'MISSING'
+                    }
+                    dataPoints.append(data)
+                
+                return dataPoints
 
-        if timeZone != None:
-            tz = timeZone
-        else:
-            tz = self.defaults.timeZone          
+            if timeZone != None:
+                tz = timeZone
+            else:
+                tz = self.defaults.timeZone          
 
-        fromTimepoint = TimeUtils._inputTimestamp(fromTimepoint, tz)
-        toTimepoint = TimeUtils._inputTimestamp(toTimepoint, tz)
+            fromTimepoint = TimeUtils._inputTimestamp(fromTimepoint, tz)
+            toTimepoint = TimeUtils._inputTimestamp(toTimepoint, tz)
 
-        inventory = core.inventories(where=f'name eq "{inventoryName}"')
-        sys_inventoryId = inventory.loc[0, 'inventoryId']
+            inventory = core.inventories(where=f'name eq "{inventoryName}"')
+            sys_inventoryId = inventory.loc[0, 'inventoryId']
 
-        if inventoryItemIds == None and where == None:
-            Utils._error(self, f"No id list of items and no where-criteria were provided.")
-            return
+            if inventoryItemIds == None and where == None:
+                Utils._error(self, f"No id list of items and no where-criteria were provided.")
+                return
 
-        if inventoryItemIds != None and where != None:
-            logger.warning(f"List of items and where-criteria has been provided. Item list is used.")
+            if inventoryItemIds != None and where != None:
+                logger.warning(f"List of items and where-criteria has been provided. Item list is used.")
 
-        if where != None:
-            df = core.items(inventoryName, fields=['sys_inventoryItemId','resolution'], where=where)
-            if df.empty:
-                logger.info(f"The where criteria '{where}' led to no results.")
+            if where != None:
+                df = core.items(inventoryName, fields=['sys_inventoryItemId','resolution'], where=where)
+                if df.empty:
+                    logger.info(f"The where criteria '{where}' led to no results.")
+                    return
+                
+            if inventoryItemIds != None:
+                idList = '['
+                for item in inventoryItemIds:
+                    idList += f'"{item}", '
+                idList += ']'
+                df = core.items(inventoryName, fields=['sys_inventoryItemId','resolution'], where=f'sys_inventoryItemId in {idList}')
+
+            if force == True:
+                confirm = 'y'
+            else:
+                confirm = input(f"Press 'y' to delete values for {len(df)} time series items: ")
+            if confirm != 'y':
                 return
-            
-        if inventoryItemIds != None:
-            idList = '['
-            for item in inventoryItemIds:
-                idList += f'"{item}", '
-            idList += ']'
-            df = core.items(inventoryName, fields=['sys_inventoryItemId','resolution'], where=f'sys_inventoryItemId in {idList}')
-
-        if force == True:
-            confirm = 'y'
-        else:
-            confirm = input(f"Press 'y' to delete values for {len(df)} time series items: ")
-        if confirm != 'y':
-            return
 
-        for ts in df.iterrows():
+            for ts in df.iterrows():
 
-            sys_inventoryItemId = ts[1]['sys_inventoryItemId']
-            timeUnit = ts[1]['resolution'].split(' ')[1]
-            factor = ts[1]['resolution'].split(' ')[0]
-            dataPoints = createDataPoints(fromTimepoint, toTimepoint, timeUnit, factor)
-            resolution = {'timeUnit':timeUnit, 'factor':factor}
-
-            timeSeries = [{
-                'sys_inventoryId': sys_inventoryId,
-                'sys_inventoryItemId': sys_inventoryItemId,
-                'data':
-                    {
-                    'resolution': resolution,
-                    'dataPoints': dataPoints
-                    }
-                }]
+                sys_inventoryItemId = ts[1]['sys_inventoryItemId']
+                timeUnit = ts[1]['resolution'].split(' ')[1]
+                factor = ts[1]['resolution'].split(' ')[0]
+                dataPoints = createDataPoints(fromTimepoint, toTimepoint, timeUnit, factor)
+                resolution = {'timeUnit':timeUnit, 'factor':factor}
+
+                timeSeries = [{
+                    'sys_inventoryId': sys_inventoryId,
+                    'sys_inventoryItemId': sys_inventoryItemId,
+                    'data':
+                        {
+                        'resolution': resolution,
+                        'dataPoints': dataPoints
+                        }
+                    }]
 
-            self.setTimeSeriesDataCollection(timeSeries)
-        logger.info(f"Deleted values for {len(df)} time series items")
+                self.setTimeSeriesDataCollection(timeSeries)
+            logger.info(f"Deleted values for {len(df)} time series items")
 
-        return
+            return
 
     def items(
         self, 
         inventoryName:str, 
         references:bool=False, 
         fields:list=None,
         where:Union[list,tuple,str]=None, 
@@ -1284,106 +1292,107 @@
                 'appartments',
                 fields=['address', 'owner'],
                 where=['city == "Berlin"', 'rooms > 2'],
                 orderBy={'size':'DESC', price:'ASC'}
                 )
         """
 
-        if inventoryName not in self.inventory:
-            Utils._error(self, f"'{inventoryName}' does not exist.")
-            return
+        correlationId = str(uuid4())
+        with logger.contextualize(correlation_id=correlationId):
+            if inventoryName not in self.inventory:
+                Utils._error(self, f"'{inventoryName}' does not exist.")
+                return
 
-        # where
-        try:
-            topLevelWhere, resolvedFilterDict = Utils._handleWhere(self, where, inventoryName)
-        except:
-            return
+            # where
+            try:
+                topLevelWhere, resolvedFilterDict = Utils._handleWhere(self, where, inventoryName)
+            except:
+                return
 
-        validityDate = Utils._argNone('validityDate', validityDate)
-        allValidityPeriods = Utils._argNone('allValidityPeriods', allValidityPeriods)
-        
+            validityDate = Utils._argNone('validityDate', validityDate)
+            allValidityPeriods = Utils._argNone('allValidityPeriods', allValidityPeriods)
+            
 
-        # core
-        deleteId = False
-        propertyDict = Utils._properties(self.scheme, inventoryName, recursive=True, 
-            sysProperties=includeSysProperties)            
-        if fields != None:
-            if type(fields) != list:
-                fields = [fields]
-            if 'sys_inventoryItemId' not in fields:
-                deleteId = True
-                fields += ['sys_inventoryItemId']
-            _fields = Utils._queryFields(fields, propertyDict['arrayTypeFields'], arrayPageSize, 
-                filter=resolvedFilterDict, recursive=True)
-        else: 
-            properties = Utils._propertyList(propertyDict['properties'], recursive=references)
-            _fields = UtilsTimeSeries._queryFields(properties, propertyDict['arrayTypeFields'], 
-                arrayPageSize, filter=resolvedFilterDict, recursive=references)
-        logger.debug(f"Fields: {_fields}")
+            # core
+            deleteId = False
+            propertyDict = Utils._properties(self.scheme, inventoryName, recursive=True, 
+                sysProperties=includeSysProperties)            
+            if fields != None:
+                if type(fields) != list:
+                    fields = [fields]
+                if 'sys_inventoryItemId' not in fields:
+                    deleteId = True
+                    fields += ['sys_inventoryItemId']
+                _fields = Utils._queryFields(fields, propertyDict['arrayTypeFields'], arrayPageSize, 
+                    filter=resolvedFilterDict, recursive=True)
+            else: 
+                properties = Utils._propertyList(propertyDict['properties'], recursive=references)
+                _fields = UtilsTimeSeries._queryFields(properties, propertyDict['arrayTypeFields'], 
+                    arrayPageSize, filter=resolvedFilterDict, recursive=references)
+            logger.debug(f"Fields: {_fields}")
 
-        if len(_fields) == 0:
-            Utils._error(self, f"Inventory '{inventoryName}' not found.")
-            return
+            if len(_fields) == 0:
+                Utils._error(self, f"Inventory '{inventoryName}' not found.")
+                return
 
-        order = Utils._orderItems(self, orderBy, asc)
-        if order == None: return
+            order = Utils._orderItems(self, orderBy, asc)
+            if order == None: return
 
-        result = []
-        count = 0
-        stop = False
-        lastId = ''
-
-        while True:
-
-            # Handling top (premature stop)
-            if top != None:
-                loadedItems = pageSize * count
-                if top - loadedItems <= pageSize:
-                    stop = True
-                    pageSize = top - loadedItems
-
-            graphQLString= f''' query getItems {{
-                    {inventoryName} (
-                            pageSize: {pageSize}
-                            {order}
-                            {allValidityPeriods}
-                            {validityDate}
-                            {lastId}
-                            {topLevelWhere}
-                            ) {{
-                        {_fields}
+            result = []
+            count = 0
+            stop = False
+            lastId = ''
+
+            while True:
+
+                # Handling top (premature stop)
+                if top != None:
+                    loadedItems = pageSize * count
+                    if top - loadedItems <= pageSize:
+                        stop = True
+                        pageSize = top - loadedItems
+
+                graphQLString= f''' query getItems {{
+                        {inventoryName} (
+                                pageSize: {pageSize}
+                                {order}
+                                {allValidityPeriods}
+                                {validityDate}
+                                {lastId}
+                                {topLevelWhere}
+                                ) {{
+                            {_fields}
+                        }}
                     }}
-                }}
-                '''
-
-            _result = Utils._executeGraphQL(self, graphQLString)     
-            
-            if _result[inventoryName]:
-                result += _result[inventoryName]
-                count += 1
-            try:
-                cursor = _result[inventoryName][-1]['sys_inventoryItemId']
-                lastId = f'lastId: "{cursor}"'
-            except: 
-                break
+                    '''
 
-            if stop == True: break
+                _result = Utils._executeGraphQL(self, graphQLString)     
+                
+                if _result[inventoryName]:
+                    result += _result[inventoryName]
+                    count += 1
+                try:
+                    cursor = _result[inventoryName][-1]['sys_inventoryItemId']
+                    lastId = f'lastId: "{cursor}"'
+                except: 
+                    break
 
-        df = pd.json_normalize(result)
-       
-        if fields != None: #sorts dataframe according to given fields
-            try: # for array field this does not work
-                df = df[fields]
-            except: pass
-        if deleteId: 
-            try: del df['sys_inventoryItemId']
-            except: pass
+                if stop == True: break
 
-        return df
+            df = pd.json_normalize(result)
+        
+            if fields != None: #sorts dataframe according to given fields
+                try: # for array field this does not work
+                    df = df[fields]
+                except: pass
+            if deleteId: 
+                try: del df['sys_inventoryItemId']
+                except: pass
 
+            return df
 
     def units(self) -> pd.DataFrame:
         """
         Returns a DataFrame of existing units.
 
         Examples:
         >>> units()
@@ -1397,18 +1406,20 @@
             factor
             isBaseUnit
             aggregation
             }}
         }}
         '''
 
-        result = Utils._executeGraphQL(self, graphQLString)
-        if result == None: return
+        correlationId = str(uuid4())
+        with logger.contextualize(correlation_id=correlationId):
+            result = Utils._executeGraphQL(self, graphQLString)
+            if result == None: return
 
-        return pd.json_normalize(result['units'])
+            return pd.json_normalize(result['units'])
 
     def createUnit(self, unit:str, baseUnit:str, factor:int, aggregation:str) -> None:
         """
         Creates a unit on basis of a base unit.
 
         Parameters:
         ----------
@@ -1423,35 +1434,37 @@
             kind of aggregation is used for integral units (kW -> kWh), which are not supported 
             yet.
 
         Example:
         >>> createUnit('kW', 'W', 1000, 'AVG')
         """
 
-        graphQLString = f'''
-            mutation createUnit {{
-                createUnit(input: {{
-                    name: "{unit}"
-                    baseUnit: "{baseUnit}"
-                    factor: {factor}
-                    aggregation: {aggregation}}})
-                {{
-                    {Utils.errors}
+        correlationId = str(uuid4())
+        with logger.contextualize(correlation_id=correlationId):
+            graphQLString = f'''
+                mutation createUnit {{
+                    createUnit(input: {{
+                        name: "{unit}"
+                        baseUnit: "{baseUnit}"
+                        factor: {factor}
+                        aggregation: {aggregation}}})
+                    {{
+                        {Utils.errors}
+                    }}
                 }}
-            }}
-        '''
-        result = Utils._executeGraphQL(self, graphQLString)
-        if result == None: return
+            '''
+            result = Utils._executeGraphQL(self, graphQLString)
+            if result == None: return
 
-        key = f'createUnit'
-        if result[key]['errors']:
-            Utils._listGraphQlErrors(result, key)
-        else:
-            logger.info(f"Unit {unit} created.")
-        return
+            key = f'createUnit'
+            if result[key]['errors']:
+                Utils._listGraphQlErrors(result, key)
+            else:
+                logger.info(f"Unit {unit} created.")
+            return
 
     def createBaseUnit(self, baseUnit:str, aggregation:str) -> None:
         """
         Creates a base unit.
 
         Parameters:
         ----------
@@ -1460,34 +1473,36 @@
         aggregation : str
             The enum value for default aggregation. Possible are 'SUM' and 'AVG'.
 
         Example:
         >>> createBaseUnit('W', 'AVG')
         """
 
-        graphQLString = f'''
-            mutation createBaseUnit {{
-                createBaseUnit(input: {{
-                    name: "{baseUnit}"
-                    aggregation: {aggregation}}})
-                {{
-                    {Utils.errors}
+        correlationId = str(uuid4())
+        with logger.contextualize(correlation_id=correlationId):
+            graphQLString = f'''
+                mutation createBaseUnit {{
+                    createBaseUnit(input: {{
+                        name: "{baseUnit}"
+                        aggregation: {aggregation}}})
+                    {{
+                        {Utils.errors}
+                    }}
                 }}
-            }}
-        '''
-        result = Utils._executeGraphQL(self, graphQLString)
-        if result == None: return
+            '''
+            result = Utils._executeGraphQL(self, graphQLString)
+            if result == None: return
 
-        key = f'createBaseUnit'
-        if result[key]['errors']:
-            Utils._listGraphQlErrors(result, key)
-        else:
-            logger.info(f"Unit {baseUnit} created.")
+            key = f'createBaseUnit'
+            if result[key]['errors']:
+                Utils._listGraphQlErrors(result, key)
+            else:
+                logger.info(f"Unit {baseUnit} created.")
 
-        return
+            return
 
     def updateUnit(self, unit:str, baseUnit:str=None, factor:int=None, aggregation:str=None) -> None:
         """
         Updates a unit.
 
         Parameters:
         ----------
@@ -1500,41 +1515,42 @@
         aggregation : str
             The enum value for default aggregation. Possible enums are 'SUM' and 'AVG' 
 
         Example:
         >>> updateUnit('kW', 'W', 1000, 'AVG')
         """
 
-        baseUnit = Utils._argNone('baseUnit', baseUnit)
-        factor = Utils._argNone('factor', factor)
-        aggregation = Utils._argNone('aggregation', aggregation, enum=True)
-
-        graphQLString = f'''
-            mutation updateUnit {{
-                updateUnit(input: {{
-                    name: "{unit}"
-                    {baseUnit}
-                    {factor}
-                    {aggregation}
-                    }})
-                {{
-                    {Utils.errors}
+        correlationId = str(uuid4())
+        with logger.contextualize(correlation_id=correlationId):
+            baseUnit = Utils._argNone('baseUnit', baseUnit)
+            factor = Utils._argNone('factor', factor)
+            aggregation = Utils._argNone('aggregation', aggregation, enum=True)
+
+            graphQLString = f'''
+                mutation updateUnit {{
+                    updateUnit(input: {{
+                        name: "{unit}"
+                        {baseUnit}
+                        {factor}
+                        {aggregation}
+                        }})
+                    {{
+                        {Utils.errors}
+                    }}
                 }}
-            }}
-        '''
-        result = Utils._executeGraphQL(self, graphQLString)
-        if result == None: return
-
-        key = f'updateUnit'
-        if result[key]['errors']:
-            Utils._listGraphQlErrors(result, key)
-        else:
-            logger.info(f"Unit {unit} updated.")
-        return
+            '''
+            result = Utils._executeGraphQL(self, graphQLString)
+            if result == None: return
 
+            key = f'updateUnit'
+            if result[key]['errors']:
+                Utils._listGraphQlErrors(result, key)
+            else:
+                logger.info(f"Unit {unit} updated.")
+            return
 
     def deleteUnit(self, unit:str, force=False) -> None:
         """
         Deletes a unit. Units can only be deleted if there are no Time Series that use this unit. 
         Base units can only be deleted, if no derived units exist.
 
         Parameters:
@@ -1544,44 +1560,48 @@
         force : bool
             Optional, use True to ignore confirmation.
         
         Example:
         >>> deleteUnit('kW', force=True)
         """
 
-        if force == False:
-            confirm = input(f"Press 'y' to delete unit '{unit}'")
-        else: confirm = 'y'
-
-        graphQLString = f'''
-        mutation deleteUnit{{
-            deleteUnit (input: {{
-                name: "{unit}"
-                }})
-                    {{
-                    {Utils.errors}
+        correlationId = str(uuid4())
+        with logger.contextualize(correlation_id=correlationId):
+            if force == False:
+                confirm = input(f"Press 'y' to delete unit '{unit}'")
+            else: confirm = 'y'
+
+            graphQLString = f'''
+            mutation deleteUnit{{
+                deleteUnit (input: {{
+                    name: "{unit}"
+                    }})
+                        {{
+                        {Utils.errors}
+                    }}
                 }}
-            }}
-            '''
+                '''
 
-        result = Utils._executeGraphQL(self, graphQLString)
-        if result == None: return
+            result = Utils._executeGraphQL(self, graphQLString)
+            if result == None: return
 
-        logger.info(f"Unit {unit} deleted.")
+            logger.info(f"Unit {unit} deleted.")
 
-        return
+            return
 
     def refreshSchema(self):
         """
         Updates the time series graphQL schema.
         """
 
-        graphQLString = f'''
-        mutation refreshSchema{{
-            refreshSchema
-            }}
-            '''
+        correlationId = str(uuid4())
+        with logger.contextualize(correlation_id=correlationId):
+            graphQLString = f'''
+            mutation refreshSchema{{
+                refreshSchema
+                }}
+                '''
 
-        result = Utils._executeGraphQL(self, graphQLString)
-        if result == None: return
+            result = Utils._executeGraphQL(self, graphQLString)
+            if result == None: return
 
-        logger.info(f"Refreshed time series schema.")
+            logger.info(f"Refreshed time series schema.")
```

### Comparing `seven2one-4.0.0/seven2one/utils/ut.py` & `seven2one-4.1.0/seven2one/utils/ut.py`

 * *Files 0% similar despite different names*

```diff
@@ -821,15 +821,15 @@
             else:
                 context_logger.error(err)
                 return
 
         try:
             headers = {
                 'authorization': 'Bearer ' + self.accessToken,
-                'X-Correlation-Id': correlationId,
+                'X-Correlation-Id': cid,
             }
             transport =  RequestsHTTPTransport(url=self.endpoint, headers=headers, verify=True, proxies=self.proxies)
             with Client(transport=transport, fetch_schema_from_transport=False) as session:
                 result = session.execute(query, variable_values=params)
         except Exception as err:
             if self.raiseException: raise Exception(err)
             else:
```

### Comparing `seven2one-4.0.0/seven2one/utils/ut_autprog.py` & `seven2one-4.1.0/seven2one/utils/ut_autprog.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one/utils/ut_fileimport.py` & `seven2one-4.1.0/seven2one/utils/ut_fileimport.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one/utils/ut_init.py` & `seven2one-4.1.0/seven2one/utils/ut_init.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one/utils/ut_log.py` & `seven2one-4.1.0/seven2one/utils/ut_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import atexit
-import os
 from loguru import logger
 from ..logging_loki import LokiQueueHandler, emitter
 from . import __version__
 from multiprocessing import Queue
 
 class LogUtils():
     def _init_logging(
@@ -11,15 +10,15 @@
         access_token: str,
         log_level: str, 
         sessionId:str, 
         clientId: str="S2O.TechStack.Python"):
 
         emitter.LokiEmitter.level_tag = "level"
         handler = LokiQueueHandler(
-            Queue(1),
+            Queue(),
             url=url,
             tags={"client": clientId},
             version="1",
             token=access_token
         )
 
         # logger.remove()
```

### Comparing `seven2one-4.0.0/seven2one/utils/ut_meta.py` & `seven2one-4.1.0/seven2one/utils/ut_meta.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one/utils/ut_time.py` & `seven2one-4.1.0/seven2one/utils/ut_time.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one/utils/ut_timeseries.py` & `seven2one-4.1.0/seven2one/utils/ut_timeseries.py`

 * *Files identical despite different names*

### Comparing `seven2one-4.0.0/seven2one.egg-info/PKG-INFO` & `seven2one-4.1.0/seven2one.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seven2one
-Version: 4.0.0
+Version: 4.1.0
 Summary: Functions to interact with the Seven2one TechStack
 Home-page: http://www.seven2one.de
 Author: Seven2one Informationssysteme GmbH
 Author-email: info@seven2one.de
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
```

### Comparing `seven2one-4.0.0/seven2one.egg-info/SOURCES.txt` & `seven2one-4.1.0/seven2one.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/omero-metadata-0.8.2.tar.gz` & `tmp/omero-metadata-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-metadata-0.8.2.tar", last modified: Tue Jul 20 14:16:42 2021, max compression
+gzip compressed data, was "omero-metadata-0.9.0.tar", last modified: Mon Aug 23 11:28:14 2021, max compression
```

## Comparing `omero-metadata-0.8.2.tar` & `omero-metadata-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 14:16:42.171210 omero-metadata-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (121)    17987 2021-07-20 14:16:40.000000 omero-metadata-0.8.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9661 2021-07-20 14:16:42.171210 omero-metadata-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7232 2021-07-20 14:16:40.000000 omero-metadata-0.8.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-20 14:16:42.171210 omero-metadata-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4753 2021-07-20 14:16:40.000000 omero-metadata-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 14:16:42.167209 omero-metadata-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 14:16:42.167209 omero-metadata-0.8.2/src/omero/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 14:16:42.167209 omero-metadata-0.8.2/src/omero/plugins/
--rwxr-xr-x   0 runner    (1001) docker     (121)      498 2021-07-20 14:16:40.000000 omero-metadata-0.8.2/src/omero/plugins/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 14:16:42.167209 omero-metadata-0.8.2/src/omero_metadata/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-20 14:16:40.000000 omero-metadata-0.8.2/src/omero_metadata/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    24179 2021-07-20 14:16:40.000000 omero-metadata-0.8.2/src/omero_metadata/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    85824 2021-07-20 14:16:40.000000 omero-metadata-0.8.2/src/omero_metadata/populate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-20 14:16:42.171210 omero-metadata-0.8.2/src/omero_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9661 2021-07-20 14:16:42.000000 omero-metadata-0.8.2/src/omero_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      395 2021-07-20 14:16:42.000000 omero-metadata-0.8.2/src/omero_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-20 14:16:42.000000 omero-metadata-0.8.2/src/omero_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-07-20 14:16:42.000000 omero-metadata-0.8.2/src/omero_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-07-20 14:16:42.000000 omero-metadata-0.8.2/src/omero_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-20 14:16:42.000000 omero-metadata-0.8.2/src/omero_metadata.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-23 11:28:14.956706 omero-metadata-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    17987 2021-08-23 11:28:12.000000 omero-metadata-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     9661 2021-08-23 11:28:14.956706 omero-metadata-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7232 2021-08-23 11:28:12.000000 omero-metadata-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-23 11:28:14.956706 omero-metadata-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4753 2021-08-23 11:28:12.000000 omero-metadata-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-23 11:28:14.952706 omero-metadata-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-23 11:28:14.952706 omero-metadata-0.9.0/src/omero/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-23 11:28:14.952706 omero-metadata-0.9.0/src/omero/plugins/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      498 2021-08-23 11:28:12.000000 omero-metadata-0.9.0/src/omero/plugins/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-23 11:28:14.952706 omero-metadata-0.9.0/src/omero_metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-23 11:28:12.000000 omero-metadata-0.9.0/src/omero_metadata/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    24179 2021-08-23 11:28:12.000000 omero-metadata-0.9.0/src/omero_metadata/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    85996 2021-08-23 11:28:12.000000 omero-metadata-0.9.0/src/omero_metadata/populate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-23 11:28:14.956706 omero-metadata-0.9.0/src/omero_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9661 2021-08-23 11:28:14.000000 omero-metadata-0.9.0/src/omero_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2021-08-23 11:28:14.000000 omero-metadata-0.9.0/src/omero_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-23 11:28:14.000000 omero-metadata-0.9.0/src/omero_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2021-08-23 11:28:14.000000 omero-metadata-0.9.0/src/omero_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-08-23 11:28:14.000000 omero-metadata-0.9.0/src/omero_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-23 11:28:14.000000 omero-metadata-0.9.0/src/omero_metadata.egg-info/zip-safe
```

### Comparing `omero-metadata-0.8.2/LICENSE.txt` & `omero-metadata-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `omero-metadata-0.8.2/PKG-INFO` & `omero-metadata-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: omero-metadata
-Version: 0.8.2
+Version: 0.9.0
 Summary: Metadata plugin for use in the OMERO CLI.
 Home-page: https://github.com/ome/omero-metadata/
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: GPL-2.0+
-Download-URL: https://github.com/ome/omero-metadata//v0.8.2.tar.gz
+Download-URL: https://github.com/ome/omero-metadata//v0.9.0.tar.gz
 Description: .. image:: https://github.com/ome/omero-metadata/workflows/OMERO/badge.svg
             :target: https://github.com/ome/omero-metadata/actions
         
         .. image:: https://badge.fury.io/py/omero-metadata.svg
             :target: https://badge.fury.io/py/omero-metadata
         
         OMERO metadata plugin
```

### Comparing `omero-metadata-0.8.2/README.rst` & `omero-metadata-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `omero-metadata-0.8.2/setup.py` & `omero-metadata-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     """
     Utility function to read the README file.
     :rtype : String
     """
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
-version = '0.8.2'
+version = '0.9.0'
 url = "https://github.com/ome/omero-metadata/"
 
 setup(
     version=version,
     packages=['', 'omero_metadata', 'omero.plugins'],
     package_dir={"": "src"},
     name='omero-metadata',
```

### Comparing `omero-metadata-0.8.2/src/omero_metadata/cli.py` & `omero-metadata-0.9.0/src/omero_metadata/cli.py`

 * *Files identical despite different names*

### Comparing `omero-metadata-0.8.2/src/omero_metadata/populate.py` & `omero-metadata-0.9.0/src/omero_metadata/populate.py`

 * *Files 1% similar despite different names*

```diff
@@ -984,15 +984,16 @@
 
 class ParsingContext(object):
     """Generic parsing context for CSV files."""
 
     def __init__(self, client, target_object, file=None, fileid=None,
                  cfg=None, cfgid=None, attach=False, column_types=None,
                  options=None, batch_size=1000, loops=10, ms=500,
-                 dry_run=False, allow_nan=False):
+                 dry_run=False, allow_nan=False,
+                 table_name=DEFAULT_TABLE_NAME):
         '''
         This lines should be handled outside of the constructor:
 
         if not file:
             raise MetadataError('file required for %s' % type(self))
         if fileid and not file:
             raise MetadataError('fileid not supported for %s' % type(self))
@@ -1008,14 +1009,17 @@
         self.column_types = column_types
         self.value_resolver = ValueResolver(client, target_object,
                                             allow_nan=allow_nan)
         self.parsing_util_factory = ParsingUtilFactory(client,
                                                        target_object,
                                                        self.value_resolver)
         self.dry_run = dry_run
+        if not table_name:
+            table_name = DEFAULT_TABLE_NAME     # just in case
+        self.table_name = table_name
 
     def create_annotation_link(self):
         self.target_class = self.target_object.__class__
         if ScreenI is self.target_class:
             return ScreenAnnotationLinkI()
         if PlateI is self.target_class:
             return PlateAnnotationLinkI()
@@ -1098,15 +1102,15 @@
         log.debug('Columns: %r' % [
             (o.name, len(o.values)) for o in self.columns])
 
     def create_table(self):
         sf = self.client.getSession()
         group = str(self.value_resolver.target_group)
         sr = sf.sharedResources()
-        table = sr.newTable(1, DEFAULT_TABLE_NAME,
+        table = sr.newTable(1, self.table_name,
                             {'omero.group': native_str(group)})
         if table is None:
             raise MetadataError(
                 "Unable to create table: %s" % DEFAULT_TABLE_NAME)
         original_file = table.getOriginalFile()
         log.info('Created new table OriginalFile:%d' % original_file.id.val)
         table.initialize(self.columns)
```

### Comparing `omero-metadata-0.8.2/src/omero_metadata.egg-info/PKG-INFO` & `omero-metadata-0.9.0/src/omero_metadata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: omero-metadata
-Version: 0.8.2
+Version: 0.9.0
 Summary: Metadata plugin for use in the OMERO CLI.
 Home-page: https://github.com/ome/omero-metadata/
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: GPL-2.0+
-Download-URL: https://github.com/ome/omero-metadata//v0.8.2.tar.gz
+Download-URL: https://github.com/ome/omero-metadata//v0.9.0.tar.gz
 Description: .. image:: https://github.com/ome/omero-metadata/workflows/OMERO/badge.svg
             :target: https://github.com/ome/omero-metadata/actions
         
         .. image:: https://badge.fury.io/py/omero-metadata.svg
             :target: https://badge.fury.io/py/omero-metadata
         
         OMERO metadata plugin
```


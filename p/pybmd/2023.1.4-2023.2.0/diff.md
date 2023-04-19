# Comparing `tmp/pybmd-2023.1.4.tar.gz` & `tmp/pybmd-2023.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybmd-2023.1.4.tar", last modified: Sat Feb 25 07:36:14 2023, max compression
+gzip compressed data, was "pybmd-2023.2.0.tar", last modified: Wed Apr 19 09:35:47 2023, max compression
```

## Comparing `pybmd-2023.1.4.tar` & `pybmd-2023.2.0.tar`

### file list

```diff
@@ -1,32 +1,28 @@
-drwxr-xr-x   0 wheheohu   (501) staff       (20)        0 2023-02-25 07:36:14.116473 pybmd-2023.1.4/
--rw-r--r--   0 wheheohu   (501) staff       (20)     7651 2022-03-20 10:43:01.000000 pybmd-2023.1.4/LICENSE
--rw-r--r--   0 wheheohu   (501) staff       (20)     1648 2023-02-25 07:36:14.116326 pybmd-2023.1.4/PKG-INFO
--rw-r--r--   0 wheheohu   (501) staff       (20)     1101 2022-09-13 10:05:42.000000 pybmd-2023.1.4/README.md
-drwxr-xr-x   0 wheheohu   (501) staff       (20)        0 2023-02-25 07:36:14.115111 pybmd-2023.1.4/pybmd/
--rw-r--r--   0 wheheohu   (501) staff       (20)       37 2023-01-10 15:05:41.000000 pybmd-2023.1.4/pybmd/__init__.py
--rw-r--r--   0 wheheohu   (501) staff       (20)     8176 2023-02-25 07:29:58.000000 pybmd-2023.1.4/pybmd/bmd.py
--rw-r--r--   0 wheheohu   (501) staff       (20)      158 2023-01-10 15:15:37.000000 pybmd-2023.1.4/pybmd/error.py
--rw-r--r--   0 wheheohu   (501) staff       (20)     1476 2022-09-22 00:27:30.000000 pybmd-2023.1.4/pybmd/folder.py
--rw-r--r--   0 wheheohu   (501) staff       (20)      149 2022-08-01 06:11:45.000000 pybmd-2023.1.4/pybmd/fusion_comp.py
--rw-r--r--   0 wheheohu   (501) staff       (20)     1845 2022-08-01 07:12:52.000000 pybmd-2023.1.4/pybmd/gallery.py
--rw-r--r--   0 wheheohu   (501) staff       (20)      139 2022-09-05 06:27:20.000000 pybmd-2023.1.4/pybmd/gallery_still.py
--rw-r--r--   0 wheheohu   (501) staff       (20)     2921 2023-02-25 06:49:59.000000 pybmd-2023.1.4/pybmd/gallery_still_album.py
--rw-r--r--   0 wheheohu   (501) staff       (20)    10524 2022-08-22 01:46:45.000000 pybmd-2023.1.4/pybmd/media_pool.py
--rw-r--r--   0 wheheohu   (501) staff       (20)     7747 2022-09-22 00:27:19.000000 pybmd-2023.1.4/pybmd/media_pool_item.py
--rw-r--r--   0 wheheohu   (501) staff       (20)     3576 2022-08-16 16:01:10.000000 pybmd-2023.1.4/pybmd/media_storage.py
--rw-r--r--   0 wheheohu   (501) staff       (20)    10188 2023-02-25 07:35:47.000000 pybmd-2023.1.4/pybmd/project.py
--rw-r--r--   0 wheheohu   (501) staff       (20)     7038 2022-08-05 16:36:04.000000 pybmd-2023.1.4/pybmd/project_manager.py
--rw-r--r--   0 wheheohu   (501) staff       (20)    14261 2023-02-25 06:49:59.000000 pybmd-2023.1.4/pybmd/timeline.py
--rw-r--r--   0 wheheohu   (501) staff       (20)    14963 2022-09-22 00:26:54.000000 pybmd-2023.1.4/pybmd/timeline_item.py
--rw-r--r--   0 wheheohu   (501) staff       (20)     3097 2022-10-31 16:20:04.000000 pybmd-2023.1.4/pybmd/toolkits.py
-drwxr-xr-x   0 wheheohu   (501) staff       (20)        0 2023-02-25 07:36:14.115816 pybmd-2023.1.4/pybmd.egg-info/
--rw-r--r--   0 wheheohu   (501) staff       (20)     1648 2023-02-25 07:36:14.000000 pybmd-2023.1.4/pybmd.egg-info/PKG-INFO
--rw-r--r--   0 wheheohu   (501) staff       (20)      525 2023-02-25 07:36:14.000000 pybmd-2023.1.4/pybmd.egg-info/SOURCES.txt
--rw-r--r--   0 wheheohu   (501) staff       (20)        1 2023-02-25 07:36:14.000000 pybmd-2023.1.4/pybmd.egg-info/dependency_links.txt
--rw-r--r--   0 wheheohu   (501) staff       (20)       17 2023-02-25 07:36:14.000000 pybmd-2023.1.4/pybmd.egg-info/requires.txt
--rw-r--r--   0 wheheohu   (501) staff       (20)       11 2023-02-25 07:36:14.000000 pybmd-2023.1.4/pybmd.egg-info/top_level.txt
--rw-r--r--   0 wheheohu   (501) staff       (20)       38 2023-02-25 07:36:14.116515 pybmd-2023.1.4/setup.cfg
--rw-r--r--   0 wheheohu   (501) staff       (20)      780 2023-02-25 07:35:58.000000 pybmd-2023.1.4/setup.py
-drwxr-xr-x   0 wheheohu   (501) staff       (20)        0 2023-02-25 07:36:14.116141 pybmd-2023.1.4/test/
--rw-r--r--   0 wheheohu   (501) staff       (20)        0 2023-01-12 03:20:05.000000 pybmd-2023.1.4/test/__init__.py
--rw-r--r--   0 wheheohu   (501) staff       (20)    14868 2023-01-13 03:44:25.000000 pybmd-2023.1.4/test/test_bmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:35:47.206812 pybmd-2023.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-19 09:35:34.000000 pybmd-2023.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-19 09:35:47.206812 pybmd-2023.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-19 09:35:34.000000 pybmd-2023.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:35:47.206812 pybmd-2023.2.0/pybmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/bmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/fusion_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/gallery_still.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/gallery_still_album.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/media_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/media_pool_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/media_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/project_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14261 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/timeline_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-19 09:35:34.000000 pybmd-2023.2.0/pybmd/toolkits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:35:47.206812 pybmd-2023.2.0/pybmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-19 09:35:47.000000 pybmd-2023.2.0/pybmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-19 09:35:47.000000 pybmd-2023.2.0/pybmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 09:35:47.000000 pybmd-2023.2.0/pybmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 09:35:47.000000 pybmd-2023.2.0/pybmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 09:35:47.206812 pybmd-2023.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-19 09:35:34.000000 pybmd-2023.2.0/setup.py
```

### Comparing `pybmd-2023.1.4/LICENSE` & `pybmd-2023.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybmd-2023.1.4/PKG-INFO` & `pybmd-2023.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pybmd
-Version: 2023.1.4
+Version: 2023.2.0
 Summary: python library for Davinci Resolve(Repack)
 Home-page: https://github.com/WheheoHu/pybmd
 Author: wheheo
 Author-email: wheheohu@outlook.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -45,8 +43,7 @@
 
     Play with APIs!
     
     Original API documentation could be found at my notion:
     [Davnci Resolve API in notion](https://wheheohu.notion.site/Davinci-Python-API-7c4f1038a36f44818b631ec7e4a537fa)
 
     Pybmd Library API documentation could be found at :[Pybmd API Documentation](https://wheheohu.github.io/pybmd/)
-
```

### Comparing `pybmd-2023.1.4/README.md` & `pybmd-2023.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pybmd-2023.1.4/pybmd/bmd.py` & `pybmd-2023.2.0/pybmd/bmd.py`

 * *Files identical despite different names*

### Comparing `pybmd-2023.1.4/pybmd/gallery.py` & `pybmd-2023.2.0/pybmd/gallery.py`

 * *Files identical despite different names*

### Comparing `pybmd-2023.1.4/pybmd/gallery_still_album.py` & `pybmd-2023.2.0/pybmd/gallery_still_album.py`

 * *Files identical despite different names*

### Comparing `pybmd-2023.1.4/pybmd/media_pool.py` & `pybmd-2023.2.0/pybmd/media_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,8 +274,23 @@
     def refresh_folders(self) -> bool:
         """Updates the folders in collaboration mode"""
         return self.media_pool.RefreshFolders()
     
     def get_unique_id(self) -> str:
         """get unique id of media pool object"""
         return self.media_pool.GetUniqueId()
+    
+    ##########################################################################################################################
+    #Add at DR18.5.0
+    
+    def import_folder_from_file(self,file_path:str,source_clips_path:str) -> bool:
+        """Returns true if import from given DRB filePath is successful, false otherwise
+
+        Args:
+            file_path (str): file path to DRB file
+            source_clips_path (str): sourceClipsPath is a string that specifies a filesystem path to search for source clips if the media is inaccessible in their original path, empty by default
+
+        Returns:
+            bool: Returns true if import from given DRB filePath is successful, false otherwise
+        """        
+        return self.media_pool.ImportFolderFromFile(file_path,source_clips_path)
```

### Comparing `pybmd-2023.1.4/pybmd/media_pool_item.py` & `pybmd-2023.2.0/pybmd/media_pool_item.py`

 * *Files identical despite different names*

### Comparing `pybmd-2023.1.4/pybmd/media_storage.py` & `pybmd-2023.2.0/pybmd/media_storage.py`

 * *Files identical despite different names*

### Comparing `pybmd-2023.1.4/pybmd/project.py` & `pybmd-2023.2.0/pybmd/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -258,20 +258,33 @@
     def get_unique_id(self) -> str:
         """Returns unique id of the project Object."""
         return self.project.GetUniqueId()
 
     ##############################################################################################################################
     # Add at DR18.1.3
 
-    # TODO add InsertAudioToCurrentTrackAtPlayhead
     def insert_audio_to_current_track_at_playhead(self, media_path: str, start_offset_in_samples: int, duration_in_samples: int) -> bool:
         """Inserts the media specified by mediaPath (string) with startOffsetInSamples (int) and durationInSamples (int) at the playhead on a selected track on the Fairlight page. 
         
         Args:
             media_path (str)
             start_offset_in_samples (int)
             duration_in_samples (int)
 
         Returns:
             bool: Returns True if successful, otherwise False.
         """        
         return self.project.InsertAudioToCurrentTrackAtPlayhead(media_path, start_offset_in_samples, duration_in_samples)
+
+    ##############################################################################################################################
+    # Add at DR18.5.0
+    
+    def load_burn_in_preset(self,preset_name:str) -> bool:
+        """Loads user defined data burn in preset for project when supplied presetName (string). 
+
+        Args:
+            preset_name (str): preset name
+
+        Returns:
+            bool: Returns true if successful.
+        """        
+        return self.project.LoadBurnInPreset(preset_name)
```

### Comparing `pybmd-2023.1.4/pybmd/project_manager.py` & `pybmd-2023.2.0/pybmd/project_manager.py`

 * *Files identical despite different names*

### Comparing `pybmd-2023.1.4/pybmd/timeline.py` & `pybmd-2023.2.0/pybmd/timeline.py`

 * *Files identical despite different names*

### Comparing `pybmd-2023.1.4/pybmd/timeline_item.py` & `pybmd-2023.2.0/pybmd/timeline_item.py`

 * *Files 7% similar despite different names*

```diff
@@ -356,8 +356,59 @@
         """Updates sidecar file for BRAW clips or RMD file for R3D clips."""
         return self.timeline_item.UpdateSidecar()
 
     def get_unique_id(self) -> str:
         """Returns a unique ID for the timeline item"""
         return self.timeline_item.GetUniqueId()
 
-    ########################################################################################################################
+    ##########################################################################################################################
+    # Add at DR18.5.0
+    
+    def apply_arri_cdl_lut(self) -> bool:
+        """Applies ARRI CDL and LUT.
+
+        Returns:
+            bool: Returns True if successful, False otherwise.
+        """        
+        return self.timeline_item.ApplyArriCdlLut()
+    
+    def set_clip_enabled(self,bool_value:bool) -> bool:
+        """Sets clip enabled based on argument.
+
+        Args:
+            bool_value (bool): Sets clip enabled based on argument.
+
+        Returns:
+            bool: True for clip is enabled
+        """        
+        return self.timeline_item.SetClipEnabled(bool_value)
+    
+    def get_clip_enabled(self) -> bool:
+        """Gets clip enabled status.
+
+        Returns:
+            bool: clip enabled status 
+        """        
+        return self.timeline_item.GetClipEnabled()
+    
+    def load_burn_in_preset(self,preset_name:str) -> bool:
+        """Loads user defined data burn in preset for clip when supplied presetName (string). Returns true if successful.
+
+        Args:
+            preset_name (str): burn-in preset name
+
+        Returns:
+            bool: Returns true if successful
+        """        
+        return self.timeline_item.LoadBurnInPreset(preset_name)
+    
+    def get_node_label(self,node_index:int) -> str:
+        """Returns the label of the node at nodeIndex.
+
+        Args:
+            node_index (int): node index
+
+        Returns:
+            str: node label
+        """        
+        return self.timeline_item.GetNodeLabel(node_index)
+
```

### Comparing `pybmd-2023.1.4/pybmd/toolkits.py` & `pybmd-2023.2.0/pybmd/toolkits.py`

 * *Files identical despite different names*

### Comparing `pybmd-2023.1.4/pybmd.egg-info/PKG-INFO` & `pybmd-2023.2.0/pybmd.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pybmd
-Version: 2023.1.4
+Version: 2023.2.0
 Summary: python library for Davinci Resolve(Repack)
 Home-page: https://github.com/WheheoHu/pybmd
 Author: wheheo
 Author-email: wheheohu@outlook.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -45,8 +43,7 @@
 
     Play with APIs!
     
     Original API documentation could be found at my notion:
     [Davnci Resolve API in notion](https://wheheohu.notion.site/Davinci-Python-API-7c4f1038a36f44818b631ec7e4a537fa)
 
     Pybmd Library API documentation could be found at :[Pybmd API Documentation](https://wheheohu.github.io/pybmd/)
-
```

### Comparing `pybmd-2023.1.4/setup.py` & `pybmd-2023.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as rm:
     long_description = rm.read()
 
 setuptools.setup(
     name="pybmd",
-    version="2023.1.4",
+    version="2023.2.0",
     author="wheheo",
     author_email="wheheohu@outlook.com",
     description="python library for Davinci Resolve(Repack)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/WheheoHu/pybmd",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows"
     ],
-    install_requires=[
-        "multipledispatch"
-        ],
 
 )
```


# Comparing `tmp/xmipp_metadata-1.0.7.tar.gz` & `tmp/xmipp_metadata-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmipp_metadata-1.0.7.tar", last modified: Wed Mar 29 11:54:03 2023, max compression
+gzip compressed data, was "xmipp_metadata-1.0.8.tar", last modified: Wed Apr 19 08:14:13 2023, max compression
```

## Comparing `xmipp_metadata-1.0.7.tar` & `xmipp_metadata-1.0.8.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:54:03.991082 xmipp_metadata-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 11:53:38.000000 xmipp_metadata-1.0.7/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-29 11:53:38.000000 xmipp_metadata-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-29 11:53:38.000000 xmipp_metadata-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-29 11:54:03.991082 xmipp_metadata-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-29 11:53:38.000000 xmipp_metadata-1.0.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-29 11:53:38.000000 xmipp_metadata-1.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 11:54:03.991082 xmipp_metadata-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-29 11:53:38.000000 xmipp_metadata-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:54:03.987081 xmipp_metadata-1.0.7/xmipp_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-29 11:53:38.000000 xmipp_metadata-1.0.7/xmipp_metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:54:03.987081 xmipp_metadata-1.0.7/xmipp_metadata/image_handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-29 11:53:38.000000 xmipp_metadata-1.0.7/xmipp_metadata/image_handler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5553 2023-03-29 11:53:38.000000 xmipp_metadata-1.0.7/xmipp_metadata/image_handler/image_handler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8255 2023-03-29 11:53:38.000000 xmipp_metadata-1.0.7/xmipp_metadata/image_handler/image_spider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:54:03.987081 xmipp_metadata-1.0.7/xmipp_metadata/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-03-29 11:53:38.000000 xmipp_metadata-1.0.7/xmipp_metadata/metadata/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9073 2023-03-29 11:53:38.000000 xmipp_metadata-1.0.7/xmipp_metadata/metadata/xmipp_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:54:03.991082 xmipp_metadata-1.0.7/xmipp_metadata/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 11:53:38.000000 xmipp_metadata-1.0.7/xmipp_metadata/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-03-29 11:53:38.000000 xmipp_metadata-1.0.7/xmipp_metadata/tests/test_image_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-03-29 11:53:38.000000 xmipp_metadata-1.0.7/xmipp_metadata/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-03-29 11:53:38.000000 xmipp_metadata-1.0.7/xmipp_metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:54:03.987081 xmipp_metadata-1.0.7/xmipp_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-29 11:54:03.000000 xmipp_metadata-1.0.7/xmipp_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-29 11:54:03.000000 xmipp_metadata-1.0.7/xmipp_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 11:54:03.000000 xmipp_metadata-1.0.7/xmipp_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-29 11:54:03.000000 xmipp_metadata-1.0.7/xmipp_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-29 11:54:03.000000 xmipp_metadata-1.0.7/xmipp_metadata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.299775 xmipp_metadata-1.0.8/xmipp_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2566 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_em.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16132 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_handler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3039 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_mrc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9178 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_spider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/xmipp_metadata/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/metadata/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9142 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/metadata/xmipp_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.303775 xmipp_metadata-1.0.8/xmipp_metadata/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/tests/test_image_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-19 08:11:50.000000 xmipp_metadata-1.0.8/xmipp_metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:14:13.299775 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-19 08:14:13.000000 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-19 08:14:13.000000 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:14:13.000000 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-19 08:14:13.000000 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 08:14:13.000000 xmipp_metadata-1.0.8/xmipp_metadata.egg-info/top_level.txt
```

### Comparing `xmipp_metadata-1.0.7/LICENSE` & `xmipp_metadata-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.7/PKG-INFO` & `xmipp_metadata-1.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: xmipp_metadata
-Version: 1.0.7
+Version: 1.0.8
 Summary: Package to handle Xmipp Metadata and image binary data
 Home-page: https://github.com/DavidHerreros/xmipp_metadata
 Author: David Herreros
 Author-email: dherreros@cnb.csic.es
 License: UNKNOWN
 Description: =======================
         Xmipp Metadata Handler
@@ -16,10 +16,11 @@
         Included functionalities
         ==========================
         
         - **XmippMetadata** class: Reading and writing of Xmipp Metadata files (.xmd)
         - **ImageHandler** class: Reading and writing of image binaries stored in the metadata. It support the following formats:
             - MRC files (reading and writing) for stacks and volumes (.mrcs and .mrc)
             - Spider files (reading and writing) for stacks and volumes (.stk and .vol)
+            - EM files (reading and writing) for stack and images (.ems and .em)
         
 Keywords: xmipp scipion cryoem imageprocessing scipion-3.0
 Platform: UNKNOWN
```

### Comparing `xmipp_metadata-1.0.7/README.rst` & `xmipp_metadata-1.0.8/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 Included functionalities
 ==========================
 
 - **XmippMetadata** class: Reading and writing of Xmipp Metadata files (.xmd)
 - **ImageHandler** class: Reading and writing of image binaries stored in the metadata. It support the following formats:
     - MRC files (reading and writing) for stacks and volumes (.mrcs and .mrc)
     - Spider files (reading and writing) for stacks and volumes (.stk and .vol)
+    - EM files (reading and writing) for stack and images (.ems and .em)
```

### Comparing `xmipp_metadata-1.0.7/setup.py` & `xmipp_metadata-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.7/xmipp_metadata/__init__.py` & `xmipp_metadata-1.0.8/xmipp_metadata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-__version__ = "1.0.7"
+__version__ = "1.0.8"
```

### Comparing `xmipp_metadata-1.0.7/xmipp_metadata/image_handler/__init__.py` & `xmipp_metadata-1.0.8/xmipp_metadata/image_handler/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,8 +21,10 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from .image_handler import ImageHandler
-from .image_spider import ImageSpider
+from .image_spider import ImageSpider
+from .image_em import ImageEM
+from .image_mrc import ImageMRC
```

### Comparing `xmipp_metadata-1.0.7/xmipp_metadata/image_handler/image_spider.py` & `xmipp_metadata-1.0.8/xmipp_metadata/image_handler/image_spider.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,29 +24,33 @@
 # *
 # **************************************************************************
 
 
 import struct
 import numpy as np
 from pathlib import Path
+import os
 
 
 class ImageSpider(object):
     '''
     Class to read an STK image file generated with XMIPP
     '''
 
     HEADER_OFFSET = 1024
     FLOAT32_BYTES = 4
     TYPE = None
 
-    def __init__(self, filename):
-        self.stk_handler = open(filename, "rb")
-        self.header_info = self.read_header()
-        self.IMG_BYTES = self.FLOAT32_BYTES * self.header_info["n_columns"] ** 2
+    def __init__(self, filename=None):
+        if filename:
+            self.stk_handler = open(filename, "rb")
+            self.header_info = self.read_header()
+            self.IMG_BYTES = self.FLOAT32_BYTES * self.header_info["n_columns"] ** 2
+        else:
+            self.stk_handler, self.header_info, self.IMG_BYTES = None, None, None
 
     def __del__(self):
         '''
         Close the current file before deleting
         '''
         self.close()
         print("File closed succesfully!")
@@ -71,14 +75,23 @@
             return np.stack([self.read_image(ii) for ii in item])
         elif isinstance(item, slice):
             start = item.start if item.start else 0
             stop = item.stop if item.stop else len(self)
             step = item.step if item.step else 1
             return np.stack([self.read_image(ii) for ii in range(start, stop, step)])
 
+    def read(self, filename):
+        '''
+        Reads a given image
+           :param filename (str) --> Image to be read
+        '''
+        self.stk_handler = open(filename, "rb")
+        self.header_info = self.read_header()
+        self.IMG_BYTES = self.FLOAT32_BYTES * self.header_info["n_columns"] ** 2
+
     def read_binary(self, start, end):
         '''
         Read bytes between start and end
             :param start (int) --> Start byte
             :param end (int) --> End byte
             :returns the bytes read
         '''
@@ -105,15 +118,16 @@
         '''
         Reads the header of the current file as a dictionary
             :returns The current header as a dictionary
         '''
         header = self.read_numpy(0, self.HEADER_OFFSET)
 
         header = dict(img_size=int(header[1]), n_images=int(header[25]), offset=int(header[21]),
-                      n_rows=int(header[1]), n_columns=int(header[11]), n_slices=int(header[0]))
+                      n_rows=int(header[1]), n_columns=int(header[11]), n_slices=int(header[0]),
+                      sr=float(header[20]))
 
         self.TYPE = "stack" if header["n_images"] > 1 else "volume"
 
         return header
 
     def read_image(self, iid):
         '''
@@ -126,69 +140,73 @@
             start = 2 * self.header_info["offset"] + iid * (self.IMG_BYTES + self.header_info["offset"])
         else:
             start = self.header_info["offset"] + iid * self.IMG_BYTES
 
         img_size = self.header_info["n_columns"]
         return self.read_numpy(start, self.IMG_BYTES).reshape([img_size, img_size])
 
-    def write(self, data, filename=None, overwrite=False):
+    def write(self, data, filename=None, overwrite=False, sr=1.0):
         data = data.astype(np.float32)
+        sr = 1.0 if sr == 0.0 else sr
+
+        if overwrite and os.path.isfile(filename):
+            os.remove(filename)
 
         if filename:
             mode = Path(filename).suffix
             fid = open(filename, "wb")
             if len(data.shape) == 3:
                 # Write first header
-                header = self.makeSpiderHeader(data, mode=mode)
+                header = self.makeSpiderHeader(data, mode=mode, sr=sr)
                 fid.writelines(header)
 
                 # Write slices
                 for slice in data:
                     if mode == ".stk":
-                        header = self.makeSpiderHeader(slice[None, ...], mode=mode)
+                        header = self.makeSpiderHeader(slice[None, ...], mode=mode, sr=sr)
                         fid.writelines(header)
                     fid.writelines(slice)
             else:
                 mode = ".vol"
                 # Write image
                 data = data[None, ...] if len(data.shape) == 2 else data
-                header = self.makeSpiderHeader(data, mode=mode)
+                header = self.makeSpiderHeader(data, mode=mode, sr=sr)
                 fid.writelines(header)
                 fid.writelines(data)
             fid.close()
         else:
             filename = self.stk_handler.name
             mode = Path(filename).suffix
             if data.shape[0] == len(self) or overwrite:
                 fid = open(filename, "wb")
                 if len(data.shape) == 3:
                     # Write first header
-                    header = self.makeSpiderHeader(data, mode=mode)
+                    header = self.makeSpiderHeader(data, mode=mode, sr=sr)
                     fid.writelines(header)
 
                     # Write slices
                     for slice in data:
                         if mode == ".stk":
-                            header = self.makeSpiderHeader(slice[None, ...], mode=mode)
+                            header = self.makeSpiderHeader(slice[None, ...], mode=mode, sr=sr)
                             fid.writelines(header)
                         fid.writelines(slice)
                 else:
                     mode = ".vol"
                     # Write image
                     data = data[None, ...] if len(data.shape) == 2 else data
-                    header = self.makeSpiderHeader(data, mode=mode)
+                    header = self.makeSpiderHeader(data, mode=mode, sr=sr)
                     fid.writelines(header)
                     fid.writelines(data)
                 fid.close()
             else:
                 raise Exception("Cannot save file. Number of images "
                                 "in new data is different. Please, set overwrite to True "
                                 "if you are sure you want to do this.")
 
-    def makeSpiderHeader(self, im, mode):
+    def makeSpiderHeader(self, im, mode, sr=1.0):
         n_slice, nsam, nrow = im.shape
         lenbyt = nsam * 4  # There are labrec records in the header
         labrec = int(1024 / lenbyt)
         if 1024 % lenbyt != 0:
             labrec += 1
         labbyt = labrec * lenbyt
         nvalues = int(labbyt / 4)
@@ -202,24 +220,32 @@
         # NB these are Fortran indices
         hdr[1] = float(n_slice) if mode == ".vol" else 1.0  # nslice (=1 for an image)
         hdr[2] = float(nrow)  # number of rows per slice
         hdr[3] = float(nrow)  # number of records in the image
         hdr[5] = 1.0 if mode == ".stk" else 3.0
         hdr[12] = float(nsam)  # number of pixels per line
         hdr[13] = float(labrec)  # number of records in file header
+        hdr[21] = float(sr)  # sampling rate
         hdr[22] = float(labbyt)  # total number of bytes in header
         hdr[23] = float(lenbyt)  # record length in bytes
         hdr[24] = 2.0 if mode == ".stk" else 0.0
         hdr[25] = 1.0 if mode == ".stk" else 0.0
         hdr[26] = float(n_slice) if mode == ".stk" else 1.0  # nobjects (=1 for an image/vol)
 
         # adjust for Fortran indexing
         hdr = hdr[1:]
         hdr.append(0.0)
         # pack binary data into a string
         return [struct.pack("f", v) for v in hdr]
 
+    def getSamplingRate(self):
+        if self.header_info is not None:
+            return self.header_info["sr"]
+        else:
+            return None
+
     def close(self):
         '''
         Closes the current file
         '''
-        self.stk_handler.close()
+        if self.stk_handler is not None:
+            self.stk_handler.close()
```

### Comparing `xmipp_metadata-1.0.7/xmipp_metadata/metadata/__init__.py` & `xmipp_metadata-1.0.8/xmipp_metadata/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.7/xmipp_metadata/metadata/xmipp_metadata.py` & `xmipp_metadata-1.0.8/xmipp_metadata/metadata/xmipp_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         self.binaries = ImageHandler(binary_file)
 
         # Fill non-existing columns
         remain = set(self.DEFAULT_COLUMN_NAMES).difference(set(self.getMetaDataLabels()))
         for label in remain:
             self.table[label] = 0.0
 
-    def write(self, filename, overwrite=False):
+    def write(self, filename, overwrite=False, updateImagePaths=False):
         '''
         Write current metadata to file
         '''
         # Filename path
         filename_path = Path(filename).resolve().parent
 
         # Image path
@@ -143,18 +143,19 @@
 
             # Recompose path
             if index:
                 image = index + "@" + file
 
             return image
 
-        for idx in range(len(self)):
-            image = self.getMetadataItems(idx, "image")[0]
-            image = composeImageRelPath(image, filename_path)
-            self.setMetaDataItems(image, idx, "image")
+        if updateImagePaths:
+            for idx in range(len(self)):
+                image = self.getMetadataItems(idx, "image")[0]
+                image = composeImageRelPath(image, filename_path)
+                self.setMetaDataItems(image, idx, "image")
         starfile.write(self.table, filename, overwrite=overwrite)
 
     def __del__(self):
         '''
         Closes the Metadata file and binaries to save memory
         '''
         self.binaries.close()
```

### Comparing `xmipp_metadata-1.0.7/xmipp_metadata/tests/test_metadata.py` & `xmipp_metadata-1.0.8/xmipp_metadata/tests/test_metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,9 +54,13 @@
 metadata = XmippMetaData("input_particles.xmd")
 
 
 # Get image with ImageHandler
 img = metadata.getMetaDataImage(0)
 
 
-# Write metadata
-metadata.write(filename=os.path.join("test_outputs", "test.xmd"))
+# Write metadata (do not update paths)
+metadata.write(filename=os.path.join("test_outputs", "test_same_paths.xmd"))
+
+
+# Write metadata (update paths)
+metadata.write(filename=os.path.join("test_outputs", "test_new_paths.xmd"), updateImagePaths=True)
```

### Comparing `xmipp_metadata-1.0.7/xmipp_metadata/utils.py` & `xmipp_metadata-1.0.8/xmipp_metadata/utils.py`

 * *Files identical despite different names*

### Comparing `xmipp_metadata-1.0.7/xmipp_metadata.egg-info/PKG-INFO` & `xmipp_metadata-1.0.8/xmipp_metadata.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: xmipp-metadata
-Version: 1.0.7
+Version: 1.0.8
 Summary: Package to handle Xmipp Metadata and image binary data
 Home-page: https://github.com/DavidHerreros/xmipp_metadata
 Author: David Herreros
 Author-email: dherreros@cnb.csic.es
 License: UNKNOWN
 Description: =======================
         Xmipp Metadata Handler
@@ -16,10 +16,11 @@
         Included functionalities
         ==========================
         
         - **XmippMetadata** class: Reading and writing of Xmipp Metadata files (.xmd)
         - **ImageHandler** class: Reading and writing of image binaries stored in the metadata. It support the following formats:
             - MRC files (reading and writing) for stacks and volumes (.mrcs and .mrc)
             - Spider files (reading and writing) for stacks and volumes (.stk and .vol)
+            - EM files (reading and writing) for stack and images (.ems and .em)
         
 Keywords: xmipp scipion cryoem imageprocessing scipion-3.0
 Platform: UNKNOWN
```

### Comparing `xmipp_metadata-1.0.7/xmipp_metadata.egg-info/SOURCES.txt` & `xmipp_metadata-1.0.8/xmipp_metadata.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 xmipp_metadata/utils.py
 xmipp_metadata.egg-info/PKG-INFO
 xmipp_metadata.egg-info/SOURCES.txt
 xmipp_metadata.egg-info/dependency_links.txt
 xmipp_metadata.egg-info/requires.txt
 xmipp_metadata.egg-info/top_level.txt
 xmipp_metadata/image_handler/__init__.py
+xmipp_metadata/image_handler/image_em.py
 xmipp_metadata/image_handler/image_handler.py
+xmipp_metadata/image_handler/image_mrc.py
 xmipp_metadata/image_handler/image_spider.py
 xmipp_metadata/metadata/__init__.py
 xmipp_metadata/metadata/xmipp_metadata.py
 xmipp_metadata/tests/__init__.py
 xmipp_metadata/tests/test_image_handler.py
 xmipp_metadata/tests/test_metadata.py
```


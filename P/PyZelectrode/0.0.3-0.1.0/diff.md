# Comparing `tmp/PyZelectrode-0.0.3.tar.gz` & `tmp/PyZelectrode-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyZelectrode-0.0.3.tar", last modified: Mon Jan  9 17:29:07 2023, max compression
+gzip compressed data, was "PyZelectrode-0.1.0.tar", last modified: Tue Apr 18 22:29:37 2023, max compression
```

## Comparing `PyZelectrode-0.0.3.tar` & `PyZelectrode-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-01-09 17:29:07.828147 PyZelectrode-0.0.3/
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     1146 2023-01-09 17:29:07.828147 PyZelectrode-0.0.3/PKG-INFO
-drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-01-09 17:29:07.828147 PyZelectrode-0.0.3/PyZelectrode/
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    10055 2023-01-09 17:19:42.000000 PyZelectrode-0.0.3/PyZelectrode/DataExplorer.py
--rw-r--r--   0 aguimera  (1000) aguimera  (1000)    10004 2023-01-09 17:21:37.000000 PyZelectrode-0.0.3/PyZelectrode/GuiDataExplorer_v2.ui
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)      473 2022-10-27 17:02:29.000000 PyZelectrode-0.0.3/PyZelectrode/Helper.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)      111 2022-10-27 15:52:34.000000 PyZelectrode-0.0.3/PyZelectrode/__init__.py
-drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-01-09 17:29:07.828147 PyZelectrode-0.0.3/PyZelectrode.egg-info/
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     1146 2023-01-09 17:29:07.000000 PyZelectrode-0.0.3/PyZelectrode.egg-info/PKG-INFO
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)      274 2023-01-09 17:29:07.000000 PyZelectrode-0.0.3/PyZelectrode.egg-info/SOURCES.txt
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)        1 2023-01-09 17:29:07.000000 PyZelectrode-0.0.3/PyZelectrode.egg-info/dependency_links.txt
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       13 2023-01-09 17:29:07.000000 PyZelectrode-0.0.3/PyZelectrode.egg-info/top_level.txt
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     6211 2022-10-27 15:44:25.000000 PyZelectrode-0.0.3/README.md
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       38 2023-01-09 17:29:07.828147 PyZelectrode-0.0.3/setup.cfg
--rwxrwxr-x   0 aguimera  (1000) aguimera  (1000)     2615 2023-01-09 17:25:18.000000 PyZelectrode-0.0.3/setup.py
+drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-04-18 22:29:37.604830 PyZelectrode-0.1.0/
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     1146 2023-04-18 22:29:37.604830 PyZelectrode-0.1.0/PKG-INFO
+drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-04-18 22:29:37.604830 PyZelectrode-0.1.0/PyZelectrode/
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    10216 2023-04-18 21:50:52.000000 PyZelectrode-0.1.0/PyZelectrode/DataExplorer.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    10004 2023-01-09 17:21:37.000000 PyZelectrode-0.1.0/PyZelectrode/GuiDataExplorer_v2.ui
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     4937 2023-04-18 18:44:22.000000 PyZelectrode-0.1.0/PyZelectrode/Helper.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     2613 2023-04-18 21:23:00.000000 PyZelectrode-0.1.0/PyZelectrode/IES_Fitting.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)      111 2022-10-27 15:52:34.000000 PyZelectrode-0.1.0/PyZelectrode/__init__.py
+drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-04-18 22:29:37.604830 PyZelectrode-0.1.0/PyZelectrode.egg-info/
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     1146 2023-04-18 22:29:37.000000 PyZelectrode-0.1.0/PyZelectrode.egg-info/PKG-INFO
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)      302 2023-04-18 22:29:37.000000 PyZelectrode-0.1.0/PyZelectrode.egg-info/SOURCES.txt
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)        1 2023-04-18 22:29:37.000000 PyZelectrode-0.1.0/PyZelectrode.egg-info/dependency_links.txt
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       13 2023-04-18 22:29:37.000000 PyZelectrode-0.1.0/PyZelectrode.egg-info/top_level.txt
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     6211 2022-10-27 15:44:25.000000 PyZelectrode-0.1.0/README.md
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       38 2023-04-18 22:29:37.604830 PyZelectrode-0.1.0/setup.cfg
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     2615 2023-04-18 22:24:13.000000 PyZelectrode-0.1.0/setup.py
```

### Comparing `PyZelectrode-0.0.3/PKG-INFO` & `PyZelectrode-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyZelectrode
-Version: 0.0.3
+Version: 0.1.0
 Summary: Z Analysis tools
 Home-page: https://git.csic.es/77114102R/pyzelectrode
 Download-URL: https://git.csic.es/77114102R/pyzelectrode
 Author: Anton Guimera-Brunet
 Author-email: anton.guimera@csic.es
 Maintainer: Anton Guimera-Brunet
 Maintainer-email: anton.guimera@csic.es
```

### Comparing `PyZelectrode-0.0.3/PyZelectrode/DataExplorer.py` & `PyZelectrode-0.1.0/PyZelectrode/DataExplorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,18 @@
                         continue
                     try:
                         if self.CheckLines.isChecked():
                             ax.plot(xVar, v.transpose(),
                                     color=Col,
                                     alpha=0.8,
                                     label=gn)
+                        if 'fit'+parn in row:
+                            ax.plot(xVar, row['fit'+parn].transpose(),
+                                    'k-.')
+
                         Vals = np.vstack((Vals, v)) if Vals.size else v
                     except:
                         pass
 
                 if Vals.size == 0:
                     continue
```

### Comparing `PyZelectrode-0.0.3/PyZelectrode/GuiDataExplorer_v2.ui` & `PyZelectrode-0.1.0/PyZelectrode/GuiDataExplorer_v2.ui`

 * *Files identical despite different names*

### Comparing `PyZelectrode-0.0.3/PyZelectrode.egg-info/PKG-INFO` & `PyZelectrode-0.1.0/PyZelectrode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyZelectrode
-Version: 0.0.3
+Version: 0.1.0
 Summary: Z Analysis tools
 Home-page: https://git.csic.es/77114102R/pyzelectrode
 Download-URL: https://git.csic.es/77114102R/pyzelectrode
 Author: Anton Guimera-Brunet
 Author-email: anton.guimera@csic.es
 Maintainer: Anton Guimera-Brunet
 Maintainer-email: anton.guimera@csic.es
```

### Comparing `PyZelectrode-0.0.3/README.md` & `PyZelectrode-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `PyZelectrode-0.0.3/setup.py` & `PyZelectrode-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with Foobar.  If not, see <http://www.gnu.org/licenses/>.
 
 
 from setuptools import setup, find_packages
 
-_version = '0.0.3'
+_version = '0.1.0'
 
 long_description = """
                       Library for electrode Impedance analysis
                    """
 
 install_requires = [ ]
```


# Comparing `tmp/study_id_generator-0.0.3.tar.gz` & `tmp/study_id_generator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "study_id_generator-0.0.3.tar", last modified: Fri Apr 14 12:29:04 2023, max compression
+gzip compressed data, was "study_id_generator-0.0.4.tar", last modified: Wed Apr 19 12:49:40 2023, max compression
```

## Comparing `study_id_generator-0.0.3.tar` & `study_id_generator-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 12:29:04.983619 study_id_generator-0.0.3/
--rw-rw-rw-   0        0        0     1380 2023-04-14 12:29:04.982890 study_id_generator-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      798 2023-04-14 01:28:57.000000 study_id_generator-0.0.3/README.md
--rw-rw-rw-   0        0        0      873 2023-04-14 12:26:47.000000 study_id_generator-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 12:29:04.984269 study_id_generator-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 12:29:04.966441 study_id_generator-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 12:29:04.972479 study_id_generator-0.0.3/src/study_id_generator/
--rw-rw-rw-   0        0        0        0 2023-04-13 18:17:34.000000 study_id_generator-0.0.3/src/study_id_generator/__init__.py
--rw-rw-rw-   0        0        0     5742 2023-04-14 12:11:38.000000 study_id_generator-0.0.3/src/study_id_generator/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:29:04.981229 study_id_generator-0.0.3/src/study_id_generator.egg-info/
--rw-rw-rw-   0        0        0     1380 2023-04-14 12:29:04.000000 study_id_generator-0.0.3/src/study_id_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-04-14 12:29:04.000000 study_id_generator-0.0.3/src/study_id_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 12:29:04.000000 study_id_generator-0.0.3/src/study_id_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-04-14 12:29:04.000000 study_id_generator-0.0.3/src/study_id_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-14 12:29:04.000000 study_id_generator-0.0.3/src/study_id_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 12:49:40.330704 study_id_generator-0.0.4/
+-rw-rw-rw-   0        0        0     1380 2023-04-19 12:49:40.329706 study_id_generator-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2023-04-14 01:28:57.000000 study_id_generator-0.0.4/README.md
+-rw-rw-rw-   0        0        0      873 2023-04-19 12:07:41.000000 study_id_generator-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 12:49:40.330704 study_id_generator-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 12:49:40.311765 study_id_generator-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 12:49:40.318742 study_id_generator-0.0.4/src/study_id_generator/
+-rw-rw-rw-   0        0        0        0 2023-04-13 18:17:34.000000 study_id_generator-0.0.4/src/study_id_generator/__init__.py
+-rw-rw-rw-   0        0        0     6117 2023-04-19 12:44:02.000000 study_id_generator-0.0.4/src/study_id_generator/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 12:49:40.327713 study_id_generator-0.0.4/src/study_id_generator.egg-info/
+-rw-rw-rw-   0        0        0     1380 2023-04-19 12:49:40.000000 study_id_generator-0.0.4/src/study_id_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-04-19 12:49:40.000000 study_id_generator-0.0.4/src/study_id_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 12:49:40.000000 study_id_generator-0.0.4/src/study_id_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-04-19 12:49:40.000000 study_id_generator-0.0.4/src/study_id_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-19 12:49:40.000000 study_id_generator-0.0.4/src/study_id_generator.egg-info/top_level.txt
```

### Comparing `study_id_generator-0.0.3/PKG-INFO` & `study_id_generator-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: study_id_generator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Study ID Generator.
 Author-email: Sushant Obeja <sobeja@umich.edu>, Adam Patterson <adpatter@umich.edu>
 Project-URL: Homepage, https://git.umms.med.umich.edu/feldman-lab/study_id_generator
 Project-URL: Bug Tracker, https://git.umms.med.umich.edu/feldman-lab/study_id_generator/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `study_id_generator-0.0.3/README.md` & `study_id_generator-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `study_id_generator-0.0.3/pyproject.toml` & `study_id_generator-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "study_id_generator"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Sushant Obeja", email="sobeja@umich.edu" },
     { name="Adam Patterson", email="adpatter@umich.edu" },
 ]
 description = "Study ID Generator."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `study_id_generator-0.0.3/src/study_id_generator/__main__.py` & `study_id_generator-0.0.4/src/study_id_generator/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,57 +6,68 @@
 import configparser
 import requests
 import pandas as pd
 import numpy as np
 from sklearn.metrics.pairwise import paired_distances
 import wx
 
-CONFIG_PATH = pathlib.Path.home().joinpath(".config/study_id_generator/config.ini")
+CONFIG_PATH = pathlib.Path.home().joinpath(
+    ".config/study_id_generator/config.ini")
 
-class MainFrame(wx.Frame):    
-    def __init__(self):
-        super().__init__(parent=None, title='Study ID Generator', size=(400,300))
 
-        self.panel = wx.Panel(self)        
-        vbox = wx.BoxSizer(wx.VERTICAL)  
-        hbox = wx.BoxSizer(wx.HORIZONTAL)  
+class MainFrame(wx.Frame):
+    def __init__(self):
+        super().__init__(parent=None, title='Study ID Generator', size=(400, 300))
 
-        l1 = wx.StaticText(self.panel, 1, "Study ID") 
-        self.study_id_window = wx.TextCtrl(self.panel, style=wx.TE_READONLY | wx.TE_RICH)
+        self.panel = wx.Panel(self)
+        vbox = wx.BoxSizer(wx.VERTICAL)
+        hbox = wx.BoxSizer(wx.HORIZONTAL)
+
+        l1 = wx.StaticText(self.panel, 1, "Study ID")
+        self.study_id_window = wx.TextCtrl(
+            self.panel, style=wx.TE_READONLY | wx.TE_RICH)
         self.study_id_window.SetDefaultStyle(wx.TextAttr(wx.RED))
 
-        hbox.Add(l1, proportion=0, flag=wx.ALIGN_LEFT | wx.ALL, border=5) 
-        hbox.Add(self.study_id_window, proportion=0, flag= wx.ALIGN_LEFT | wx.ALL, border=0) 
+        hbox.Add(l1, proportion=0, flag=wx.ALIGN_LEFT | wx.ALL, border=5)
+        hbox.Add(self.study_id_window, proportion=0,
+                 flag=wx.ALIGN_LEFT | wx.ALL, border=0)
 
         button = wx.Button(self.panel, label='Generate Study ID')
         button.Bind(wx.EVT_BUTTON, self.on_press, id=wx.ID_ANY)
-      
-        self.log_window = wx.TextCtrl(self.panel, style=wx.TE_MULTILINE | wx.TE_READONLY | wx.HSCROLL)
+
+        self.log_window = wx.TextCtrl(
+            self.panel, style=wx.TE_MULTILINE | wx.TE_READONLY | wx.HSCROLL)
 
         vbox.Add(hbox, flag=wx.ALL, border=5)
-        vbox.Add(self.log_window, proportion=1, flag=wx.EXPAND)     
-        vbox.Add(button, proportion=0, flag=wx.ALL | wx.ALIGN_RIGHT, border=5)        
+        vbox.Add(self.log_window, proportion=1, flag=wx.EXPAND)
+        vbox.Add(button, proportion=0, flag=wx.ALL | wx.ALIGN_RIGHT, border=5)
 
         self.panel.SetSizerAndFit(vbox)
 
         self.Show()
 
-        self.log_window.AppendText(f"Loading configuration at {CONFIG_PATH}.\n")
+        self.log_window.AppendText(
+            f"Loading configuration at {CONFIG_PATH}.\n")
 
-        config_path = pathlib.Path(CONFIG_PATH)
-        config = configparser.ConfigParser()
-        config.read(config_path)
-
-        self._MIN_ID = int(config['DEFAULT']['MIN_ID'])
-        self._MAX_ID = int(config['DEFAULT']['MAX_ID'])
-        self._ID_WIDTH = int(config['DEFAULT']['ID_WIDTH'])
-        self._ID_FILLCHAR = config['DEFAULT']['ID_FILLCHAR']
-        self._SAMPLE_FRAC = float(config['DEFAULT']['SAMPLE_FRAC'])
-
-        self._section = {section:config[section] for section in config.sections()}
+        try:
+            config_path = pathlib.Path(CONFIG_PATH)
+            config = configparser.ConfigParser()
+            config.read(config_path)
+
+            self._MIN_ID = int(config['DEFAULT']['MIN_ID'])
+            self._MAX_ID = int(config['DEFAULT']['MAX_ID'])
+            self._ID_WIDTH = int(config['DEFAULT']['ID_WIDTH'])
+            self._ID_FILLCHAR = config['DEFAULT']['ID_FILLCHAR']
+            self._SAMPLE_FRAC = float(config['DEFAULT']['SAMPLE_FRAC'])
+
+            self._section = {section: config[section] for section in config.sections()}
+
+            self.log_window.AppendText(f"Configuration loaded.\n")
+        except:
+            self.log_window.AppendText(f"Configuration failed.\n")
 
     def on_press(self, event):
 
         try:
             self.panel.SetCursor(wx.Cursor(wx.CURSOR_ARROWWAIT))
 
             self.study_id_window.Clear()
@@ -69,31 +80,34 @@
                     'token': section['API_KEY'],
                     'content': 'record',
                     'format': 'json',
                     'type': 'flat',
                     'fields[0]': section['FIELD_NAME']
                 }
 
-                self.log_window.AppendText(f"Requesting identifiers from {section_name}.\n")
+                self.log_window.AppendText(
+                    f"Requesting identifiers from {section_name}.\n")
 
                 with requests.post(section['URL'], data=data, verify=section['CERT_PATH'], timeout=60) as res:
                     if not res.ok:
                         raise Exception(f"""Status Code: {res.status_code}  Content: {res.content}""")
 
                 df = pd.DataFrame(res.json())
 
+                df[section['FIELD_NAME']] = df[section['FIELD_NAME']].str.replace(r'[^\d]', '', regex=True)
+
                 df = df.loc[df[section['FIELD_NAME']].str.contains(section['ID_REGEX']) == True]
 
                 ids.append(df[section['FIELD_NAME']])
 
             ds = pd.concat(ids)
-                        
+
             ds = ds.drop_duplicates()
 
-            df = ds.to_frame(name='id') # type: ignore
+            df = ds.to_frame(name='id')  # type: ignore
 
             df['id'] = df['id'].astype(str).str.pad(self._ID_WIDTH, side='left', fillchar=self._ID_FILLCHAR)
 
             id_variants = pd.Series(range(self._MIN_ID, self._MAX_ID))
 
             id_variants = id_variants.astype(str).str.pad(self._ID_WIDTH, side='left', fillchar=self._ID_FILLCHAR)
 
@@ -106,21 +120,24 @@
             df = df.explode('id_variant')
 
             self.log_window.AppendText(f"Calculating pairwise distance between {df.shape[0]} pairs of identifiers...\n")
 
             df['id_vector'] = df['id'].apply(lambda x: [int(i) for i in list(x)])
 
             df['id_variant_vector'] = df['id_variant'].apply(lambda x: [int(i) for i in list(x)])
-            
-            df['dist'] = paired_distances(np.array(df['id_vector'].tolist()), np.array(df['id_variant_vector'].tolist()))
+
+            df['dist'] = paired_distances(
+                np.array(df['id_vector'].tolist()),
+                np.array(df['id_variant_vector'].tolist())
+            )
 
             df = df.groupby(['id_variant'])['dist'].agg(['mean'])
 
             df = df.loc[df['mean'] == df['mean'].max()]
-            
+
             df = df.sample(n=1)
 
             study_id = df.index[0]
 
             self.study_id_window.AppendText(study_id)
 
             self.panel.SetCursor(wx.Cursor(wx.CURSOR_ARROW))
@@ -128,37 +145,37 @@
         except Exception as e:
             logger.error(f'{traceback.format_exc()}')
 
         finally:
             pass
 
 
-
 if __name__ == '__main__':
 
     try:
         signal.signal(signal.SIGTERM, lambda signalnum, frame: sys.exit(0))
         signal.signal(signal.SIGINT, lambda signalnum, frame: sys.exit(0))
 
         logger = logging.getLogger()
-        formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+        formatter = logging.Formatter(
+            '%(asctime)s - %(name)s - %(levelname)s - %(message)s')
         ch = logging.StreamHandler(stream=sys.stdout)
         ch.setLevel(logging.INFO)
         ch.setFormatter(formatter)
         for handler in logger.handlers.copy():
             logger.removeHandler(handler)
             logger.addHandler(ch)
 
         app = wx.App()
         frame = MainFrame()
         app.MainLoop()
 
     except Exception as e:
         raise e
-    
+
     except BaseException as e:
         logger.warning('Exiting.')
         logger.error(f'{traceback.format_exc()}')
         raise e
-    
+
     finally:
         pass
```

### Comparing `study_id_generator-0.0.3/src/study_id_generator.egg-info/PKG-INFO` & `study_id_generator-0.0.4/src/study_id_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: study-id-generator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Study ID Generator.
 Author-email: Sushant Obeja <sobeja@umich.edu>, Adam Patterson <adpatter@umich.edu>
 Project-URL: Homepage, https://git.umms.med.umich.edu/feldman-lab/study_id_generator
 Project-URL: Bug Tracker, https://git.umms.med.umich.edu/feldman-lab/study_id_generator/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/pycup-0.1.6.tar.gz` & `tmp/pycup-0.1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pycup-0.1.6.tar", last modified: Sun Apr 16 14:48:12 2023, max compression
+gzip compressed data, was "dist\pycup-0.1.6.1.tar", last modified: Wed Apr 19 17:33:58 2023, max compression
```

## Comparing `pycup-0.1.6.tar` & `pycup-0.1.6.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 14:48:12.380022 pycup-0.1.6/
--rw-rw-rw-   0        0        0     6321 2023-04-16 14:48:12.379105 pycup-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     5075 2023-04-16 08:17:22.000000 pycup-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 14:48:12.364019 pycup-0.1.6/pycup/
--rw-rw-rw-   0        0        0    17161 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/GLUE.py
--rw-rw-rw-   0        0        0    38271 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/GWO.py
--rw-rw-rw-   0        0        0    33260 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/MFO.py
--rw-rw-rw-   0        0        0    14600 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/MODE.py
--rw-rw-rw-   0        0        0    24212 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/MOPSO.py
--rw-rw-rw-   0        0        0    14937 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/NSGA2.py
--rw-rw-rw-   0        0        0    19098 2023-04-16 07:43:22.000000 pycup-0.1.6/pycup/PESTclasses.py
--rw-rw-rw-   0        0        0    35498 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/PSO.py
--rw-rw-rw-   0        0        0    15659 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/Reslib.py
--rw-rw-rw-   0        0        0    30073 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/SCA.py
--rw-rw-rw-   0        0        0    32941 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/SOA.py
--rw-rw-rw-   0        0        0    32160 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/SSA.py
--rw-rw-rw-   0        0        0     5757 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/TOPSIS.py
--rw-rw-rw-   0        0        0    33343 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/TSA.py
--rw-rw-rw-   0        0        0    32912 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/WOA.py
--rw-rw-rw-   0        0        0      946 2023-04-16 14:04:48.000000 pycup-0.1.6/pycup/__init__.py
--rw-rw-rw-   0        0        0    10042 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/calc_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:48:12.376021 pycup-0.1.6/pycup/document/
--rw-rw-rw-   0        0        0   826264 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/document/Documentation.pdf
--rw-rw-rw-   0        0        0     4027 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/evaluation_metrics.py
--rw-rw-rw-   0        0        0    53479 2023-04-16 14:25:15.000000 pycup-0.1.6/pycup/integrate.py
--rw-rw-rw-   0        0        0     7263 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/multi_jobs.py
--rw-rw-rw-   0        0        0   125408 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/plot.py
--rw-rw-rw-   0        0        0      460 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/progress_bar.py
--rw-rw-rw-   0        0        0    10352 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/sampling.py
--rw-rw-rw-   0        0        0    18935 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/save.py
--rw-rw-rw-   0        0        0     2068 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/template.py
--rw-rw-rw-   0        0        0        0 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/test.py
--rw-rw-rw-   0        0        0     6055 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/test_functions.py
--rw-rw-rw-   0        0        0    69170 2023-04-16 07:43:22.000000 pycup-0.1.6/pycup/uncertainty_analysis_fun.py
--rw-rw-rw-   0        0        0    17048 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/utilize.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:48:12.373020 pycup-0.1.6/pycup.egg-info/
--rw-rw-rw-   0        0        0     6321 2023-04-16 14:48:12.000000 pycup-0.1.6/pycup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-16 14:48:12.000000 pycup-0.1.6/pycup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 14:48:12.000000 pycup-0.1.6/pycup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-16 14:48:12.000000 pycup-0.1.6/pycup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-16 14:48:12.000000 pycup-0.1.6/pycup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 14:48:12.380022 pycup-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      953 2023-04-16 08:01:45.000000 pycup-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:33:58.471872 pycup-0.1.6.1/
+-rw-rw-rw-   0        0        0     6333 2023-04-19 17:33:58.470872 pycup-0.1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5077 2023-04-19 15:26:08.000000 pycup-0.1.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 17:33:58.454869 pycup-0.1.6.1/pycup/
+-rw-rw-rw-   0        0        0    17161 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/GLUE.py
+-rw-rw-rw-   0        0        0    38271 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/GWO.py
+-rw-rw-rw-   0        0        0    33260 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/MFO.py
+-rw-rw-rw-   0        0        0    14600 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/MODE.py
+-rw-rw-rw-   0        0        0    24212 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/MOPSO.py
+-rw-rw-rw-   0        0        0    14937 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/NSGA2.py
+-rw-rw-rw-   0        0        0    19287 2023-04-19 17:27:49.000000 pycup-0.1.6.1/pycup/PESTclasses.py
+-rw-rw-rw-   0        0        0    35498 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/PSO.py
+-rw-rw-rw-   0        0        0    15659 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/Reslib.py
+-rw-rw-rw-   0        0        0    30073 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/SCA.py
+-rw-rw-rw-   0        0        0    32941 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/SOA.py
+-rw-rw-rw-   0        0        0    32160 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/SSA.py
+-rw-rw-rw-   0        0        0     5757 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/TOPSIS.py
+-rw-rw-rw-   0        0        0    33343 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/TSA.py
+-rw-rw-rw-   0        0        0    32912 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/WOA.py
+-rw-rw-rw-   0        0        0      946 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/__init__.py
+-rw-rw-rw-   0        0        0    10042 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/calc_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:33:58.467872 pycup-0.1.6.1/pycup/document/
+-rw-rw-rw-   0        0        0   826264 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/document/Documentation.pdf
+-rw-rw-rw-   0        0        0     4027 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/evaluation_metrics.py
+-rw-rw-rw-   0        0        0    53886 2023-04-19 17:14:13.000000 pycup-0.1.6.1/pycup/integrate.py
+-rw-rw-rw-   0        0        0     7263 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/multi_jobs.py
+-rw-rw-rw-   0        0        0   125408 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/plot.py
+-rw-rw-rw-   0        0        0      460 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/progress_bar.py
+-rw-rw-rw-   0        0        0    10352 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/sampling.py
+-rw-rw-rw-   0        0        0    18935 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/save.py
+-rw-rw-rw-   0        0        0     2068 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/template.py
+-rw-rw-rw-   0        0        0        0 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/test.py
+-rw-rw-rw-   0        0        0     6055 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/test_functions.py
+-rw-rw-rw-   0        0        0    69170 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/uncertainty_analysis_fun.py
+-rw-rw-rw-   0        0        0    17048 2023-04-19 15:26:08.000000 pycup-0.1.6.1/pycup/utilize.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:33:58.464925 pycup-0.1.6.1/pycup.egg-info/
+-rw-rw-rw-   0        0        0     6333 2023-04-19 17:33:58.000000 pycup-0.1.6.1/pycup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-19 17:33:58.000000 pycup-0.1.6.1/pycup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 17:33:58.000000 pycup-0.1.6.1/pycup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-19 17:33:58.000000 pycup-0.1.6.1/pycup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 17:33:58.000000 pycup-0.1.6.1/pycup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 17:33:58.471872 pycup-0.1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      955 2023-04-19 17:32:30.000000 pycup-0.1.6.1/setup.py
```

### Comparing `pycup-0.1.6/PKG-INFO` & `pycup-0.1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycup
-Version: 0.1.6
+Version: 0.1.6.1
 Summary: An auto-calibration tool for environmental models based on heuristic algorithms and uncertainty estimation theory.
 Home-page: https://github.com/QianyangWang/PyCUP
 Author: Qianyang Wang
 Author-email: wqy07010944@hotmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/QianyangWang/PyCUP/DOCUMENT
 Project-URL: Source, https://github.com/QianyangWang/PyCUP/pycup
@@ -85,14 +85,15 @@
         3. The example in folder 'Example03-multiobjective' contains an SWMM multi-objective calibration project using EOMOPSO. 
         4. The example in folder 'Example04-validation&prediction' shows how to use our (Ensemble)Validator/(Ensemble)Predictor objects for the validation and prediction of the model using the calibrated parameter (set).
         5. The example in folder 'Example05-multi-station&event' shows how to use the pycup.Reslib.SimulationResult object for the storage of multi-station & multi-event simulation results, as well as the further analysis using them.
         
         <div align=center>
         <img src="https://user-images.githubusercontent.com/116932670/209893309-e67c425f-0eff-47b4-a552-b30d717a138b.png">
         </div>
+        
         ## Example PEST++ conversion project (with a Xinanjiang hydrologic model)
         
         1. The example in folder 'Example06-PESTintegration' contains a PEST++ Xinanjiang model calibration project and the python script to run a PyCUP calibration based on it.
         
 Keywords: optimization
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `pycup-0.1.6/README.md` & `pycup-0.1.6.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -75,10 +75,11 @@
 3. The example in folder 'Example03-multiobjective' contains an SWMM multi-objective calibration project using EOMOPSO. 
 4. The example in folder 'Example04-validation&prediction' shows how to use our (Ensemble)Validator/(Ensemble)Predictor objects for the validation and prediction of the model using the calibrated parameter (set).
 5. The example in folder 'Example05-multi-station&event' shows how to use the pycup.Reslib.SimulationResult object for the storage of multi-station & multi-event simulation results, as well as the further analysis using them.
 
 <div align=center>
 <img src="https://user-images.githubusercontent.com/116932670/209893309-e67c425f-0eff-47b4-a552-b30d717a138b.png">
 </div>
+
 ## Example PEST++ conversion project (with a Xinanjiang hydrologic model)
 
 1. The example in folder 'Example06-PESTintegration' contains a PEST++ Xinanjiang model calibration project and the python script to run a PyCUP calibration based on it.
```

### Comparing `pycup-0.1.6/pycup/GLUE.py` & `pycup-0.1.6.1/pycup/GLUE.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/GWO.py` & `pycup-0.1.6.1/pycup/GWO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/MFO.py` & `pycup-0.1.6.1/pycup/MFO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/MODE.py` & `pycup-0.1.6.1/pycup/MODE.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/MOPSO.py` & `pycup-0.1.6.1/pycup/MOPSO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/NSGA2.py` & `pycup-0.1.6.1/pycup/NSGA2.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/PESTclasses.py` & `pycup-0.1.6.1/pycup/PESTclasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,15 +415,15 @@
                     v += i
         self.commands.extend(verbs)
 
     def to_cmd_obj(self,verb):
         if re.match("l[0-9]+",verb):
             return PESTLineAdvance(verb)
         elif re.match("{}.*?{}".format(self.dlmt,self.dlmt),verb):
-            return PESTDelimiter(verb)
+            return PESTDelimiter(verb,self.dlmt)
         elif verb == "w":
             return PESTwhitespace(verb)
         elif re.match("!.*?!",verb):
             return PESTNoneFixedData(verb)
         elif re.match("\[.*?][0-9]+:[0-9]+",verb):
             return PESTFixedData(verb)
         elif re.match("\(.*?\)[0-9]+:[0-9]+",verb):
@@ -528,17 +528,17 @@
         rowcursor, linecursor = kwargs["rowcursor"], kwargs["linecursor"]
         linecursor = self.end
         return rowcursor,linecursor
 
 
 class PESTDelimiter(PESTinscmd):
 
-    def __init__(self,verb):
+    def __init__(self,verb,dlmt):
         super().__init__(verb)
-        self.keyword = re.findall("~(.*?)~",verb)
+        self.keyword = re.findall("{}(.*?){}".format(dlmt,dlmt),verb)
 
     def update_cursor(self,**kwargs):
         rowcursor, linecursor,contents = kwargs["rowcursor"], kwargs["linecursor"],kwargs["contents"]
         rowcursor, linecursor = self.skip_to(rowcursor,linecursor,contents)
         return rowcursor,linecursor
 
     def skip_to(self,rowcursor, linecursor,contents):
@@ -612,11 +612,13 @@
                     self.data.append(data)
                     self.data_name.append(name)
 
 
 
 
 
-
+if __name__ == "__main__":
+    ins = PESTinsReader(r"D:\PESTEXAMPLES\pestpp_v5_data_release_barf\mf6_freyberg\freyberg6.lst.ins")
+    print(ins.cmd_obj)
```

### Comparing `pycup-0.1.6/pycup/PSO.py` & `pycup-0.1.6.1/pycup/PSO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/Reslib.py` & `pycup-0.1.6.1/pycup/Reslib.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/SCA.py` & `pycup-0.1.6.1/pycup/SCA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/SOA.py` & `pycup-0.1.6.1/pycup/SOA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/SSA.py` & `pycup-0.1.6.1/pycup/SSA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/TOPSIS.py` & `pycup-0.1.6.1/pycup/TOPSIS.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/TSA.py` & `pycup-0.1.6.1/pycup/TSA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/WOA.py` & `pycup-0.1.6.1/pycup/WOA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/__init__.py` & `pycup-0.1.6.1/pycup/__init__.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/calc_utils.py` & `pycup-0.1.6.1/pycup/calc_utils.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/document/Documentation.pdf` & `pycup-0.1.6.1/pycup/document/Documentation.pdf`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/evaluation_metrics.py` & `pycup-0.1.6.1/pycup/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/integrate.py` & `pycup-0.1.6.1/pycup/integrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -571,17 +571,21 @@
 
     def _call_simMP(self,X):
         pid = os.getpid()
         dirs = os.listdir(self.workspace)
         dst_folder = self.workspace+"\\pycup_process{}".format(pid)
         os.mkdir(dst_folder)
         for f in dirs:
-            if os.path.basename(f) != "pestpp.exe"  and os.path.basename(f) != "tsproc.exe" and "pycup_process" not in f:
-                shutil.copy(self.workspace +"\\"+ f,dst_folder+"\\"+os.path.basename(f))
-
+            if "pycup_process" not in f:
+                abs_path = self.workspace +"\\"+ f
+                if os.path.isfile(abs_path):
+                    if os.path.basename(f) != "pestpp.exe"  and os.path.basename(f) != "tsproc.exe":
+                        shutil.copy(abs_path,dst_folder+"\\"+os.path.basename(f))
+                else:
+                    shutil.copytree(abs_path,dst_folder+"\\"+ f)
         os.chdir(dst_folder)
         self.UpdateParam(X,subfolder="pycup_process{}".format(pid))
         self.CallExe(subfolder="pycup_process{}".format(pid))
         # a list of observation group results
         lgpres = self.ReadResult(subfolder="pycup_process{}".format(pid))
         return pid,lgpres
 
@@ -590,36 +594,42 @@
         pid = mp.current_process().name.split("-")[-1]
         dirs = os.listdir(self.workspace)
         pid = int(pid) % n_jobs + 1
         dst_folder = self.workspace+"\\pycup_process{}".format(pid)
         if not os.path.exists(dst_folder):
             os.mkdir(dst_folder)
             for f in dirs:
-                if os.path.basename(f) != "pestpp.exe"  and os.path.basename(f) != "tsproc.exe" and "pycup_process" not in f:
-                    shutil.copy(self.workspace +"\\"+ f,dst_folder+"\\"+os.path.basename(f))
+                if "pycup_process" not in f:
+                    abs_path = self.workspace + "\\" + f
+                    if os.path.isfile(abs_path):
+                        if os.path.basename(f) != "pestpp.exe" and os.path.basename(f) != "tsproc.exe":
+                            shutil.copy(abs_path, dst_folder + "\\" + os.path.basename(f))
+                    else:
+                        shutil.copytree(abs_path, dst_folder + "\\" + f)
         os.chdir(dst_folder)
         self.UpdateParam(X,subfolder="pycup_process{}".format(pid))
         self.CallExe(subfolder="pycup_process{}".format(pid))
         # a list of observation group results
         lgpres = self.ReadResult(subfolder="pycup_process{}".format(pid))
         #print(len(lgpres[0].idx),len(lgpres[0].res),len(self.obs["i_mod_est"].index))
         return pid,lgpres
 
 
     def _rm_dirMP(self,pid):
         os.chdir(self.workspace)
+        abs_path = self.workspace + "\\" + "pycup_process{}".format(pid)
         try:
             # remove the folder.
-            shutil.rmtree(self.workspace + "\\" + "pycup_process{}".format(pid))
+            shutil.rmtree(abs_path)
         except:
             # sometimes the exe program has not been finished completely, close the exe and then remove the folder.
-            files = glob.glob(self.workspace + "\\" + "pycup_process{}\\*.exe".format(pid))
+            files = glob.glob(abs_path+"\\**\\*.exe",recursive=True)
             for f in files:
                 p = subprocess.call(["taskkill","/F","/IM",f],stdout=subprocess.PIPE,stderr=subprocess.PIPE)
-            shutil.rmtree(self.workspace + "\\" + "pycup_process{}".format(pid))
+            os.system("rd/s/q {}".format(abs_path))
 
     def _closeExeMPF(self,pid):
         files = glob.glob(self.workspace + "\\" + "pycup_process{}\\*.exe".format(pid))
         for f in files:
             p = subprocess.call(["taskkill", "/F", "/IM", f], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
```

### Comparing `pycup-0.1.6/pycup/multi_jobs.py` & `pycup-0.1.6.1/pycup/multi_jobs.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/plot.py` & `pycup-0.1.6.1/pycup/plot.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/sampling.py` & `pycup-0.1.6.1/pycup/sampling.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/save.py` & `pycup-0.1.6.1/pycup/save.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/template.py` & `pycup-0.1.6.1/pycup/template.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/test_functions.py` & `pycup-0.1.6.1/pycup/test_functions.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/uncertainty_analysis_fun.py` & `pycup-0.1.6.1/pycup/uncertainty_analysis_fun.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup/utilize.py` & `pycup-0.1.6.1/pycup/utilize.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/pycup.egg-info/PKG-INFO` & `pycup-0.1.6.1/pycup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycup
-Version: 0.1.6
+Version: 0.1.6.1
 Summary: An auto-calibration tool for environmental models based on heuristic algorithms and uncertainty estimation theory.
 Home-page: https://github.com/QianyangWang/PyCUP
 Author: Qianyang Wang
 Author-email: wqy07010944@hotmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/QianyangWang/PyCUP/DOCUMENT
 Project-URL: Source, https://github.com/QianyangWang/PyCUP/pycup
@@ -85,14 +85,15 @@
         3. The example in folder 'Example03-multiobjective' contains an SWMM multi-objective calibration project using EOMOPSO. 
         4. The example in folder 'Example04-validation&prediction' shows how to use our (Ensemble)Validator/(Ensemble)Predictor objects for the validation and prediction of the model using the calibrated parameter (set).
         5. The example in folder 'Example05-multi-station&event' shows how to use the pycup.Reslib.SimulationResult object for the storage of multi-station & multi-event simulation results, as well as the further analysis using them.
         
         <div align=center>
         <img src="https://user-images.githubusercontent.com/116932670/209893309-e67c425f-0eff-47b4-a552-b30d717a138b.png">
         </div>
+        
         ## Example PEST++ conversion project (with a Xinanjiang hydrologic model)
         
         1. The example in folder 'Example06-PESTintegration' contains a PEST++ Xinanjiang model calibration project and the python script to run a PyCUP calibration based on it.
         
 Keywords: optimization
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `pycup-0.1.6/pycup.egg-info/SOURCES.txt` & `pycup-0.1.6.1/pycup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycup-0.1.6/setup.py` & `pycup-0.1.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open(r"README.md",encoding="utf-8") as f:
   long_description = f.read()
 
 
 setup(
     name='pycup',
-  version='0.1.6',
+  version='0.1.6.1',
   description='An auto-calibration tool for environmental models based on heuristic algorithms and uncertainty estimation theory.',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author='Qianyang Wang',
   author_email='wqy07010944@hotmail.com',
   url='https://github.com/QianyangWang/PyCUP',
   license='MIT License',
```


# Comparing `tmp/Hefesto-0.3.8.tar.gz` & `tmp/Hefesto-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hefesto-0.3.8.tar", last modified: Mon Mar 13 23:08:57 2023, max compression
+gzip compressed data, was "Hefesto-0.3.9.tar", last modified: Wed Apr 19 08:27:39 2023, max compression
```

## Comparing `Hefesto-0.3.8.tar` & `Hefesto-0.3.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-03-13 23:08:57.647997 Hefesto-0.3.8/
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-03-13 23:08:57.647997 Hefesto-0.3.8/Hefesto/
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-11-01 09:45:17.000000 Hefesto-0.3.8/Hefesto/__init__.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    10295 2023-03-13 23:06:32.000000 Hefesto-0.3.8/Hefesto/main.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     8249 2023-03-09 13:00:45.000000 Hefesto-0.3.8/Hefesto/template.py
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-03-13 23:08:57.647997 Hefesto-0.3.8/Hefesto.egg-info/
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-03-13 23:08:57.000000 Hefesto-0.3.8/Hefesto.egg-info/PKG-INFO
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-03-13 23:08:57.000000 Hefesto-0.3.8/Hefesto.egg-info/SOURCES.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-03-13 23:08:57.000000 Hefesto-0.3.8/Hefesto.egg-info/dependency_links.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-03-13 23:08:57.000000 Hefesto-0.3.8/Hefesto.egg-info/top_level.txt
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-11-01 09:45:17.000000 Hefesto-0.3.8/MANIFEST.in
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-03-13 23:08:57.647997 Hefesto-0.3.8/PKG-INFO
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      719 2023-03-09 11:26:42.000000 Hefesto-0.3.8/README.md
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       31 2023-03-09 11:26:42.000000 Hefesto-0.3.8/requirements.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-03-13 23:08:57.647997 Hefesto-0.3.8/setup.cfg
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-03-13 23:08:26.000000 Hefesto-0.3.8/setup.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-04-19 08:27:39.389428 Hefesto-0.3.9/
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-04-19 08:27:39.389428 Hefesto-0.3.9/Hefesto/
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.3.9/Hefesto/__init__.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    12019 2023-04-19 08:22:40.000000 Hefesto-0.3.9/Hefesto/main.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     8595 2023-04-19 07:55:36.000000 Hefesto-0.3.9/Hefesto/template.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-04-19 08:27:39.389428 Hefesto-0.3.9/Hefesto.egg-info/
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-04-19 08:27:39.000000 Hefesto-0.3.9/Hefesto.egg-info/PKG-INFO
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-04-19 08:27:39.000000 Hefesto-0.3.9/Hefesto.egg-info/SOURCES.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-04-19 08:27:39.000000 Hefesto-0.3.9/Hefesto.egg-info/dependency_links.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-04-19 08:27:39.000000 Hefesto-0.3.9/Hefesto.egg-info/top_level.txt
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.3.9/MANIFEST.in
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-04-19 08:27:39.389428 Hefesto-0.3.9/PKG-INFO
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      719 2023-02-08 11:49:59.000000 Hefesto-0.3.9/README.md
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       31 2023-02-10 09:50:43.000000 Hefesto-0.3.9/requirements.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-04-19 08:27:39.389428 Hefesto-0.3.9/setup.cfg
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-04-19 08:27:35.000000 Hefesto-0.3.9/setup.py
```

### Comparing `Hefesto-0.3.8/Hefesto/main.py` & `Hefesto-0.3.9/Hefesto/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from perseo.main import milisec
 # from template import Template
 from Hefesto.template import Template
 import sys
 import yaml
 import math
 import requests
-import numpy as np
 
 class Hefesto():
 
     def __init__(self, datainput, reset = False):
         # Create an object as dictonary to reduce duplicate calls:
         self.reg = dict()
 
@@ -77,25 +76,24 @@
         for index, row in resulting_df.iterrows():
             for k,v in datatype_relationship.items():
 
                 # value ---> value_DATATYPE:
                 if row["value_datatype"] == k:
                     resulting_df.at[index, v] = resulting_df["value"][index]
 
-        del resulting_df["value"]
-
-        resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
-
-        for index, row in resulting_df.iterrows():
-            for k,v in datatype_relationship.items():
+                # # valueIRI ---> process_type for Disability
+                # if row["model"] == "Disability" and row["valueIRI"] != None:
+                #     resulting_df.at[index, "process_type"] = resulting_df["valueIRI"][index]
+                #     resulting_df["valueIRI"][index] = None
 
                 # enddate correction:
-                if np.isnan(row["enddate"]) or row["enddate"] == None:
+                if row["startdate"] != None and row["enddate"] == None:
                     resulting_df["enddate"][index] = resulting_df["startdate"][index]
 
+        del resulting_df["value"]
 
 
         # # valueIRI ---> valueAttributeIRI:
         # del resulting_df["valueAttributeIRI"]
         # resulting_df.rename(columns={'valueIRI':'valueAttributeIRI'}, inplace=True)
 
         # uniqid generation:
@@ -143,42 +141,85 @@
                             dict_element = {element[0]:row[1][r]}
                             row_df[milisec_point].update(dict_element)
 
                 # Store formed element into the final table:
                 final_row_df = pd.DataFrame(row_df[milisec_point], index=[1])
                 resulting_df = pd.concat([resulting_df, final_row_df])
 
-        # Reset Dataframe index
+        # Reset Index:    
         resulting_df = resulting_df.reset_index(drop=True)
+        # Turn any nan to None:
+        resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
 
-        if clean_blanks:
-            # Replace all nan to None to easier removal
-            resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
-
-            # Empty value row removal
-            for row_final in resulting_df.iterrows():
-                if row_final[1]["valueOutput_date"] == None and row_final[1]["valueOutput_string"] == None and row_final[1]["valueOutput_float"] == None:
-                    resulting_df = resulting_df.drop(row_final[0])
+        # Datatype:
+        datatype_relationship = {
+            "xsd:string":"value_string",
+            "xsd:date" : "value_date",
+            "xsd:float": "value_float",
+            "xsd:integer":"value_integer"
+        }
+
+        # Value edition:
+        for index, row in resulting_df.iterrows():
+            for k,v in datatype_relationship.items():
+                
 
-            # Reset Dataframe index again
-            resulting_df = resulting_df.reset_index(drop=True)
+                # value ---> value_DATATYPE:
+                if row["value_datatype"] == k:
+                    resulting_df.at[index, v] = resulting_df["value"][index]
+
+                # # valueIRI ---> process_type for Disability
+                # if row["model"] == "Disability" and row["valueIRI"] != None:
+                #     resulting_df.at[index, "process_type"] = resulting_df["valueIRI"][index]
+                #     resulting_df["valueIRI"][index] = None
+
+                # enddate correction:
+                if row["startdate"] != None and row["enddate"] == None:
+                    resulting_df["enddate"][index] = resulting_df["startdate"][index]
+
+
+        # clean blanks
+        for row_final in resulting_df.iterrows():
+            if row_final[1]["value"] == None and row_final[1]["attribute_id"] == None:
+                resulting_df = resulting_df.drop(row_final[0])
+                
+        del resulting_df["value"]
+
+
+        # # valueIRI ---> valueAttributeIRI:
+        # del resulting_df["valueAttributeIRI"]
+        # resulting_df.rename(columns={'valueIRI':'valueAttributeIRI'}, inplace=True)
+
+        # uniqid generation:
+        resulting_df['uniqid'] = ""
+        for i in resulting_df.index:
+            resulting_df.at[i, "uniqid"] = milisec()
+
+
+        # # Empty value row removal
+        # for row_final in resulting_df.iterrows():
+        #     if row_final[1]["valueOutput_date"] == None and row_final[1]["valueOutput_string"] == None and row_final[1]["valueOutput_float"] == None:
+        #         resulting_df = resulting_df.drop(row_final[0])
+
+        #     # Reset Dataframe index again
+        #     resulting_df = resulting_df.reset_index(drop=True)
                     
-        # uniqid (re)generation:
-        resulting_df = resulting_df.reset_index(drop=True)
+        # # uniqid (re)generation:
+        # resulting_df = resulting_df.reset_index(drop=True)
 
-        if uniqid_generation:
-            resulting_df['uniqid'] = ""
-            for i in resulting_df.index:
-                resulting_df.at[i, "uniqid"] = milisec()
-
-        # context_id (re)generation:
-        if contextid_generation:
-            resulting_df['context_id'] = ""
-            for i in resulting_df.index:
-                resulting_df.at[i, "context_id"] = milisec()
+        # if uniqid_generation:
+        #     resulting_df['uniqid'] = ""
+        #     for i in resulting_df.index:
+        #         resulting_df.at[i, "uniqid"] = milisec()
+
+        # # context_id (re)generation:
+        # if contextid_generation:
+        #     resulting_df['context_id'] = ""
+        #     for i in resulting_df.index:
+        #         resulting_df.at[i, "context_id"] = milisec()
 
         
         print("Structural transformation: Done")
         new = Hefesto.__init__(self, datainput= resulting_df, reset = True)
         return new
 
     def get_uri(self, col, ont):
@@ -255,23 +296,23 @@
             self.df_data[col] = self.df_data[col].replace([key],value) 
 
         print("Replacement from " + key + "to "+ value + " at column " + col +": Done")
         new = Hefesto.__init__(self, datainput= self.df_data, reset = True)
         return new
         
 
-# Test 1:
+# # Test 1:
 
-# test = Hefesto(datainput = "../data/NEWDATA.csv")
+# test = Hefesto(datainput = "../data/INPUT_DATA.csv")
 # transform = test.transform_Fiab()
-# transform.to_csv ("../data/CDEresult_888.csv", index = False, header=True)
+# transform.to_csv ("../data/OUTPUT_DATA.csv", index = False, header=True)
 
 # # Test 2
 # with open("../data/CDEconfig.yaml") as file:
 #     configuration = yaml.load(file, Loader=yaml.FullLoader)
 
-# test = Hefesto(datainput = "../data/input2.csv")
+# test = Hefesto(datainput = "../data/INPUT_DATA2.csv")
 # transform = test.transform_shape(configuration=configuration, clean_blanks = True) #, clean_blanks=False
 # # label = test.get_label("output_type")
 # # url_from_label= test.get_uri("output_type_label","ncit")
 # # repl= test.replacement("output_type_label", "Date","DateXXX", duplicate=False)
-# transform.to_csv ("../data/result6.csv", index = False, header=True)
+# transform.to_csv ("../data/OUTPUT_DATA2.csv", index = False, header=True)
```

### Comparing `Hefesto-0.3.8/Hefesto/template.py` & `Hefesto-0.3.9/Hefesto/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 
 class Template:
 
   template_model = dict(
 
+    Age = dict(
+      process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
+      output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
+      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C25150",
+      value_datatype = "xsd:date",
+      startdate = None,
+      enddate = None,
+      pid = None,
+      context_id = None
+    ),
+
     Birthdate = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
       attribute_type = "http://purl.obolibrary.org/obo/NCIT_C68615",
       value_datatype = "xsd:date",
       startdate = None,
       enddate = None,
@@ -104,15 +115,15 @@
     #   pid = None,
     #   context_id = None
     # ),
 
     Genetic = dict(
       process_type= "http://purl.obolibrary.org/obo/NCIT_C15709",
       output_type= "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C3367",
+      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C103223",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
@@ -154,37 +165,37 @@
     #   pid = None,
     #   context_id = None
     # ),
 
     Consent_contacted = dict(
       process_type= "http://purl.obolibrary.org/obo/OBI_0000810",
       output_type = "http://purl.obolibrary.org/obo/OBIB_0000488",
-      # attribute_type= "http://purl.obolibrary.org/obo/NCIT_C25460",
+      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C25460",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Consent_used = dict(
       process_type= "http://purl.obolibrary.org/obo/OBI_0000810",
       output_type = "http://purl.obolibrary.org/obo/DUO_0000001",
-      # attribute_type= "http://purl.obolibrary.org/obo/NCIT_C25460",
+      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C25460",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Biobank = dict(
       process_type= "http://purl.obolibrary.org/obo/OMIABIS_0000061",
       output_type= "http://purl.obolibrary.org/obo/NCIT_C115570",
-      # attribute_type= "http://purl.obolibrary.org/obo/NCIT_C25429",
+      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C25429",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
@@ -197,15 +208,15 @@
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Body_measurement = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470" ,
-      output_type=  "http://purl.obolibrary.org/obo/NCIT_C93940" ,
+      output_type=  "http://purl.obolibrary.org/obo/NCIT_C70856" ,
       value_datatype= "xsd:float" ,
       startdate= None ,
       enddate= None ,
       comments= None ,
       pid= None ,
       context_id= None 
     ),
@@ -221,15 +232,15 @@
       pid= None ,
       context_id= None 
     ),
 
 
     Imaging = dict(
       process_type = None ,
-      output_type =  "http://purl.obolibrary.org/obo/NCIT_C19477" ,
+      output_type =  "http://purl.obolibrary.org/obo/NCIT_C70856" ,
       value_datatype = "xsd:string" ,
       startdate= None ,
       enddate= None ,
       comments= None ,
       pid = None ,
       context_id= None 
     ),
```

### Comparing `Hefesto-0.3.8/README.md` & `Hefesto-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `Hefesto-0.3.8/setup.py` & `Hefesto-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #     readme = readme_file.read()
 
 # with open('requirements.txt') as f:
 #     requirements = f.read().splitlines()
 
 setup(
     name="Hefesto",
-    version="0.3.8",
+    version="0.3.9",
     packages=["Hefesto"],
     author="Pablo Alarcón Moreno",
     author_email="pabloalarconmoreno@gmail.com",
     url="https://github.com/pabloalarconm/hefesto",
     description="Preprocessing datatable toolkit",
     license="MIT",
     keywords=["EJP","CDE"]
```


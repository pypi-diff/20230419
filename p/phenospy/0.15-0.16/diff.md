# Comparing `tmp/phenospy-0.15.tar.gz` & `tmp/phenospy-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenospy-0.15.tar", last modified: Wed Apr 19 14:03:47 2023, max compression
+gzip compressed data, was "phenospy-0.16.tar", last modified: Wed Apr 19 15:44:31 2023, max compression
```

## Comparing `phenospy-0.15.tar` & `phenospy-0.16.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-19 14:03:47.133095 phenospy-0.15/
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1080 2023-03-13 19:55:04.000000 phenospy-0.15/LICENSE.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       31 2023-03-13 20:40:28.000000 phenospy-0.15/MANIFEST.in
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3384 2023-04-19 14:03:47.132893 phenospy-0.15/PKG-INFO
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2539 2023-04-18 19:03:17.000000 phenospy-0.15/README.md
-drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-19 14:03:47.127190 phenospy-0.15/phenospy/
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      370 2023-04-03 16:35:02.000000 phenospy-0.15/phenospy/__init__.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    18969 2023-04-17 16:25:07.000000 phenospy-0.15/phenospy/nl_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1109 2023-04-03 16:31:49.000000 phenospy-0.15/phenospy/nl_owlToMd.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2258 2023-04-03 16:50:14.000000 phenospy-0.15/phenospy/nl_owlToMd_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2403 2023-03-28 14:23:07.000000 phenospy-0.15/phenospy/owl_make_phsOntology.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      631 2023-03-28 17:14:38.000000 phenospy-0.15/phenospy/owl_owlready_config.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     4013 2023-03-28 18:24:24.000000 phenospy-0.15/phenospy/owl_xml2owl_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    16700 2023-04-17 06:49:33.000000 phenospy-0.15/phenospy/owl_xmlToOwl.py
-drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-19 14:03:47.132517 phenospy-0.15/phenospy/package-data/
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6148 2023-03-28 19:11:16.000000 phenospy-0.15/phenospy/package-data/.DS_Store
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      591 2023-03-27 19:35:46.000000 phenospy-0.15/phenospy/package-data/phenoscript.obda
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    18495 2023-03-27 19:35:46.000000 phenospy-0.15/phenospy/package-data/phenoscript.owl
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      127 2023-03-27 19:35:46.000000 phenospy-0.15/phenospy/package-data/phenoscript.properties
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3224 2023-04-19 08:58:27.000000 phenospy-0.15/phenospy/package-data/phs-config.yaml
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7502 2023-03-27 17:52:38.000000 phenospy-0.15/phenospy/package-data/snippets-default.json
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1065 2023-03-15 14:43:16.000000 phenospy-0.15/phenospy/phs_addXmlMeta.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5390 2023-03-28 18:02:16.000000 phenospy-0.15/phenospy/phs_grammar.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2232 2023-03-28 18:15:48.000000 phenospy-0.15/phenospy/phs_mainConvert.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3898 2023-03-28 18:28:37.000000 phenospy-0.15/phenospy/phs_parser_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3153 2023-03-28 18:28:31.000000 phenospy-0.15/phenospy/phs_various_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    14872 2023-03-28 18:12:47.000000 phenospy-0.15/phenospy/phs_xml.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6508 2023-03-28 18:13:03.000000 phenospy-0.15/phenospy/phs_xmlTranslateTerms.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7009 2023-03-28 17:14:38.000000 phenospy-0.15/phenospy/snips_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    10953 2023-04-19 14:00:48.000000 phenospy-0.15/phenospy/snips_makeFromYaml.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5201 2023-03-28 18:13:28.000000 phenospy-0.15/phenospy/snips_readFromJSON.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2366 2023-04-17 06:49:33.000000 phenospy-0.15/phenospy/xml_recodeThis.py
-drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-19 14:03:47.128876 phenospy-0.15/phenospy.egg-info/
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3384 2023-04-19 14:03:47.000000 phenospy-0.15/phenospy.egg-info/PKG-INFO
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      944 2023-04-19 14:03:47.000000 phenospy-0.15/phenospy.egg-info/SOURCES.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        1 2023-04-19 14:03:47.000000 phenospy-0.15/phenospy.egg-info/dependency_links.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       43 2023-04-19 14:03:47.000000 phenospy-0.15/phenospy.egg-info/requires.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        9 2023-04-19 14:03:47.000000 phenospy-0.15/phenospy.egg-info/top_level.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       38 2023-04-19 14:03:47.133149 phenospy-0.15/setup.cfg
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1238 2023-04-19 14:02:56.000000 phenospy-0.15/setup.py
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-19 15:44:31.277626 phenospy-0.16/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1080 2023-03-13 19:55:04.000000 phenospy-0.16/LICENSE.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       31 2023-03-13 20:40:28.000000 phenospy-0.16/MANIFEST.in
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3384 2023-04-19 15:44:31.277423 phenospy-0.16/PKG-INFO
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2539 2023-04-18 19:03:17.000000 phenospy-0.16/README.md
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-19 15:44:31.273752 phenospy-0.16/phenospy/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      370 2023-04-03 16:35:02.000000 phenospy-0.16/phenospy/__init__.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    18969 2023-04-17 16:25:07.000000 phenospy-0.16/phenospy/nl_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1109 2023-04-03 16:31:49.000000 phenospy-0.16/phenospy/nl_owlToMd.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2258 2023-04-03 16:50:14.000000 phenospy-0.16/phenospy/nl_owlToMd_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2403 2023-03-28 14:23:07.000000 phenospy-0.16/phenospy/owl_make_phsOntology.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      631 2023-03-28 17:14:38.000000 phenospy-0.16/phenospy/owl_owlready_config.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     4013 2023-03-28 18:24:24.000000 phenospy-0.16/phenospy/owl_xml2owl_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    16700 2023-04-17 06:49:33.000000 phenospy-0.16/phenospy/owl_xmlToOwl.py
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-19 15:44:31.277125 phenospy-0.16/phenospy/package-data/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6148 2023-03-28 19:11:16.000000 phenospy-0.16/phenospy/package-data/.DS_Store
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      591 2023-03-27 19:35:46.000000 phenospy-0.16/phenospy/package-data/phenoscript.obda
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    18495 2023-03-27 19:35:46.000000 phenospy-0.16/phenospy/package-data/phenoscript.owl
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      127 2023-03-27 19:35:46.000000 phenospy-0.16/phenospy/package-data/phenoscript.properties
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3224 2023-04-19 08:58:27.000000 phenospy-0.16/phenospy/package-data/phs-config.yaml
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7502 2023-03-27 17:52:38.000000 phenospy-0.16/phenospy/package-data/snippets-default.json
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1065 2023-03-15 14:43:16.000000 phenospy-0.16/phenospy/phs_addXmlMeta.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5390 2023-03-28 18:02:16.000000 phenospy-0.16/phenospy/phs_grammar.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2232 2023-03-28 18:15:48.000000 phenospy-0.16/phenospy/phs_mainConvert.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3898 2023-03-28 18:28:37.000000 phenospy-0.16/phenospy/phs_parser_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3153 2023-03-28 18:28:31.000000 phenospy-0.16/phenospy/phs_various_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    14872 2023-03-28 18:12:47.000000 phenospy-0.16/phenospy/phs_xml.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6508 2023-03-28 18:13:03.000000 phenospy-0.16/phenospy/phs_xmlTranslateTerms.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7009 2023-03-28 17:14:38.000000 phenospy-0.16/phenospy/snips_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    10953 2023-04-19 14:00:48.000000 phenospy-0.16/phenospy/snips_makeFromYaml.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5312 2023-04-19 15:37:02.000000 phenospy-0.16/phenospy/snips_readFromJSON.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2366 2023-04-17 06:49:33.000000 phenospy-0.16/phenospy/xml_recodeThis.py
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-19 15:44:31.274987 phenospy-0.16/phenospy.egg-info/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3384 2023-04-19 15:44:31.000000 phenospy-0.16/phenospy.egg-info/PKG-INFO
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      944 2023-04-19 15:44:31.000000 phenospy-0.16/phenospy.egg-info/SOURCES.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        1 2023-04-19 15:44:31.000000 phenospy-0.16/phenospy.egg-info/dependency_links.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       43 2023-04-19 15:44:31.000000 phenospy-0.16/phenospy.egg-info/requires.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        9 2023-04-19 15:44:31.000000 phenospy-0.16/phenospy.egg-info/top_level.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       38 2023-04-19 15:44:31.277680 phenospy-0.16/setup.cfg
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1238 2023-04-19 15:44:08.000000 phenospy-0.16/setup.py
```

### Comparing `phenospy-0.15/LICENSE.txt` & `phenospy-0.16/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/PKG-INFO` & `phenospy-0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenospy
-Version: 0.15
+Version: 0.16
 Summary: Tools for making and processing computable phenotype descriptions
 Home-page: https://github.com/sergeitarasov/PhenoScript
 Author: Sergei Tarasov
 Author-email: sergei.tarasov@helsinki.fi
 License: MIT
 Project-URL: Project Logo, https://raw.githubusercontent.com/sergeitarasov/PhenoScript/main/Phenoscript_logo.png
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `phenospy-0.15/README.md` & `phenospy-0.16/README.md`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/nl_fun.py` & `phenospy-0.16/phenospy/nl_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/nl_owlToMd.py` & `phenospy-0.16/phenospy/nl_owlToMd.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/nl_owlToMd_fun.py` & `phenospy-0.16/phenospy/nl_owlToMd_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/owl_make_phsOntology.py` & `phenospy-0.16/phenospy/owl_make_phsOntology.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/owl_owlready_config.py` & `phenospy-0.16/phenospy/owl_owlready_config.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/owl_xml2owl_fun.py` & `phenospy-0.16/phenospy/owl_xml2owl_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/owl_xmlToOwl.py` & `phenospy-0.16/phenospy/owl_xmlToOwl.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/package-data/.DS_Store` & `phenospy-0.16/phenospy/package-data/.DS_Store`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/package-data/phenoscript.obda` & `phenospy-0.16/phenospy/package-data/phenoscript.obda`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/package-data/phenoscript.owl` & `phenospy-0.16/phenospy/package-data/phenoscript.owl`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/package-data/phs-config.yaml` & `phenospy-0.16/phenospy/package-data/phs-config.yaml`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/package-data/snippets-default.json` & `phenospy-0.16/phenospy/package-data/snippets-default.json`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/phs_addXmlMeta.py` & `phenospy-0.16/phenospy/phs_addXmlMeta.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/phs_grammar.py` & `phenospy-0.16/phenospy/phs_grammar.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/phs_mainConvert.py` & `phenospy-0.16/phenospy/phs_mainConvert.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/phs_parser_fun.py` & `phenospy-0.16/phenospy/phs_parser_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/phs_various_fun.py` & `phenospy-0.16/phenospy/phs_various_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/phs_xml.py` & `phenospy-0.16/phenospy/phs_xml.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/phs_xmlTranslateTerms.py` & `phenospy-0.16/phenospy/phs_xmlTranslateTerms.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/snips_fun.py` & `phenospy-0.16/phenospy/snips_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/snips_makeFromYaml.py` & `phenospy-0.16/phenospy/snips_makeFromYaml.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy/snips_readFromJSON.py` & `phenospy-0.16/phenospy/snips_readFromJSON.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import codecs
 from phenospy.snips_fun import *
 
 # -----------------------------------------
 # Read VScode snips in JSON and make dictionaries
 # -----------------------------------------
 
 # yaml_file = '/Users/taravser/Documents/My_papers/PhenoScript_main/PhenoScript/phenospy_package/phenospy/package-data/phs-config.yaml'
@@ -21,17 +22,19 @@
     # Read JSON snippets
     # -----------------------------------------
 
     f_path = phs_yaml['snippet-dir']
     f_path = os.path.join(f_path, "phs-snippets.json")
     print(f"{Fore.BLUE}Reading snippets from JSON:{Style.RESET_ALL}", f_path)
 
-    f = open(f_path)
-    json_file = json.load(f)
-    f.close()
+    with codecs.open(f_path, 'r', encoding='utf-8') as f:
+        json_file = json.load(f)
+    # f = open(f_path)
+    # json_file = json.load(f)
+    # f.close()
     print(f"{Fore.GREEN}Good! File is read!{Style.RESET_ALL}")
 
     # for i in json_file:
     #     print(json_file[i]['prefix'])
     # ss= {}
     # ss.update({'ro-bearer_of': 'http://purl.obolibrary.org/obo/RO_0000053'})
     # ss.update({'>>': 'http://purl.obolibrary.org/obo/RO_0000053'})
```

### Comparing `phenospy-0.15/phenospy/xml_recodeThis.py` & `phenospy-0.16/phenospy/xml_recodeThis.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/phenospy.egg-info/PKG-INFO` & `phenospy-0.16/phenospy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenospy
-Version: 0.15
+Version: 0.16
 Summary: Tools for making and processing computable phenotype descriptions
 Home-page: https://github.com/sergeitarasov/PhenoScript
 Author: Sergei Tarasov
 Author-email: sergei.tarasov@helsinki.fi
 License: MIT
 Project-URL: Project Logo, https://raw.githubusercontent.com/sergeitarasov/PhenoScript/main/Phenoscript_logo.png
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `phenospy-0.15/phenospy.egg-info/SOURCES.txt` & `phenospy-0.16/phenospy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phenospy-0.15/setup.py` & `phenospy-0.16/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phenospy',
-    version='0.15',
+    version='0.16',
     packages=find_packages(exclude=['tests*', 'devel*', 'build*']),
     license='MIT',
     description='Tools for making and processing computable phenotype descriptions',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     install_requires=['Owlready2',
                       'PyYAML',
```


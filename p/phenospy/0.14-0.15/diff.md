# Comparing `tmp/phenospy-0.14.tar.gz` & `tmp/phenospy-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenospy-0.14.tar", last modified: Mon Apr 17 16:26:49 2023, max compression
+gzip compressed data, was "phenospy-0.15.tar", last modified: Wed Apr 19 14:03:47 2023, max compression
```

## Comparing `phenospy-0.14.tar` & `phenospy-0.15.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-17 16:26:49.160378 phenospy-0.14/
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1080 2023-03-13 19:55:04.000000 phenospy-0.14/LICENSE.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       31 2023-03-13 20:40:28.000000 phenospy-0.14/MANIFEST.in
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3666 2023-04-17 16:26:49.160182 phenospy-0.14/PKG-INFO
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2821 2023-04-17 14:30:21.000000 phenospy-0.14/README.md
-drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-17 16:26:49.155407 phenospy-0.14/phenospy/
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      370 2023-04-03 16:35:02.000000 phenospy-0.14/phenospy/__init__.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    18969 2023-04-17 16:25:07.000000 phenospy-0.14/phenospy/nl_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1109 2023-04-03 16:31:49.000000 phenospy-0.14/phenospy/nl_owlToMd.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2258 2023-04-03 16:50:14.000000 phenospy-0.14/phenospy/nl_owlToMd_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2403 2023-03-28 14:23:07.000000 phenospy-0.14/phenospy/owl_make_phsOntology.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      631 2023-03-28 17:14:38.000000 phenospy-0.14/phenospy/owl_owlready_config.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     4013 2023-03-28 18:24:24.000000 phenospy-0.14/phenospy/owl_xml2owl_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    16700 2023-04-17 06:49:33.000000 phenospy-0.14/phenospy/owl_xmlToOwl.py
-drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-17 16:26:49.159929 phenospy-0.14/phenospy/package-data/
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6148 2023-03-28 19:11:16.000000 phenospy-0.14/phenospy/package-data/.DS_Store
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      591 2023-03-27 19:35:46.000000 phenospy-0.14/phenospy/package-data/phenoscript.obda
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    18495 2023-03-27 19:35:46.000000 phenospy-0.14/phenospy/package-data/phenoscript.owl
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      127 2023-03-27 19:35:46.000000 phenospy-0.14/phenospy/package-data/phenoscript.properties
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2690 2023-04-17 08:10:21.000000 phenospy-0.14/phenospy/package-data/phs-config.yaml
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7502 2023-03-27 17:52:38.000000 phenospy-0.14/phenospy/package-data/snippets-default.json
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1065 2023-03-15 14:43:16.000000 phenospy-0.14/phenospy/phs_addXmlMeta.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5390 2023-03-28 18:02:16.000000 phenospy-0.14/phenospy/phs_grammar.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2232 2023-03-28 18:15:48.000000 phenospy-0.14/phenospy/phs_mainConvert.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3898 2023-03-28 18:28:37.000000 phenospy-0.14/phenospy/phs_parser_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3153 2023-03-28 18:28:31.000000 phenospy-0.14/phenospy/phs_various_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    14872 2023-03-28 18:12:47.000000 phenospy-0.14/phenospy/phs_xml.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6508 2023-03-28 18:13:03.000000 phenospy-0.14/phenospy/phs_xmlTranslateTerms.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7009 2023-03-28 17:14:38.000000 phenospy-0.14/phenospy/snips_fun.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    10935 2023-03-28 18:13:20.000000 phenospy-0.14/phenospy/snips_makeFromYaml.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5201 2023-03-28 18:13:28.000000 phenospy-0.14/phenospy/snips_readFromJSON.py
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2366 2023-04-17 06:49:33.000000 phenospy-0.14/phenospy/xml_recodeThis.py
-drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-17 16:26:49.157012 phenospy-0.14/phenospy.egg-info/
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3666 2023-04-17 16:26:49.000000 phenospy-0.14/phenospy.egg-info/PKG-INFO
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      944 2023-04-17 16:26:49.000000 phenospy-0.14/phenospy.egg-info/SOURCES.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        1 2023-04-17 16:26:49.000000 phenospy-0.14/phenospy.egg-info/dependency_links.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       43 2023-04-17 16:26:49.000000 phenospy-0.14/phenospy.egg-info/requires.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        9 2023-04-17 16:26:49.000000 phenospy-0.14/phenospy.egg-info/top_level.txt
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       38 2023-04-17 16:26:49.160432 phenospy-0.14/setup.cfg
--rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1238 2023-04-17 16:26:37.000000 phenospy-0.14/setup.py
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-19 14:03:47.133095 phenospy-0.15/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1080 2023-03-13 19:55:04.000000 phenospy-0.15/LICENSE.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       31 2023-03-13 20:40:28.000000 phenospy-0.15/MANIFEST.in
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3384 2023-04-19 14:03:47.132893 phenospy-0.15/PKG-INFO
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2539 2023-04-18 19:03:17.000000 phenospy-0.15/README.md
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-19 14:03:47.127190 phenospy-0.15/phenospy/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      370 2023-04-03 16:35:02.000000 phenospy-0.15/phenospy/__init__.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    18969 2023-04-17 16:25:07.000000 phenospy-0.15/phenospy/nl_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1109 2023-04-03 16:31:49.000000 phenospy-0.15/phenospy/nl_owlToMd.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2258 2023-04-03 16:50:14.000000 phenospy-0.15/phenospy/nl_owlToMd_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2403 2023-03-28 14:23:07.000000 phenospy-0.15/phenospy/owl_make_phsOntology.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      631 2023-03-28 17:14:38.000000 phenospy-0.15/phenospy/owl_owlready_config.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     4013 2023-03-28 18:24:24.000000 phenospy-0.15/phenospy/owl_xml2owl_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    16700 2023-04-17 06:49:33.000000 phenospy-0.15/phenospy/owl_xmlToOwl.py
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-19 14:03:47.132517 phenospy-0.15/phenospy/package-data/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6148 2023-03-28 19:11:16.000000 phenospy-0.15/phenospy/package-data/.DS_Store
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      591 2023-03-27 19:35:46.000000 phenospy-0.15/phenospy/package-data/phenoscript.obda
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    18495 2023-03-27 19:35:46.000000 phenospy-0.15/phenospy/package-data/phenoscript.owl
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      127 2023-03-27 19:35:46.000000 phenospy-0.15/phenospy/package-data/phenoscript.properties
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3224 2023-04-19 08:58:27.000000 phenospy-0.15/phenospy/package-data/phs-config.yaml
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7502 2023-03-27 17:52:38.000000 phenospy-0.15/phenospy/package-data/snippets-default.json
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1065 2023-03-15 14:43:16.000000 phenospy-0.15/phenospy/phs_addXmlMeta.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5390 2023-03-28 18:02:16.000000 phenospy-0.15/phenospy/phs_grammar.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2232 2023-03-28 18:15:48.000000 phenospy-0.15/phenospy/phs_mainConvert.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3898 2023-03-28 18:28:37.000000 phenospy-0.15/phenospy/phs_parser_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3153 2023-03-28 18:28:31.000000 phenospy-0.15/phenospy/phs_various_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    14872 2023-03-28 18:12:47.000000 phenospy-0.15/phenospy/phs_xml.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     6508 2023-03-28 18:13:03.000000 phenospy-0.15/phenospy/phs_xmlTranslateTerms.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     7009 2023-03-28 17:14:38.000000 phenospy-0.15/phenospy/snips_fun.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)    10953 2023-04-19 14:00:48.000000 phenospy-0.15/phenospy/snips_makeFromYaml.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     5201 2023-03-28 18:13:28.000000 phenospy-0.15/phenospy/snips_readFromJSON.py
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     2366 2023-04-17 06:49:33.000000 phenospy-0.15/phenospy/xml_recodeThis.py
+drwxr-xr-x   0 taravser (1128288419) ATKK\hyad-all (984178727)        0 2023-04-19 14:03:47.128876 phenospy-0.15/phenospy.egg-info/
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     3384 2023-04-19 14:03:47.000000 phenospy-0.15/phenospy.egg-info/PKG-INFO
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)      944 2023-04-19 14:03:47.000000 phenospy-0.15/phenospy.egg-info/SOURCES.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        1 2023-04-19 14:03:47.000000 phenospy-0.15/phenospy.egg-info/dependency_links.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       43 2023-04-19 14:03:47.000000 phenospy-0.15/phenospy.egg-info/requires.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)        9 2023-04-19 14:03:47.000000 phenospy-0.15/phenospy.egg-info/top_level.txt
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)       38 2023-04-19 14:03:47.133149 phenospy-0.15/setup.cfg
+-rw-r--r--   0 taravser (1128288419) ATKK\hyad-all (984178727)     1238 2023-04-19 14:02:56.000000 phenospy-0.15/setup.py
```

### Comparing `phenospy-0.14/LICENSE.txt` & `phenospy-0.15/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/PKG-INFO` & `phenospy-0.15/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenospy
-Version: 0.14
+Version: 0.15
 Summary: Tools for making and processing computable phenotype descriptions
 Home-page: https://github.com/sergeitarasov/PhenoScript
 Author: Sergei Tarasov
 Author-email: sergei.tarasov@helsinki.fi
 License: MIT
 Project-URL: Project Logo, https://raw.githubusercontent.com/sergeitarasov/PhenoScript/main/Phenoscript_logo.png
 Classifier: Development Status :: 3 - Alpha
@@ -37,14 +37,18 @@
 ## What can I do with Phenospy?
 
 - Create snippets based on selected ontologies for writing semantic phenotypes with the VS Code Phenoscript extension.
 - Convert the Phenoscript description into an OWL file.
 - Convert the Phenoscript description into an annotated Natural Language description (Markdown format).
 - Automatically compare species and phenotypes (under development).
 
+## Documentation
+
+See [Wiki for details](https://github.com/sergeitarasov/PhenoScript/wiki).
+
 ## Requirements
 
 * `Python >=3.0`
 
 If you are a new user with Python 2 installed, you should uninstall it and install Python 3 instead. For more information, please refer to [this discussion](https://stackoverflow.com/questions/3819449/how-to-uninstall-python-2-7-on-a-mac-os-x-10-6-4).
 
 
@@ -53,20 +57,8 @@
 
 ```{bash}
 pip install phenospy
 ```
 
 ## Issues
 
--  Phenospy is dependent on [Owlready2](https://github.com/pwin/owlready2), which uses the sqlite library. The latest versions of sqlite library (e.g., 3.40.0) are known to be very slow. If Phenospy package is slow, for example, when you make your snippets, downgrade your sqlite library version. In my case, 3.39.0 worked fine.
-
-## Quick start guide
-
-Coming soon.
-
-### Let's create snippets
-
-Coming soon.
-
-### Let's convert Phenoscript into OWL
-
-Coming soon.
+See [issues for details](https://github.com/sergeitarasov/PhenoScript/wiki/Issues).
```

### Comparing `phenospy-0.14/README.md` & `phenospy-0.15/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 ## What can I do with Phenospy?
 
 - Create snippets based on selected ontologies for writing semantic phenotypes with the VS Code Phenoscript extension.
 - Convert the Phenoscript description into an OWL file.
 - Convert the Phenoscript description into an annotated Natural Language description (Markdown format).
 - Automatically compare species and phenotypes (under development).
 
+## Documentation
+
+See [Wiki for details](https://github.com/sergeitarasov/PhenoScript/wiki).
+
 ## Requirements
 
 * `Python >=3.0`
 
 If you are a new user with Python 2 installed, you should uninstall it and install Python 3 instead. For more information, please refer to [this discussion](https://stackoverflow.com/questions/3819449/how-to-uninstall-python-2-7-on-a-mac-os-x-10-6-4).
 
 
@@ -33,20 +37,8 @@
 
 ```{bash}
 pip install phenospy
 ```
 
 ## Issues
 
--  Phenospy is dependent on [Owlready2](https://github.com/pwin/owlready2), which uses the sqlite library. The latest versions of sqlite library (e.g., 3.40.0) are known to be very slow. If Phenospy package is slow, for example, when you make your snippets, downgrade your sqlite library version. In my case, 3.39.0 worked fine.
-
-## Quick start guide
-
-Coming soon.
-
-### Let's create snippets
-
-Coming soon.
-
-### Let's convert Phenoscript into OWL
-
-Coming soon.
+See [issues for details](https://github.com/sergeitarasov/PhenoScript/wiki/Issues).
```

### Comparing `phenospy-0.14/phenospy/nl_fun.py` & `phenospy-0.15/phenospy/nl_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/nl_owlToMd.py` & `phenospy-0.15/phenospy/nl_owlToMd.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/nl_owlToMd_fun.py` & `phenospy-0.15/phenospy/nl_owlToMd_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/owl_make_phsOntology.py` & `phenospy-0.15/phenospy/owl_make_phsOntology.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/owl_owlready_config.py` & `phenospy-0.15/phenospy/owl_owlready_config.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/owl_xml2owl_fun.py` & `phenospy-0.15/phenospy/owl_xml2owl_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/owl_xmlToOwl.py` & `phenospy-0.15/phenospy/owl_xmlToOwl.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/package-data/.DS_Store` & `phenospy-0.15/phenospy/package-data/.DS_Store`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/package-data/phenoscript.obda` & `phenospy-0.15/phenospy/package-data/phenoscript.obda`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/package-data/phenoscript.owl` & `phenospy-0.15/phenospy/package-data/phenoscript.owl`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/package-data/phs-config.yaml` & `phenospy-0.15/phenospy/package-data/phs-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,45 @@
+# Specify the snippet directory that is used by your VS code
+# It looks something like: /.vscode/extensions/tarasov-lab.phenoscript-0.0.12/snippets/
+# Depending on your system it is located in:
 #   Win: `%USERPROFILE%\.vscode\extensions`
 #   Mac:`$HOME/.vscode/extensions`
 #   Linux: `$HOME/.vscode/extensions`
-snippet-dir: /Users/taravser/.vscode/extensions/tarasov-lab.phenoscript-0.0.12/snippets/
+# ADD CORRECT DIRECTORY
+snippet-dir: /.../.vscode/extensions/tarasov-lab.phenoscript-0.0.12/snippets/
+# ADD the names of the authors
 authors:
   'First1 Last1': https://orcid.org/0000-0001-xxxx-xxxx
   'First2 Last2': https://orcid.org/0000-0001-xxxx-xxxx
+# ADD a short title for your project
+project-title: "My New species"
 importOntologies:
-  - https://raw.githubusercontent.com/insect-morphology/colao/master/colao.owl
-  - https://raw.githubusercontent.com/hymao/hao/master/hao.owl
   - https://raw.githubusercontent.com/insect-morphology/aism/master/aism.owl
+  - https://raw.githubusercontent.com/insect-morphology/colao/master/colao.owl
+  # - https://raw.githubusercontent.com/hymao/hao/master/hao.owl
   - https://raw.githubusercontent.com/pato-ontology/pato/master/pato.owl
   - https://raw.githubusercontent.com/obophenotype/biological-spatial-ontology/master/bspo.owl
   - https://raw.githubusercontent.com/evoinfo/cdao/master/cdao.owl
   - https://raw.githubusercontent.com/information-artifact-ontology/IAO/v2020-12-09/iao.owl
   - https://raw.githubusercontent.com/oborel/obo-relations/master/ro.owl
   - https://raw.githubusercontent.com/bio-ontology-research-group/unit-ontology/master/uo.owl
   - http://camwebb.info/dsw/dsw.owl
-  - https://raw.githubusercontent.com/sergeitarasov/taxonomy-repo/main/owl/taxonomy-repo.owl # taxonomy
-  - https://raw.githubusercontent.com/sergeitarasov/PhenoScript/main/phenospy_package/phenospy/package-data/phenoscript.owl # phenoscript
-  - https://raw.githubusercontent.com/BiodiversityOntologies/bco/master/bco.owl # Biological Collections Ontology
+  # - https://raw.githubusercontent.com/sergeitarasov/taxonomy-repo/main/owl/taxonomy-repo.owl                                  # taxonomy
+  - https://raw.githubusercontent.com/sergeitarasov/PhenoScript/main/phenospy_package/phenospy/package-data/phenoscript.owl     # phenoscript
+  - https://raw.githubusercontent.com/BiodiversityOntologies/bco/master/bco.owl                                                 # Biological Collections Ontology
+  - http://purl.obolibrary.org/obo/uberon/uberon-base.owl                                                                       # UBERON
 namespace:
   default:    http://www.w3.org/2002/07/owl#
   others:
     rdfs:     http://www.w3.org/2000/01/rdf-schema#
     formats:  http://www.geneontology.org/formats/oboInOwl#
     dc:       http://purl.org/dc/
     hao:      http://purl.obolibrary.org/obo/HAO_
     aism:     http://purl.obolibrary.org/obo/AISM_
-    colao:     http://purl.obolibrary.org/obo/COLAO_
+    colao:    http://purl.obolibrary.org/obo/COLAO_
     bfo:      http://purl.obolibrary.org/obo/BFO_
     ro:       http://purl.obolibrary.org/obo/RO_
     obi:      http://purl.obolibrary.org/obo/OBI_
     ncbi:     http://purl.obolibrary.org/obo/NCBITaxon_
     iao:      http://purl.obolibrary.org/obo/IAO_
     bspo:     http://purl.obolibrary.org/obo/BSPO_
     pato:     http://purl.obolibrary.org/obo/PATO_
@@ -40,9 +48,9 @@
     cdao:     http://purl.obolibrary.org/obo/CDAO_
     unit:     http://purl.obolibrary.org/obo/UO_
     dsw:      http://purl.org/dsw/
     dwc:      http://rs.tdwg.org/dwc/terms/
     zoo:      http://zoobank.org/
     gbif:     https://www.gbif.org/species/
     phs:      https://github.com/sergeitarasov/PhenoScript/PHS_
-    uberon: http://purl.obolibrary.org/obo/UBERON_
+    uberon:   http://purl.obolibrary.org/obo/UBERON_
     # obo: http://purl.obolibrary.org/obo/
```

### Comparing `phenospy-0.14/phenospy/package-data/snippets-default.json` & `phenospy-0.15/phenospy/package-data/snippets-default.json`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/phs_addXmlMeta.py` & `phenospy-0.15/phenospy/phs_addXmlMeta.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/phs_grammar.py` & `phenospy-0.15/phenospy/phs_grammar.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/phs_mainConvert.py` & `phenospy-0.15/phenospy/phs_mainConvert.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/phs_parser_fun.py` & `phenospy-0.15/phenospy/phs_parser_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/phs_various_fun.py` & `phenospy-0.15/phenospy/phs_various_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/phs_xml.py` & `phenospy-0.15/phenospy/phs_xml.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/phs_xmlTranslateTerms.py` & `phenospy-0.15/phenospy/phs_xmlTranslateTerms.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/snips_fun.py` & `phenospy-0.15/phenospy/snips_fun.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/snips_makeFromYaml.py` & `phenospy-0.15/phenospy/snips_makeFromYaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,12 +266,12 @@
     snips_out = snips_default + ',' + snips_new
     snips_out = '{\n' + snips_out + '\n}'
     # save
     f_out = phs_yaml['snippet-dir']
     f_out = os.path.join(f_out, "phs-snippets.json")
     print(f"{Fore.BLUE}Saving snippets to:{Style.RESET_ALL}", f_out)
     # f_out = '/Users/taravser/Documents/My_papers/PhenoScript_main/PhenoScript/phenospy_package/phenospy/package-data/phs-snippets.json'
-    with open(f_out, 'w') as f:
+    with open(f_out, 'w', encoding='utf-8') as f:
         f.write(snips_out)
         f.close()
 
     print(f"{Fore.GREEN}DONE!{Style.RESET_ALL}")
```

### Comparing `phenospy-0.14/phenospy/snips_readFromJSON.py` & `phenospy-0.15/phenospy/snips_readFromJSON.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy/xml_recodeThis.py` & `phenospy-0.15/phenospy/xml_recodeThis.py`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/phenospy.egg-info/PKG-INFO` & `phenospy-0.15/phenospy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenospy
-Version: 0.14
+Version: 0.15
 Summary: Tools for making and processing computable phenotype descriptions
 Home-page: https://github.com/sergeitarasov/PhenoScript
 Author: Sergei Tarasov
 Author-email: sergei.tarasov@helsinki.fi
 License: MIT
 Project-URL: Project Logo, https://raw.githubusercontent.com/sergeitarasov/PhenoScript/main/Phenoscript_logo.png
 Classifier: Development Status :: 3 - Alpha
@@ -37,14 +37,18 @@
 ## What can I do with Phenospy?
 
 - Create snippets based on selected ontologies for writing semantic phenotypes with the VS Code Phenoscript extension.
 - Convert the Phenoscript description into an OWL file.
 - Convert the Phenoscript description into an annotated Natural Language description (Markdown format).
 - Automatically compare species and phenotypes (under development).
 
+## Documentation
+
+See [Wiki for details](https://github.com/sergeitarasov/PhenoScript/wiki).
+
 ## Requirements
 
 * `Python >=3.0`
 
 If you are a new user with Python 2 installed, you should uninstall it and install Python 3 instead. For more information, please refer to [this discussion](https://stackoverflow.com/questions/3819449/how-to-uninstall-python-2-7-on-a-mac-os-x-10-6-4).
 
 
@@ -53,20 +57,8 @@
 
 ```{bash}
 pip install phenospy
 ```
 
 ## Issues
 
--  Phenospy is dependent on [Owlready2](https://github.com/pwin/owlready2), which uses the sqlite library. The latest versions of sqlite library (e.g., 3.40.0) are known to be very slow. If Phenospy package is slow, for example, when you make your snippets, downgrade your sqlite library version. In my case, 3.39.0 worked fine.
-
-## Quick start guide
-
-Coming soon.
-
-### Let's create snippets
-
-Coming soon.
-
-### Let's convert Phenoscript into OWL
-
-Coming soon.
+See [issues for details](https://github.com/sergeitarasov/PhenoScript/wiki/Issues).
```

### Comparing `phenospy-0.14/phenospy.egg-info/SOURCES.txt` & `phenospy-0.15/phenospy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phenospy-0.14/setup.py` & `phenospy-0.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phenospy',
-    version='0.14',
+    version='0.15',
     packages=find_packages(exclude=['tests*', 'devel*', 'build*']),
     license='MIT',
     description='Tools for making and processing computable phenotype descriptions',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     install_requires=['Owlready2',
                       'PyYAML',
```


# Comparing `tmp/pe-configurator-0.1.1.tar.gz` & `tmp/pe-configurator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pe-configurator-0.1.1.tar", last modified: Wed Apr 19 17:30:36 2023, max compression
+gzip compressed data, was "pe-configurator-0.1.2.tar", last modified: Wed Apr 19 17:35:51 2023, max compression
```

## Comparing `pe-configurator-0.1.1.tar` & `pe-configurator-0.1.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11456 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10809 2023-04-19 17:29:14.000000 pe-configurator-0.1.1/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.245027 pe-configurator-0.1.1/blueprints/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      192 2023-04-19 17:29:14.000000 pe-configurator-0.1.1/blueprints/test.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.245027 pe-configurator-0.1.1/data/
--rw-r--r--   0 daniel    (1000) daniel    (1000)  2290335 2023-04-13 09:58:40.000000 pe-configurator-0.1.1/data/calibration_files.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.255027 pe-configurator-0.1.1/examples/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8196 2023-04-19 17:29:14.000000 pe-configurator-0.1.1/examples/.DS_Store
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.255027 pe-configurator-0.1.1/examples/test_GW190412/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   821276 2023-04-19 17:29:14.000000 pe-configurator-0.1.1/examples/test_GW190412/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      669 2023-04-19 17:29:14.000000 pe-configurator-0.1.1/examples/test_GW190412/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8592 2023-04-19 17:29:14.000000 pe-configurator-0.1.1/examples/test_GW190412/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.255027 pe-configurator-0.1.1/examples/test_GW190521/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   822260 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW190521/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      710 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW190521/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8565 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW190521/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/examples/test_GW190814/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   844645 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW190814/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      699 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW190814/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8839 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW190814/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/examples/test_GW191109/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   846106 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW191109/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      682 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW191109/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8663 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW191109/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/pe_configurator.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11456 2023-04-19 17:30:36.000000 pe-configurator-0.1.1/pe_configurator.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1024 2023-04-19 17:30:36.000000 pe-configurator-0.1.1/pe_configurator.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-19 17:30:36.000000 pe-configurator-0.1.1/pe_configurator.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-04-19 17:30:36.000000 pe-configurator-0.1.1/pe_configurator.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       94 2023-04-19 17:30:36.000000 pe-configurator-0.1.1/pe_configurator.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       15 2023-04-19 17:30:36.000000 pe-configurator-0.1.1/pe_configurator.egg-info/top_level.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/peconfigurator/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5977 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/peconfigurator/asimov.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       73 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/peconfigurator/asimov_template.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/peconfigurator/auxiliary/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/peconfigurator/auxiliary/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10401 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/peconfigurator/auxiliary/make_report.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7114 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/peconfigurator/auxiliary/run_analyzer.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10105 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/peconfigurator/get_settings.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    15907 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/peconfigurator/proc_samples.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2897 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/peconfigurator/run_on_many_events.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1313 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/pyproject.toml
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/setup.cfg
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/tests/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6015 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/tests/test_get_settings.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:35:51.554949 pe-configurator-0.1.2/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11456 2023-04-19 17:35:51.554949 pe-configurator-0.1.2/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10809 2023-04-19 17:29:14.000000 pe-configurator-0.1.2/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:35:51.544949 pe-configurator-0.1.2/blueprints/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      192 2023-04-19 17:29:14.000000 pe-configurator-0.1.2/blueprints/test.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:35:51.544949 pe-configurator-0.1.2/data/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)  2290335 2023-04-13 09:58:40.000000 pe-configurator-0.1.2/data/calibration_files.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:35:51.544949 pe-configurator-0.1.2/examples/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8196 2023-04-19 17:29:14.000000 pe-configurator-0.1.2/examples/.DS_Store
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:35:51.554949 pe-configurator-0.1.2/examples/test_GW190412/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   821276 2023-04-19 17:29:14.000000 pe-configurator-0.1.2/examples/test_GW190412/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      669 2023-04-19 17:29:14.000000 pe-configurator-0.1.2/examples/test_GW190412/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8592 2023-04-19 17:29:14.000000 pe-configurator-0.1.2/examples/test_GW190412/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:35:51.554949 pe-configurator-0.1.2/examples/test_GW190521/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   822260 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/examples/test_GW190521/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      710 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/examples/test_GW190521/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8565 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/examples/test_GW190521/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:35:51.554949 pe-configurator-0.1.2/examples/test_GW190814/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   844645 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/examples/test_GW190814/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      699 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/examples/test_GW190814/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8839 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/examples/test_GW190814/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:35:51.554949 pe-configurator-0.1.2/examples/test_GW191109/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   846106 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/examples/test_GW191109/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      682 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/examples/test_GW191109/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8663 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/examples/test_GW191109/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:35:51.554949 pe-configurator-0.1.2/pe_configurator.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11456 2023-04-19 17:35:51.000000 pe-configurator-0.1.2/pe_configurator.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1024 2023-04-19 17:35:51.000000 pe-configurator-0.1.2/pe_configurator.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-19 17:35:51.000000 pe-configurator-0.1.2/pe_configurator.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-04-19 17:35:51.000000 pe-configurator-0.1.2/pe_configurator.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       94 2023-04-19 17:35:51.000000 pe-configurator-0.1.2/pe_configurator.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       15 2023-04-19 17:35:51.000000 pe-configurator-0.1.2/pe_configurator.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:35:51.554949 pe-configurator-0.1.2/peconfigurator/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5953 2023-04-19 17:35:08.000000 pe-configurator-0.1.2/peconfigurator/asimov.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       73 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/peconfigurator/asimov_template.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:35:51.554949 pe-configurator-0.1.2/peconfigurator/auxiliary/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/peconfigurator/auxiliary/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10401 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/peconfigurator/auxiliary/make_report.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7114 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/peconfigurator/auxiliary/run_analyzer.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10105 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/peconfigurator/get_settings.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    15907 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/peconfigurator/proc_samples.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2897 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/peconfigurator/run_on_many_events.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1313 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/pyproject.toml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-04-19 17:35:51.554949 pe-configurator-0.1.2/setup.cfg
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:35:51.554949 pe-configurator-0.1.2/tests/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6015 2023-04-19 17:29:15.000000 pe-configurator-0.1.2/tests/test_get_settings.py
```

### Comparing `pe-configurator-0.1.1/PKG-INFO` & `pe-configurator-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe-configurator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tools to identify waveform settings and prior bounds for gravitational wave parameter estimation.
 Author-email: Hector Estelles <hector.estelles@ligo.org>, Serguei Ossokine <serguei.ossokine@ligo.org>, Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/pe/get_eob_settings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pe-configurator-0.1.1/README.md` & `pe-configurator-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/data/calibration_files.txt` & `pe-configurator-0.1.2/data/calibration_files.txt`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/examples/.DS_Store` & `pe-configurator-0.1.2/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/examples/test_GW190412/test.html` & `pe-configurator-0.1.2/examples/test_GW190412/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/examples/test_GW190412/test.json` & `pe-configurator-0.1.2/examples/test_GW190412/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/examples/test_GW190412/test.pdf` & `pe-configurator-0.1.2/examples/test_GW190412/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/examples/test_GW190521/test.html` & `pe-configurator-0.1.2/examples/test_GW190521/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/examples/test_GW190521/test.json` & `pe-configurator-0.1.2/examples/test_GW190521/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/examples/test_GW190521/test.pdf` & `pe-configurator-0.1.2/examples/test_GW190521/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/examples/test_GW190814/test.html` & `pe-configurator-0.1.2/examples/test_GW190814/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/examples/test_GW190814/test.json` & `pe-configurator-0.1.2/examples/test_GW190814/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/examples/test_GW190814/test.pdf` & `pe-configurator-0.1.2/examples/test_GW190814/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/examples/test_GW191109/test.html` & `pe-configurator-0.1.2/examples/test_GW191109/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/examples/test_GW191109/test.json` & `pe-configurator-0.1.2/examples/test_GW191109/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/examples/test_GW191109/test.pdf` & `pe-configurator-0.1.2/examples/test_GW191109/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/pe_configurator.egg-info/PKG-INFO` & `pe-configurator-0.1.2/pe_configurator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe-configurator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tools to identify waveform settings and prior bounds for gravitational wave parameter estimation.
 Author-email: Hector Estelles <hector.estelles@ligo.org>, Serguei Ossokine <serguei.ossokine@ligo.org>, Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/pe/get_eob_settings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pe-configurator-0.1.1/pe_configurator.egg-info/SOURCES.txt` & `pe-configurator-0.1.2/pe_configurator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/peconfigurator/asimov.py` & `pe-configurator-0.1.2/peconfigurator/asimov.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         name = self.production.name
         ini = self.production.event.repository.find_prods(name,
                                                           self.category)[0]
 
         meta = self.production.meta
         executable = f"{os.path.join(config.get('pipelines', 'environment'), 'bin', self._pipeline_command)}"
         command = ["--dataset", f"{meta['dataset']}",
-                   "--json_file", os.path.join(self.production.rundir, "results", "recommendations.json"),
+                   "--json_file", os.path.join("results", "recommendations.json"),
 	           "--q-min", f"{meta['minimum mass ratio']}",
                    ]
         if "higher modes" in meta['checks']:
             command += ["--HM"]
         if "luminosity distance" in meta['checks']:
             command += ["--include_dL_recommendations"]
         if "no safety" in meta['checks']:
```

### Comparing `pe-configurator-0.1.1/peconfigurator/auxiliary/make_report.py` & `pe-configurator-0.1.2/peconfigurator/auxiliary/make_report.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/peconfigurator/auxiliary/run_analyzer.py` & `pe-configurator-0.1.2/peconfigurator/auxiliary/run_analyzer.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/peconfigurator/get_settings.py` & `pe-configurator-0.1.2/peconfigurator/get_settings.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/peconfigurator/proc_samples.py` & `pe-configurator-0.1.2/peconfigurator/proc_samples.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/peconfigurator/run_on_many_events.py` & `pe-configurator-0.1.2/peconfigurator/run_on_many_events.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/pyproject.toml` & `pe-configurator-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.1/tests/test_get_settings.py` & `pe-configurator-0.1.2/tests/test_get_settings.py`

 * *Files identical despite different names*


# Comparing `tmp/pe-configurator-0.1.0.tar.gz` & `tmp/pe-configurator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pe-configurator-0.1.0.tar", last modified: Fri Apr 14 09:53:00 2023, max compression
+gzip compressed data, was "pe-configurator-0.1.1.tar", last modified: Wed Apr 19 17:30:36 2023, max compression
```

## Comparing `pe-configurator-0.1.0.tar` & `pe-configurator-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,46 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:53:00.686336 pe-configurator-0.1.0/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11580 2023-04-14 09:53:00.686336 pe-configurator-0.1.0/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10933 2023-04-14 09:37:19.000000 pe-configurator-0.1.0/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:53:00.676336 pe-configurator-0.1.0/blueprints/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      192 2023-04-13 13:58:42.000000 pe-configurator-0.1.0/blueprints/test.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:53:00.676336 pe-configurator-0.1.0/data/
--rw-r--r--   0 daniel    (1000) daniel    (1000)  2290335 2023-04-13 09:58:40.000000 pe-configurator-0.1.0/data/calibration_files.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:53:00.676336 pe-configurator-0.1.0/examples/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8196 2023-04-13 10:04:58.000000 pe-configurator-0.1.0/examples/.DS_Store
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:53:00.676336 pe-configurator-0.1.0/examples/test_GW190412/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   821276 2023-04-13 10:04:58.000000 pe-configurator-0.1.0/examples/test_GW190412/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      669 2023-04-13 10:04:58.000000 pe-configurator-0.1.0/examples/test_GW190412/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8592 2023-04-13 10:04:58.000000 pe-configurator-0.1.0/examples/test_GW190412/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:53:00.676336 pe-configurator-0.1.0/examples/test_GW190521/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   822260 2023-04-13 10:04:58.000000 pe-configurator-0.1.0/examples/test_GW190521/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      710 2023-04-13 10:04:58.000000 pe-configurator-0.1.0/examples/test_GW190521/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8565 2023-04-13 10:04:58.000000 pe-configurator-0.1.0/examples/test_GW190521/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:53:00.676336 pe-configurator-0.1.0/examples/test_GW190814/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   844645 2023-04-13 10:04:58.000000 pe-configurator-0.1.0/examples/test_GW190814/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      699 2023-04-13 10:04:58.000000 pe-configurator-0.1.0/examples/test_GW190814/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8839 2023-04-13 10:04:58.000000 pe-configurator-0.1.0/examples/test_GW190814/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:53:00.676336 pe-configurator-0.1.0/examples/test_GW191109/
--rw-r--r--   0 daniel    (1000) daniel    (1000)   846106 2023-04-13 10:04:58.000000 pe-configurator-0.1.0/examples/test_GW191109/test.html
--rw-r--r--   0 daniel    (1000) daniel    (1000)      682 2023-04-13 10:04:58.000000 pe-configurator-0.1.0/examples/test_GW191109/test.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8663 2023-04-13 10:04:58.000000 pe-configurator-0.1.0/examples/test_GW191109/test.pdf
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:53:00.676336 pe-configurator-0.1.0/pe_configurator.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11580 2023-04-14 09:53:00.000000 pe-configurator-0.1.0/pe_configurator.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1094 2023-04-14 09:53:00.000000 pe-configurator-0.1.0/pe_configurator.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-14 09:53:00.000000 pe-configurator-0.1.0/pe_configurator.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-04-14 09:53:00.000000 pe-configurator-0.1.0/pe_configurator.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       94 2023-04-14 09:53:00.000000 pe-configurator-0.1.0/pe_configurator.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       15 2023-04-14 09:53:00.000000 pe-configurator-0.1.0/pe_configurator.egg-info/top_level.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:53:00.676336 pe-configurator-0.1.0/peconfigurator/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      609 2023-04-14 09:49:35.000000 pe-configurator-0.1.0/peconfigurator/O3b_run_map.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5626 2023-04-14 09:49:35.000000 pe-configurator-0.1.0/peconfigurator/asimov.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       73 2023-04-14 09:49:35.000000 pe-configurator-0.1.0/peconfigurator/asimov_template.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:53:00.686336 pe-configurator-0.1.0/peconfigurator/auxiliary/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:49:35.000000 pe-configurator-0.1.0/peconfigurator/auxiliary/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10968 2023-04-14 09:49:35.000000 pe-configurator-0.1.0/peconfigurator/auxiliary/make_report.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7114 2023-04-14 09:49:35.000000 pe-configurator-0.1.0/peconfigurator/auxiliary/run_analyzer.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     7669 2023-04-14 09:49:35.000000 pe-configurator-0.1.0/peconfigurator/get_EOB_settings.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     4710 2023-04-14 09:49:35.000000 pe-configurator-0.1.0/peconfigurator/proc_event_repo.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    15874 2023-04-14 09:49:35.000000 pe-configurator-0.1.0/peconfigurator/proc_samples.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2897 2023-04-14 09:49:35.000000 pe-configurator-0.1.0/peconfigurator/run_on_many_events.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1284 2023-04-14 09:49:35.000000 pe-configurator-0.1.0/pyproject.toml
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-04-14 09:53:00.686336 pe-configurator-0.1.0/setup.cfg
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:53:00.686336 pe-configurator-0.1.0/tests/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5967 2023-04-13 10:04:58.000000 pe-configurator-0.1.0/tests/test_get_settings.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11456 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10809 2023-04-19 17:29:14.000000 pe-configurator-0.1.1/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.245027 pe-configurator-0.1.1/blueprints/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      192 2023-04-19 17:29:14.000000 pe-configurator-0.1.1/blueprints/test.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.245027 pe-configurator-0.1.1/data/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)  2290335 2023-04-13 09:58:40.000000 pe-configurator-0.1.1/data/calibration_files.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.255027 pe-configurator-0.1.1/examples/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8196 2023-04-19 17:29:14.000000 pe-configurator-0.1.1/examples/.DS_Store
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.255027 pe-configurator-0.1.1/examples/test_GW190412/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   821276 2023-04-19 17:29:14.000000 pe-configurator-0.1.1/examples/test_GW190412/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      669 2023-04-19 17:29:14.000000 pe-configurator-0.1.1/examples/test_GW190412/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8592 2023-04-19 17:29:14.000000 pe-configurator-0.1.1/examples/test_GW190412/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.255027 pe-configurator-0.1.1/examples/test_GW190521/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   822260 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW190521/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      710 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW190521/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8565 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW190521/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/examples/test_GW190814/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   844645 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW190814/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      699 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW190814/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8839 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW190814/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/examples/test_GW191109/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)   846106 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW191109/test.html
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      682 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW191109/test.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8663 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/examples/test_GW191109/test.pdf
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/pe_configurator.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    11456 2023-04-19 17:30:36.000000 pe-configurator-0.1.1/pe_configurator.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1024 2023-04-19 17:30:36.000000 pe-configurator-0.1.1/pe_configurator.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-19 17:30:36.000000 pe-configurator-0.1.1/pe_configurator.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      142 2023-04-19 17:30:36.000000 pe-configurator-0.1.1/pe_configurator.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       94 2023-04-19 17:30:36.000000 pe-configurator-0.1.1/pe_configurator.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       15 2023-04-19 17:30:36.000000 pe-configurator-0.1.1/pe_configurator.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/peconfigurator/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5977 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/peconfigurator/asimov.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       73 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/peconfigurator/asimov_template.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/peconfigurator/auxiliary/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/peconfigurator/auxiliary/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10401 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/peconfigurator/auxiliary/make_report.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7114 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/peconfigurator/auxiliary/run_analyzer.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    10105 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/peconfigurator/get_settings.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    15907 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/peconfigurator/proc_samples.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2897 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/peconfigurator/run_on_many_events.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1313 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/pyproject.toml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/setup.cfg
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:30:36.265027 pe-configurator-0.1.1/tests/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6015 2023-04-19 17:29:15.000000 pe-configurator-0.1.1/tests/test_get_settings.py
```

### Comparing `pe-configurator-0.1.0/PKG-INFO` & `pe-configurator-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 Metadata-Version: 2.1
 Name: pe-configurator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools to identify waveform settings and prior bounds for gravitational wave parameter estimation.
 Author-email: Hector Estelles <hector.estelles@ligo.org>, Serguei Ossokine <serguei.ossokine@ligo.org>, Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/pe/get_eob_settings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: asimov
 
 # Introduction
-In this repo we provide scripts that automatically try to determine some
-settings that must be applied for time domain EOB waveforms to run. 
+This package provides scripts that automatically try to determine some settings that must be applied for PE runs, especially for time-domain waveforms.
+The settings try to strike a balance between being conservative and being feasible.
 
 ### Top-level description
-The main script to use is `proc_samples.py`.  Given a preliminary PE run, it will perform some basic checks and then generate recommended PE settings. It can also optionally generate a `json` format result for automatic ingestion by the robot and a more detailed standalone report (still under construction). 
-
-NB: the script is intended to be used for "vanilla" BBH events. 
+The main script to use is `proc_samples.py`.  Given a preliminary PE run, it will perform some basic checks and then generate recommended PE settings. It can also optionally generate a `json` format result for automatic ingestion by `asimov` and a more detailed standalone, human-readable report. Users are _highly_ encouraged to take a look at the report.
 
 ### Usage
 Here is a typical usage example:
 ```
-peconfigurator --HM /home/zoheyr.doctor/public_html/O3/O3aCatalog/data_release/all_posterior_samples/GW190413_052954_comoving.h5  --dataset C01:SEOBNRv4P --json_file test.json --report_file test.pdf
+peconfigurator --HM posterior_samples.h5  --dataset C01:IMRPhenomXPHM --json_file test.json --report_file test.pdf
 ```
 
 For all the available options, please check
 ```
 peconfigurator -h
 ```
 
-If all goes right it will print something like 
+If all goes right, it will print something like
 ```
 Processing....
 Estimating seglen based on posterior samples
 100%|███████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 10885/10885 [02:22<00:00, 76.48it/s]
 Estimating srate based on posterior samples
 Using ell = 3 for Nyquist check
 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 10885/10885 [00:00<00:00, 30557.61it/s]
@@ -63,98 +61,83 @@
 Checking that f_ref is not above f_MECO: PASSED
 
 ++++++++++++++++++++++++++++++ Suggested settings ++++++++++++++++++++++++++++++
 Real required srate  753.7701187444659, as power of 2: 1024
 Real seglen: 4.046571094240219, with padding+rollon: 6.44657109424022, as power of 2: 8.0
 Check from samples:
 Real seglen: 0.8090184427276651, with padding+rollon: 3.209018442727665, as power of 2: 4.0
-f_start: 13.333333333333334, as amp_order: 1
+f_start: 13.333333333333334
 Real bounds on chirp mass: [25.004179128030085,53.95741304487518], suggested bounds: [20.00334330242407,64.74889565385021]
 Real distance max: 8000.0
 
 ```
 
 The `test.json` file contains some machine-readable information as shown below:
 
 ```json
 {
     "srate": 1024,
     "f_start": 13.333333333333334,
     "f_ref": 20.0,
-    "amp_order": 1,
     "seglen": 8.0,
     "chirpmass_min": 20.00334330242407,
     "chirpmass_max": 64.74889565385021,
     "metadata": {
         "date": "2020-11-05 04:38:55.172784",
-        "command_line_args": "Namespace(HM=True, bounds_tol=0.2, dataset='C01:SEOBNRv4P', ell_max=3, f_ref=20.0, flow=20.0, json_file='test.json', nbins=50, q_min=None, report_file='test.pdf', samples_file='/home/zoheyr.doctor/public_html/O3/O3aCatalog/data_release/all_posterior_samples/GW190413_052954_comoving.h5', tolerance=2.0)"
+        "command_line_args": "Namespace(HM=True, bounds_tol=0.2, dataset='C01:IMRPhenomXPHM', ell_max=3, f_ref=20.0, flow=20.0, json_file='test.json', nbins=50, q_min=None, report_file='test.pdf', samples_file='./posterior_samples.h5', tolerance=2.0)"
     }
 ```
 
-An example of the generated report can be seen here:
-
-https://ldas-jobs.ligo.caltech.edu/~serguei.ossokine/LVC/O3b_settings/test.html
-
-It is recommended that the report is reviewed carefully before the settings are approved.
+An `html` report will also be generated.
 
 ### Running on many events
 To run on many events, a separate script, `run_on_many_events.py` is provided. The most important settings to it are the path to the repo containing the superevents (specified via `--repo`) and a json file containing the names of events to run on and the corresponding preferred data set inside the PEsummary metafile (specified via `--run_map`). An example of such a json file is below:
 ```json
 {
-    "S191105e":"EXP1",
-    "S191129u":"EXP4"
+    "S150914":"EXP1",
+    "S190521":"EXP4"
 }
 ```
 Here is an example of calling the script:
 ```bash
-python  run_on_many_events.py --repo /home/gareth.davies/git_repos/o3b_catalog_events/ --run_map ../test_run_map.json --json_output --full_reports --output_dir example
+python  run_on_many_events.py --repo ./my_events/ --run_map ../test_run_map.json --json_output --full_reports --output_dir example
 ```
-With these options, a separate directory will be created for each superevent inside the `example` directory. Inside each directory there will be 4 files, corresponding to the raw log (ending in `.log`), the machine readable json file with recommended settings (ending in `.json`), and 2 files corresponding to a more verbose report (ending with `.ipynb` and `.html`). The `html` report is the exectued and rendered version of the `ipynb` file, provided for debugging purposes. 
+With these options, a separate directory will be created for each superevent inside the `example` directory. Inside each directory there will be 4 files, corresponding to the raw log (ending in `.log`), the machine readable json file with recommended settings (ending in `.json`), and 2 files corresponding to a more verbose report (ending with `.ipynb` and `.html`). The `html` report is the executed and rendered version of the `ipynb` file, provided for debugging purposes.
 
-An example of the directory and output can be found here:
-https://ldas-jobs.ligo.caltech.edu/~serguei.ossokine/LVC/O3b_settings/full_test/
+Examples can be found in `example` folder.
 
 
 ### Detailed description of internal logic
 This section describes the detailed logic used in deciding the various settings.  Many of these settings depend on the masses of the binary and are thus affected by proposed changes to the chirp mass prior which is described below.  For every setting we generate 2 estimates: one coming directly from the samples and a conservative one, which takes into account the wider chirp mass prior. In particular,  the following strategy is adopted:
 
 1. Estimate the quantity of interest from the samples.
 2. Pick the most extreme value of the quantity of interest (e.g. max seglen or min $f_{\rm start}$) and find its parameters (mass ratio and spins)
 3. Use either the lower or upper proposed chirp mass bounds (as appropriate) and the mass ratio from step 2 to estimate a new total mass
 4. Use this total mass along with the other params (as appropriate) to produce a new estimate of the quantity of interest
 
 
 
 #### Deciding the chirp mass bounds for the prior
-The script suggests a chirp mass prior that is wider than the minimum and maximum chirp masses found in the samples, to guard against the moving around of the posterior due to e.g. using a different waveform model. 
+The script suggests a chirp mass prior that is wider than the minimum and maximum chirp masses found in the samples, to guard against the moving around of the posterior due to e.g. using a different waveform model.
 
 The script proposes chirp mass bounds in 2 steps:
 1. Given the preliminary PE run, it checks of railing is present in the chirp mass posterior. This process involves a couple of free parameters that control how strict this check is. This is governed by the options `--tolerance` and `nbins`. See `-h` for more details.
-2. If no railing is found, the proposed bounds are given by $`[(1-f)\mathcal{M}_{\rm min},(1+f)\mathcal{M}_{\rm max}]`$ where $`f`$ is a free parameter, given by the option `--bounds_tol` with the default value of **0.2**.
+2. If no railing is found, the proposed bounds are computed depending on the width of the chirp mass posterior $`\Delta\mathcal{M}=\mathcal{M}_{\rm max}-\mathcal{M}_{\rm min}`$. If the width is greater than $`30M_{\otol}`$, then the proposed bounds are given by $`[(1-f)\mathcal{M}_{\rm min},(1+f)\mathcal{M}_{\rm max}]`$ where $`f`$ is a free parameter, given by the option `--bounds_tol` with the default value of **0.2**. If the width is smaller than $`30M_{\otol}`$, then the bound are given by $`[\mathcal{M}_{\rm min}-f\Delta\mathcal{M},\mathcal{M}_{\rm max}+f\Delta\mathcal{M}f]`$.
 
 
 #### Deciding the sampling rate
-The sampling rate is determined by the requirement that it's high enough to resolve the highest frequency we are interested in. This is generally given by the frequency of the highest $`(\ell,m)`$ mode in the ringdown. This is estimated by using the `SEOBNRv4HM` routines.  The user is given control which $`\ell`$ is used for this Nyquist frequency check via the option `--ell-max`. By default it is set to **3**.  To be precise, the sampling rate is computed as $`2f_{\rm max}`$ and then rounded up to the next power of 2. 
+The sampling rate is determined by the requirement that it's high enough to resolve the highest frequency we are interested in. This is generally given by the frequency of the highest $`(\ell,m)`$ mode in the ringdown. This is estimated by using the `SEOBNRv4HM` routines.  The user is given control which $`\ell`$ is used for this Nyquist frequency check via the option `--ell-max`. By default it is set to **3**.  To be precise, the sampling rate is computed as $`2f_{\rm max}`$ and then rounded up to the next power of 2.
 
 #### Deciding the starting frequency
-The starting frequency determines the length of the generated waveform. For `SEOBNR` time-domain family of waveforms there are two considerations that come into play:
-1. The starting frequency (which corresponds to the frequency of the (2,2) mode) has to be such that the desired $`(\ell,m)`$ mode is present at the provided `flow` (which gives the lower bound of the likelihood integral and is an argument supplied by the user, set by default to **20 Hz**). The script uses the PN relation (valid in the inspiral) that $`f_{\ell m}=\frac{m}{2}f_{22}`$ to dermine this. _In principle, this consideration applies to any time-domain waveform._
-2. The starting frequency is not too close to merger. This is a limitation of the `SEOBNR` time domain waveforms due to the need i) for a long enough inspiral to attach ringdown ii) to generate quasi-circular initial conditions. The script uses the same condition as the waveform model internally to check if the starting frequency is below this frequency limit. 
+The starting frequency determines the length of the generated waveform. For time-domain family of waveforms there are two considerations that may come into play:
+1. The starting frequency (which corresponds to the frequency of the (2,2) mode) has to be such that the desired $`(\ell,m)`$ mode is present at the provided `flow` (which gives the lower bound of the likelihood integral and is an argument supplied by the user, set by default to **20 Hz**). The script uses the PN relation (valid in the inspiral) that $`f_{\ell m}=\frac{m}{2}f_{22}`$ to dermine this. _In principle, this consideration applies to any time-domain waveform, but need not be used for frequency-domain waveforms_
+2. The starting frequency is not too close to merger. This is a limitation of the `SEOBNR` time domain waveforms due to the need i) for a long enough inspiral to attach ringdown ii) to generate quasi-circular initial conditions. The script uses the same condition as the waveform model internally to check if the starting frequency is below this frequency limit.
 
 #### Deciding the seglen
 The raw segment length is determined by the following formula
 $`t = T(1+s)+t_{\rm pad}+t_{\rm rollon}`$, where $`T`$ is an estimate of the duration of the waveform, including inspiral, merger and ringdown; $`s`$ is a safety factor (default value of 0.03), $`t_{\rm pad}`$ is padding (default is 2 seconds) and $`t_{\rm rollon}`$ is the Tukey window roll on duration (default is 0.4 seconds).  The duration $`T`$ is taken to be a function of the 2 component masses $`m_{i}`$, the z-components of the dimensionless spin $`\chi_{i}`$ and of course the low frequency cutoff `flow` and computed using the SEOBNRv4_ROM function.  *Notice that this means explicitly that we only care about the duration of the waveform from `flow` onwards and not from `f_start`*.   Finally the seglen is rounded to the next power of 2.
 
 
 #### Checking the reference frequency
-The reference frequency is an **input** parameter, encoded in the option `--f_ref` with a default value of **20 Hz**. The script then computes the MECO frequency for all the samples, and checks that $`f_{\rm ref}\leq 0.97f_{\rm MECO}`$. If not, a message is printed out and even if specified a `json` report is **not** generated.  **Note that the script does not provide a recommendation for the reference frequency as this should be guided by physics.**
-
-Note that the failing of any railing checks and the reference frequency check can be ignored by passing the flag `--override_safeties`. 
-
-
-
-
-
-
-
-
+The reference frequency is an **input** parameter, encoded in the option `--f_ref` with a default value of **20 Hz**. The script then computes the MECO frequency for all the samples, and checks that $`f_{\rm ref}\leq 0.97f_{\rm MECO}`$. If not, a message is printed out and $`f_{\rm ref}`$ is overwritten to be $`0.97f_{\rm MECO}`$ (or $`f_{\rm start}`$ if this is greater).
 
+**Note that the failing of any railing checks and the reference frequency check can be ignored by passing the flag `--override_safeties`.**
```

### Comparing `pe-configurator-0.1.0/README.md` & `pe-configurator-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # Introduction
-In this repo we provide scripts that automatically try to determine some
-settings that must be applied for time domain EOB waveforms to run. 
+This package provides scripts that automatically try to determine some settings that must be applied for PE runs, especially for time-domain waveforms.
+The settings try to strike a balance between being conservative and being feasible.
 
 ### Top-level description
-The main script to use is `proc_samples.py`.  Given a preliminary PE run, it will perform some basic checks and then generate recommended PE settings. It can also optionally generate a `json` format result for automatic ingestion by the robot and a more detailed standalone report (still under construction). 
-
-NB: the script is intended to be used for "vanilla" BBH events. 
+The main script to use is `proc_samples.py`.  Given a preliminary PE run, it will perform some basic checks and then generate recommended PE settings. It can also optionally generate a `json` format result for automatic ingestion by `asimov` and a more detailed standalone, human-readable report. Users are _highly_ encouraged to take a look at the report.
 
 ### Usage
 Here is a typical usage example:
 ```
-peconfigurator --HM /home/zoheyr.doctor/public_html/O3/O3aCatalog/data_release/all_posterior_samples/GW190413_052954_comoving.h5  --dataset C01:SEOBNRv4P --json_file test.json --report_file test.pdf
+peconfigurator --HM posterior_samples.h5  --dataset C01:IMRPhenomXPHM --json_file test.json --report_file test.pdf
 ```
 
 For all the available options, please check
 ```
 peconfigurator -h
 ```
 
-If all goes right it will print something like 
+If all goes right, it will print something like
 ```
 Processing....
 Estimating seglen based on posterior samples
 100%|███████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 10885/10885 [02:22<00:00, 76.48it/s]
 Estimating srate based on posterior samples
 Using ell = 3 for Nyquist check
 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 10885/10885 [00:00<00:00, 30557.61it/s]
@@ -48,98 +46,83 @@
 Checking that f_ref is not above f_MECO: PASSED
 
 ++++++++++++++++++++++++++++++ Suggested settings ++++++++++++++++++++++++++++++
 Real required srate  753.7701187444659, as power of 2: 1024
 Real seglen: 4.046571094240219, with padding+rollon: 6.44657109424022, as power of 2: 8.0
 Check from samples:
 Real seglen: 0.8090184427276651, with padding+rollon: 3.209018442727665, as power of 2: 4.0
-f_start: 13.333333333333334, as amp_order: 1
+f_start: 13.333333333333334
 Real bounds on chirp mass: [25.004179128030085,53.95741304487518], suggested bounds: [20.00334330242407,64.74889565385021]
 Real distance max: 8000.0
 
 ```
 
 The `test.json` file contains some machine-readable information as shown below:
 
 ```json
 {
     "srate": 1024,
     "f_start": 13.333333333333334,
     "f_ref": 20.0,
-    "amp_order": 1,
     "seglen": 8.0,
     "chirpmass_min": 20.00334330242407,
     "chirpmass_max": 64.74889565385021,
     "metadata": {
         "date": "2020-11-05 04:38:55.172784",
-        "command_line_args": "Namespace(HM=True, bounds_tol=0.2, dataset='C01:SEOBNRv4P', ell_max=3, f_ref=20.0, flow=20.0, json_file='test.json', nbins=50, q_min=None, report_file='test.pdf', samples_file='/home/zoheyr.doctor/public_html/O3/O3aCatalog/data_release/all_posterior_samples/GW190413_052954_comoving.h5', tolerance=2.0)"
+        "command_line_args": "Namespace(HM=True, bounds_tol=0.2, dataset='C01:IMRPhenomXPHM', ell_max=3, f_ref=20.0, flow=20.0, json_file='test.json', nbins=50, q_min=None, report_file='test.pdf', samples_file='./posterior_samples.h5', tolerance=2.0)"
     }
 ```
 
-An example of the generated report can be seen here:
-
-https://ldas-jobs.ligo.caltech.edu/~serguei.ossokine/LVC/O3b_settings/test.html
-
-It is recommended that the report is reviewed carefully before the settings are approved.
+An `html` report will also be generated.
 
 ### Running on many events
 To run on many events, a separate script, `run_on_many_events.py` is provided. The most important settings to it are the path to the repo containing the superevents (specified via `--repo`) and a json file containing the names of events to run on and the corresponding preferred data set inside the PEsummary metafile (specified via `--run_map`). An example of such a json file is below:
 ```json
 {
-    "S191105e":"EXP1",
-    "S191129u":"EXP4"
+    "S150914":"EXP1",
+    "S190521":"EXP4"
 }
 ```
 Here is an example of calling the script:
 ```bash
-python  run_on_many_events.py --repo /home/gareth.davies/git_repos/o3b_catalog_events/ --run_map ../test_run_map.json --json_output --full_reports --output_dir example
+python  run_on_many_events.py --repo ./my_events/ --run_map ../test_run_map.json --json_output --full_reports --output_dir example
 ```
-With these options, a separate directory will be created for each superevent inside the `example` directory. Inside each directory there will be 4 files, corresponding to the raw log (ending in `.log`), the machine readable json file with recommended settings (ending in `.json`), and 2 files corresponding to a more verbose report (ending with `.ipynb` and `.html`). The `html` report is the exectued and rendered version of the `ipynb` file, provided for debugging purposes. 
+With these options, a separate directory will be created for each superevent inside the `example` directory. Inside each directory there will be 4 files, corresponding to the raw log (ending in `.log`), the machine readable json file with recommended settings (ending in `.json`), and 2 files corresponding to a more verbose report (ending with `.ipynb` and `.html`). The `html` report is the executed and rendered version of the `ipynb` file, provided for debugging purposes.
 
-An example of the directory and output can be found here:
-https://ldas-jobs.ligo.caltech.edu/~serguei.ossokine/LVC/O3b_settings/full_test/
+Examples can be found in `example` folder.
 
 
 ### Detailed description of internal logic
 This section describes the detailed logic used in deciding the various settings.  Many of these settings depend on the masses of the binary and are thus affected by proposed changes to the chirp mass prior which is described below.  For every setting we generate 2 estimates: one coming directly from the samples and a conservative one, which takes into account the wider chirp mass prior. In particular,  the following strategy is adopted:
 
 1. Estimate the quantity of interest from the samples.
 2. Pick the most extreme value of the quantity of interest (e.g. max seglen or min $f_{\rm start}$) and find its parameters (mass ratio and spins)
 3. Use either the lower or upper proposed chirp mass bounds (as appropriate) and the mass ratio from step 2 to estimate a new total mass
 4. Use this total mass along with the other params (as appropriate) to produce a new estimate of the quantity of interest
 
 
 
 #### Deciding the chirp mass bounds for the prior
-The script suggests a chirp mass prior that is wider than the minimum and maximum chirp masses found in the samples, to guard against the moving around of the posterior due to e.g. using a different waveform model. 
+The script suggests a chirp mass prior that is wider than the minimum and maximum chirp masses found in the samples, to guard against the moving around of the posterior due to e.g. using a different waveform model.
 
 The script proposes chirp mass bounds in 2 steps:
 1. Given the preliminary PE run, it checks of railing is present in the chirp mass posterior. This process involves a couple of free parameters that control how strict this check is. This is governed by the options `--tolerance` and `nbins`. See `-h` for more details.
-2. If no railing is found, the proposed bounds are given by $`[(1-f)\mathcal{M}_{\rm min},(1+f)\mathcal{M}_{\rm max}]`$ where $`f`$ is a free parameter, given by the option `--bounds_tol` with the default value of **0.2**.
+2. If no railing is found, the proposed bounds are computed depending on the width of the chirp mass posterior $`\Delta\mathcal{M}=\mathcal{M}_{\rm max}-\mathcal{M}_{\rm min}`$. If the width is greater than $`30M_{\otol}`$, then the proposed bounds are given by $`[(1-f)\mathcal{M}_{\rm min},(1+f)\mathcal{M}_{\rm max}]`$ where $`f`$ is a free parameter, given by the option `--bounds_tol` with the default value of **0.2**. If the width is smaller than $`30M_{\otol}`$, then the bound are given by $`[\mathcal{M}_{\rm min}-f\Delta\mathcal{M},\mathcal{M}_{\rm max}+f\Delta\mathcal{M}f]`$.
 
 
 #### Deciding the sampling rate
-The sampling rate is determined by the requirement that it's high enough to resolve the highest frequency we are interested in. This is generally given by the frequency of the highest $`(\ell,m)`$ mode in the ringdown. This is estimated by using the `SEOBNRv4HM` routines.  The user is given control which $`\ell`$ is used for this Nyquist frequency check via the option `--ell-max`. By default it is set to **3**.  To be precise, the sampling rate is computed as $`2f_{\rm max}`$ and then rounded up to the next power of 2. 
+The sampling rate is determined by the requirement that it's high enough to resolve the highest frequency we are interested in. This is generally given by the frequency of the highest $`(\ell,m)`$ mode in the ringdown. This is estimated by using the `SEOBNRv4HM` routines.  The user is given control which $`\ell`$ is used for this Nyquist frequency check via the option `--ell-max`. By default it is set to **3**.  To be precise, the sampling rate is computed as $`2f_{\rm max}`$ and then rounded up to the next power of 2.
 
 #### Deciding the starting frequency
-The starting frequency determines the length of the generated waveform. For `SEOBNR` time-domain family of waveforms there are two considerations that come into play:
-1. The starting frequency (which corresponds to the frequency of the (2,2) mode) has to be such that the desired $`(\ell,m)`$ mode is present at the provided `flow` (which gives the lower bound of the likelihood integral and is an argument supplied by the user, set by default to **20 Hz**). The script uses the PN relation (valid in the inspiral) that $`f_{\ell m}=\frac{m}{2}f_{22}`$ to dermine this. _In principle, this consideration applies to any time-domain waveform._
-2. The starting frequency is not too close to merger. This is a limitation of the `SEOBNR` time domain waveforms due to the need i) for a long enough inspiral to attach ringdown ii) to generate quasi-circular initial conditions. The script uses the same condition as the waveform model internally to check if the starting frequency is below this frequency limit. 
+The starting frequency determines the length of the generated waveform. For time-domain family of waveforms there are two considerations that may come into play:
+1. The starting frequency (which corresponds to the frequency of the (2,2) mode) has to be such that the desired $`(\ell,m)`$ mode is present at the provided `flow` (which gives the lower bound of the likelihood integral and is an argument supplied by the user, set by default to **20 Hz**). The script uses the PN relation (valid in the inspiral) that $`f_{\ell m}=\frac{m}{2}f_{22}`$ to dermine this. _In principle, this consideration applies to any time-domain waveform, but need not be used for frequency-domain waveforms_
+2. The starting frequency is not too close to merger. This is a limitation of the `SEOBNR` time domain waveforms due to the need i) for a long enough inspiral to attach ringdown ii) to generate quasi-circular initial conditions. The script uses the same condition as the waveform model internally to check if the starting frequency is below this frequency limit.
 
 #### Deciding the seglen
 The raw segment length is determined by the following formula
 $`t = T(1+s)+t_{\rm pad}+t_{\rm rollon}`$, where $`T`$ is an estimate of the duration of the waveform, including inspiral, merger and ringdown; $`s`$ is a safety factor (default value of 0.03), $`t_{\rm pad}`$ is padding (default is 2 seconds) and $`t_{\rm rollon}`$ is the Tukey window roll on duration (default is 0.4 seconds).  The duration $`T`$ is taken to be a function of the 2 component masses $`m_{i}`$, the z-components of the dimensionless spin $`\chi_{i}`$ and of course the low frequency cutoff `flow` and computed using the SEOBNRv4_ROM function.  *Notice that this means explicitly that we only care about the duration of the waveform from `flow` onwards and not from `f_start`*.   Finally the seglen is rounded to the next power of 2.
 
 
 #### Checking the reference frequency
-The reference frequency is an **input** parameter, encoded in the option `--f_ref` with a default value of **20 Hz**. The script then computes the MECO frequency for all the samples, and checks that $`f_{\rm ref}\leq 0.97f_{\rm MECO}`$. If not, a message is printed out and even if specified a `json` report is **not** generated.  **Note that the script does not provide a recommendation for the reference frequency as this should be guided by physics.**
-
-Note that the failing of any railing checks and the reference frequency check can be ignored by passing the flag `--override_safeties`. 
-
-
-
-
-
-
-
-
+The reference frequency is an **input** parameter, encoded in the option `--f_ref` with a default value of **20 Hz**. The script then computes the MECO frequency for all the samples, and checks that $`f_{\rm ref}\leq 0.97f_{\rm MECO}`$. If not, a message is printed out and $`f_{\rm ref}`$ is overwritten to be $`0.97f_{\rm MECO}`$ (or $`f_{\rm start}`$ if this is greater).
 
+**Note that the failing of any railing checks and the reference frequency check can be ignored by passing the flag `--override_safeties`.**
```

### Comparing `pe-configurator-0.1.0/data/calibration_files.txt` & `pe-configurator-0.1.1/data/calibration_files.txt`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.0/examples/.DS_Store` & `pe-configurator-0.1.1/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.0/examples/test_GW190412/test.html` & `pe-configurator-0.1.1/examples/test_GW190412/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.0/examples/test_GW190412/test.json` & `pe-configurator-0.1.1/examples/test_GW190412/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.0/examples/test_GW190412/test.pdf` & `pe-configurator-0.1.1/examples/test_GW190412/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.0/examples/test_GW190521/test.html` & `pe-configurator-0.1.1/examples/test_GW190521/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.0/examples/test_GW190521/test.json` & `pe-configurator-0.1.1/examples/test_GW190521/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.0/examples/test_GW190521/test.pdf` & `pe-configurator-0.1.1/examples/test_GW190521/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.0/examples/test_GW190814/test.html` & `pe-configurator-0.1.1/examples/test_GW190814/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.0/examples/test_GW190814/test.json` & `pe-configurator-0.1.1/examples/test_GW190814/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.0/examples/test_GW190814/test.pdf` & `pe-configurator-0.1.1/examples/test_GW190814/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.0/examples/test_GW191109/test.html` & `pe-configurator-0.1.1/examples/test_GW191109/test.html`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.0/examples/test_GW191109/test.json` & `pe-configurator-0.1.1/examples/test_GW191109/test.json`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.0/examples/test_GW191109/test.pdf` & `pe-configurator-0.1.1/examples/test_GW191109/test.pdf`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.0/pe_configurator.egg-info/PKG-INFO` & `pe-configurator-0.1.1/pe_configurator.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 Metadata-Version: 2.1
 Name: pe-configurator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools to identify waveform settings and prior bounds for gravitational wave parameter estimation.
 Author-email: Hector Estelles <hector.estelles@ligo.org>, Serguei Ossokine <serguei.ossokine@ligo.org>, Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/pe/get_eob_settings
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: asimov
 
 # Introduction
-In this repo we provide scripts that automatically try to determine some
-settings that must be applied for time domain EOB waveforms to run. 
+This package provides scripts that automatically try to determine some settings that must be applied for PE runs, especially for time-domain waveforms.
+The settings try to strike a balance between being conservative and being feasible.
 
 ### Top-level description
-The main script to use is `proc_samples.py`.  Given a preliminary PE run, it will perform some basic checks and then generate recommended PE settings. It can also optionally generate a `json` format result for automatic ingestion by the robot and a more detailed standalone report (still under construction). 
-
-NB: the script is intended to be used for "vanilla" BBH events. 
+The main script to use is `proc_samples.py`.  Given a preliminary PE run, it will perform some basic checks and then generate recommended PE settings. It can also optionally generate a `json` format result for automatic ingestion by `asimov` and a more detailed standalone, human-readable report. Users are _highly_ encouraged to take a look at the report.
 
 ### Usage
 Here is a typical usage example:
 ```
-peconfigurator --HM /home/zoheyr.doctor/public_html/O3/O3aCatalog/data_release/all_posterior_samples/GW190413_052954_comoving.h5  --dataset C01:SEOBNRv4P --json_file test.json --report_file test.pdf
+peconfigurator --HM posterior_samples.h5  --dataset C01:IMRPhenomXPHM --json_file test.json --report_file test.pdf
 ```
 
 For all the available options, please check
 ```
 peconfigurator -h
 ```
 
-If all goes right it will print something like 
+If all goes right, it will print something like
 ```
 Processing....
 Estimating seglen based on posterior samples
 100%|███████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 10885/10885 [02:22<00:00, 76.48it/s]
 Estimating srate based on posterior samples
 Using ell = 3 for Nyquist check
 100%|████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████████| 10885/10885 [00:00<00:00, 30557.61it/s]
@@ -63,98 +61,83 @@
 Checking that f_ref is not above f_MECO: PASSED
 
 ++++++++++++++++++++++++++++++ Suggested settings ++++++++++++++++++++++++++++++
 Real required srate  753.7701187444659, as power of 2: 1024
 Real seglen: 4.046571094240219, with padding+rollon: 6.44657109424022, as power of 2: 8.0
 Check from samples:
 Real seglen: 0.8090184427276651, with padding+rollon: 3.209018442727665, as power of 2: 4.0
-f_start: 13.333333333333334, as amp_order: 1
+f_start: 13.333333333333334
 Real bounds on chirp mass: [25.004179128030085,53.95741304487518], suggested bounds: [20.00334330242407,64.74889565385021]
 Real distance max: 8000.0
 
 ```
 
 The `test.json` file contains some machine-readable information as shown below:
 
 ```json
 {
     "srate": 1024,
     "f_start": 13.333333333333334,
     "f_ref": 20.0,
-    "amp_order": 1,
     "seglen": 8.0,
     "chirpmass_min": 20.00334330242407,
     "chirpmass_max": 64.74889565385021,
     "metadata": {
         "date": "2020-11-05 04:38:55.172784",
-        "command_line_args": "Namespace(HM=True, bounds_tol=0.2, dataset='C01:SEOBNRv4P', ell_max=3, f_ref=20.0, flow=20.0, json_file='test.json', nbins=50, q_min=None, report_file='test.pdf', samples_file='/home/zoheyr.doctor/public_html/O3/O3aCatalog/data_release/all_posterior_samples/GW190413_052954_comoving.h5', tolerance=2.0)"
+        "command_line_args": "Namespace(HM=True, bounds_tol=0.2, dataset='C01:IMRPhenomXPHM', ell_max=3, f_ref=20.0, flow=20.0, json_file='test.json', nbins=50, q_min=None, report_file='test.pdf', samples_file='./posterior_samples.h5', tolerance=2.0)"
     }
 ```
 
-An example of the generated report can be seen here:
-
-https://ldas-jobs.ligo.caltech.edu/~serguei.ossokine/LVC/O3b_settings/test.html
-
-It is recommended that the report is reviewed carefully before the settings are approved.
+An `html` report will also be generated.
 
 ### Running on many events
 To run on many events, a separate script, `run_on_many_events.py` is provided. The most important settings to it are the path to the repo containing the superevents (specified via `--repo`) and a json file containing the names of events to run on and the corresponding preferred data set inside the PEsummary metafile (specified via `--run_map`). An example of such a json file is below:
 ```json
 {
-    "S191105e":"EXP1",
-    "S191129u":"EXP4"
+    "S150914":"EXP1",
+    "S190521":"EXP4"
 }
 ```
 Here is an example of calling the script:
 ```bash
-python  run_on_many_events.py --repo /home/gareth.davies/git_repos/o3b_catalog_events/ --run_map ../test_run_map.json --json_output --full_reports --output_dir example
+python  run_on_many_events.py --repo ./my_events/ --run_map ../test_run_map.json --json_output --full_reports --output_dir example
 ```
-With these options, a separate directory will be created for each superevent inside the `example` directory. Inside each directory there will be 4 files, corresponding to the raw log (ending in `.log`), the machine readable json file with recommended settings (ending in `.json`), and 2 files corresponding to a more verbose report (ending with `.ipynb` and `.html`). The `html` report is the exectued and rendered version of the `ipynb` file, provided for debugging purposes. 
+With these options, a separate directory will be created for each superevent inside the `example` directory. Inside each directory there will be 4 files, corresponding to the raw log (ending in `.log`), the machine readable json file with recommended settings (ending in `.json`), and 2 files corresponding to a more verbose report (ending with `.ipynb` and `.html`). The `html` report is the executed and rendered version of the `ipynb` file, provided for debugging purposes.
 
-An example of the directory and output can be found here:
-https://ldas-jobs.ligo.caltech.edu/~serguei.ossokine/LVC/O3b_settings/full_test/
+Examples can be found in `example` folder.
 
 
 ### Detailed description of internal logic
 This section describes the detailed logic used in deciding the various settings.  Many of these settings depend on the masses of the binary and are thus affected by proposed changes to the chirp mass prior which is described below.  For every setting we generate 2 estimates: one coming directly from the samples and a conservative one, which takes into account the wider chirp mass prior. In particular,  the following strategy is adopted:
 
 1. Estimate the quantity of interest from the samples.
 2. Pick the most extreme value of the quantity of interest (e.g. max seglen or min $f_{\rm start}$) and find its parameters (mass ratio and spins)
 3. Use either the lower or upper proposed chirp mass bounds (as appropriate) and the mass ratio from step 2 to estimate a new total mass
 4. Use this total mass along with the other params (as appropriate) to produce a new estimate of the quantity of interest
 
 
 
 #### Deciding the chirp mass bounds for the prior
-The script suggests a chirp mass prior that is wider than the minimum and maximum chirp masses found in the samples, to guard against the moving around of the posterior due to e.g. using a different waveform model. 
+The script suggests a chirp mass prior that is wider than the minimum and maximum chirp masses found in the samples, to guard against the moving around of the posterior due to e.g. using a different waveform model.
 
 The script proposes chirp mass bounds in 2 steps:
 1. Given the preliminary PE run, it checks of railing is present in the chirp mass posterior. This process involves a couple of free parameters that control how strict this check is. This is governed by the options `--tolerance` and `nbins`. See `-h` for more details.
-2. If no railing is found, the proposed bounds are given by $`[(1-f)\mathcal{M}_{\rm min},(1+f)\mathcal{M}_{\rm max}]`$ where $`f`$ is a free parameter, given by the option `--bounds_tol` with the default value of **0.2**.
+2. If no railing is found, the proposed bounds are computed depending on the width of the chirp mass posterior $`\Delta\mathcal{M}=\mathcal{M}_{\rm max}-\mathcal{M}_{\rm min}`$. If the width is greater than $`30M_{\otol}`$, then the proposed bounds are given by $`[(1-f)\mathcal{M}_{\rm min},(1+f)\mathcal{M}_{\rm max}]`$ where $`f`$ is a free parameter, given by the option `--bounds_tol` with the default value of **0.2**. If the width is smaller than $`30M_{\otol}`$, then the bound are given by $`[\mathcal{M}_{\rm min}-f\Delta\mathcal{M},\mathcal{M}_{\rm max}+f\Delta\mathcal{M}f]`$.
 
 
 #### Deciding the sampling rate
-The sampling rate is determined by the requirement that it's high enough to resolve the highest frequency we are interested in. This is generally given by the frequency of the highest $`(\ell,m)`$ mode in the ringdown. This is estimated by using the `SEOBNRv4HM` routines.  The user is given control which $`\ell`$ is used for this Nyquist frequency check via the option `--ell-max`. By default it is set to **3**.  To be precise, the sampling rate is computed as $`2f_{\rm max}`$ and then rounded up to the next power of 2. 
+The sampling rate is determined by the requirement that it's high enough to resolve the highest frequency we are interested in. This is generally given by the frequency of the highest $`(\ell,m)`$ mode in the ringdown. This is estimated by using the `SEOBNRv4HM` routines.  The user is given control which $`\ell`$ is used for this Nyquist frequency check via the option `--ell-max`. By default it is set to **3**.  To be precise, the sampling rate is computed as $`2f_{\rm max}`$ and then rounded up to the next power of 2.
 
 #### Deciding the starting frequency
-The starting frequency determines the length of the generated waveform. For `SEOBNR` time-domain family of waveforms there are two considerations that come into play:
-1. The starting frequency (which corresponds to the frequency of the (2,2) mode) has to be such that the desired $`(\ell,m)`$ mode is present at the provided `flow` (which gives the lower bound of the likelihood integral and is an argument supplied by the user, set by default to **20 Hz**). The script uses the PN relation (valid in the inspiral) that $`f_{\ell m}=\frac{m}{2}f_{22}`$ to dermine this. _In principle, this consideration applies to any time-domain waveform._
-2. The starting frequency is not too close to merger. This is a limitation of the `SEOBNR` time domain waveforms due to the need i) for a long enough inspiral to attach ringdown ii) to generate quasi-circular initial conditions. The script uses the same condition as the waveform model internally to check if the starting frequency is below this frequency limit. 
+The starting frequency determines the length of the generated waveform. For time-domain family of waveforms there are two considerations that may come into play:
+1. The starting frequency (which corresponds to the frequency of the (2,2) mode) has to be such that the desired $`(\ell,m)`$ mode is present at the provided `flow` (which gives the lower bound of the likelihood integral and is an argument supplied by the user, set by default to **20 Hz**). The script uses the PN relation (valid in the inspiral) that $`f_{\ell m}=\frac{m}{2}f_{22}`$ to dermine this. _In principle, this consideration applies to any time-domain waveform, but need not be used for frequency-domain waveforms_
+2. The starting frequency is not too close to merger. This is a limitation of the `SEOBNR` time domain waveforms due to the need i) for a long enough inspiral to attach ringdown ii) to generate quasi-circular initial conditions. The script uses the same condition as the waveform model internally to check if the starting frequency is below this frequency limit.
 
 #### Deciding the seglen
 The raw segment length is determined by the following formula
 $`t = T(1+s)+t_{\rm pad}+t_{\rm rollon}`$, where $`T`$ is an estimate of the duration of the waveform, including inspiral, merger and ringdown; $`s`$ is a safety factor (default value of 0.03), $`t_{\rm pad}`$ is padding (default is 2 seconds) and $`t_{\rm rollon}`$ is the Tukey window roll on duration (default is 0.4 seconds).  The duration $`T`$ is taken to be a function of the 2 component masses $`m_{i}`$, the z-components of the dimensionless spin $`\chi_{i}`$ and of course the low frequency cutoff `flow` and computed using the SEOBNRv4_ROM function.  *Notice that this means explicitly that we only care about the duration of the waveform from `flow` onwards and not from `f_start`*.   Finally the seglen is rounded to the next power of 2.
 
 
 #### Checking the reference frequency
-The reference frequency is an **input** parameter, encoded in the option `--f_ref` with a default value of **20 Hz**. The script then computes the MECO frequency for all the samples, and checks that $`f_{\rm ref}\leq 0.97f_{\rm MECO}`$. If not, a message is printed out and even if specified a `json` report is **not** generated.  **Note that the script does not provide a recommendation for the reference frequency as this should be guided by physics.**
-
-Note that the failing of any railing checks and the reference frequency check can be ignored by passing the flag `--override_safeties`. 
-
-
-
-
-
-
-
-
+The reference frequency is an **input** parameter, encoded in the option `--f_ref` with a default value of **20 Hz**. The script then computes the MECO frequency for all the samples, and checks that $`f_{\rm ref}\leq 0.97f_{\rm MECO}`$. If not, a message is printed out and $`f_{\rm ref}`$ is overwritten to be $`0.97f_{\rm MECO}`$ (or $`f_{\rm start}`$ if this is greater).
 
+**Note that the failing of any railing checks and the reference frequency check can be ignored by passing the flag `--override_safeties`.**
```

### Comparing `pe-configurator-0.1.0/pe_configurator.egg-info/SOURCES.txt` & `pe-configurator-0.1.1/pe_configurator.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,18 +17,16 @@
 examples/test_GW191109/test.pdf
 pe_configurator.egg-info/PKG-INFO
 pe_configurator.egg-info/SOURCES.txt
 pe_configurator.egg-info/dependency_links.txt
 pe_configurator.egg-info/entry_points.txt
 pe_configurator.egg-info/requires.txt
 pe_configurator.egg-info/top_level.txt
-peconfigurator/O3b_run_map.json
 peconfigurator/asimov.py
 peconfigurator/asimov_template.yaml
-peconfigurator/get_EOB_settings.py
-peconfigurator/proc_event_repo.py
+peconfigurator/get_settings.py
 peconfigurator/proc_samples.py
 peconfigurator/run_on_many_events.py
 peconfigurator/auxiliary/__init__.py
 peconfigurator/auxiliary/make_report.py
 peconfigurator/auxiliary/run_analyzer.py
 tests/test_get_settings.py
```

### Comparing `pe-configurator-0.1.0/peconfigurator/asimov.py` & `pe-configurator-0.1.1/peconfigurator/asimov.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from asimov.utils import set_directory
 
 class AsimovPipeline(Pipeline):
     """
     An asimov pipeline for heron.
     """
     name = "peconfigurator"
-    config_template = importlib.resources.path("peconfigurator", "asimov_template.yaml")
+    config_template = os.path.join(os.path.dirname(__file__), "asimov_template.yaml")
+    #importlib.resources.path(__package__, "asimov_template.yaml")
     _pipeline_command = "peconfigurator"
 
 
     def _find_posterior(self):
         """
         Find the input posterior samples.
         """
@@ -43,15 +44,15 @@
         name = self.production.name
         ini = self.production.event.repository.find_prods(name,
                                                           self.category)[0]
 
         meta = self.production.meta
         executable = f"{os.path.join(config.get('pipelines', 'environment'), 'bin', self._pipeline_command)}"
         command = ["--dataset", f"{meta['dataset']}",
-                   "--json_file", os.path.join("results", "recommendations.json"),
+                   "--json_file", os.path.join(self.production.rundir, "results", "recommendations.json"),
 	           "--q-min", f"{meta['minimum mass ratio']}",
                    ]
         if "higher modes" in meta['checks']:
             command += ["--HM"]
         if "luminosity distance" in meta['checks']:
             command += ["--include_dL_recommendations"]
         if "no safety" in meta['checks']:
@@ -63,15 +64,20 @@
         
         description = {
             "executable": executable,
             "arguments": " ".join(command),
             "output": f"{name}.out",
             "error": f"{name}.err",
             "log": f"{name}.log",
+            "getenv": "True",
+            "request_memory": "4096 MB",
+            "request_disk": "100 MB",
             "batch_name": f"{self.name}/{self.production.event.name}/{name}",
+            "accounting_group_user": config.get('condor', 'user'),
+            "accounting_group": self.production.meta['scheduler']["accounting group"],
         }
 
         job = htcondor.Submit(description)
         os.makedirs(self.production.rundir, exist_ok=True)
         with set_directory(self.production.rundir):
             os.makedirs("results", exist_ok=True)
```

### Comparing `pe-configurator-0.1.0/peconfigurator/auxiliary/make_report.py` & `pe-configurator-0.1.1/peconfigurator/auxiliary/make_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,64 +1,44 @@
 # Copyright (C) 2020  Serguei Ossokine <cserguei.ossokine@ligo.org>
 # Based on pesummary file make_public.py by Charlie Hoy.
 
-from .run_analyzer import SNR_threshold, distance_checks, mass_ratio_checks
+from .run_analyzer import SNR_threshold, distance_checks, mass_ratio_checks, NS_check, spin_checks
 import datetime
 import hashlib
 import os
 import subprocess as sp
 
 import numpy as np
 import pandas as pd
+from importlib.metadata import version 
 from pesummary import __version__
 from pesummary.io import read
 #from run_analyzer import *
 from pesummary.core.notebook import (
     NoteBook,
     imports,
     pesummary_read,
     posterior_samples,
     samples_dict_plot,
 )
 
-
-def get_git_rev(fl=None):
-    origdir = os.getcwd()
-    if fl is None:
-        os.chdir(os.path.dirname(__file__))
-    else:
-        os.chdir(os.path.dirname(fl))
-
-    try:
-        git_rev = sp.check_output("git rev-parse HEAD", shell=True).strip().decode()
-    except sp.CalledProcessError:
-        git_rev = "N/A"
-    try:
-        sp.check_call("git diff --quiet", shell=True)
-        status = "CLEAN"
-    except sp.CalledProcessError:
-        status = "DIRTY"
-    os.chdir(origdir)
-    return f"{git_rev}__{status}"
-
-
 def md5(fname):
     hash_md5 = hashlib.md5()
     with open(fname, "rb") as f:
         hash_md5.update(f.read())
     return hash_md5.hexdigest()
 
 
-def markdown_table_writer_extra(date, git_hash, complete_args):
+def markdown_table_writer_extra(date, version, complete_args):
     """Write the extra metadata"""
     body = f"""
 |  |  |
 |--|--|
 |Date| {date}|
-|Script revision| {git_hash}|
+|Script revision| {version}|
 |Complete arguments | {complete_args}|
 """
     return body
 
 
 def markdown_writer_heuristics(samples):
     """Write the rules-based analysis out
@@ -139,16 +119,15 @@
     body = f"""
 **Data provenance**
 
 |  |  |
 |--|--|
 | PE summary file | {dc['samples_file']} |
 |  Data set       |  {dc['dataset']}     |
-| md5sum of file      |     {auxillary_vars['hash']}     |
-| git revision of data | {auxillary_vars['git_hash']} | 
+| md5sum of file      |     {auxillary_vars['hash']}     | 
 
 **Settings**
 
 | | |
 |--|--|
 """
     for i in range(len(input_settings_headers)):
@@ -196,16 +175,15 @@
             "are {}".format(analysis, pesummary_file, ", ".join(f.labels))
         )
     samples = f.samples_dict[analysis]
     # Header
     cell = f"# configurator report\n This notebook contains the automatic `configurator` report based on preliminary PE results.\n"
     nb.add_cell(cell, markdown=True)
 
-    git_hash_data = get_git_rev(fl=pesummary_file)
-    auxillary_vars = dict(hash=md5(pesummary_file), git_hash=git_hash_data)
+    auxillary_vars = dict(hash=md5(pesummary_file))
     # Config table
     config_table = make_config_table(args, auxillary_vars)
     nb.add_cell(config_table, markdown=True)
 
     # Imports (hidden)
     text, cell = imports(
         module_imports=["pesummary", "pesummary.io:read"],
@@ -354,14 +332,14 @@
 
     # The suggested settings
     nb.add_cell("## Recommended settings", markdown=True)
     settings = markdown_table_writer_settings(recommended_settings)
     nb.add_cell(settings, markdown=True)
 
     # Additional info
-    git_hash = get_git_rev()
+    script_version = version('pe-configurator')
     date = datetime.datetime.now()
     complete_args = str(args)
-    extra = markdown_table_writer_extra(date, git_hash, complete_args)
+    extra = markdown_table_writer_extra(date, script_version, complete_args)
     nb.add_cell("## Extra information", markdown=True)
     nb.add_cell(extra, markdown=True)
     nb.write(filename=filename, outdir=outdir)
```

### Comparing `pe-configurator-0.1.0/peconfigurator/auxiliary/run_analyzer.py` & `pe-configurator-0.1.1/peconfigurator/auxiliary/run_analyzer.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.0/peconfigurator/get_EOB_settings.py` & `pe-configurator-0.1.1/peconfigurator/get_settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,74 @@
 #!/usr/bin/env python
 import argparse
 import numpy as np
 import lal
 import lalsimulation as LS
 import click
+from typing import Tuple
 
 
-def MECO_freq(m_total, q, chi1z, chi2z):
+def MECO_freq(m_total: float, q: float, chi1z: float, chi2z: float) -> float:
+    """Compute an estimate of the MECO frequency. Uses IMRPhenomX
+    functions.
+
+    Args:
+        m_total (float): Total mass in solar masses
+        q (float): Mass ratio >=1
+        chi1z (float): Dimensionless spin of primary
+        chi2z (float): Dimensionless spin of secondary
+
+    Returns:
+        float: MECO frequency in Hz
+    """
     eta = q / (1.0 + q) ** 2
     fmeco_tmp = LS.SimIMRPhenomXfMECO(eta, chi1z, chi2z)
     fmeco = LS.SimIMRPhenomXUtilsMftoHz(fmeco_tmp, m_total)
     return fmeco
 
 
 def estimate_seglen(
-    fLow, m_total_min, safety_factor=0.03, q=5.0, chi1z=0.99, chi2z=0.99
-):
-
+    fLow: float,
+    m_total_min: float,
+    safety_factor: float = 0.03,
+    q: float = 5.0,
+    chi1z: float = 0.99,
+    chi2z: float = 0.99,
+) -> Tuple[float]:
+    """Estimate the required segment length. By default uses the SEOBNRv4ROM
+    function + some additional esimtate of the length of the ringdown. Assumes
+    a 0.4 second roll-on plus 2 second pad.
+    Also cross checks with IMRPhenomXAS.
+
+    Args:
+        fLow (float): The starting frequency to use for the length estimate
+        m_total_min (float): The total mass to use for length estimate
+        safety_factor (float, optional): Safety factor. Defaults to 0.03.
+        q (float, optional): Mass ratio >=1 to use of length estimate. Defaults to 5.0.
+        chi1z (float, optional): Dimensionless spin of the primary. Defaults to 0.99.
+        chi2z (float, optional): Dimensionsless spin of secondary. Defaults to 0.99.
+
+    Returns:
+        tuple: (length with no padding, length with padding, next power of 2)
+    """
     m1 = m_total_min * q / (1.0 + q) * lal.MSUN_SI
     m2 = m_total_min * 1.0 / (1.0 + q) * lal.MSUN_SI
     # Longest signal - aligned maximal spins
     s = LS.SimInspiralFinalBlackHoleSpinBound(chi1z, chi2z)
     tmerge = LS.SimInspiralMergeTimeBound(m1, m2) + LS.SimInspiralRingdownTimeBound(
         m1 + m2, s
     )
     wf_len = LS.SimIMRSEOBNRv4ROMTimeOfFrequency(fLow, m1, m2, chi1z, chi2z)
     wf_len_xas = LS.SimIMRPhenomXASDuration(m1, m2, chi1z, chi2z, fLow)
 
     # Check if SEOB and PhenomX prediction for duration differ more than 20%
-    if np.abs(wf_len-wf_len_xas)/wf_len > 0.2:
-        print(f"Warning: different waveform length estimation between SEOBNRv4={wf_len}s and IMRPhenomXAS={wf_len_xas}. Using longest one.")
+    if np.abs(wf_len - wf_len_xas) / wf_len > 0.2:
+        print(
+            f"Warning: different waveform length estimation between SEOBNRv4={wf_len}s and IMRPhenomXAS={wf_len_xas}. Using longest one."
+        )
         if wf_len_xas > wf_len:
             wf_len = wf_len_xas
 
     wf_len += tmerge
     # Make the waveform slightly longer just for safety
     safe_len = wf_len * (1.0 + safety_factor)
     full_len = safe_len + 2 + 0.4  # Padding and roll-on
@@ -41,16 +76,31 @@
     return safe_len, full_len, seglen
 
 
 def next_power_of_2(x):
     return 1 if x == 0 else 2 ** (x - 1).bit_length()
 
 
-def Get_freqQNM_SEOBNRv4HM_SI_units(q, mtot, chi1z, chi2z, lm):
-    # mtot must be in solar masses
+def Get_freqQNM_SEOBNRv4HM_SI_units(
+    q: float, mtot: float, chi1z: float, chi2z: float, lm: Tuple[int]
+) -> float:
+    """Compute the QNM frequency in Hz for the given binary and lm mode.
+    Uses SEOBNRv4 functions
+
+    Args:
+        q (float): Mass ratio >=1
+        mtot (float): Total mass in solar masses
+        chi1z (float): Dimensionless spin of primary
+        chi2z (float): Dimensionless spin of secondary
+        lm (Tuple[int]): (ell,m) of the mode
+
+    Returns:
+        float: real part of the QNM frequency in Hz
+    """
+
     # It first computes the QNM omega in geometric units and then it rescale it with the total mass
     M = 100.0  # will be ignored
     Ms = M * lal.MTSUN_SI
     m1 = M * q / (1 + q)
     m2 = M * 1 / (1 + q)
     complexQNM = lal.CreateCOMPLEX16Vector(1)
     LS.SimIMREOBGenerateQNMFreqV2(
@@ -63,15 +113,35 @@
         lm[1],
         1,
         LS.SEOBNRv4,
     )
     return Ms * np.real(complexQNM.data[0]) / (lal.MTSUN_SI * mtot * 2.0 * np.pi)
 
 
-def min_sampling_rate_EOB(mtot, q=2.0, chi1z=0.5, chi2z=0.5, HM=False, ell_max=3):
+def min_sampling_rate_EOB(
+    mtot: float,
+    q: float = 2.0,
+    chi1z: float = 0.5,
+    chi2z: float = 0.5,
+    HM: bool = False,
+    ell_max: int = 3,
+):
+    """Compute the sampling rate needed
+
+    Args:
+        mtot (float): Total mass in solar masses
+        q (float, optional): Mass ratio >=. Defaults to 2.0.
+        chi1z (float, optional): Dimensionless spin of primary. Defaults to 0.5.
+        chi2z (float, optional): Dimensionless spin of secondary. Defaults to 0.5.
+        HM (bool, optional): Use higher modes?. Defaults to False.
+        ell_max (int, optional): Which (l,m) to use to estimate QNM frequency. Defaults to 3.
+
+    Returns:
+        Union[float,float]: Sampling rate, next power of 2
+    """
     # mtot must be in solar masses
     if HM:
         fmax = Get_freqQNM_SEOBNRv4HM_SI_units(
             q, mtot, chi1z, chi2z, (ell_max, ell_max)
         )
     else:
         fmax = Get_freqQNM_SEOBNRv4HM_SI_units(q, mtot, chi1z, chi2z, (2, 2))
```

### Comparing `pe-configurator-0.1.0/peconfigurator/proc_samples.py` & `pe-configurator-0.1.1/peconfigurator/proc_samples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #!/usr/bin/env python3
 
 import argparse
 from copy import deepcopy
 import datetime
 import json
 import subprocess as sp
-import os
-import sys
 
 import click
 import numpy as np
 import pandas as pd
 from pesummary.gw.file.read import read
 from tqdm import tqdm
 
-from .get_EOB_settings import *
+from .get_settings import *
 from .auxiliary.make_report import make_report
 from .auxiliary.run_analyzer import railing_check
 
 # This script will iterate through a repository and check for a preferred run,
 # use that to determine the seglen, srate and amp-order for Production runs,
 # and Check the ini files for those
 
@@ -212,14 +210,15 @@
 
     eta_min = q_min / (1 + q_min) ** 2
 
     click.echo("Processing....")
     click.echo("Estimating seglen based on posterior samples")
 
     # seglen section
+    # Compute the seglen from the actual samples
     safelens, fulllens, seglens = zip(
         *[
             estimate_seglen(args.flow, mt, q=1.0 / qp, chi1z=s1z, chi2z=s2z)
             for mt, qp, s1z, s2z in tqdm(list(zip(mtot, q, chi1z, chi2z)))
         ]
     )
     nopad_len = np.max(safelens)
@@ -243,14 +242,15 @@
         chi1z=chi1z[idx_max],
         chi2z=chi2z[idx_max],
     )
 
     # seglen section ends
 
     # srate section
+    # Compute sampling rate from the samples
     click.echo("Estimating srate based on posterior samples")
     click.secho(f"Using ell = {args.ell_max} for Nyquist check", bold=True)
     real_srates, srates = zip(
         *[
             min_sampling_rate_EOB(
                 mt, q=1.0 / qp, HM=args.HM, chi1z=s1z, chi2z=s2z, ell_max=args.ell_max
             )
@@ -392,15 +392,15 @@
         click.secho(
             f"The reference frequency ({f_ref}) is too close to the new MECO frequency, {f_meco} Hz, overwritting reference frequency to f_ref=0.95*f_MECO",
             fg="red",
         )
         checks["f_ref"] = False
         f_ref = 0.95 * f_meco
         new_checks["f_ref"] = True
-    
+
     if f_ref < f_start:
         click.secho(
             f"The reference frequency ({f_ref}) is lower than the starting waveform generation frequency, {f_start} Hz, overwritting reference frequency to f_start.",
             fg="red",
         )
         checks["f_ref"] = False
         f_ref = f_start
@@ -417,15 +417,15 @@
     )
 
     click.echo("Check from samples:")
     click.echo(
         f"Real seglen: {nopad_len}, with padding+rollon: {np.max(fulllens)}, as power of 2: {max_seglen}"
     )
 
-    click.echo(f"f_start: {f_start}, as amp_order: {seobp_amporder}")
+    click.echo(f"f_start: {f_start}")
     click.echo(
         f"Real bounds on chirp mass: [{chirpmass_min},{chirpmass_max}], suggested bounds: [{chirpmass_min_bound},{chirpmass_max_bound}]"
     )
     click.echo(f"Real distance max: {dist_max}")
     recommended_settings = dict(
         srate=int(max_srate),
         f_start=f_start,
```

### Comparing `pe-configurator-0.1.0/peconfigurator/run_on_many_events.py` & `pe-configurator-0.1.1/peconfigurator/run_on_many_events.py`

 * *Files identical despite different names*

### Comparing `pe-configurator-0.1.0/pyproject.toml` & `pe-configurator-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -45,13 +45,14 @@
 [project.scripts]
 peconfigurator = "peconfigurator.proc_samples:main"
 
 [project.urls]
 "Source code" = "https://git.ligo.org/pe/get_eob_settings"
 
 [tool.setuptools]
+include-package-data = true
 packages = [
 	"peconfigurator",
 ]
 
 [project.entry-points.'asimov.pipelines']
-peconfigurator = 'peconfigurator.asimov:AsimovPipeline'
+peconfigurator = 'peconfigurator.asimov:AsimovPipeline'
```

### Comparing `pe-configurator-0.1.0/tests/test_get_settings.py` & `pe-configurator-0.1.1/tests/test_get_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 
 import numpy as np
+import os
 import pytest
-import sys
 import lal
 import lalsimulation as lalsim
 
-sys.path.append("../")
-from get_EOB_settings import (
+
+from peconfigurator.get_settings import (
     get_amp_order,
     estimate_seglen,
     min_sampling_rate_EOB,
     next_power_of_2,
 )
 
 
@@ -117,17 +117,20 @@
         (200, True, 5, [3, 8]),
     ],
 )
 def test_get_amp_order(m_total, HM, m_HM, expected):
     """"Check that the starting frequency and amp_order are as expected"""
     amp_order, f_start, _ = get_amp_order(m_total, HM=HM, m_HM=m_HM)
     assert amp_order == expected[0], "amp_order was not correct!"
-    assert np.allclose(f_start, expected[1],rtol=2e-2), "f_start was not correct!"
+    assert np.allclose(f_start, expected[1], rtol=2e-2), "f_start was not correct!"
 
 
+@pytest.mark.skipif(
+    "LAL_DATA_PATH" not in os.environ, reason="LAL_DATA_PATH not found",
+)
 @pytest.mark.parametrize(
     "m1,m2,chi1z,chi2z,flow",
     [
         (40.0, 20.0, 0.8, 0.8, 20.0),
         (40.0, 20.0, -0.99, -0.99, 20.0),
         (40.0, 20.0, 0.8, 0.8, 10.0),
         (80.0, 20.0, 0.99, -0.8, 10.0),
@@ -179,10 +182,7 @@
     assert np.allclose(
         raw_srate, raw_srate_check, rtol=0.1
     ), "Raw sampling rates are not the same!"
     print(f"raw = {raw_srate}, raw_check = {raw_srate_check}")
     print(f"srate = {srate}, srate_check = {srate_check}")
     assert np.allclose(srate, srate_check), "Final sampling rates are not the same!"
 
-
-def test_MECO_frequency():
-    pass
```


# Comparing `tmp/asimov-gwdata-0.1.0.tar.gz` & `tmp/asimov-gwdata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asimov-gwdata-0.1.0.tar", last modified: Fri Apr 14 09:59:27 2023, max compression
+gzip compressed data, was "asimov-gwdata-0.1.1.tar", last modified: Wed Apr 19 17:28:08 2023, max compression
```

## Comparing `asimov-gwdata-0.1.0.tar` & `asimov-gwdata-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:59:27.086194 asimov-gwdata-0.1.0/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      655 2023-04-14 09:59:27.086194 asimov-gwdata-0.1.0/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      148 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.0/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:59:27.086194 asimov-gwdata-0.1.0/asimov_gwdata.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      655 2023-04-14 09:59:27.000000 asimov-gwdata-0.1.0/asimov_gwdata.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      452 2023-04-14 09:59:27.000000 asimov-gwdata-0.1.0/asimov_gwdata.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-14 09:59:27.000000 asimov-gwdata-0.1.0/asimov_gwdata.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      104 2023-04-14 09:59:27.000000 asimov-gwdata-0.1.0/asimov_gwdata.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       45 2023-04-14 09:59:27.000000 asimov-gwdata-0.1.0/asimov_gwdata.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2023-04-14 09:59:27.000000 asimov-gwdata-0.1.0/asimov_gwdata.egg-info/top_level.txt
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:59:27.086194 asimov-gwdata-0.1.0/blueprints/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      168 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.0/blueprints/asimov-analysis.yaml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:59:27.086194 asimov-gwdata-0.1.0/datafind/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        5 2023-02-19 16:31:31.000000 asimov-gwdata-0.1.0/datafind/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5447 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.0/datafind/asimov.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1273 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.0/datafind/datafind_template.yml
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3349 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.0/datafind/main.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1037 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.0/pyproject.toml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-14 09:59:27.086194 asimov-gwdata-0.1.0/scripts/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      251 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.0/scripts/asimov-test-script.sh
--rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.0/scripts/test-calibration-dump.yaml
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-04-14 09:59:27.086194 asimov-gwdata-0.1.0/setup.cfg
--rw-r--r--   0 daniel    (1000) daniel    (1000)      122 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.0/test_settings.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:28:08.755037 asimov-gwdata-0.1.1/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      655 2023-04-19 17:28:08.755037 asimov-gwdata-0.1.1/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      148 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.1/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:28:08.755037 asimov-gwdata-0.1.1/asimov_gwdata.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      655 2023-04-19 17:28:08.000000 asimov-gwdata-0.1.1/asimov_gwdata.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      452 2023-04-19 17:28:08.000000 asimov-gwdata-0.1.1/asimov_gwdata.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-19 17:28:08.000000 asimov-gwdata-0.1.1/asimov_gwdata.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      104 2023-04-19 17:28:08.000000 asimov-gwdata-0.1.1/asimov_gwdata.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       45 2023-04-19 17:28:08.000000 asimov-gwdata-0.1.1/asimov_gwdata.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2023-04-19 17:28:08.000000 asimov-gwdata-0.1.1/asimov_gwdata.egg-info/top_level.txt
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:28:08.755037 asimov-gwdata-0.1.1/blueprints/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      168 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.1/blueprints/asimov-analysis.yaml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:28:08.755037 asimov-gwdata-0.1.1/datafind/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        5 2023-02-19 16:31:31.000000 asimov-gwdata-0.1.1/datafind/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5650 2023-04-19 17:27:01.000000 asimov-gwdata-0.1.1/datafind/asimov.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1273 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.1/datafind/datafind_template.yml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3349 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.1/datafind/main.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1037 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.1/pyproject.toml
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-04-19 17:28:08.755037 asimov-gwdata-0.1.1/scripts/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      251 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.1/scripts/asimov-test-script.sh
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      121 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.1/scripts/test-calibration-dump.yaml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-04-19 17:28:08.755037 asimov-gwdata-0.1.1/setup.cfg
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      122 2023-04-14 09:58:44.000000 asimov-gwdata-0.1.1/test_settings.yaml
```

### Comparing `asimov-gwdata-0.1.0/PKG-INFO` & `asimov-gwdata-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asimov-gwdata
-Version: 0.1.0
+Version: 0.1.1
 Summary: An asimov plugin to make downloading gravitational wave data easier
 Author-email: Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/asimov/asimov-gwdatahelp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asimov-gwdata-0.1.0/asimov_gwdata.egg-info/PKG-INFO` & `asimov-gwdata-0.1.1/asimov_gwdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asimov-gwdata
-Version: 0.1.0
+Version: 0.1.1
 Summary: An asimov plugin to make downloading gravitational wave data easier
 Author-email: Daniel Williams <daniel.williams@ligo.org>
 License: MIT
 Project-URL: Source code, https://git.ligo.org/asimov/asimov-gwdatahelp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `asimov-gwdata-0.1.0/datafind/asimov.py` & `asimov-gwdata-0.1.1/datafind/asimov.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         on the fly to prevent hard-coding things at any stage.
         """
         name = self.production.name
         ini = self.production.event.repository.find_prods(name, self.category)[0]
         with open(ini, "r") as config_file:
             data = config_file.read()
         data = data.replace("<event>", self.production.event.name)
-        data = data.replace("<gid>", self.production.event.meta['ligo']['gid'])
+        data = data.replace("<gid>", self.production.event.meta['ligo']['preferred event'])
         print(data)
         with open(ini, "w") as config_file:
             config_file.write(data)
         
     def build_dag(self, dryrun=False):
         """
         Create a condor submission description.
@@ -48,21 +48,24 @@
         executable = os.path.join(config.get('pipelines', 'environment'), 'bin', self._pipeline_command)
         command  = ["--settings", ini]
         full_command = executable + " " + " ".join(command)
         self.logger.info(full_command)
 
         description = {
             "executable": f"{executable}",
-            "arguments": f"{command}",
+            "arguments": f"{' '.join(command)}",
             "output": f"{name}.out",
             "error": f"{name}.err",
             "log": f"{name}.log",
             "request_disk": "1024",
             "request_memory": "1024",
             "batch_name": f"gwdata/{name}",
+            "accounting_group_user": config.get('condor', 'user'),
+            "accounting_group": self.production.meta['scheduler']["accounting group"],
+
         }
 
         job = htcondor.Submit(description)
         os.makedirs(self.production.rundir, exist_ok=True)
         with set_directory(self.production.rundir):
             with open(f"{name}.sub", "w") as subfile:
                 subfile.write(job.__str__())
@@ -78,14 +81,15 @@
             except configparser.NoOptionError:
                 schedulers = htcondor.Collector().locate(htcondor.DaemonTypes.Schedd)
             schedd = htcondor.Schedd(schedulers)
             with schedd.transaction() as txn:
                 cluster_id = job.queue(txn)
 
         self.production.job_id = int(cluster_id)
+        print(cluster_id)
         self.clusterid = cluster_id
 
     def submit_dag(self, dryrun=False):
         self.production.status = "running"
         self.production.job_id = int(self.clusterid)
         return self.clusterid
```

### Comparing `asimov-gwdata-0.1.0/datafind/datafind_template.yml` & `asimov-gwdata-0.1.1/datafind/datafind_template.yml`

 * *Files identical despite different names*

### Comparing `asimov-gwdata-0.1.0/datafind/main.py` & `asimov-gwdata-0.1.1/datafind/main.py`

 * *Files identical despite different names*

### Comparing `asimov-gwdata-0.1.0/pyproject.toml` & `asimov-gwdata-0.1.1/pyproject.toml`

 * *Files identical despite different names*


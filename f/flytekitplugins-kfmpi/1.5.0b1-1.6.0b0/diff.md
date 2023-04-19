# Comparing `tmp/flytekitplugins-kfmpi-1.5.0b1.tar.gz` & `tmp/flytekitplugins-kfmpi-1.6.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kfmpi-1.5.0b1.tar", last modified: Wed Mar 29 18:58:40 2023, max compression
+gzip compressed data, was "flytekitplugins-kfmpi-1.6.0b0.tar", last modified: Wed Apr 19 20:54:31 2023, max compression
```

## Comparing `flytekitplugins-kfmpi-1.5.0b1.tar` & `flytekitplugins-kfmpi-1.6.0b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:40.116243 flytekitplugins-kfmpi-1.5.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-29 18:58:40.116243 flytekitplugins-kfmpi-1.5.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-29 18:58:20.000000 flytekitplugins-kfmpi-1.5.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:40.116243 flytekitplugins-kfmpi-1.5.0b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:40.116243 flytekitplugins-kfmpi-1.5.0b1/flytekitplugins/kfmpi/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-29 18:58:20.000000 flytekitplugins-kfmpi-1.5.0b1/flytekitplugins/kfmpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-03-29 18:58:20.000000 flytekitplugins-kfmpi-1.5.0b1/flytekitplugins/kfmpi/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 18:58:40.116243 flytekitplugins-kfmpi-1.5.0b1/flytekitplugins_kfmpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-29 18:58:40.000000 flytekitplugins-kfmpi-1.5.0b1/flytekitplugins_kfmpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-29 18:58:40.000000 flytekitplugins-kfmpi-1.5.0b1/flytekitplugins_kfmpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 18:58:40.000000 flytekitplugins-kfmpi-1.5.0b1/flytekitplugins_kfmpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-29 18:58:40.000000 flytekitplugins-kfmpi-1.5.0b1/flytekitplugins_kfmpi.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-29 18:58:40.000000 flytekitplugins-kfmpi-1.5.0b1/flytekitplugins_kfmpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-29 18:58:40.000000 flytekitplugins-kfmpi-1.5.0b1/flytekitplugins_kfmpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 18:58:40.116243 flytekitplugins-kfmpi-1.5.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-29 18:58:35.000000 flytekitplugins-kfmpi-1.5.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:31.159097 flytekitplugins-kfmpi-1.6.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-19 20:54:31.159097 flytekitplugins-kfmpi-1.6.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-19 20:54:06.000000 flytekitplugins-kfmpi-1.6.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:31.159097 flytekitplugins-kfmpi-1.6.0b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:31.159097 flytekitplugins-kfmpi-1.6.0b0/flytekitplugins/kfmpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-19 20:54:06.000000 flytekitplugins-kfmpi-1.6.0b0/flytekitplugins/kfmpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-04-19 20:54:06.000000 flytekitplugins-kfmpi-1.6.0b0/flytekitplugins/kfmpi/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:54:31.159097 flytekitplugins-kfmpi-1.6.0b0/flytekitplugins_kfmpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-19 20:54:31.000000 flytekitplugins-kfmpi-1.6.0b0/flytekitplugins_kfmpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-19 20:54:31.000000 flytekitplugins-kfmpi-1.6.0b0/flytekitplugins_kfmpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:54:31.000000 flytekitplugins-kfmpi-1.6.0b0/flytekitplugins_kfmpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:31.000000 flytekitplugins-kfmpi-1.6.0b0/flytekitplugins_kfmpi.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-19 20:54:31.000000 flytekitplugins-kfmpi-1.6.0b0/flytekitplugins_kfmpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 20:54:31.000000 flytekitplugins-kfmpi-1.6.0b0/flytekitplugins_kfmpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:54:31.159097 flytekitplugins-kfmpi-1.6.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-19 20:54:25.000000 flytekitplugins-kfmpi-1.6.0b0/setup.py
```

### Comparing `flytekitplugins-kfmpi-1.5.0b1/PKG-INFO` & `flytekitplugins-kfmpi-1.6.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfmpi
-Version: 1.5.0b1
+Version: 1.6.0b0
 Summary: K8s based MPI plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfmpi-1.5.0b1/flytekitplugins/kfmpi/task.py` & `flytekitplugins-kfmpi-1.6.0b0/flytekitplugins/kfmpi/task.py`

 * *Files 20% similar despite different names*

```diff
@@ -129,9 +129,66 @@
             num_workers=self.task_config.num_workers,
             num_launcher_replicas=self.task_config.num_launcher_replicas,
             slots=self.task_config.slots,
         )
         return MessageToDict(job.to_flyte_idl())
 
 
+@dataclass
+class HorovodJob(object):
+    slots: int
+    num_launcher_replicas: int = 1
+    num_workers: int = 1
+
+
+class HorovodFunctionTask(MPIFunctionTask):
+    """
+    For more info, check out https://github.com/horovod/horovod
+    """
+
+    # Customize your setup here. Please ensure the cmd, path, volume, etc are available in the pod.
+    ssh_command = "/usr/sbin/sshd -De -f /home/jobuser/.sshd_config"
+    discovery_script_path = "/etc/mpi/discover_hosts.sh"
+
+    def __init__(self, task_config: HorovodJob, task_function: Callable, **kwargs):
+
+        super().__init__(
+            task_config=task_config,
+            task_function=task_function,
+            **kwargs,
+        )
+
+    def get_command(self, settings: SerializationSettings) -> List[str]:
+        cmd = super().get_command(settings)
+        mpi_cmd = self._get_horovod_prefix() + cmd
+        return mpi_cmd
+
+    def get_config(self, settings: SerializationSettings) -> Dict[str, str]:
+        config = super().get_config(settings)
+        return {**config, "worker_spec_command": self.ssh_command}
+
+    def _get_horovod_prefix(self) -> List[str]:
+        np = self.task_config.num_workers * self.task_config.slots
+        base_cmd = [
+            "horovodrun",
+            "-np",
+            f"{np}",
+            "--verbose",
+            "--log-level",
+            "INFO",
+            "--network-interface",
+            "eth0",
+            "--min-np",
+            f"{np}",
+            "--max-np",
+            f"{np}",
+            "--slots-per-host",
+            f"{self.task_config.slots}",
+            "--host-discovery-script",
+            self.discovery_script_path,
+        ]
+        return base_cmd
+
+
 # Register the MPI Plugin into the flytekit core plugin system
 TaskPlugins.register_pythontask_plugin(MPIJob, MPIFunctionTask)
+TaskPlugins.register_pythontask_plugin(HorovodJob, HorovodFunctionTask)
```

### Comparing `flytekitplugins-kfmpi-1.5.0b1/flytekitplugins_kfmpi.egg-info/PKG-INFO` & `flytekitplugins-kfmpi-1.6.0b0/flytekitplugins_kfmpi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfmpi
-Version: 1.5.0b1
+Version: 1.6.0b0
 Summary: K8s based MPI plugin for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfmpi-1.5.0b1/setup.py` & `flytekitplugins-kfmpi-1.6.0b0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "kfmpi"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "flyteidl>=0.21.4"]
 
-__version__ = "1.5.0b1"
+__version__ = "1.6.0b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based MPI plugin for flytekit",
```


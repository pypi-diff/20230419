# Comparing `tmp/gitlab-runner-tart-driver-0.1.1.tar.gz` & `tmp/gitlab-runner-tart-driver-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-runner-tart-driver-0.1.1.tar", last modified: Thu Apr 13 05:38:28 2023, max compression
+gzip compressed data, was "gitlab-runner-tart-driver-0.1.2.tar", last modified: Wed Apr 19 08:06:31 2023, max compression
```

## Comparing `gitlab-runner-tart-driver-0.1.1.tar` & `gitlab-runner-tart-driver-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 05:38:28.762127 gitlab-runner-tart-driver-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     3303 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    13625 2023-04-13 05:38:28.761127 gitlab-runner-tart-driver-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    13104 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 05:38:28.756127 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 05:38:28.759127 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/config.py
--rw-rw-rw-   0 root         (0) root         (0)     5787 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/prepare.py
--rw-rw-rw-   0 root         (0) root         (0)     3300 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 05:38:28.761127 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      996 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
--rw-rw-rw-   0 root         (0) root         (0)     5231 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/tart.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 05:38:28.758127 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13625 2023-04-13 05:38:28.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      986 2023-04-13 05:38:28.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 05:38:28.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-04-13 05:38:28.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 05:38:28.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-13 05:38:28.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-13 05:38:28.000000 gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 05:38:28.762127 gitlab-runner-tart-driver-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-13 05:38:17.000000 gitlab-runner-tart-driver-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:06:31.868012 gitlab-runner-tart-driver-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)     3303 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    14631 2023-04-19 08:06:31.868012 gitlab-runner-tart-driver-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    14110 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:06:31.862012 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:06:31.866012 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8981 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/prepare.py
+-rw-rw-rw-   0 root         (0) root         (0)     2145 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:06:31.867012 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6622 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/tart.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 08:06:31.864012 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14631 2023-04-19 08:06:31.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      986 2023-04-19 08:06:31.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 08:06:31.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-19 08:06:31.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 08:06:31.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-19 08:06:31.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-19 08:06:31.000000 gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 08:06:31.868012 gitlab-runner-tart-driver-0.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-04-19 08:06:20.000000 gitlab-runner-tart-driver-0.1.2/setup.py
```

### Comparing `gitlab-runner-tart-driver-0.1.1/LICENSE.txt` & `gitlab-runner-tart-driver-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.1/PKG-INFO` & `gitlab-runner-tart-driver-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
@@ -262,14 +262,24 @@
     run_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     run_args = [ "run", '-x', '/opt/homebrew/bin/tart' ]
 
     cleanup_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     cleanup_args = [ "cleanup", '-x', '/opt/homebrew/bin/tart' ]
 ```
 
+### Host Cache and Builds directories
+
+With `tart` it is possible to mount local directories into the VM. Mounting local directories brings a number of benefits like up tp 30% higher IO performance as well as a correct caching mechanism.
+To enable Host-local caching and builds, simply pass `--builds-dir` and `--cache-dir` to the `prepare` command
+
+```ini
+prepare_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
+prepare_args = [ "prepare", '-x', '/opt/homebrew/bin/tart', '--concurrency', '2', '--auto-resources', '--cache-dir', '/Users/gitlab/gitlab-runner/cache', '--builds-dir', '/Users/gitlab/gitlab-runner/builds']
+```
+
 ### Auto Host Resource Distribution
 
 `tart` images come with a pre-defined number of CPUs and Memory allocation. Typical numbers for default images are `cpu_count=4` and `memory=8192`. With the concurrency limitation of two VMs/images running at the same time this might not utilize your host system completely.
 Per default, `--auto-resources` is enable for the `gitlab-runner-tart-driver` which will split the host resources equally to the VMs defined by `--concurrency`. The default concurrency is `1` and therefore will assign all host resources to the VM.
 
 > **ATTENTION** make sure your `gitlab-runner` concurrency setting is the same as the `--concurrency` parameter you are passing to the `prepare` command
 
@@ -320,44 +330,50 @@
 
 ```
 Usage: gitlab-runner-tart-driver prepare [OPTIONS]
 
   Prepare the environment and start the tart VM.
 
 Options:
+  --default-ssh-username TEXT     username to login to a tart vm
+  --default-ssh-password TEXT     password to login to a tart vm
   --pull-policy [always|if-not-present|never]
                                   define how runners pull tart images from
                                   registries
   --registry-username TEXT        username to login to a oci registry
-  --registry-password TEXT        passowrd to login to a oci registry
+  --registry-password TEXT        password to login to a oci registry
   --registry TEXT                 username to login to a oci registry
   --cpu INTEGER                   Number of CPUs associated to VM
   --memory INTEGER                VM memory size in megabytes associated to VM
   --display TEXT                  VM display resolution in a format of
                                   <width>x<height>. For example, 1200x800
   --auto-resources / --no-auto-resources
                                   If enabled, the driver will divide system
                                   resources equally to the concurrent VMs.
   --concurrency INTEGER           Number of concurrent processes that are
                                   supported. ATTENTION tart currently only
                                   support two concurrent VMs
+  --cache-dir TEXT                Caching dir to be used.
+  --builds-dir TEXT               Path to the builds directory.
+  --timeout INTEGER               Timeout in seconds for the VM to be
+                                  reachable via SSH.
   -x, --tart-executable TEXT      Path to the tart executable.
   --help                          Show this message and exit.
 ```
 
 ### Command `run`
 
 ```
 Usage: gitlab-runner-tart-driver run [OPTIONS] SCRIPT STAGE
 
   Run commands.
 
 Options:
   --default-ssh-username TEXT  username to login to a tart vm
-  --default-ssh-password TEXT  passowrd to login to a tart vm
+  --default-ssh-password TEXT  password to login to a tart vm
   -x, --tart-executable TEXT   Path to the tart executable.
   --shell TEXT                 Path to the shell to be used for commands over
                                ssh.
   --help                       Show this message and exit.
 ```
 
 ### Command `cleanup`
```

### Comparing `gitlab-runner-tart-driver-0.1.1/README.md` & `gitlab-runner-tart-driver-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -247,14 +247,24 @@
     run_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     run_args = [ "run", '-x', '/opt/homebrew/bin/tart' ]
 
     cleanup_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     cleanup_args = [ "cleanup", '-x', '/opt/homebrew/bin/tart' ]
 ```
 
+### Host Cache and Builds directories
+
+With `tart` it is possible to mount local directories into the VM. Mounting local directories brings a number of benefits like up tp 30% higher IO performance as well as a correct caching mechanism.
+To enable Host-local caching and builds, simply pass `--builds-dir` and `--cache-dir` to the `prepare` command
+
+```ini
+prepare_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
+prepare_args = [ "prepare", '-x', '/opt/homebrew/bin/tart', '--concurrency', '2', '--auto-resources', '--cache-dir', '/Users/gitlab/gitlab-runner/cache', '--builds-dir', '/Users/gitlab/gitlab-runner/builds']
+```
+
 ### Auto Host Resource Distribution
 
 `tart` images come with a pre-defined number of CPUs and Memory allocation. Typical numbers for default images are `cpu_count=4` and `memory=8192`. With the concurrency limitation of two VMs/images running at the same time this might not utilize your host system completely.
 Per default, `--auto-resources` is enable for the `gitlab-runner-tart-driver` which will split the host resources equally to the VMs defined by `--concurrency`. The default concurrency is `1` and therefore will assign all host resources to the VM.
 
 > **ATTENTION** make sure your `gitlab-runner` concurrency setting is the same as the `--concurrency` parameter you are passing to the `prepare` command
 
@@ -305,44 +315,50 @@
 
 ```
 Usage: gitlab-runner-tart-driver prepare [OPTIONS]
 
   Prepare the environment and start the tart VM.
 
 Options:
+  --default-ssh-username TEXT     username to login to a tart vm
+  --default-ssh-password TEXT     password to login to a tart vm
   --pull-policy [always|if-not-present|never]
                                   define how runners pull tart images from
                                   registries
   --registry-username TEXT        username to login to a oci registry
-  --registry-password TEXT        passowrd to login to a oci registry
+  --registry-password TEXT        password to login to a oci registry
   --registry TEXT                 username to login to a oci registry
   --cpu INTEGER                   Number of CPUs associated to VM
   --memory INTEGER                VM memory size in megabytes associated to VM
   --display TEXT                  VM display resolution in a format of
                                   <width>x<height>. For example, 1200x800
   --auto-resources / --no-auto-resources
                                   If enabled, the driver will divide system
                                   resources equally to the concurrent VMs.
   --concurrency INTEGER           Number of concurrent processes that are
                                   supported. ATTENTION tart currently only
                                   support two concurrent VMs
+  --cache-dir TEXT                Caching dir to be used.
+  --builds-dir TEXT               Path to the builds directory.
+  --timeout INTEGER               Timeout in seconds for the VM to be
+                                  reachable via SSH.
   -x, --tart-executable TEXT      Path to the tart executable.
   --help                          Show this message and exit.
 ```
 
 ### Command `run`
 
 ```
 Usage: gitlab-runner-tart-driver run [OPTIONS] SCRIPT STAGE
 
   Run commands.
 
 Options:
   --default-ssh-username TEXT  username to login to a tart vm
-  --default-ssh-password TEXT  passowrd to login to a tart vm
+  --default-ssh-password TEXT  password to login to a tart vm
   -x, --tart-executable TEXT   Path to the tart executable.
   --shell TEXT                 Path to the shell to be used for commands over
                                ssh.
   --help                       Show this message and exit.
 ```
 
 ### Command `cleanup`
```

### Comparing `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/cli.py` & `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/cli.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/cleanup.py` & `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/cleanup.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/config.py` & `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 @click.command()
 def config():
     """Implementation of the CONFIG stage of the Custom Executor.
     Details on how to use this command can be found at
     https://docs.gitlab.com/runner/executors/custom.html#config."""
 
     c = GitLabCustomDriverConfig(
-        builds_dir="/Users/admin/build",
-        cache_dir="/Users/admin/cache",
+        builds_dir="/opt/builds",
+        cache_dir="/opt/cache",
         hostname=socket.gethostname(),
         driver=GitLabCustomDriver(name="tart", version=__version__),
     )
 
     click.echo(c.json(exclude_none=True))
```

### Comparing `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/commands/run.py` & `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/commands/run.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import os
 import sys
 
 import click
-from paramiko import MissingHostKeyPolicy
-from paramiko import SSHClient
 
 from gitlab_runner_tart_driver.modules.gitlab_custom_command_config import GitLabCustomCommandConfig
 from gitlab_runner_tart_driver.modules.tart import Tart
 
 
 @click.command()
 @click.option(
     "--default-ssh-username", default="admin", required=False, type=str, help="username to login to a tart vm"
 )
 @click.option(
-    "--default-ssh-password", default="admin", required=False, type=str, help="passowrd to login to a tart vm"
+    "--default-ssh-password", default="admin", required=False, type=str, help="password to login to a tart vm"
 )
 @click.option(
     "-x",
     "--tart-executable",
     required=False,
     default="tart",
     type=str,
@@ -46,50 +44,23 @@
     # Connect to VM
     ######################################################################
     tart = Tart(exec_path=tart_executable)
     tart_vm_name = p.vm_name()
     tart_ip = tart.ip(tart_vm_name, timeout=30)
     click.echo(f"[INFO] Establishing SSH conntection to '{p.tart_ssh_username}@{tart_ip}'")
 
-    ssh_client = SSHClient()
-    ssh_client.set_missing_host_key_policy(MissingHostKeyPolicy())
-    ssh_client.connect(tart_ip, username=p.tart_ssh_username, password=p.tart_ssh_password)
-
-    click.echo("[INFO] Preparing workspace'")
-    remote_build_dir = "/opt/build/"
-    remote_script_dir = "/opt/temp"
-    remote_cache_dir = "/opt/cache"
-    exec_ssh_command(
-        ssh_client,
-        f"sudo mkdir -p {remote_build_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_build_dir}",
-    )
-    exec_ssh_command(
-        ssh_client,
-        f"sudo mkdir -p {remote_script_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_script_dir}",
-    )
-    exec_ssh_command(
-        ssh_client,
-        f"sudo mkdir -p {remote_cache_dir} && sudo chown {p.tart_ssh_username}:{p.tart_ssh_username} {remote_cache_dir}",
-    )
+    ssh_session = tart.ssh_session(name=p.vm_name(), username=p.tart_ssh_username, password=p.tart_ssh_password)
+
+    click.echo("[INFO] Preparing workspace")
+    remote_temp_dir = "/opt/temp"
 
     script_name = os.path.basename(script)
-    remote_script_path = os.path.join(remote_script_dir, stage + "-" + script_name)
+    remote_script_path = os.path.join(remote_temp_dir, stage + "-" + script_name)
 
-    sftp = ssh_client.open_sftp()
+    sftp = ssh_session.ssh_client.open_sftp()
     sftp.put(script, remote_script_path)
     sftp.close()
 
-    exec_ssh_command(ssh_client, f"cd {remote_build_dir}")
-    script_exit_code = exec_ssh_command(ssh_client, f"{shell} -l {remote_script_path}", get_pty=True)
+    # ssh_session.exec_ssh_command(f"cd {remote_build_dir}")
+    script_exit_code = ssh_session.exec_ssh_command(f"{shell} -l {remote_script_path}", get_pty=True)
 
     sys.exit(script_exit_code)
-
-
-def exec_ssh_command(ssh_client, command, get_pty=True):
-    """Executes an ssh command and prints it's output continously to stdout/stderr"""
-    _, stdout, stderr = ssh_client.exec_command(command, get_pty=get_pty)
-    for line in iter(stdout.readline, ""):
-        click.echo(line, nl=False)
-    for line in iter(stderr.readline, ""):
-        click.echo(line, nl=False, err=True)
-
-    return stdout.channel.recv_exit_status()
```

### Comparing `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py` & `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 class GitLabCustomCommandConfig(BaseSettings):
     """Config parameters needed throughout the process read from the environment"""
 
     ci_job_image: str
     ci_pipeline_id: str
     ci_job_id: str
     ci_concurrent_id: str
+    ci_concurrent_project_id: str
+    ci_runner_short_token: str
     ci_project_name: str
     ci_registry: str
     ci_registry_user: str
     ci_registry_password: str
 
     tart_registry_username: Optional[str]
     tart_registry_password: Optional[str]
```

### Comparing `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/tart.py` & `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/tart.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+import os
 import re
 import subprocess
 
+import click
+from paramiko import MissingHostKeyPolicy
+from paramiko import SSHClient
 from pydantic import BaseModel
 from pydantic import Field
 from tabulate import tabulate
 
 
 class TartImage(BaseModel):
     source: str = Field()
@@ -18,14 +22,38 @@
     memory: int
     disk: int
     display: str
     running: bool
     ip_address: str
 
 
+class TartMount(BaseModel):
+    source: str
+    dest: str
+
+
+class TartSshSession:
+    def __init__(self, username, password, ip):
+        self.user = username
+        self.ip = ip
+        self.password = password
+        self.ssh_client = SSHClient()
+        self.ssh_client.set_missing_host_key_policy(MissingHostKeyPolicy())
+        self.ssh_client.connect(ip, username=username, password=password)
+
+    def exec_ssh_command(self, command, get_pty=True):
+        """Executes an ssh command and prints it's output continously to stdout/stderr"""
+        _, stdout, stderr = self.ssh_client.exec_command(command, get_pty=get_pty)
+        for line in iter(stdout.readline, ""):
+            click.echo(line, nl=False)
+        for line in iter(stderr.readline, ""):
+            click.echo(line, nl=False, err=True)
+        return stdout.channel.recv_exit_status()
+
+
 class Tart(object):
     def __init__(self, exec_path="tart"):
         self.tart_executable = exec_path
 
     def version(self) -> str:
         """Returns the tart version"""
         return self.exec(["--version"]).strip()
@@ -98,20 +126,24 @@
         ]
         print(tabulate(data, headers=["CPU", "Memory", "Disk", "Display", "Running", "IP Address"], tablefmt=tablefmt))
 
     def stop(self, name) -> None:
         """stops a given tart VM"""
         self.exec(["stop", name])
 
-    def run(self, name, no_graphics=True) -> None:
+    def run(self, name: str, dirs: list[TartMount] = [], no_graphics=True) -> None:
         """starts a given tart VM"""
         args = ["run", name]
         if no_graphics:
             args.append("--no-graphics")
 
+        if dirs:
+            for d in dirs:
+                args.extend(["--dir", f"{d.dest}:{os.path.abspath(os.path.expanduser(d.source))}"])
+
         try:
             self.spawn_exec(args)
         except Exception as e:
             print(f"Error when running VM {name}")
             raise e
 
     def ip(self, name, timeout=30, resolver="dhcp") -> str:
@@ -153,7 +185,14 @@
 
     def spawn_exec(self, cmd):
         """Spawns a new main process using 'nohup'"""
         exec_cmd = ["nohup", self.tart_executable]
         if cmd:
             exec_cmd.extend(cmd)
         subprocess.Popen(exec_cmd, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+
+    def ssh_session(self, name, username, password) -> TartSshSession:
+        ip = self.ip(name=name)
+        if not ip:
+            raise ValueError("Could not retrievew IP")
+
+        return TartSshSession(ip=ip, username=username, password=password)
```

### Comparing `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver/modules/utils.py` & `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver/modules/utils.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/PKG-INFO` & `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
@@ -262,14 +262,24 @@
     run_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     run_args = [ "run", '-x', '/opt/homebrew/bin/tart' ]
 
     cleanup_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
     cleanup_args = [ "cleanup", '-x', '/opt/homebrew/bin/tart' ]
 ```
 
+### Host Cache and Builds directories
+
+With `tart` it is possible to mount local directories into the VM. Mounting local directories brings a number of benefits like up tp 30% higher IO performance as well as a correct caching mechanism.
+To enable Host-local caching and builds, simply pass `--builds-dir` and `--cache-dir` to the `prepare` command
+
+```ini
+prepare_exec = "/opt/homebrew/bin/gitlab-runner-tart-driver"
+prepare_args = [ "prepare", '-x', '/opt/homebrew/bin/tart', '--concurrency', '2', '--auto-resources', '--cache-dir', '/Users/gitlab/gitlab-runner/cache', '--builds-dir', '/Users/gitlab/gitlab-runner/builds']
+```
+
 ### Auto Host Resource Distribution
 
 `tart` images come with a pre-defined number of CPUs and Memory allocation. Typical numbers for default images are `cpu_count=4` and `memory=8192`. With the concurrency limitation of two VMs/images running at the same time this might not utilize your host system completely.
 Per default, `--auto-resources` is enable for the `gitlab-runner-tart-driver` which will split the host resources equally to the VMs defined by `--concurrency`. The default concurrency is `1` and therefore will assign all host resources to the VM.
 
 > **ATTENTION** make sure your `gitlab-runner` concurrency setting is the same as the `--concurrency` parameter you are passing to the `prepare` command
 
@@ -320,44 +330,50 @@
 
 ```
 Usage: gitlab-runner-tart-driver prepare [OPTIONS]
 
   Prepare the environment and start the tart VM.
 
 Options:
+  --default-ssh-username TEXT     username to login to a tart vm
+  --default-ssh-password TEXT     password to login to a tart vm
   --pull-policy [always|if-not-present|never]
                                   define how runners pull tart images from
                                   registries
   --registry-username TEXT        username to login to a oci registry
-  --registry-password TEXT        passowrd to login to a oci registry
+  --registry-password TEXT        password to login to a oci registry
   --registry TEXT                 username to login to a oci registry
   --cpu INTEGER                   Number of CPUs associated to VM
   --memory INTEGER                VM memory size in megabytes associated to VM
   --display TEXT                  VM display resolution in a format of
                                   <width>x<height>. For example, 1200x800
   --auto-resources / --no-auto-resources
                                   If enabled, the driver will divide system
                                   resources equally to the concurrent VMs.
   --concurrency INTEGER           Number of concurrent processes that are
                                   supported. ATTENTION tart currently only
                                   support two concurrent VMs
+  --cache-dir TEXT                Caching dir to be used.
+  --builds-dir TEXT               Path to the builds directory.
+  --timeout INTEGER               Timeout in seconds for the VM to be
+                                  reachable via SSH.
   -x, --tart-executable TEXT      Path to the tart executable.
   --help                          Show this message and exit.
 ```
 
 ### Command `run`
 
 ```
 Usage: gitlab-runner-tart-driver run [OPTIONS] SCRIPT STAGE
 
   Run commands.
 
 Options:
   --default-ssh-username TEXT  username to login to a tart vm
-  --default-ssh-password TEXT  passowrd to login to a tart vm
+  --default-ssh-password TEXT  password to login to a tart vm
   -x, --tart-executable TEXT   Path to the tart executable.
   --shell TEXT                 Path to the shell to be used for commands over
                                ssh.
   --help                       Show this message and exit.
 ```
 
 ### Command `cleanup`
```

### Comparing `gitlab-runner-tart-driver-0.1.1/gitlab_runner_tart_driver.egg-info/SOURCES.txt` & `gitlab-runner-tart-driver-0.1.2/gitlab_runner_tart_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.1.1/setup.py` & `gitlab-runner-tart-driver-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 # read the long description from README.md
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "0.1.1"
+version = "0.1.2"
 
 version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
 
 # read the requirements from requirements.txt
 requirements = []
 with pathlib.Path("requirements.txt").open() as requirements_txt:
     requirements = [str(requirement) for requirement in pkg_resources.parse_requirements(requirements_txt)]
```


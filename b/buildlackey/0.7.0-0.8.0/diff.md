# Comparing `tmp/buildlackey-0.7.0.tar.gz` & `tmp/buildlackey-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildlackey-0.7.0.tar", last modified: Thu Apr 13 02:36:16 2023, max compression
+gzip compressed data, was "buildlackey-0.8.0.tar", last modified: Wed Apr 19 20:36:28 2023, max compression
```

## Comparing `buildlackey-0.7.0.tar` & `buildlackey-0.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 02:36:16.521010 buildlackey-0.7.0/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-04-07 13:32:43.000000 buildlackey-0.7.0/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43932 2023-04-13 02:36:16.520880 buildlackey-0.7.0/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3752 2023-04-10 18:32:21.000000 buildlackey-0.7.0/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 02:36:16.519161 buildlackey-0.7.0/buildlackey/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7407 2023-04-13 02:34:46.000000 buildlackey-0.7.0/buildlackey/Commands.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1224 2023-04-13 00:43:49.000000 buildlackey-0.7.0/buildlackey/Environment.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      469 2023-04-08 19:28:49.000000 buildlackey-0.7.0/buildlackey/Version.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-31 14:31:31.000000 buildlackey-0.7.0/buildlackey/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 02:36:16.520319 buildlackey-0.7.0/buildlackey/exceptions/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       51 2023-02-25 02:47:03.000000 buildlackey-0.7.0/buildlackey/exceptions/ProjectNotSetException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       56 2023-02-25 02:28:42.000000 buildlackey-0.7.0/buildlackey/exceptions/ProjectsBaseNotSetException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 01:41:26.000000 buildlackey-0.7.0/buildlackey/exceptions/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 02:36:16.520641 buildlackey-0.7.0/buildlackey/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 02:21:22.000000 buildlackey-0.7.0/buildlackey/resources/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      856 2023-04-13 00:43:13.000000 buildlackey-0.7.0/buildlackey/resources/loggingConfiguration.json
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        5 2023-04-12 20:04:46.000000 buildlackey-0.7.0/buildlackey/resources/version.txt
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 02:36:16.519965 buildlackey-0.7.0/buildlackey.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43932 2023-04-13 02:36:16.000000 buildlackey-0.7.0/buildlackey.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      590 2023-04-13 02:36:16.000000 buildlackey-0.7.0/buildlackey.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-13 02:36:16.000000 buildlackey-0.7.0/buildlackey.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      215 2023-04-13 02:36:16.000000 buildlackey-0.7.0/buildlackey.egg-info/entry_points.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-04-13 02:36:16.000000 buildlackey-0.7.0/buildlackey.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-04-13 02:36:16.000000 buildlackey-0.7.0/buildlackey.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-13 02:36:16.521045 buildlackey-0.7.0/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1331 2023-04-10 17:51:20.000000 buildlackey-0.7.0/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-19 20:36:28.056637 buildlackey-0.8.0/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-04-07 13:32:43.000000 buildlackey-0.8.0/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43932 2023-04-19 20:36:28.056497 buildlackey-0.8.0/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3752 2023-04-10 18:32:21.000000 buildlackey-0.8.0/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-19 20:36:28.054820 buildlackey-0.8.0/buildlackey/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     8853 2023-04-19 20:34:54.000000 buildlackey-0.8.0/buildlackey/Commands.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1224 2023-04-13 00:43:49.000000 buildlackey-0.8.0/buildlackey/Environment.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      469 2023-04-08 19:28:49.000000 buildlackey-0.8.0/buildlackey/Version.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-31 14:31:31.000000 buildlackey-0.8.0/buildlackey/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-19 20:36:28.055939 buildlackey-0.8.0/buildlackey/exceptions/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       51 2023-02-25 02:47:03.000000 buildlackey-0.8.0/buildlackey/exceptions/ProjectNotSetException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       56 2023-02-25 02:28:42.000000 buildlackey-0.8.0/buildlackey/exceptions/ProjectsBaseNotSetException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 01:41:26.000000 buildlackey-0.8.0/buildlackey/exceptions/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-19 20:36:28.056271 buildlackey-0.8.0/buildlackey/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 02:21:22.000000 buildlackey-0.8.0/buildlackey/resources/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      856 2023-04-13 00:43:13.000000 buildlackey-0.8.0/buildlackey/resources/loggingConfiguration.json
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        5 2023-04-19 14:51:17.000000 buildlackey-0.8.0/buildlackey/resources/version.txt
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-19 20:36:28.055594 buildlackey-0.8.0/buildlackey.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43932 2023-04-19 20:36:28.000000 buildlackey-0.8.0/buildlackey.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      590 2023-04-19 20:36:28.000000 buildlackey-0.8.0/buildlackey.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-19 20:36:28.000000 buildlackey-0.8.0/buildlackey.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      215 2023-04-19 20:36:28.000000 buildlackey-0.8.0/buildlackey.egg-info/entry_points.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-04-19 20:36:28.000000 buildlackey-0.8.0/buildlackey.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-04-19 20:36:28.000000 buildlackey-0.8.0/buildlackey.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-19 20:36:28.056670 buildlackey-0.8.0/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1331 2023-04-10 17:51:20.000000 buildlackey-0.8.0/setup.py
```

### Comparing `buildlackey-0.7.0/LICENSE` & `buildlackey-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `buildlackey-0.7.0/PKG-INFO` & `buildlackey-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildlackey
-Version: 0.7.0
+Version: 0.8.0
 Summary: Project Maintenance Scripts
 Home-page: https://github.com/buildlackey
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
```

### Comparing `buildlackey-0.7.0/README.md` & `buildlackey-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `buildlackey-0.7.0/buildlackey/Commands.py` & `buildlackey-0.8.0/buildlackey/Commands.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,28 +22,32 @@
 
 from buildlackey.Environment import EnvironmentBase
 from buildlackey.Version import Version
 
 
 # noinspection SpellCheckingInspection
 UNIT_TEST_CLI: str = 'python3 -Wdefault -m tests.TestAll'
+BUILD_WHEEL:   str = 'python -m build --sdist --wheel'
 
 DELETE_DIST_BUILD:       str = 'rm -rfv dist build'
 DELETE_GENERAL_EGG_INFO: str = "find . -type d -name '*'.egg-info -delete"
 DELETE_LOG_FILES:        str = 'find . -type f -name "*.log"      -delete'
 DELETE_EGGS:             str = 'rm -rfv .eggs'
 
 PROJECTS_BASE: str = 'PROJECTS_BASE'
 PROJECT:       str = 'PROJECT'
 
 RESOURCES_PACKAGE_NAME:       str = 'buildlackey.resources'
 JSON_LOGGING_CONFIG_FILENAME: str = "loggingConfiguration.json"
 
-STATUS_NO_SUCH_PATH:     int = 23
-STATUS_UNIT_TEST_FAILED: int = 77
+STATUS_NO_SUCH_PATH:                 int = 23
+STATUS_UNIT_TEST_FAILED:             int = 77
+STATUS_MISSING_ENVIRONMENT_VARIABLE: int = 42
+
+MESSAGE_MISSING_ENVIRONMENT_VARIABLE: str = 'Missing an environment variable'
 
 
 def changeToProjectRoot(projectsBase: str, project: str):
 
     fullPath: str = f'{projectsBase}{osSep}{project}'
     chdir(fullPath)
 
@@ -74,32 +78,39 @@
 
 @command()
 @version_option(version=f'{Version().version}', message='%(prog)s version %(version)s')
 @option('--input-file', '-i', required=False,   help='Use input file to list the unit tests to execute')
 def runtests(input_file: str):
     """
     \b
-    Runs the unit tests for the project specified by the following environment variables;
+    Runs the unit tests for the project specified by the environment variables listed below;
+    \b
+    Use the -i/--input-file option to list a set of module names to execute as your
+    unit tests
     \b
 
         PROJECTS_BASE -  The local directory where the python projects are based
         PROJECT       -  The name of the project;  It should be a directory name
+    
     \b
     \b
     However, if one or the other is not defined the command assumes it is executing in a CI
     environment and thus the current working directory is the project base directory.
 
     \b
     By default, buildlackey runs the module named tests.TestAll
 
     """
     setUpLogging()
     envBase: EnvironmentBase = EnvironmentBase()
     if envBase.validProjectsBase is True and envBase.validProjectDirectory() is True:
         changeToProjectRoot(projectsBase=envBase.projectsBase, project=envBase.projectDirectory)
+    else:
+        secho(f'{MESSAGE_MISSING_ENVIRONMENT_VARIABLE}')
+        exit(STATUS_MISSING_ENVIRONMENT_VARIABLE)
 
     if input_file is None:
         secho(f'{UNIT_TEST_CLI}')
         status: int = osSystem(f'{UNIT_TEST_CLI}')
         secho(f'{status=}')
     else:
         path: Path = Path(input_file)
@@ -176,35 +187,62 @@
 
     status: int = osSystem(RUN_MYPY)
     secho(f'{status=}')
 
 
 @command()
 @version_option(version=f'{Version().version}', message='%(prog)s version %(version)s')
-@argument('projects_base', envvar=PROJECTS_BASE)
-@argument('project',       envvar=PROJECT)
-def deploy(projects_base: str, project: str):
+@option('--input-file', '-i', required=False,   help='Use input file to specify a set of commands to execute')
+def deploy(input_file: str):
     """
     \b
-    Creates the deployable for the project specified by the following environment variables
+    Creates the deployable for the project specified by the environment variables listed below
+    \b
+    Use the -i/--input-file option to specify a set of custom commands to execute to build
+    your deployable
+
+
     \b
         PROJECTS_BASE -  The local directory where the python projects are based
         PROJECT       -  The name of the project;  It should be a directory name
+
     """
-    doCommandStart(projects_base, project)
+    setUpLogging()
+    envBase: EnvironmentBase = EnvironmentBase()
+    if envBase.validProjectsBase is True and envBase.validProjectDirectory() is True:
+        changeToProjectRoot(projectsBase=envBase.projectsBase, project=envBase.projectDirectory)
+    else:
+        secho(f'{MESSAGE_MISSING_ENVIRONMENT_VARIABLE}')
+        exit(STATUS_MISSING_ENVIRONMENT_VARIABLE)
 
-    BUILD_WHEEL:   str = 'python -m build --sdist --wheel'
-    secho(f'{BUILD_WHEEL}')
-    status: int = osSystem(BUILD_WHEEL)
-    secho(f'{status=}')
+    doCommandStart(envBase.projectsBase, envBase.projectDirectory)
 
-    CHECK_PACKAGE: str = 'twine check dist/*'
-    secho(f'{CHECK_PACKAGE}')
-    status = osSystem(CHECK_PACKAGE)
-    secho(f'{status=}')
+    if input_file is None:
+        secho(f'{BUILD_WHEEL}')
+        status: int = osSystem(BUILD_WHEEL)
+        secho(f'{status=}')
+
+        CHECK_PACKAGE: str = 'twine check dist/*'
+        secho(f'{CHECK_PACKAGE}')
+        status = osSystem(CHECK_PACKAGE)
+        secho(f'{status=}')
+    else:
+        path: Path = Path(input_file)
+        if path.exists() is True:
+            with path.open(mode='r') as fd:
+                cmd: str = fd.readline()
+                while cmd != '':
+                    secho(f'{cmd}')
+                    status = osSystem(f'{cmd}')
+                    if status != 0:
+                        exit(status)
+                    cmd = fd.readline()
+        else:
+            secho(f'No such file: {input_file}')
+            exit(STATUS_NO_SUCH_PATH)
 
 
 @command()
 @version_option(version=f'{Version().version}', message='%(prog)s version %(version)s')
 @argument('projects_base', envvar=PROJECTS_BASE)
 @argument('project', envvar=PROJECT)
 def prodpush(projects_base: str, project: str):
@@ -222,8 +260,8 @@
     secho(f'{PYPI_PUSH}')
     status = osSystem(PYPI_PUSH)
     secho(f'{status=}')
 
 
 if __name__ == "__main__":
 
-    runtests()
+    deploy()
```

### Comparing `buildlackey-0.7.0/buildlackey/Environment.py` & `buildlackey-0.8.0/buildlackey/Environment.py`

 * *Files identical despite different names*

### Comparing `buildlackey-0.7.0/buildlackey/resources/loggingConfiguration.json` & `buildlackey-0.8.0/buildlackey/resources/loggingConfiguration.json`

 * *Files identical despite different names*

### Comparing `buildlackey-0.7.0/buildlackey.egg-info/PKG-INFO` & `buildlackey-0.8.0/buildlackey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildlackey
-Version: 0.7.0
+Version: 0.8.0
 Summary: Project Maintenance Scripts
 Home-page: https://github.com/buildlackey
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
```

### Comparing `buildlackey-0.7.0/buildlackey.egg-info/SOURCES.txt` & `buildlackey-0.8.0/buildlackey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildlackey-0.7.0/setup.py` & `buildlackey-0.8.0/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/jillw-0.2.3.tar.gz` & `tmp/jillw-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jillw-0.2.3.tar", max compression
+gzip compressed data, was "jillw-0.2.4.tar", max compression
```

## Comparing `jillw-0.2.3.tar` & `jillw-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     2509 2022-11-06 14:44:29.993356 jillw-0.2.3/jillw/__init__.py
--rw-r--r--   0        0        0     4129 2022-11-07 06:32:50.354418 jillw-0.2.3/jillw/cli.py
--rw-r--r--   0        0        0     3246 2022-11-04 05:38:24.671798 jillw-0.2.3/jillw/configloader.py
--rw-r--r--   0        0        0     1103 2022-11-02 02:59:49.249144 jillw-0.2.3/LICENSE.md
--rw-r--r--   0        0        0      504 2022-11-07 06:34:16.400420 jillw-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2827 2022-11-04 05:32:44.212673 jillw-0.2.3/README.md
--rw-r--r--   0        0        0     3662 1970-01-01 00:00:00.000000 jillw-0.2.3/setup.py
--rw-r--r--   0        0        0     3367 1970-01-01 00:00:00.000000 jillw-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2509 2022-11-06 14:44:30.000000 jillw-0.2.4/jillw/__init__.py
+-rw-r--r--   0        0        0     4130 2023-04-19 08:06:24.940717 jillw-0.2.4/jillw/cli.py
+-rw-r--r--   0        0        0     3246 2022-11-04 05:38:25.000000 jillw-0.2.4/jillw/configloader.py
+-rw-r--r--   0        0        0     1103 2023-04-19 07:30:37.164860 jillw-0.2.4/LICENSE.md
+-rw-r--r--   0        0        0      504 2023-04-19 08:04:16.453916 jillw-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2827 2023-04-19 07:30:37.165847 jillw-0.2.4/README.md
+-rw-r--r--   0        0        0     3418 1970-01-01 00:00:00.000000 jillw-0.2.4/PKG-INFO
```

### Comparing `jillw-0.2.3/jillw/__init__.py` & `jillw-0.2.4/jillw/__init__.py`

 * *Files identical despite different names*

### Comparing `jillw-0.2.3/jillw/cli.py` & `jillw-0.2.4/jillw/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         envdict["VIRTUAL_ENV"] = str(env)
         try:
             del envdict["PYTHONHOME"]
         except KeyError:
             pass
         envdict['PATH'] = append_PATH(os.environ["PATH"], jlbindir, env, env / "bin")
 
-    subprocess.run(cmd, env=envdict, shell=True)
+    subprocess.run(cmd, env=envdict, shell=False)
 
 class Main:
     @staticmethod
     def switch(name: str):
         """Switch to the specified environment"""
         with cmd_session():
             env = Ops.env(name)
```

### Comparing `jillw-0.2.3/jillw/configloader.py` & `jillw-0.2.4/jillw/configloader.py`

 * *Files identical despite different names*

### Comparing `jillw-0.2.3/LICENSE.md` & `jillw-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jillw-0.2.3/README.md` & `jillw-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `jillw-0.2.3/setup.py` & `jillw-0.2.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,119 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: jillw
+Version: 0.2.4
+Summary: The wrapper for jill.py and manage Julia environments with Python virtualenv
+License: MIT
+Author: Suzhou-tongyuan
+Author-email: support@tongyuan.cc
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: jill (>=0.11.1,<0.12.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: wisepy2 (>=1.3,<2.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['jillw']
+# JILL Wrapper
 
-package_data = \
-{'': ['*']}
+JILL Wrapper (`jillw`) is a lightweight and cross-platform Julia version manager. This work is based on [johnnychen94/jill.py](https://github.com/johnnychen94/jill.py) and [Python venv](https://docs.python.org/3/library/venv.html).
 
-install_requires = \
-['jill>=0.11.1,<0.12.0', 'tomli>=2.0.1,<3.0.0', 'wisepy2>=1.3,<2.0']
-
-entry_points = \
-{'console_scripts': ['jillw = jillw.cli:main', 'julia = jillw.cli:julia']}
-
-setup_kwargs = {
-    'name': 'jillw',
-    'version': '0.2.3',
-    'description': 'The wrapper for jill.py and manage Julia environments with Python virtualenv',
-    'long_description': '# JILL Wrapper\n\nJILL Wrapper (`jillw`) is a lightweight and cross-platform Julia version manager. This work is based on [johnnychen94/jill.py](https://github.com/johnnychen94/jill.py) and [Python venv](https://docs.python.org/3/library/venv.html).\n\n`jillw` targets several different use cases:\n\n1. cross-platform julia installation\n2. cross-platform julia version management (create, switch, remove, etc.)\n3. providing the "one Julia, one Python" installation\n\n## Installation\n\n```bash\npip install -U jillw\n```\n\n## Usage\n\n### Create environments\n\n```shell\n> jillw create --help\nusage: create [-h] [--name NAME] [--upstream UPSTREAM] [--version VERSION] [--confirm] [--unstable] [name] [upstream] [version]\n\n# create a new environment using Julia 1.8\n> jillw create myenv --version 1.8\n```\n\nThe explanations of the arguments except `name` are referred to [johnnychen94/jill.py](https://github.com/johnnychen94/jill.py).\n\n### Activate environments\n\n```shell\n> jillw switch <envname>\n\n> jillw switch myenv\n```\n\n### Start `julia` under environments\n\n```shell\n> jillw switch myenv\n> julia --compile=min --quiet\njulia> Sys.which("julia")\n"~/.jlenvs/myenv/julia/julia-1.8/bin/julia.exe"\n```\n\n### List environments\n\n```shell\n> jillw list\nmyenv => ~/.jlenvs/myenv\nlatest => ~/.jlenvs/latest\n```\n\n### Remove environments\n\n```shell\n> jillw remove latest\nEnvironment latest removed.\n```\n\n### Run commands under environments\n\n```shell\n> jillw switch myenv\n> jillw run \'echo %VIRTUAL_ENV%\'\n~/.jlenvs/myenv\n```\n\n\n### Configuring the `julia` command (Experimental)\n\nBy creating a `Development.toml` at a working directory, you can conveniently configure the `julia` command to have the following features:\n\n- reduce the startup time by using interpreted mode\n- activate a project on startup\n- preload some specified files on startup\n- preload some modules on startup\n\nUse `jillw devhere` to create a template `Development.toml` at the current working directory.\n\nThe following options can be modified to fit your needs:\n\n- `min-latency`: a boolean that tells whether to use interpreted mode. This makes Julia code slow, but much faster at Julia startup and first-time module loading.\n\n- `no-startup-file`: a boolean that tells whether to load the `~/.julia/config/startup.jl` file.\n\n- `project`: a string thats indicates the path to the project that is expected to be activated on startup.\n\n- `sysimage`: a string thats indicates the path to the sysimage that is expected to be used on startup.\n\n- `using`: a list of strings that indicates the modules that are expected to be preloaded on startup.\n\n- `files`: a list of strings that indicates the files that are expected to be preloaded on startup.\n\n## License\n\nSee [LICENSE.md](./LICENSE.md).\n',
-    'author': 'Suzhou-tongyuan',
-    'author_email': 'support@tongyuan.cc',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+`jillw` targets several different use cases:
 
+1. cross-platform julia installation
+2. cross-platform julia version management (create, switch, remove, etc.)
+3. providing the "one Julia, one Python" installation
+
+## Installation
+
+```bash
+pip install -U jillw
+```
+
+## Usage
+
+### Create environments
+
+```shell
+> jillw create --help
+usage: create [-h] [--name NAME] [--upstream UPSTREAM] [--version VERSION] [--confirm] [--unstable] [name] [upstream] [version]
+
+# create a new environment using Julia 1.8
+> jillw create myenv --version 1.8
+```
+
+The explanations of the arguments except `name` are referred to [johnnychen94/jill.py](https://github.com/johnnychen94/jill.py).
+
+### Activate environments
+
+```shell
+> jillw switch <envname>
+
+> jillw switch myenv
+```
+
+### Start `julia` under environments
+
+```shell
+> jillw switch myenv
+> julia --compile=min --quiet
+julia> Sys.which("julia")
+"~/.jlenvs/myenv/julia/julia-1.8/bin/julia.exe"
+```
+
+### List environments
+
+```shell
+> jillw list
+myenv => ~/.jlenvs/myenv
+latest => ~/.jlenvs/latest
+```
+
+### Remove environments
+
+```shell
+> jillw remove latest
+Environment latest removed.
+```
+
+### Run commands under environments
+
+```shell
+> jillw switch myenv
+> jillw run 'echo %VIRTUAL_ENV%'
+~/.jlenvs/myenv
+```
+
+
+### Configuring the `julia` command (Experimental)
+
+By creating a `Development.toml` at a working directory, you can conveniently configure the `julia` command to have the following features:
+
+- reduce the startup time by using interpreted mode
+- activate a project on startup
+- preload some specified files on startup
+- preload some modules on startup
+
+Use `jillw devhere` to create a template `Development.toml` at the current working directory.
+
+The following options can be modified to fit your needs:
+
+- `min-latency`: a boolean that tells whether to use interpreted mode. This makes Julia code slow, but much faster at Julia startup and first-time module loading.
+
+- `no-startup-file`: a boolean that tells whether to load the `~/.julia/config/startup.jl` file.
+
+- `project`: a string thats indicates the path to the project that is expected to be activated on startup.
+
+- `sysimage`: a string thats indicates the path to the sysimage that is expected to be used on startup.
+
+- `using`: a list of strings that indicates the modules that are expected to be preloaded on startup.
+
+- `files`: a list of strings that indicates the files that are expected to be preloaded on startup.
+
+## License
+
+See [LICENSE.md](./LICENSE.md).
 
-setup(**setup_kwargs)
```


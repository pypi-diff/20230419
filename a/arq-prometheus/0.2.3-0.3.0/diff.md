# Comparing `tmp/arq-prometheus-0.2.3.tar.gz` & `tmp/arq_prometheus-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arq-prometheus-0.2.3.tar", max compression
+gzip compressed data, was "arq_prometheus-0.3.0.tar", max compression
```

## Comparing `arq-prometheus-0.2.3.tar` & `arq_prometheus-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11357 2022-08-26 09:08:26.418433 arq-prometheus-0.2.3/LICENSE
--rw-r--r--   0        0        0     3041 2022-08-26 09:08:26.418433 arq-prometheus-0.2.3/README.md
--rw-r--r--   0        0        0      115 2022-08-26 09:08:26.418433 arq-prometheus-0.2.3/arq_prometheus/__init__.py
--rw-r--r--   0        0        0     7175 2022-08-26 09:08:26.418433 arq-prometheus-0.2.3/arq_prometheus/client.py
--rw-r--r--   0        0        0     1263 2022-08-26 09:08:26.418433 arq-prometheus-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3810 2022-08-26 09:09:52.576555 arq-prometheus-0.2.3/setup.py
--rw-r--r--   0        0        0     3803 2022-08-26 09:09:52.576892 arq-prometheus-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-19 13:10:10.641709 arq_prometheus-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3041 2023-04-19 13:10:10.641709 arq_prometheus-0.3.0/README.md
+-rw-r--r--   0        0        0      115 2023-04-19 13:10:10.641709 arq_prometheus-0.3.0/arq_prometheus/__init__.py
+-rw-r--r--   0        0        0     7175 2023-04-19 13:10:10.641709 arq_prometheus-0.3.0/arq_prometheus/client.py
+-rw-r--r--   0        0        0     1276 2023-04-19 13:10:10.641709 arq_prometheus-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3951 1970-01-01 00:00:00.000000 arq_prometheus-0.3.0/PKG-INFO
```

### Comparing `arq-prometheus-0.2.3/LICENSE` & `arq_prometheus-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arq-prometheus-0.2.3/README.md` & `arq_prometheus-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `arq-prometheus-0.2.3/arq_prometheus/client.py` & `arq_prometheus-0.3.0/arq_prometheus/client.py`

 * *Files identical despite different names*

### Comparing `arq-prometheus-0.2.3/pyproject.toml` & `arq_prometheus-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "arq-prometheus"
-version = "0.2.3"
+version = "0.3.0"
 description = "Prometheus metrics for arq job queues"
 authors = ["Santiago Fraire Willemoes <santiago.fraire@kpn.com>"]
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 readme = "README.md"
 keywords = ["arq", "prometheus", "metrics"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-prometheus-client = "^0.14.1"
-arq = "^0.23"
+prometheus-client = ">=0.14.1,<1.0.0"
+arq = ">0.23,<1.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
 mypy = "^0.961"
 black = "^22.6.0"
 ipython = "^8.4.0"
 isort = "^5.10.1"
@@ -28,15 +28,15 @@
 pytest-cov = "^3.0.0"
 pytest-asyncio = "^0.19.0"
 pytest-mock = "^3.8.2"
 Flake8-pyproject = "^1.1.0"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.3"
+version = "0.3.0"
 version_files = [
   "pyproject.toml:version",
   "arq_prometheus/__init__.py:__version__",
 ]
 update_changelog_on_bump = true
 
 [build-system]
```

### Comparing `arq-prometheus-0.2.3/setup.py` & `arq_prometheus-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,111 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['arq_prometheus']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['arq>=0.23,<0.24', 'prometheus-client>=0.14.1,<0.15.0']
-
-setup_kwargs = {
-    'name': 'arq-prometheus',
-    'version': '0.2.3',
-    'description': 'Prometheus metrics for arq job queues',
-    'long_description': '# Arq-prometheus\n\n![Build status](https://github.com/kpn/arq-prometheus/actions/workflows/test.yaml/badge.svg)\n[![PyPI Package latest release](https://img.shields.io/pypi/v/arq-prometheus.svg?style=flat-square)](https://pypi.org/project/arq-prometheus/)\n[![PyPI Package download count (per month)](https://img.shields.io/pypi/dm/arq-prometheus?style=flat-square)](https://pypi.org/project/arq-prometheus/)\n[![Supported versions](https://img.shields.io/pypi/pyversions/arq-prometheus.svg?style=flat-square)](https://pypi.org/project/arq-prometheus/)\n[![Codecov](https://img.shields.io/codecov/c/github/kpn/arq-prometheus.svg?style=flat-square)](https://codecov.io/gh/kpn/arq-prometheus)\n\n\nPrometheus metrics for [arq](https://github.com/samuelcolvin/arq)\n\n⚠️ WARNING! This is a project in alpha phase ⚠️\n\n## Installation\n\n[Pip](https://pip.pypa.io/en/stable/)\n\n```sh\npip install -U arq-prometheus\n```\n\n[Poetry](https://python-poetry.org/)\n\n```sh\npoetry add arq-prometheus\n```\n\n## Description\n\nThe metrics exposed are the same as the health check.\n\n| Metric name             | Description                      |\n| ----------------------- | -------------------------------- |\n| `arq_jobs_completed`    | The number of jobs completed     |\n| `arq_jobs_failed`       | The total number of errored jobs |\n| `arq_jobs_retried`      | The total number of retried jobs |\n| `arq_ongoing_jobs`      | The number of jobs in progress   |\n| `arq_queued_inprogress` | The number of jobs in progress   |\n\nWhen working with `arq` I found some limitations, it was specially hard to get access to\nthe worker in order to retrieve information like the `queue_name` or `health_check_key`.\nThe startup and shutdown functions only make available a `ctx` with the redis connection.\nThis means that if you provide a custom `queue_name` or `health_check_key`, you will\nalso have to provide them to `ArqPrometheusMetrics`.\n\n## Usage\n\n````python\n# example_worker.py\nfrom arq_prometheus import ArqPrometheusMetrics\n\nasync def startup(ctx):\n    arq_prometheus = ArqPrometheusMetrics(ctx, delay=delay)\n    ctx["arq_prometheus"] = await arq_prometheus.start()\n\nasync def shutdown(ctx):\n    await ctx["arq_prometheus"].stop()\n\nclass WorkerSettings:\n    on_startup = startup\n    on_shutdown = shutdown\n    function = []  # your arq jobs\n    ... # other settings\n\n````\n\nStart your arq worker,\n\n```sh\narq example_worker.WorkerSettings\n```\n\nMake request to `localhost:8081` (or open in browser).\n\n```sh\ncurl localhost:8081\n```\n\n\n## Arguments\n\n- `ctx: dict`: arq context\n- `queue_name: str = default_queue_name`: name of the arq queue\n- `health_check_key: Optional[str] = None`: arq health key\n- `delay: datetime.timedelta = datetime.timedelta(seconds=5)`: a datetime.timedelta\n- `enable_webserver: bool = True`: set to True if you want a web server exposing the metrics\n- `addr: str = "0.0.0.0"`: webserver address\n- `port: int = 8081`: webserver port\n- `registry: prom.CollectorRegistry = prom.REGISTRY`: the prometheus registry, usually you do not have to override this',
-    'author': 'Santiago Fraire Willemoes',
-    'author_email': 'santiago.fraire@kpn.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: arq-prometheus
+Version: 0.3.0
+Summary: Prometheus metrics for arq job queues
+Keywords: arq,prometheus,metrics
+Author: Santiago Fraire Willemoes
+Author-email: santiago.fraire@kpn.com
+Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Requires-Dist: arq (>0.23,<1.0)
+Requires-Dist: prometheus-client (>=0.14.1,<1.0.0)
+Description-Content-Type: text/markdown
+
+# Arq-prometheus
+
+![Build status](https://github.com/kpn/arq-prometheus/actions/workflows/test.yaml/badge.svg)
+[![PyPI Package latest release](https://img.shields.io/pypi/v/arq-prometheus.svg?style=flat-square)](https://pypi.org/project/arq-prometheus/)
+[![PyPI Package download count (per month)](https://img.shields.io/pypi/dm/arq-prometheus?style=flat-square)](https://pypi.org/project/arq-prometheus/)
+[![Supported versions](https://img.shields.io/pypi/pyversions/arq-prometheus.svg?style=flat-square)](https://pypi.org/project/arq-prometheus/)
+[![Codecov](https://img.shields.io/codecov/c/github/kpn/arq-prometheus.svg?style=flat-square)](https://codecov.io/gh/kpn/arq-prometheus)
+
+
+Prometheus metrics for [arq](https://github.com/samuelcolvin/arq)
+
+⚠️ WARNING! This is a project in alpha phase ⚠️
+
+## Installation
+
+[Pip](https://pip.pypa.io/en/stable/)
+
+```sh
+pip install -U arq-prometheus
+```
+
+[Poetry](https://python-poetry.org/)
+
+```sh
+poetry add arq-prometheus
+```
+
+## Description
+
+The metrics exposed are the same as the health check.
+
+| Metric name             | Description                      |
+| ----------------------- | -------------------------------- |
+| `arq_jobs_completed`    | The number of jobs completed     |
+| `arq_jobs_failed`       | The total number of errored jobs |
+| `arq_jobs_retried`      | The total number of retried jobs |
+| `arq_ongoing_jobs`      | The number of jobs in progress   |
+| `arq_queued_inprogress` | The number of jobs in progress   |
+
+When working with `arq` I found some limitations, it was specially hard to get access to
+the worker in order to retrieve information like the `queue_name` or `health_check_key`.
+The startup and shutdown functions only make available a `ctx` with the redis connection.
+This means that if you provide a custom `queue_name` or `health_check_key`, you will
+also have to provide them to `ArqPrometheusMetrics`.
+
+## Usage
+
+````python
+# example_worker.py
+from arq_prometheus import ArqPrometheusMetrics
+
+async def startup(ctx):
+    arq_prometheus = ArqPrometheusMetrics(ctx, delay=delay)
+    ctx["arq_prometheus"] = await arq_prometheus.start()
+
+async def shutdown(ctx):
+    await ctx["arq_prometheus"].stop()
+
+class WorkerSettings:
+    on_startup = startup
+    on_shutdown = shutdown
+    function = []  # your arq jobs
+    ... # other settings
+
+````
+
+Start your arq worker,
+
+```sh
+arq example_worker.WorkerSettings
+```
+
+Make request to `localhost:8081` (or open in browser).
+
+```sh
+curl localhost:8081
+```
+
+
+## Arguments
+
+- `ctx: dict`: arq context
+- `queue_name: str = default_queue_name`: name of the arq queue
+- `health_check_key: Optional[str] = None`: arq health key
+- `delay: datetime.timedelta = datetime.timedelta(seconds=5)`: a datetime.timedelta
+- `enable_webserver: bool = True`: set to True if you want a web server exposing the metrics
+- `addr: str = "0.0.0.0"`: webserver address
+- `port: int = 8081`: webserver port
+- `registry: prom.CollectorRegistry = prom.REGISTRY`: the prometheus registry, usually you do not have to override this
```


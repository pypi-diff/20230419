# Comparing `tmp/graph-scheduler-1.1.1.tar.gz` & `tmp/graph-scheduler-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/graph-scheduler-1.1.1.tar", last modified: Tue Apr 19 00:57:30 2022, max compression
+gzip compressed data, was "graph-scheduler-1.1.2.tar", last modified: Wed Apr 19 00:41:46 2023, max compression
```

## Comparing `graph-scheduler-1.1.1.tar` & `graph-scheduler-1.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwx------   0 katherine  (1000) katherine  (1000)        0 2022-04-19 00:57:30.000000 graph-scheduler-1.1.1/
--rw-------   0 katherine  (1000) katherine  (1000)    11358 2021-07-29 00:04:25.000000 graph-scheduler-1.1.1/LICENSE.txt
--rw-------   0 katherine  (1000) katherine  (1000)      290 2021-07-29 00:30:32.000000 graph-scheduler-1.1.1/MANIFEST.in
--rw-------   0 katherine  (1000) katherine  (1000)     3069 2022-04-19 00:57:30.000000 graph-scheduler-1.1.1/PKG-INFO
--rw-------   0 katherine  (1000) katherine  (1000)     1828 2021-10-21 23:30:50.000000 graph-scheduler-1.1.1/README.md
--rw-------   0 katherine  (1000) katherine  (1000)     2623 2021-07-29 00:04:25.000000 graph-scheduler-1.1.1/conftest.py
--rw-------   0 katherine  (1000) katherine  (1000)      181 2022-04-19 00:57:10.000000 graph-scheduler-1.1.1/dev_requirements.txt
-drwx------   0 katherine  (1000) katherine  (1000)        0 2022-04-19 00:57:30.000000 graph-scheduler-1.1.1/docs/
--rw-------   0 katherine  (1000) katherine  (1000)      133 2021-07-29 00:30:32.000000 graph-scheduler-1.1.1/docs/Condition.rst
--rw-------   0 katherine  (1000) katherine  (1000)      634 2021-07-29 00:30:32.000000 graph-scheduler-1.1.1/docs/Makefile
--rw-------   0 katherine  (1000) katherine  (1000)      133 2021-07-29 00:30:32.000000 graph-scheduler-1.1.1/docs/Scheduler.rst
--rw-------   0 katherine  (1000) katherine  (1000)      118 2021-07-29 00:30:32.000000 graph-scheduler-1.1.1/docs/Time.rst
--rw-------   0 katherine  (1000) katherine  (1000)     2672 2021-07-29 00:30:32.000000 graph-scheduler-1.1.1/docs/conf.py
--rw-------   0 katherine  (1000) katherine  (1000)      442 2021-07-29 00:30:32.000000 graph-scheduler-1.1.1/docs/index.rst
--rw-------   0 katherine  (1000) katherine  (1000)      760 2021-07-29 00:30:32.000000 graph-scheduler-1.1.1/docs/make.bat
--rw-------   0 katherine  (1000) katherine  (1000)       54 2022-04-19 00:57:10.000000 graph-scheduler-1.1.1/docs_requirements.txt
--rw-------   0 katherine  (1000) katherine  (1000)      127 2021-07-29 00:04:25.000000 graph-scheduler-1.1.1/pyproject.toml
--rw-------   0 katherine  (1000) katherine  (1000)       20 2022-04-19 00:57:10.000000 graph-scheduler-1.1.1/requirements.txt
--rw-------   0 katherine  (1000) katherine  (1000)     2550 2022-04-19 00:57:30.000000 graph-scheduler-1.1.1/setup.cfg
--rw-------   0 katherine  (1000) katherine  (1000)      591 2021-07-29 00:30:32.000000 graph-scheduler-1.1.1/setup.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2022-04-19 00:57:30.000000 graph-scheduler-1.1.1/src/
-drwx------   0 katherine  (1000) katherine  (1000)        0 2022-04-19 00:57:30.000000 graph-scheduler-1.1.1/src/graph_scheduler/
--rw-------   0 katherine  (1000) katherine  (1000)     1244 2021-08-19 23:56:30.000000 graph-scheduler-1.1.1/src/graph_scheduler/__init__.py
--rw-------   0 katherine  (1000) katherine  (1000)      497 2022-04-19 00:57:30.000000 graph-scheduler-1.1.1/src/graph_scheduler/_version.py
--rw-------   0 katherine  (1000) katherine  (1000)    76898 2022-03-12 03:11:54.000000 graph-scheduler-1.1.1/src/graph_scheduler/condition.py
--rw-------   0 katherine  (1000) katherine  (1000)    41990 2021-10-21 23:30:50.000000 graph-scheduler-1.1.1/src/graph_scheduler/scheduler.py
--rw-------   0 katherine  (1000) katherine  (1000)    25903 2022-03-12 03:11:54.000000 graph-scheduler-1.1.1/src/graph_scheduler/time.py
--rw-------   0 katherine  (1000) katherine  (1000)     2704 2021-07-29 00:04:25.000000 graph-scheduler-1.1.1/src/graph_scheduler/utilities.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2022-04-19 00:57:30.000000 graph-scheduler-1.1.1/src/graph_scheduler.egg-info/
--rw-------   0 katherine  (1000) katherine  (1000)     3069 2022-04-19 00:57:30.000000 graph-scheduler-1.1.1/src/graph_scheduler.egg-info/PKG-INFO
--rw-------   0 katherine  (1000) katherine  (1000)      835 2022-04-19 00:57:30.000000 graph-scheduler-1.1.1/src/graph_scheduler.egg-info/SOURCES.txt
--rw-------   0 katherine  (1000) katherine  (1000)        1 2022-04-19 00:57:30.000000 graph-scheduler-1.1.1/src/graph_scheduler.egg-info/dependency_links.txt
--rw-------   0 katherine  (1000) katherine  (1000)      275 2022-04-19 00:57:30.000000 graph-scheduler-1.1.1/src/graph_scheduler.egg-info/requires.txt
--rw-------   0 katherine  (1000) katherine  (1000)       16 2022-04-19 00:57:30.000000 graph-scheduler-1.1.1/src/graph_scheduler.egg-info/top_level.txt
-drwx------   0 katherine  (1000) katherine  (1000)        0 2022-04-19 00:57:30.000000 graph-scheduler-1.1.1/tests/
-drwx------   0 katherine  (1000) katherine  (1000)        0 2022-04-19 00:57:30.000000 graph-scheduler-1.1.1/tests/documentation/
--rw-------   0 katherine  (1000) katherine  (1000)      506 2021-07-29 00:04:25.000000 graph-scheduler-1.1.1/tests/documentation/test_module_docs.py
-drwx------   0 katherine  (1000) katherine  (1000)        0 2022-04-19 00:57:30.000000 graph-scheduler-1.1.1/tests/scheduling/
--rw-------   0 katherine  (1000) katherine  (1000)     1635 2021-07-29 00:30:32.000000 graph-scheduler-1.1.1/tests/scheduling/conftest.py
--rw-------   0 katherine  (1000) katherine  (1000)    57241 2022-03-12 03:11:54.000000 graph-scheduler-1.1.1/tests/scheduling/test_condition.py
--rw-------   0 katherine  (1000) katherine  (1000)    95802 2022-04-19 00:57:10.000000 graph-scheduler-1.1.1/tests/scheduling/test_scheduler.py
--rw-------   0 katherine  (1000) katherine  (1000)     8785 2022-03-12 03:11:54.000000 graph-scheduler-1.1.1/tests/scheduling/test_time.py
--rw-------   0 katherine  (1000) katherine  (1000)    78254 2021-07-29 00:04:25.000000 graph-scheduler-1.1.1/versioneer.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-04-19 00:41:46.431227 graph-scheduler-1.1.2/
+-rw-------   0 katherine  (1000) katherine  (1000)    11358 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/LICENSE.txt
+-rw-------   0 katherine  (1000) katherine  (1000)      290 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/MANIFEST.in
+-rw-------   0 katherine  (1000) katherine  (1000)     2660 2023-04-19 00:41:46.431227 graph-scheduler-1.1.2/PKG-INFO
+-rw-------   0 katherine  (1000) katherine  (1000)     1828 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/README.md
+-rw-------   0 katherine  (1000) katherine  (1000)     2623 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/conftest.py
+-rw-------   0 katherine  (1000) katherine  (1000)      140 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/dev_requirements.txt
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-04-19 00:41:46.427227 graph-scheduler-1.1.2/docs/
+-rw-------   0 katherine  (1000) katherine  (1000)      133 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/docs/Condition.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      634 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/docs/Makefile
+-rw-------   0 katherine  (1000) katherine  (1000)      133 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/docs/Scheduler.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      118 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/docs/Time.rst
+-rw-------   0 katherine  (1000) katherine  (1000)     2672 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/docs/conf.py
+-rw-------   0 katherine  (1000) katherine  (1000)      442 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/docs/index.rst
+-rw-------   0 katherine  (1000) katherine  (1000)      760 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/docs/make.bat
+-rw-------   0 katherine  (1000) katherine  (1000)       54 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/docs_requirements.txt
+-rw-------   0 katherine  (1000) katherine  (1000)      127 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/pyproject.toml
+-rw-------   0 katherine  (1000) katherine  (1000)       29 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/requirements.txt
+-rw-------   0 katherine  (1000) katherine  (1000)     2550 2023-04-19 00:41:46.431227 graph-scheduler-1.1.2/setup.cfg
+-rw-------   0 katherine  (1000) katherine  (1000)      591 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/setup.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-04-19 00:41:46.427227 graph-scheduler-1.1.2/src/
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-04-19 00:41:46.431227 graph-scheduler-1.1.2/src/graph_scheduler/
+-rw-------   0 katherine  (1000) katherine  (1000)     1244 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/src/graph_scheduler/__init__.py
+-rw-------   0 katherine  (1000) katherine  (1000)      497 2023-04-19 00:41:46.431227 graph-scheduler-1.1.2/src/graph_scheduler/_version.py
+-rw-------   0 katherine  (1000) katherine  (1000)    76898 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/src/graph_scheduler/condition.py
+-rw-------   0 katherine  (1000) katherine  (1000)    42008 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/src/graph_scheduler/scheduler.py
+-rw-------   0 katherine  (1000) katherine  (1000)    26192 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/src/graph_scheduler/time.py
+-rw-------   0 katherine  (1000) katherine  (1000)     2704 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/src/graph_scheduler/utilities.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-04-19 00:41:46.427227 graph-scheduler-1.1.2/src/graph_scheduler.egg-info/
+-rw-------   0 katherine  (1000) katherine  (1000)     2660 2023-04-19 00:41:46.000000 graph-scheduler-1.1.2/src/graph_scheduler.egg-info/PKG-INFO
+-rw-------   0 katherine  (1000) katherine  (1000)      835 2023-04-19 00:41:46.000000 graph-scheduler-1.1.2/src/graph_scheduler.egg-info/SOURCES.txt
+-rw-------   0 katherine  (1000) katherine  (1000)        1 2023-04-19 00:41:46.000000 graph-scheduler-1.1.2/src/graph_scheduler.egg-info/dependency_links.txt
+-rw-------   0 katherine  (1000) katherine  (1000)      236 2023-04-19 00:41:46.000000 graph-scheduler-1.1.2/src/graph_scheduler.egg-info/requires.txt
+-rw-------   0 katherine  (1000) katherine  (1000)       16 2023-04-19 00:41:46.000000 graph-scheduler-1.1.2/src/graph_scheduler.egg-info/top_level.txt
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-04-19 00:41:46.427227 graph-scheduler-1.1.2/tests/
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-04-19 00:41:46.427227 graph-scheduler-1.1.2/tests/documentation/
+-rw-------   0 katherine  (1000) katherine  (1000)      506 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/tests/documentation/test_module_docs.py
+drwx------   0 katherine  (1000) katherine  (1000)        0 2023-04-19 00:41:46.431227 graph-scheduler-1.1.2/tests/scheduling/
+-rw-------   0 katherine  (1000) katherine  (1000)     1635 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/tests/scheduling/conftest.py
+-rw-------   0 katherine  (1000) katherine  (1000)    57241 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/tests/scheduling/test_condition.py
+-rw-------   0 katherine  (1000) katherine  (1000)    95802 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/tests/scheduling/test_scheduler.py
+-rw-------   0 katherine  (1000) katherine  (1000)     8785 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/tests/scheduling/test_time.py
+-rw-------   0 katherine  (1000) katherine  (1000)    78254 2023-04-18 23:03:00.000000 graph-scheduler-1.1.2/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `graph-scheduler-1.1.1/LICENSE.txt` & `graph-scheduler-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.1/PKG-INFO` & `graph-scheduler-1.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,77 @@
 Metadata-Version: 2.1
 Name: graph-scheduler
-Version: 1.1.1
+Version: 1.1.2
 Summary: A graph-based scheduler of nodes based on structure and conditions
 Home-page: https://github.com/kmantel/graph-scheduler
 Author: Katherine Mantel, Princeton University
 Author-email: kmantel@princeton.edu
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kmantel/graph-scheduler/issues
-Description: # Graph Scheduler
-        
-        [![CI](https://github.com/kmantel/graph-scheduler/actions/workflows/ci.yml/badge.svg)](https://github.com/kmantel/graph-scheduler/actions/workflows/ci.yml)
-        [![Coverage Status](https://coveralls.io/repos/github/kmantel/graph-scheduler/badge.svg)](https://coveralls.io/github/kmantel/graph-scheduler)
-        
-        A graph scheduler generates the order in which the nodes of a directed
-        acyclic graph (DAG) are executed using the structure of the graph and
-        expressive
-        [conditions](https://kmantel.github.io/graph-scheduler/Condition.html).
-        Specifically, a scheduler uses a topological ordering of the nodes as a
-        base sequence of execution and further restricts execution based on
-        predefined or custom conditions provided by the user. Patterns of
-        execution are linked to abstract units of time and may optionally be
-        mapped to real time units using [pint](https://pint.readthedocs.io/).
-        
-        Documentation is available on github-pages [for the current
-        release](https://kmantel.github.io/graph-scheduler/) and [for the
-        current main
-        branch](https://kmantel.github.io/graph-scheduler/branch/main). For
-        prior releases, go to
-        ``https://kmantel.github.io/graph-scheduler/tag/<tag_name>``.
-        
-        ## Installation
-        
-        Install from pypi:
-        
-        ```sh
-        pip install graph-scheduler
-        ```
-        
-        ## Example
-        
-        The graph is specified here in dependency dictionary format, but
-        [networkx](https://github.com/networkx/networkx) Digraphs are also
-        supported.
-        
-        ```python
-        >>> import graph_scheduler
-        
-        >>> graph = {
-            'A': set(),
-            'B': {'A'},
-            'C': {'A'},
-            'D': {'B', 'C'},
-        }
-        
-        >>> sched = graph_scheduler.Scheduler(graph=graph)
-        >>> sched.add_condition('C', graph_scheduler.EveryNCalls('A', 2))
-        >>> sched.add_condition('D', graph_scheduler.EveryNCalls('C', 2))
-        
-        >>> print(list(sched.run()))
-        [{'A'}, {'B'}, {'A'}, {'C', 'B'}, {'A'}, {'B'}, {'A'}, {'C', 'B'}, {'D'}]
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE.txt
+
+# Graph Scheduler
+
+[![CI](https://github.com/kmantel/graph-scheduler/actions/workflows/ci.yml/badge.svg)](https://github.com/kmantel/graph-scheduler/actions/workflows/ci.yml)
+[![Coverage Status](https://coveralls.io/repos/github/kmantel/graph-scheduler/badge.svg)](https://coveralls.io/github/kmantel/graph-scheduler)
+
+A graph scheduler generates the order in which the nodes of a directed
+acyclic graph (DAG) are executed using the structure of the graph and
+expressive
+[conditions](https://kmantel.github.io/graph-scheduler/Condition.html).
+Specifically, a scheduler uses a topological ordering of the nodes as a
+base sequence of execution and further restricts execution based on
+predefined or custom conditions provided by the user. Patterns of
+execution are linked to abstract units of time and may optionally be
+mapped to real time units using [pint](https://pint.readthedocs.io/).
+
+Documentation is available on github-pages [for the current
+release](https://kmantel.github.io/graph-scheduler/) and [for the
+current main
+branch](https://kmantel.github.io/graph-scheduler/branch/main). For
+prior releases, go to
+``https://kmantel.github.io/graph-scheduler/tag/<tag_name>``.
+
+## Installation
+
+Install from pypi:
+
+```sh
+pip install graph-scheduler
+```
+
+## Example
+
+The graph is specified here in dependency dictionary format, but
+[networkx](https://github.com/networkx/networkx) Digraphs are also
+supported.
+
+```python
+>>> import graph_scheduler
+
+>>> graph = {
+    'A': set(),
+    'B': {'A'},
+    'C': {'A'},
+    'D': {'B', 'C'},
+}
+
+>>> sched = graph_scheduler.Scheduler(graph=graph)
+>>> sched.add_condition('C', graph_scheduler.EveryNCalls('A', 2))
+>>> sched.add_condition('D', graph_scheduler.EveryNCalls('C', 2))
+
+>>> print(list(sched.run()))
+[{'A'}, {'B'}, {'A'}, {'C', 'B'}, {'A'}, {'B'}, {'A'}, {'C', 'B'}, {'D'}]
+```
+
+
```

### Comparing `graph-scheduler-1.1.1/README.md` & `graph-scheduler-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.1/conftest.py` & `graph-scheduler-1.1.2/conftest.py`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.1/docs/Makefile` & `graph-scheduler-1.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.1/docs/conf.py` & `graph-scheduler-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.1/docs/make.bat` & `graph-scheduler-1.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.1/setup.cfg` & `graph-scheduler-1.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 	raise .*Error
 	assert False.*
 	
 	if 0:
 	if __name__ == .__main__.:
 
 [versioneer]
-vcs = git
+VCS = git
 style = pep440
 versionfile_source = src/graph_scheduler/_version.py
 versionfile_build = graph_scheduler/_version.py
 tag_prefix = v
 parentdir_prefix = graph_scheduler-
 
 [egg_info]
```

### Comparing `graph-scheduler-1.1.1/setup.py` & `graph-scheduler-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.1/src/graph_scheduler/__init__.py` & `graph-scheduler-1.1.2/src/graph_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.1/src/graph_scheduler/condition.py` & `graph-scheduler-1.1.2/src/graph_scheduler/condition.py`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.1/src/graph_scheduler/scheduler.py` & `graph-scheduler-1.1.2/src/graph_scheduler/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,15 +309,15 @@
 from toposort import toposort
 
 from graph_scheduler import _unit_registry
 from graph_scheduler.condition import (
     All, AllHaveRun, Always, Condition, ConditionSet, EveryNCalls, Never,
     _parse_absolute_unit, _quantity_as_integer,
 )
-from graph_scheduler.time import Clock, TimeScale
+from graph_scheduler.time import _get_pint_unit, Clock, TimeScale
 
 __all__ = [
     'Scheduler', 'SchedulerError', 'SchedulingMode',
 ]
 
 logger = logging.getLogger(__name__)
 
@@ -415,15 +415,15 @@
     def __init__(
         self,
         graph,
         conditions=None,
         termination_conds=None,
         default_execution_id=None,
         mode: SchedulingMode = SchedulingMode.STANDARD,
-        default_absolute_time_unit: typing.Union[str, pint.Quantity] = 1 * _unit_registry.ms,
+        default_absolute_time_unit: typing.Union[str, pint.Quantity] = _get_pint_unit(1, 'ms'),
         **kwargs
     ):
         """
         :param self:
         :param conditions: (ConditionSet) - a :keyword:`ConditionSet` to be scheduled
         """
         self.conditions = ConditionSet(conditions)
```

### Comparing `graph-scheduler-1.1.1/src/graph_scheduler/time.py` & `graph-scheduler-1.1.2/src/graph_scheduler/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,22 @@
 _alias_docs_warning_str = """
 
 .. note:: This documentation was modified from the original due to environment-specific TimeScale renamings. If there is any confusion, please see the original documentation at https://www.github.com/kmantel/graph-scheduler
 
 """
 
 
+# use a cached call because each call to getattr on a pint unit_registry
+# creates new instances of Unit, and this becomes a significant time
+# cost compared even to deepcopying
+@functools.lru_cache()
+def _get_pint_unit(num, unit):
+    return num * getattr(_unit_registry, unit)
+
+
 class TimeScaleError(Exception):
 
     def __init__(self, error_value):
         self.error_value = error_value
 
     def __str__(self):
         return repr(self.error_value)
@@ -228,16 +236,16 @@
     def __init__(
         self,
         consideration_set_execution=0,
         pass_=0,
         environment_state_update=0,
         environment_sequence=0,
         life=0,
-        absolute=0 * _unit_registry.ms,
-        absolute_interval=1 * _unit_registry.ms,
+        absolute=_get_pint_unit(0, 'ms'),
+        absolute_interval=_get_pint_unit(1, 'ms'),
         absolute_time_unit_scale=TimeScale.CONSIDERATION_SET_EXECUTION,
         absolute_enabled=False,
         **alias_time_values,
     ):
         time_scale_values = {}
         for ts in TimeScale:
             time_scale_values[ts] = locals()[_time_scale_to_attr_str(ts)]
@@ -248,16 +256,16 @@
             if _time_scale_aliases[ts].lower() in alias_time_values
         })
 
         super().__init__(
             **{
                 _time_scale_to_attr_str(ts): v for ts, v in time_scale_values.items()
             },
-            absolute=0 * _unit_registry.ms,
-            absolute_interval=1 * _unit_registry.ms,
+            absolute=_get_pint_unit(0, 'ms'),
+            absolute_interval=_get_pint_unit(1, 'ms'),
             absolute_time_unit_scale=TimeScale.CONSIDERATION_SET_EXECUTION,
             absolute_enabled=False,
         )
 
     def __repr__(self):
         abs_str = f'{self.absolute}, ' if self.absolute_enabled else ''
         ts_str = self._time_repr(exclusions={TimeScale.LIFE})
```

### Comparing `graph-scheduler-1.1.1/src/graph_scheduler/utilities.py` & `graph-scheduler-1.1.2/src/graph_scheduler/utilities.py`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.1/src/graph_scheduler.egg-info/PKG-INFO` & `graph-scheduler-1.1.2/src/graph_scheduler.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,77 @@
 Metadata-Version: 2.1
 Name: graph-scheduler
-Version: 1.1.1
+Version: 1.1.2
 Summary: A graph-based scheduler of nodes based on structure and conditions
 Home-page: https://github.com/kmantel/graph-scheduler
 Author: Katherine Mantel, Princeton University
 Author-email: kmantel@princeton.edu
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kmantel/graph-scheduler/issues
-Description: # Graph Scheduler
-        
-        [![CI](https://github.com/kmantel/graph-scheduler/actions/workflows/ci.yml/badge.svg)](https://github.com/kmantel/graph-scheduler/actions/workflows/ci.yml)
-        [![Coverage Status](https://coveralls.io/repos/github/kmantel/graph-scheduler/badge.svg)](https://coveralls.io/github/kmantel/graph-scheduler)
-        
-        A graph scheduler generates the order in which the nodes of a directed
-        acyclic graph (DAG) are executed using the structure of the graph and
-        expressive
-        [conditions](https://kmantel.github.io/graph-scheduler/Condition.html).
-        Specifically, a scheduler uses a topological ordering of the nodes as a
-        base sequence of execution and further restricts execution based on
-        predefined or custom conditions provided by the user. Patterns of
-        execution are linked to abstract units of time and may optionally be
-        mapped to real time units using [pint](https://pint.readthedocs.io/).
-        
-        Documentation is available on github-pages [for the current
-        release](https://kmantel.github.io/graph-scheduler/) and [for the
-        current main
-        branch](https://kmantel.github.io/graph-scheduler/branch/main). For
-        prior releases, go to
-        ``https://kmantel.github.io/graph-scheduler/tag/<tag_name>``.
-        
-        ## Installation
-        
-        Install from pypi:
-        
-        ```sh
-        pip install graph-scheduler
-        ```
-        
-        ## Example
-        
-        The graph is specified here in dependency dictionary format, but
-        [networkx](https://github.com/networkx/networkx) Digraphs are also
-        supported.
-        
-        ```python
-        >>> import graph_scheduler
-        
-        >>> graph = {
-            'A': set(),
-            'B': {'A'},
-            'C': {'A'},
-            'D': {'B', 'C'},
-        }
-        
-        >>> sched = graph_scheduler.Scheduler(graph=graph)
-        >>> sched.add_condition('C', graph_scheduler.EveryNCalls('A', 2))
-        >>> sched.add_condition('D', graph_scheduler.EveryNCalls('C', 2))
-        
-        >>> print(list(sched.run()))
-        [{'A'}, {'B'}, {'A'}, {'C', 'B'}, {'A'}, {'B'}, {'A'}, {'C', 'B'}, {'D'}]
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE.txt
+
+# Graph Scheduler
+
+[![CI](https://github.com/kmantel/graph-scheduler/actions/workflows/ci.yml/badge.svg)](https://github.com/kmantel/graph-scheduler/actions/workflows/ci.yml)
+[![Coverage Status](https://coveralls.io/repos/github/kmantel/graph-scheduler/badge.svg)](https://coveralls.io/github/kmantel/graph-scheduler)
+
+A graph scheduler generates the order in which the nodes of a directed
+acyclic graph (DAG) are executed using the structure of the graph and
+expressive
+[conditions](https://kmantel.github.io/graph-scheduler/Condition.html).
+Specifically, a scheduler uses a topological ordering of the nodes as a
+base sequence of execution and further restricts execution based on
+predefined or custom conditions provided by the user. Patterns of
+execution are linked to abstract units of time and may optionally be
+mapped to real time units using [pint](https://pint.readthedocs.io/).
+
+Documentation is available on github-pages [for the current
+release](https://kmantel.github.io/graph-scheduler/) and [for the
+current main
+branch](https://kmantel.github.io/graph-scheduler/branch/main). For
+prior releases, go to
+``https://kmantel.github.io/graph-scheduler/tag/<tag_name>``.
+
+## Installation
+
+Install from pypi:
+
+```sh
+pip install graph-scheduler
+```
+
+## Example
+
+The graph is specified here in dependency dictionary format, but
+[networkx](https://github.com/networkx/networkx) Digraphs are also
+supported.
+
+```python
+>>> import graph_scheduler
+
+>>> graph = {
+    'A': set(),
+    'B': {'A'},
+    'C': {'A'},
+    'D': {'B', 'C'},
+}
+
+>>> sched = graph_scheduler.Scheduler(graph=graph)
+>>> sched.add_condition('C', graph_scheduler.EveryNCalls('A', 2))
+>>> sched.add_condition('D', graph_scheduler.EveryNCalls('C', 2))
+
+>>> print(list(sched.run()))
+[{'A'}, {'B'}, {'A'}, {'C', 'B'}, {'A'}, {'B'}, {'A'}, {'C', 'B'}, {'D'}]
+```
+
+
```

### Comparing `graph-scheduler-1.1.1/src/graph_scheduler.egg-info/SOURCES.txt` & `graph-scheduler-1.1.2/src/graph_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.1/tests/scheduling/conftest.py` & `graph-scheduler-1.1.2/tests/scheduling/conftest.py`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.1/tests/scheduling/test_condition.py` & `graph-scheduler-1.1.2/tests/scheduling/test_condition.py`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.1/tests/scheduling/test_scheduler.py` & `graph-scheduler-1.1.2/tests/scheduling/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.1/tests/scheduling/test_time.py` & `graph-scheduler-1.1.2/tests/scheduling/test_time.py`

 * *Files identical despite different names*

### Comparing `graph-scheduler-1.1.1/versioneer.py` & `graph-scheduler-1.1.2/versioneer.py`

 * *Files identical despite different names*


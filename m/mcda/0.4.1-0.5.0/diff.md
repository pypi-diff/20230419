# Comparing `tmp/mcda-0.4.1.tar.gz` & `tmp/mcda-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcda-0.4.1.tar", last modified: Mon Feb 27 10:21:34 2023, max compression
+gzip compressed data, was "mcda-0.5.0.tar", last modified: Wed Apr 19 15:55:27 2023, max compression
```

## Comparing `mcda-0.4.1.tar` & `mcda-0.5.0.tar`

### file list

```diff
@@ -1,55 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:21:34.652101 mcda-0.4.1/
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-02-27 10:21:21.000000 mcda-0.4.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-02-27 10:21:21.000000 mcda-0.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1809 2023-02-27 10:21:34.652101 mcda-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-02-27 10:21:21.000000 mcda-0.4.1/README.PYPI.md
--rw-rw-rw-   0 root         (0) root         (0)     2288 2023-02-27 10:21:21.000000 mcda-0.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:21:34.638100 mcda-0.4.1/mcda/
--rw-rw-rw-   0 root         (0) root         (0)      868 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:21:34.644100 mcda-0.4.1/mcda/core/
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/core/aliases.py
--rw-rw-rw-   0 root         (0) root         (0)    13744 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/core/functions.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/core/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     8727 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/core/matrices.py
--rw-rw-rw-   0 root         (0) root         (0)    16474 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/core/performance_table.py
--rw-rw-rw-   0 root         (0) root         (0)    18792 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/core/relations.py
--rw-rw-rw-   0 root         (0) root         (0)    19797 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/core/scales.py
--rw-rw-rw-   0 root         (0) root         (0)    21193 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/core/set_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:21:34.644100 mcda-0.4.1/mcda/dea/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/dea/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:21:34.645100 mcda-0.4.1/mcda/mavt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/mavt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14794 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/mavt/aggregators.py
--rw-rw-rw-   0 root         (0) root         (0)    24114 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/mavt/uta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:21:34.647101 mcda-0.4.1/mcda/outranking/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/outranking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    32021 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/outranking/electre.py
--rw-rw-rw-   0 root         (0) root         (0)    14392 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/outranking/promethee.py
--rw-rw-rw-   0 root         (0) root         (0)    40467 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/outranking/srmp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:21:34.647101 mcda-0.4.1/mcda/plot/
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    41564 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/plot/plot.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-02-27 10:21:21.000000 mcda-0.4.1/mcda/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:21:34.640100 mcda-0.4.1/mcda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1809 2023-02-27 10:21:34.000000 mcda-0.4.1/mcda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      972 2023-02-27 10:21:34.000000 mcda-0.4.1/mcda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-27 10:21:34.000000 mcda-0.4.1/mcda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-27 10:21:34.000000 mcda-0.4.1/mcda.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       62 2023-02-27 10:21:34.000000 mcda-0.4.1/mcda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-02-27 10:21:34.000000 mcda-0.4.1/mcda.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-02-27 10:21:21.000000 mcda-0.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-27 10:21:34.652101 mcda-0.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1452 2023-02-27 10:21:21.000000 mcda-0.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 10:21:34.652101 mcda-0.4.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     8041 2023-02-27 10:21:21.000000 mcda-0.4.1/tests/test_aggregators.py
--rw-rw-rw-   0 root         (0) root         (0)    21772 2023-02-27 10:21:21.000000 mcda-0.4.1/tests/test_electre.py
--rw-rw-rw-   0 root         (0) root         (0)     5849 2023-02-27 10:21:21.000000 mcda-0.4.1/tests/test_functions.py
--rw-rw-rw-   0 root         (0) root         (0)     7568 2023-02-27 10:21:21.000000 mcda-0.4.1/tests/test_matrices.py
--rw-rw-rw-   0 root         (0) root         (0)    17667 2023-02-27 10:21:21.000000 mcda-0.4.1/tests/test_performance_table.py
--rw-rw-rw-   0 root         (0) root         (0)     9494 2023-02-27 10:21:21.000000 mcda-0.4.1/tests/test_promethee.py
--rw-rw-rw-   0 root         (0) root         (0)    11185 2023-02-27 10:21:21.000000 mcda-0.4.1/tests/test_relations.py
--rw-rw-rw-   0 root         (0) root         (0)     9394 2023-02-27 10:21:21.000000 mcda-0.4.1/tests/test_scales.py
--rw-rw-rw-   0 root         (0) root         (0)    13546 2023-02-27 10:21:21.000000 mcda-0.4.1/tests/test_set_functions.py
--rw-rw-rw-   0 root         (0) root         (0)    12821 2023-02-27 10:21:21.000000 mcda-0.4.1/tests/test_srmp.py
--rw-rw-rw-   0 root         (0) root         (0)    12100 2023-02-27 10:21:21.000000 mcda-0.4.1/tests/test_uta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:55:27.378942 mcda-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-04-19 15:55:14.000000 mcda-0.5.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-19 15:55:14.000000 mcda-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3012 2023-04-19 15:55:27.378942 mcda-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2118 2023-04-19 15:55:14.000000 mcda-0.5.0/README.PYPI.md
+-rw-rw-rw-   0 root         (0) root         (0)     2502 2023-04-19 15:55:14.000000 mcda-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:55:27.367941 mcda-0.5.0/mcda/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:55:27.374941 mcda-0.5.0/mcda/core/
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/aliases.py
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/categories.py
+-rw-rw-rw-   0 root         (0) root         (0)     6345 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/criteria_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15169 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)    21163 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/matrices.py
+-rw-rw-rw-   0 root         (0) root         (0)     8123 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/performance_table.py
+-rw-rw-rw-   0 root         (0) root         (0)    20025 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/relations.py
+-rw-rw-rw-   0 root         (0) root         (0)    20692 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/scales.py
+-rw-rw-rw-   0 root         (0) root         (0)    21193 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/set_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)    13700 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/core/values.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:55:27.374941 mcda-0.5.0/mcda/dea/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/dea/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:55:27.375941 mcda-0.5.0/mcda/mavt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/mavt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17750 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/mavt/aggregators.py
+-rw-rw-rw-   0 root         (0) root         (0)    24133 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/mavt/uta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:55:27.377941 mcda-0.5.0/mcda/outranking/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/outranking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    36397 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/outranking/electre.py
+-rw-rw-rw-   0 root         (0) root         (0)    25895 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/outranking/promethee.py
+-rw-rw-rw-   0 root         (0) root         (0)    40811 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/outranking/srmp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:55:27.378942 mcda-0.5.0/mcda/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    41564 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/plot/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-04-19 15:55:14.000000 mcda-0.5.0/mcda/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 15:55:27.369941 mcda-0.5.0/mcda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3012 2023-04-19 15:55:27.000000 mcda-0.5.0/mcda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      787 2023-04-19 15:55:27.000000 mcda-0.5.0/mcda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 15:55:27.000000 mcda-0.5.0/mcda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 15:55:27.000000 mcda-0.5.0/mcda.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-19 15:55:27.000000 mcda-0.5.0/mcda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-19 15:55:27.000000 mcda-0.5.0/mcda.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-19 15:55:14.000000 mcda-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 15:55:27.378942 mcda-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2023-04-19 15:55:14.000000 mcda-0.5.0/setup.py
```

### Comparing `mcda-0.4.1/LICENSE` & `mcda-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcda-0.4.1/README.md` & `mcda-0.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 
-Package for Multi-Criteria Decision Analysis named `mcda` (**Alpha**).
+Package for Multi-Criteria Decision Analysis named `mcda` (**Beta**).
 
 
 # Table of contents
 
 [TOC]
 
 
 # Package description
 
-This package is used as a basis to represent MCDA problems as well as solve them.
-It currently contains functionalities to accurately describe a MCDA problem.
+This package is used as a basis to represent Multi-Criteria Decision Aiding (MCDA) problems as well as solve them.
 It also contains relatively low-level plotting functions to visualize a MCDA problem and its solution.
-The repository also contains [jupyter notebooks](https://jupyter.org/) that can be used as tutorials.
 
-It is hosted on PyPI: [mcda](https://pypi.org/project/mcda/)
+It is released on PyPI as [mcda](https://pypi.org/project/mcda/).
 
-# Install
+Its documentation is available [here](https://py-mcda.readthedocs.io/).
+
+
+# Requirements
+
+To be able to plot relations and outranking graphs, this package requires that `graphviz` be installed.
+On Debian/Ubuntu this is done with:
 
-The only non-python requirement is: graphviz
-It can be installed using the following command (for Debian/Ubuntu):
 ```bash
 sudo apt-get install graphviz
 ```
 
-Package can then be installed using simply pip: `pip install mcda`
 
-It can also be installed by cloning this git, then following the instructions grouped [here](INSTALL.md) to install the package in editable mode or install its requirements for development.
+# Installation
+
+If you want to simply use this package, simply install it from [PyPI](https://pypi.org/project/mcda/):
+
+```bash
+pip install mcda
+```
+
+Once you installed our package, you can have a look at our [notebooks](examples/) section which contains examples on how to use our package.
+
+If you want to contribute to this package development, we recommend you to read [this](#contributors).
 
 
 # Documentation
 
 Documentation on this package can be found [here](https://py-mcda.readthedocs.io/).
 
 It also can be built locally by executing the following command in the package root folder:
@@ -43,28 +54,28 @@
 
 
 # Notebooks
 
 We added [jupyter notebooks](https://jupyter.org/) that can be run as examples in [examples/](examples/).
 
 
-# Developers' corner
-
-This package is [PEP8](https://www.python.org/dev/peps/pep-0008/) compliant with a maximum line length of **79**, and is statically typed using [type hints](https://docs.python.org/3/library/typing.html).
+# Contributors
 
-Documentation, unit tests and example notebooks **shall be** developed alongside the package features.
+This package is growing continuously and contributions are welcomed.
+Contributions can come in the form of new features, bug fixes, documentation improvements
+or any combination thereof.
+It can also simply come in the form of issues describing the idea for a new feature, a bug encountered, etc.
 
-A suite of linters must be set up in order to enforce those guidelines, you can use the [Makefile](Makefile) to see their parameters and options:
+If you want to contribute to this package, please read the [guidelines](https://py-mcda.readthedocs.io/en/latest/contributing.html).
+If you have any new ideas or have found bugs, feel free to [create an issue](https://gitlab.com/decide.imt-atlantique/pymcda/-/issues/new>).
+Finally, any contribution must be proposed for integration as a [Merge Request](https://gitlab.com/decide.imt-atlantique/pymcda/-/merge_requests/new).
 
-* [flake8](https://flake8.pycqa.org/en/latest/)
-* [isort](https://pycqa.github.io/isort/)
-* [black](https://pypi.org/project/black/)
-* [mypy](https://mypy.readthedocs.io/en/stable/)
 
-Changes **should not** be commited if the linters don't validate the changes and the unit tests don't run.
+# License
 
-For more details, read the [guideline](CONTRIBUTING.md).
+This software is licensed under the [European Union Public Licence (EUPL) v1.2](https://joinup.ec.europa.eu/page/eupl-text-11-12).
+For more information see [LICENSE](LICENSE).
 
 
-# Known issues
+# Citations
 
-None
+@todo write section
```

### Comparing `mcda-0.4.1/mcda/core/functions.py` & `mcda-0.5.0/mcda/core/functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,14 +45,24 @@
             self.slope = (segment[0][1] - segment[1][1]) / (
                 segment[0][0] - segment[1][0]
             )
             self.constant = (
                 segment[1][1] * segment[0][0] - segment[0][1] * segment[1][0]
             ) / (segment[0][0] - segment[1][0])
 
+    def __repr__(self) -> str:  # pragma: nocover
+        """Return string representation of function.
+
+        :return:
+        """
+        return (
+            f"{self.__class__.__name__}(constant={self.constant}, "
+            f"slope={self.slope})"
+        )
+
     def __call__(self, x: float) -> float:
         """Call affine function.
 
         :param x:
         :return: result
         """
         return self.slope * x + self.constant
@@ -81,14 +91,41 @@
                 f"Interval min value '{dmin}' bigger than max value '{dmax}'"
             )
         self.dmin = dmin
         self.dmax = dmax
         self.min_in = min_in
         self.max_in = max_in
 
+    def __hash__(self) -> int:
+        """Hash interval.
+
+        :return: hash
+        """
+        return hash(self.dmin) + hash(self.dmax)
+
+    def __str__(self) -> str:
+        """Return interval as a string.
+
+        :return:
+        """
+        return (
+            f"{'[' if self.min_in else ']'}{self.dmin}, {self.dmax}"
+            f"{']' if self.max_in else '['}"
+        )
+
+    def __repr__(self) -> str:  # pragma: nocover
+        """Return string representation of interval.
+
+        :return:
+        """
+        return (
+            f"{self.__class__.__name__}(dmin={self.dmin}, dmax={self.dmax},"
+            f"min_in={self.min_in}, max_in={self.max_in})"
+        )
+
     def is_empty(self) -> bool:
         """Check if interval is empty.
 
         :return: ``True`` if interval is empty, ``False`` otherwise.
         """
         return self.dmin == self.dmax and (not self.min_in or not self.max_in)
 
@@ -235,99 +272,120 @@
         :return:
         :raises IndexError: if `x` is not in `values`
         """
         if x not in self.values:
             raise IndexError(f"discrete value '{x}' unknown")
         return self.values[x]
 
+    def __repr__(self) -> str:  # pragma: nocover
+        """Return string representation of function.
+
+        :return:
+        """
+        return f"{self.__class__.__name__}(values={self.values})"
+
     def __call__(self, x: Any) -> Any:
         """Apply function to single value.
 
         :param x:
         :return:
         :raises IndexError: if `x` is not in `values`
         """
         return self.apply(x)
 
 
 class PieceWiseFunction:
     """This class implements piecewise MCDA function.
 
-    :param intervals: functions definition intervals
     :param functions:
     :param segments: list of segments defining piecewise linear functions
-    :raises ValueError: if number of intervals and functions are different
 
     .. note::
         * first matching interval is used to return result
         * each segment of `segments` is a list of two points, each point a
           sequence of numeric abscissa, a numeric ordinate and a :class:`bool`
           indicating if the point is included in the underlying interval
     """
 
     _TYPE = "PieceWiseFunction"
 
     def __init__(
         self,
-        intervals: List[Interval] = None,
-        functions: List[NumericFunction] = None,
+        functions: Dict[Interval, NumericFunction] = None,
         segments: List[List[List]] = None,
     ):
         """Constructor method"""
-        intervals = [] if intervals is None else intervals
-        functions = [] if functions is None else functions
         segments = [] if segments is None else segments
-        if len(intervals) != len(functions):
-            raise ValueError(
-                f"{self._TYPE} must have as many intervals as functions"
-            )
-        self.intervals = intervals
-        self.functions = functions
+        self.functions = {} if functions is None else functions
         self._parse_segments(segments=segments)
 
+    @property
+    def intervals(self) -> List[Interval]:
+        return list(self.functions.keys())
+
+    def __str__(self) -> str:
+        """Return string representation of functions.
+
+        :return:
+        """
+        _functions = {
+            str(interval): str(f) for interval, f in self.functions.items()
+        }
+        return str(_functions)
+
+    def __repr__(self) -> str:  # pragma: nocover
+        """Return string representation of piecewise function.
+
+        :return:
+        """
+        return f"{self.__class__.__name__}(functions={repr(self.functions)})"
+
     def _parse_segments(self, segments: List[List[List]]):
         """Parse segments and populate intervals and functions.
 
         Each segment of `segments` is a list of two points, each point a
         sequence of numeric abscissa, a numeric ordinate and a :class:`bool`
         indicating if the point is included in the underlying interval.
 
         :param segments:
         """
         for seg in segments:
             a = seg[0] if len(seg[0]) > 2 else seg[0] + [True]
             b = seg[1] if len(seg[1]) > 2 else seg[1] + [True]
-            self.intervals.append(Interval(a[0], b[0], a[2], b[2]))
-            self.functions.append(AffineFunction(segment=seg))
+            self.functions[Interval(a[0], b[0], a[2], b[2])] = AffineFunction(
+                segment=seg
+            )
 
     def continuous(self) -> bool:
         """Check intervals and functions are ordered and continuous.
 
         :return:
         """
         if len(self.intervals) <= 1:
             return True
-        for i in range(len(self.intervals) - 1):
-            if not self.intervals[i].continuous(self.intervals[i + 1]):
+        for interval, successor in zip(
+            self.intervals[:-1], self.intervals[1:]
+        ):
+            if not interval.continuous(successor):
                 return False
             if not math.isclose(
-                self.functions[i](self.intervals[i].dmax),
-                self.functions[i + 1](self.intervals[i + 1].dmin),
+                self.functions[interval](interval.dmax),
+                self.functions[successor](successor.dmin),
             ):
                 return False
         return True
 
     def apply(self, x: float) -> float:
         """Apply function to single value.
 
         :param x:
         :raises ValueError: if `x` is not inside an interval
         :return:
         """
-        for interval, f in zip(self.intervals, self.functions):
+        for interval, f in self.functions.items():
             if x in interval:
                 return f(x)
         raise ValueError(
             f"cannot apply piecewise function to out-of-bound value: {x}"
         )
 
     def __call__(self, x: float) -> float:
@@ -376,16 +434,15 @@
                     "FuzzyNumber abscissa must be in increasing order"
                 )
             if x1 < x2:
                 segments.append([[x1, y1], [x2, y2]])
         if len(segments) == 0:
             PieceWiseFunction.__init__(
                 self,
-                [Interval(self.abscissa[0], self.abscissa[0])],
-                [lambda x: 1],
+                {Interval(self.abscissa[0], self.abscissa[0]): lambda x: 1},
             )
         else:
             PieceWiseFunction.__init__(self, segments=segments)
 
     def __eq__(self, other) -> bool:
         """Test equality of objects.
 
@@ -393,26 +450,33 @@
         :return:
         """
         if type(other) != type(self):
             return False
         _fuzzy = cast(FuzzyNumber, other)
         return self.abscissa == _fuzzy.abscissa
 
+    def __repr__(self) -> str:  # pragma: nocover
+        """Return string representation of fuzzy number.
+
+        :return:
+        """
+        return f"{self.__class__.__name__}(abscissa={self.abscissa})"
+
     def apply(self, x: float) -> float:
         """Apply function to single value.
 
         :param x:
         :return:
 
         .. note:: returns ``0`` if value is not in the fuzzy set
         """
-        for interval, f in zip(self.intervals, self.functions):
-            if x in interval:
-                return f(x)
-        return 0
+        try:
+            return super().apply(x)
+        except ValueError:
+            return 0
 
     @property
     def average(self) -> float:
         """Computes the average of all intervals boundaries.
 
         :return:
         """
```

### Comparing `mcda-0.4.1/mcda/core/performance_table.py` & `mcda-0.5.0/mcda/core/values.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
-from typing import Any, Dict, Iterator, List, Union, cast
+from collections.abc import ItemsView, KeysView, ValuesView
+from typing import Any, Dict, Generic, Iterator, List, TypeVar, cast
 
-from pandas import DataFrame, Series
+from pandas import Series
 from pandas.api.types import is_numeric_dtype  # type: ignore
 
-from mcda.core.aliases import Function
-from mcda.core.matrices import Matrix
-from mcda.core.scales import (
-    NominalScale,
-    PreferenceDirection,
-    QuantitativeScale,
-    Scale,
+from .relations import (
+    IndifferenceRelation,
+    IPreferenceStructure,
+    PreferenceRelation,
+    PreferenceStructure,
+    Relation,
 )
+from .scales import NominalScale, PreferenceDirection, QuantitativeScale, Scale
 
 
 def series_equals(s1: Series, s2: Series) -> bool:
     """Check if two series have the same values.
 
     It will realign the indexes if they are ordered differently.
 
@@ -195,42 +196,82 @@
     def is_within_scales(self) -> bool:
         """Check whether all values are within their respective scales.
 
         :return:
         """
         return self.within_scales.data.all()
 
-    def transform_to(
-        self, out_scales: Dict[Any, Scale] | Scale
-    ) -> "ScaleValues":
+    def dominate(self, other: ScaleValues) -> bool:
+        """Check whether the scale values dominates an other one.
+
+        :param other:
+        :return:
+            ``True`` if this object dominates ``other``, ``False`` otherwise
+
+        .. note:: if :attr:`scales` are not quantitative, ``False`` is returned
+        """
+        _other = other.transform(self.scales)
+        strict_dominance = False
+        for criterion, scale in self.scales.items():
+            if not isinstance(scale, QuantitativeScale):
+                return False
+            _scale = cast(QuantitativeScale, scale)
+            if _scale.is_better(_other.data[criterion], self.data[criterion]):
+                return False
+            if _scale.is_better(self.data[criterion], _other.data[criterion]):
+                strict_dominance = True
+        return strict_dominance
+
+    def dominate_strongly(self, other: ScaleValues) -> bool:
+        """Check whether the scale values dominates strongly an other one.
+
+        :param other:
+        :return:
+            ``True`` if this object dominates strongly ``other``, ``False``
+            otherwise
+
+        .. note:: if :attr:`scales` are not quantitative, ``False`` is returned
+        """
+        _other = other.transform(self.scales)
+        for criterion, scale in self.scales.items():
+            if not isinstance(scale, QuantitativeScale):
+                return False
+            _scale = cast(QuantitativeScale, scale)
+            if not _scale.is_better(
+                self.data[criterion], _other.data[criterion]
+            ):
+                return False
+        return True
+
+    def transform(self, out_scales: Dict[Any, Scale] | Scale) -> "ScaleValues":
         """Return data transformed to the target scales.
 
         :return:
         """
         out_scales = (
             {k: out_scales for k in self.labels}
             if isinstance(out_scales, Scale)
             else out_scales
         )
         return ScaleValues(
             Series(
                 {
-                    k: self.scales[k].transform_to(v, out_scales[k])
+                    k: self.scales[k].transform(v, out_scales[k])
                     for k, v in self.data.items()
                 }
             ),
             out_scales,
         )
 
     def normalize(self) -> "ScaleValues":
         """Return normalized data.
 
         :return:
         """
-        return self.transform_to(QuantitativeScale.normal())
+        return self.transform(QuantitativeScale.normal())
 
     def sort(self, reverse: bool = False) -> "ScaleValues":
         """Return sorted data in new instance.
 
         Normalized data are used to determine the sorting order.
 
         :param reverse: if ``True``, will sort in ascending order
@@ -244,18 +285,18 @@
         return copy
 
     def copy(self) -> "ScaleValues":
         """Return a copy of the object"""
         return ScaleValues(self.data.copy(), self.scales.copy())
 
 
-class Scores(ScaleValues):
-    """This class describes a scores as a :class:`ScaleValues`.
+class Ranking(ScaleValues, IPreferenceStructure):
+    """This class describes a ranking as a :class:`ScaleValues`.
 
-    It is intended as a shorthand to create scores.
+    It is intended as a shorthand to create rankings.
 
     :param data:
     :param preference_direction:
     :raise ValueError: if `data` contains non-numeric values
 
     :attr data: internal representation of data
     :attr scales:
@@ -270,278 +311,148 @@
         preference_direction: PreferenceDirection = PreferenceDirection.MAX,
     ):
         self.preference_direction = preference_direction
         if not is_numeric_dtype(data):
             raise ValueError(f"{self.__class__} only supports numeric values")
         super().__init__(data=data, preference_direction=preference_direction)
 
-    def copy(self) -> "Scores":
-        """Return a copy of the object"""
-        return Scores(self.data.copy(), self.preference_direction)
-
-
-class PerformanceTable(Matrix):
-    """This class is used to represent performance tables.
-
-    :param data: performance table in an array-like or dict structure
-    :param scales: criteria scales (scales are inferred from data if not set)
-    :param alternatives:
-    :param criteria:
-
-    :attr df: dataframe containing the performances
-    :attr scales: criteria scales
-
-    .. note::
-        when applying pandas methods to modify the performance table, do it
-        this way: `table.df = table.df.method()` (for a method called `method`)
-
-        Also you may want to modify the criteria scales depending on such
-        modifications.
-    """
-
-    def __init__(
-        self,
-        data,
-        scales: Dict[Any, Scale] = None,
-        alternatives: List[Any] = None,
-        criteria: List[Any] = None,
-    ):
-        df = DataFrame(data, index=alternatives, columns=criteria)
-        super().__init__(df)
-        self.scales = self.bounds if scales is None else scales
-
-    def __eq__(self, other) -> bool:
-        """Check equality of performance tables.
-
-        Equality is defines as having the same set of scales, and having the
-        same dataframe.
-
-        :return: ``True`` if both are equal
-        """
-        if not isinstance(other, PerformanceTable):
-            return False
-        _table = cast(PerformanceTable, other)
-        if self.scales == _table.scales:
-            return super().__eq__(_table)
-        return False
-
-    @property
-    def criteria(self) -> List[Any]:
-        """Return performance table criteria"""
-        return self.df.columns.tolist()
-
-    @property
-    def alternatives(self) -> List[Any]:
-        """Return performance table alternatives"""
-        return self.df.index.tolist()
-
     @property
-    def alternatives_values(self) -> Iterator[ScaleValues]:
-        """Iterator on the table alternatives values"""
-        for alternative in self.alternatives:
-            yield self.get_alternative_values(alternative)
+    def preference_structure(self) -> "PreferenceStructure":
+        """Convert ranking into preference structure.
 
-    @property
-    def criteria_values(self) -> Iterator[ScaleValues]:
-        """Iterator on the table criteria values"""
-        for criterion in self.criteria:
-            yield self.get_criterion_values(criterion)
+        :return:
 
-    @property
-    def is_numeric(self) -> bool:
-        """Check whether performance table is numeric.
+        .. note::
+            The minimum number of relations representing the scores is returned
+            (w.r.t transitivity of preference and indifference relations)
+        """
+        res: List[Relation] = []
+        sorted_scores = self.sort()
+        for a, b in zip(sorted_scores.labels[:-1], sorted_scores.labels[1:]):
+            if sorted_scores[a] == sorted_scores[b]:
+                res.append(IndifferenceRelation(a, b))
+            else:
+                res.append(PreferenceRelation(a, b))
+        return PreferenceStructure(res)
+
+    @classmethod
+    def _from_preference_structure(
+        cls, preference_structure: "PreferenceStructure"
+    ) -> "Ranking":
+        """Convert preference structure to ranking.
+
+        :param preference_structure:
+        :raises ValueError: if `preference_structure` is not a total pre-order
+        :return:
+
+        .. note:: returned ranking goes for 1 to n (with 1 the best rank)
+        """
+        if not preference_structure.is_total_preorder:
+            raise ValueError(
+                "only total pre-order can be represented as Ranking"
+            )
+        s = Series(1, index=preference_structure.elements)
+        pref_copy = preference_structure.transitive_closure
+        while len(pref_copy.elements) > 0:
+            bad_alternatives = set()
+            for r in PreferenceStructure(pref_copy[PreferenceRelation]):
+                bad_alternatives.add(r.b)
+            s[[*bad_alternatives]] += 1
+            for a in set(pref_copy.elements) - bad_alternatives:
+                del pref_copy[a]
+        return Ranking(s, preference_direction=PreferenceDirection.MIN)
+
+    @classmethod
+    def cast_from(cls, data: "IPreferenceStructure") -> "Ranking":
+        """Convert any preference structure subclass instance to current type.
 
+        :param data: instance of a preference structure subclass
         :return:
-        :rtype: bool
         """
-        for col in self.df.columns:
-            if not is_numeric_dtype(self.df[col]):
-                return False
-        return True
+        return cls._from_preference_structure(data.preference_structure)
 
-    @property
-    def bounds(self) -> Dict[Any, Scale]:
-        """Return criteria scales inferred from performance table values.
+    def copy(self) -> "Ranking":
+        """Return a copy of the object"""
+        return Ranking(self.data.copy(), self.preference_direction)
 
-        .. note::
-            will always assume maximizable quantitative scales for numeric
-            criteria and nominal scales for others
-        """
-        return {
-            criterion: ScaleValues(self.df[criterion]).bounds
-            for criterion in self.criteria
-        }
 
-    def get_alternative_values(self, alternative: Any) -> ScaleValues:
-        """Get performances associated to an alternative.
+T = TypeVar("T")
 
-        :param alternative: alternative label
-        :return:
-        """
-        return ScaleValues(self.df.loc[alternative], self.scales)
 
-    def get_criterion_values(self, criterion: Any) -> ScaleValues:
-        """Get performances associated to a criterion.
+class Container(Generic[T]):
+    """This generic class is a container accessible and traversable as a dict
+    or a list.
 
-        :param criterion: criterion label
-        :return:
-        """
-        return ScaleValues(self.df[criterion], self.scales[criterion])
+    :param values:
+    """
 
-    def get_alternative_values_at(self, index: int) -> ScaleValues:
-        """Get performances associated to an alternative index.
+    def __init__(self, values: Dict[Any, T]):
+        self._values = values
 
-        :param index: alternative index
-        :return:
+    def __contains__(self, key: Any) -> bool:
+        """Check if `key` is in container.
+
+        :param key:
+        :return: ``true`` if `key` in container, ``False`` otherwise
         """
-        return ScaleValues(self.df.iloc[index], self.scales)
+        return key in self._values
 
-    def get_criterion_values_at(self, index: int) -> ScaleValues:
-        """Get performances associated to a criterion index.
+    def __len__(self) -> int:
+        """Return length of container.
 
-        :param index: criterion index
         :return:
         """
-        return ScaleValues(
-            self.df.iloc[:, index], self.scales[self.criteria[index]]
-        )
+        return len(self._values)
 
-    def apply_criteria_functions(
-        self, functions: Dict[Any, Function]
-    ) -> "PerformanceTable":
-        """Apply criteria functions to performance table and return result.
+    def __getitem__(self, key: Any) -> T:
+        """Get value by key.
 
-        :param functions: functions identified by their criterion
-        :return:
+        :param key:
+        :return: value if found
         """
-        return PerformanceTable(
-            self.df.apply(
-                lambda col: col.apply(functions.get(col.name, lambda x: x))
-            ),
-            self.scales,
-        )
-
-    def apply_criteria_weights(
-        self,
-        criteria_weights: Dict[Any, float],
-    ) -> "PerformanceTable":
-        """Apply criteria weights to a performance table and return result.
-
-        :param criteria_weights: weights identified by their criterion
-        :return:
-        """
-        return self.apply_criteria_functions(
-            {
-                criterion: (
-                    cast(
-                        Function,
-                        lambda x, w=criterion_weight: w * cast(float, x),
-                    )
-                )
-                for criterion, criterion_weight in criteria_weights.items()
-            },
-        )
+        return self._values[key]
 
-    @property
-    def within_criteria_scales(self) -> "PerformanceTable":
-        """Return a table indicating which performances are within their
-        respective criterion scale.
+    def __iter__(self) -> Iterator[T]:
+        """Return a list-like iterator on the container values.
 
         :return:
+        :yield: a contained value
         """
-        return self.apply_criteria_functions(
-            {
-                criterion: cast(
-                    Function, lambda x, c=criterion: x in self.scales[c]
-                )
-                for criterion in self.scales.keys()
-            },
-        )
+        return iter(self._values.values())
 
     @property
-    def is_within_criteria_scales(self) -> bool:
-        """Check whether all cells are within their respective criteria scales.
+    def at(self) -> List[T]:
+        """Return container as a list.
 
         :return:
         """
-        return self.within_criteria_scales.df.all(None)
-
-    def transform(
-        self,
-        out_scales: Dict[Any, Scale],
-    ) -> "PerformanceTable":
-        """Transform performances table between scales.
-
-        :param out_scales: target criteria scales
-        :return: transformed performance table
-        """
-        functions = {
-            criterion: (
-                cast(
-                    Function,
-                    lambda x, c=criterion: self.scales[c].transform_to(
-                        x, out_scales[c]
-                    ),
-                )
-            )  # https://bugs.python.org/issue13652
-            for criterion in self.scales.keys()
-        }
-        return PerformanceTable(
-            self.apply_criteria_functions(functions).df, out_scales
-        )
+        return list(self)
 
-    def normalize_without_scales(self) -> "PerformanceTable":
-        """Normalize performance table using criteria values bounds.
+    def keys(self) -> KeysView[Any]:
+        """Return container keys.
 
         :return:
-        :raise TypeError: if performance table is not numeric
+        :yield: key
         """
-        return PerformanceTable(self.df).normalize()
+        return self._values.keys()
 
-    def normalize(self) -> "PerformanceTable":
-        """Normalize performance table using criteria scales.
+    def values(self) -> ValuesView[T]:
+        """Return container values.
 
         :return:
+        :yield: value
         """
-        return self.transform(
-            {
-                criterion: QuantitativeScale.normal()
-                for criterion in self.criteria
-            }
-        )
-
-    def sum(self, axis: int = None) -> Union[Series, float]:
-        """Sum performances.
-
-        Behaviour depends on `axis` value:
+        return self._values.values()
 
-        * ``0``: returns column sums as a list
-        * ``1``: returns row sums as a list
-        * else: returns sum on both dimension as a numeric value
+    def items(self) -> ItemsView[Any, T]:
+        """Return container items as (key, value) pairs.
 
-        :param axis: axis on which the sum is made
         :return:
-
-        .. note::
-            Non-numeric values are simply ignored as well as non-numeric sums
         """
-        if axis is not None:
-            return self.df.sum(axis=axis, numeric_only=True)
-        return self.df.sum(numeric_only=True).sum()
+        return self._values.items()
 
-    def subtable(
-        self, alternatives: List[Any] = None, criteria: List[Any] = None
-    ) -> "PerformanceTable":
-        """Return the subtable containing given alternatives and criteria.
+    def to_dict(self) -> Dict[Any, T]:
+        """Return a copy of internal container dictionary.
 
-        :param alternatives:
-        :param criteria:
         :return:
         """
-        alternatives = (
-            self.alternatives if alternatives is None else alternatives
-        )
-        criteria = self.criteria if criteria is None else criteria
-        return self.__class__(
-            self.df.loc[alternatives, criteria],
-            {criterion: self.scales[criterion] for criterion in criteria},
-        )
+        return self._values.copy()
```

### Comparing `mcda-0.4.1/mcda/core/relations.py` & `mcda-0.5.0/mcda/core/relations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-from abc import ABC
+from abc import ABC, abstractmethod
 from inspect import isclass
 from typing import Any, Dict, Iterator, List, Tuple, Union, cast
 
 from graphviz import Digraph
 from numpy import fill_diagonal
-from pandas import DataFrame, Series
+from pandas import DataFrame
 
-from mcda.core.matrices import BinaryAdjacencyMatrix
-
-from .performance_table import Scores
-from .scales import PreferenceDirection
+from .matrices import BinaryAdjacencyMatrix
 
 
 class Relation(ABC):
     """This class represents a pairwise relation between two elements.
 
     :param a: first element
     :param b: second element
@@ -27,21 +24,28 @@
     DRAW_STYLE: Dict[str, Any] = {"style": "invis"}
 
     def __init__(self, a: Any, b: Any):
         self.a = a
         self.b = b
         self.validate()
 
-    def __repr__(self) -> str:
-        """Return representation of object.
+    def __str__(self) -> str:
+        """Return string representation of object.
 
         :return:
         """
         return f"{self.a} {self._RELATION_TYPE} {self.b}"
 
+    def __repr__(self) -> str:  # pragma: nocover
+        """Return representation of object.
+
+        :return:
+        """
+        return f"{self.__class__.__name__}({self.a}, {self.b})"
+
     @property
     def elements(self) -> Tuple[Any, Any]:
         """Return elements of the relation"""
         return self.a, self.b
 
     def validate(self):
         """Check whether a relation is valid or not."""
@@ -211,17 +215,57 @@
         """
         if self.a == self.b:
             raise ValueError(
                 f"Incomparable relations are irreflexive: {self.a} == {self.b}"
             )
 
 
-class PreferenceStructure:
+class IPreferenceStructure(ABC):
+    """This interface describes preference structures.
+
+    It enables conversion between any type of preference structure through
+    defined conversions from and to a :class:`PreferenceStructure`.
+    """
+
+    @property
+    @abstractmethod
+    def preference_structure(self) -> "PreferenceStructure":  # pragma: nocover
+        """Convert object to :class:`PreferenceStructure`"""
+        pass
+
+    @classmethod
+    @abstractmethod
+    def _from_preference_structure(
+        cls, preference_structure: "PreferenceStructure"
+    ) -> "IPreferenceStructure":  # pragma: nocover
+        """Convert a :class:`PreferenceStructure` to current class.
+
+        :param preference_structure:
+        :return:
+        """
+        pass
+
+    @classmethod
+    def cast_from(
+        cls, data: "IPreferenceStructure"
+    ) -> "IPreferenceStructure":  # pragma: nocover
+        """Convert any preference structure subclass instance to current type.
+
+        :param data: instance of a preference structure subclass
+        :return:
+        """
+        return cls._from_preference_structure(data.preference_structure)
+
+
+class PreferenceStructure(IPreferenceStructure):
     """This class represents a list of relations.
 
+    Any type of relations is accepted, so this represents the union of P, I and
+    R.
+
     :param data:
     """
 
     def __init__(
         self,
         data: Union[List[Relation], Relation, "PreferenceStructure"] = None,
     ):
@@ -232,14 +276,43 @@
             relations = data.relations
         else:
             relations = data
         self._relations = list(set(relations))
         self.validate()
 
     @property
+    def preference_structure(self) -> "PreferenceStructure":
+        """Return current preference structure.
+
+        .. note::
+            necessary for implementing interface :class:`IPreferenceStructure`
+        """
+        return self
+
+    @classmethod
+    def _from_preference_structure(
+        cls, preference_structure: "PreferenceStructure"
+    ) -> "PreferenceStructure":
+        """Return copy of current preference structure.
+
+        .. note::
+            necessary for implementing interface :class:`IPreferenceStructure`
+        """
+        return cls(preference_structure)
+
+    @classmethod
+    def cast_from(cls, data: "IPreferenceStructure") -> "PreferenceStructure":
+        """Convert any preference structure subclass instance to current type.
+
+        :param data: instance of a preference structure subclass
+        :return:
+        """
+        return cls._from_preference_structure(data.preference_structure)
+
+    @property
     def elements(self) -> List[Any]:
         """Return elements present in relations list."""
         return list(set(e for r in self._relations for e in r.elements))
 
     @property
     def relations(self) -> List[Relation]:
         """Return copy of relations list."""
@@ -293,20 +366,27 @@
     def __len__(self) -> int:
         """Return number of relations in the preference structure.
 
         :return:
         """
         return len(self._relations)
 
-    def __repr__(self) -> str:
+    def __str__(self) -> str:
+        """Return string representation of relations.
+
+        :return:
+        """
+        return "[" + ", ".join([str(r) for r in self._relations]) + "]"
+
+    def __repr__(self) -> str:  # pragma: nocover
         """Return representation of relations contained in structure
 
         :return:
         """
-        return self._relations.__repr__()
+        return f"{self.__class__.__name__}({repr(self._relations)})"
 
     def _relation(
         self,
         *args: Any,
     ) -> Union[Relation, "PreferenceStructure", None]:
         """Return all relations between given elements of given types.
 
@@ -418,94 +498,36 @@
 
     @property
     def transitive_closure(self) -> "PreferenceStructure":
         """Apply transitive closure to preference structure and return result.
 
         .. warning:: Does not check for a valid preference structure!
         """
-        return self.from_outranking_matrix(
-            cast(OutrankingMatrix, self.outranking_matrix.transitive_closure)
+        return PreferenceStructure.cast_from(
+            cast(
+                OutrankingMatrix,
+                OutrankingMatrix.cast_from(self).transitive_closure,
+            )
         )
 
     @property
     def transitive_reduction(self) -> "PreferenceStructure":
         """Apply transitive reduction to preference structure and return result
 
         .. warning:: Does not check for a valid preference structure!
 
         .. warning:: This function may bundle together multiple elements
         """
-        return self.from_outranking_matrix(
-            cast(OutrankingMatrix, self.outranking_matrix.transitive_reduction)
+        return PreferenceStructure.cast_from(
+            cast(
+                OutrankingMatrix,
+                OutrankingMatrix.cast_from(self).transitive_reduction,
+            )
         )
 
-    @property
-    def outranking_matrix(self) -> "OutrankingMatrix":
-        """Return corresponding outranking matrix."""
-        elements = self.elements
-        matrix = DataFrame(0, index=elements, columns=elements)
-        fill_diagonal(matrix.values, 1)
-        for r in self._relations:
-            a, b = r.elements
-            if isinstance(r, PreferenceRelation):
-                matrix.loc[matrix.index == a, matrix.columns == b] = 1
-            if isinstance(r, IndifferenceRelation):
-                matrix.loc[matrix.index == a, matrix.columns == b] = 1
-                matrix.loc[matrix.index == b, matrix.columns == a] = 1
-        return OutrankingMatrix(matrix)
-
-    @classmethod
-    def from_outranking_matrix(
-        cls, matrix: "OutrankingMatrix"
-    ) -> "PreferenceStructure":
-        """Transform an outranking matrix to a preference structure.
-
-        :param matrix: the matrix of relations
-        :return: preference structure
-        """
-        relations: List[Relation] = list()
-        for ii, i in enumerate(matrix.vertices):
-            for j in matrix.vertices[ii + 1 :]:
-                if matrix.df.loc[
-                    matrix.df.index == i, matrix.df.columns == j
-                ].all(None):
-                    if matrix.df.loc[
-                        matrix.df.index == j, matrix.df.columns == i
-                    ].all(None):
-                        relations.append(IndifferenceRelation(i, j))
-                    else:
-                        relations.append(PreferenceRelation(i, j))
-                elif matrix.df.loc[
-                    matrix.df.index == j, matrix.df.columns == i
-                ].all(None):
-                    relations.append(PreferenceRelation(j, i))
-                else:
-                    relations.append(IncomparableRelation(i, j))
-        return cls(relations)
-
-    @classmethod
-    def from_scores(cls, scores: Scores) -> "PreferenceStructure":
-        """Convert scores into preference structure.
-
-        :param scores: alternatives' score
-        :return:
-
-        .. note::
-            The minimum number of relations representing the scores is returned
-            (w.r.t transitivity of preference and indifference relations)
-        """
-        res: List[Relation] = []
-        sorted_scores = scores.sort()
-        for a, b in zip(sorted_scores.labels[:-1], sorted_scores.labels[1:]):
-            if sorted_scores[a] == sorted_scores[b]:
-                res.append(IndifferenceRelation(a, b))
-            else:
-                res.append(PreferenceRelation(a, b))
-        return cls(res)
-
     def plot(self, relation_types: List = None) -> Digraph:
         """Create a graph for list of relation.
 
         This function creates a Graph using graphviz and display it.
         """
         relation_types = (
             [PreferenceRelation, IndifferenceRelation]
@@ -528,77 +550,93 @@
         """Copy preference structure into new object.
 
         :return: copy
         """
         return PreferenceStructure(self)
 
 
-class OutrankingMatrix(BinaryAdjacencyMatrix):
+class OutrankingMatrix(BinaryAdjacencyMatrix, IPreferenceStructure):
     """This class implements an outranking matrix as an adjacency matrix.
 
     The outranking matrix is represented internally by a
     :class:`pandas.DataFrame` with vertices as the indexes and columns.
 
     :param data: adjacency matrix in an array-like or dict-structure
     :param vertices:
 
-    :attribute df: dataframe containing the adjacency matrix
+    :raise ValueError: if non-binary values are in the matrix
+    :raise ValueError: if columns and rows have different sets of labels
     """
 
     @property
     def preference_structure(self) -> PreferenceStructure:
         """Return corresponding preference structure."""
-        return PreferenceStructure.from_outranking_matrix(self)
+        relations: List[Relation] = list()
+        for ii, i in enumerate(self.vertices):
+            for j in self.vertices[ii + 1 :]:
+                if self.data.loc[
+                    self.data.index == i, self.data.columns == j
+                ].all(None):
+                    if self.data.loc[
+                        self.data.index == j, self.data.columns == i
+                    ].all(None):
+                        relations.append(IndifferenceRelation(i, j))
+                    else:
+                        relations.append(PreferenceRelation(i, j))
+                elif self.data.loc[
+                    self.data.index == j, self.data.columns == i
+                ].all(None):
+                    relations.append(PreferenceRelation(j, i))
+                else:
+                    relations.append(IncomparableRelation(i, j))
+        return PreferenceStructure(relations)
 
     @classmethod
-    def from_preference_structure(
+    def _from_preference_structure(
         cls, preference_structure: PreferenceStructure
     ) -> "OutrankingMatrix":
         """Transform a preference structure into an outranking matrix.
 
         :param preference_structure: the matrix of relations
         :return: outranking matrix
         """
-        return preference_structure.outranking_matrix
+        elements = preference_structure.elements
+        matrix = DataFrame(0, index=elements, columns=elements)
+        fill_diagonal(matrix.values, 1)
+        for r in preference_structure:
+            a, b = r.elements
+            if isinstance(r, PreferenceRelation):
+                matrix.loc[matrix.index == a, matrix.columns == b] = 1
+            if isinstance(r, IndifferenceRelation):
+                matrix.loc[matrix.index == a, matrix.columns == b] = 1
+                matrix.loc[matrix.index == b, matrix.columns == a] = 1
+        return OutrankingMatrix(matrix)
 
     @classmethod
-    def from_ranked_categories(cls, categories: List[List[Any]]):
+    def cast_from(cls, data: "IPreferenceStructure") -> "OutrankingMatrix":
+        """Convert any preference structure subclass instance to current type.
+
+        :param data: instance of a preference structure subclass
+        :return:
+        """
+        return cls._from_preference_structure(data.preference_structure)
+
+    @classmethod
+    def from_ordered_alternatives_groups(
+        cls, categories: List[List[Any]]
+    ) -> "OutrankingMatrix":
         """Convert a ranking of categories of alternatives into an outranking
         matrix.
 
         :param categories:
             the ranked categories (each category is a list of alternatives)
         :return: outranking matrix
         """
 
         alternatives = [a for ll in categories for a in ll]
         res = cls(0, vertices=alternatives)
         for category in categories:
-            res.df.loc[category, category] = 1
-            res.df.loc[
+            res.data.loc[category, category] = 1
+            res.data.loc[
                 category, alternatives[alternatives.index(category[-1]) + 1 :]
             ] = 1
         return res
-
-
-class Ranking(Scores):
-    """This class describes a ranking as a :class:`Scores`.
-
-    It is intended as a shorthand to create rankings.
-
-    :param data:
-
-    :attr data: internal representation of data
-    :attr scales:
-        scales of the data (one per value, all equals to the same
-        :class:`mcda.core.scales.QuantitativeScale` with bounds inferred from
-        data and minimize preference direction)
-    """
-
-    def __init__(self, data: Series):
-        super().__init__(
-            data=data, preference_direction=PreferenceDirection.MIN
-        )
-
-    def copy(self) -> "Ranking":
-        """Return a copy of the object"""
-        return Ranking(self.data.copy())
```

### Comparing `mcda-0.4.1/mcda/core/scales.py` & `mcda-0.5.0/mcda/core/scales.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from abc import ABC, abstractmethod
-from enum import Enum, auto
+from enum import Enum
 from typing import Any, List, cast
 
 import numpy as np
 from pandas import Series
 from pandas.api.types import is_numeric_dtype  # type: ignore
 
 from .functions import FuzzyNumber, Interval
 
 
 class PreferenceDirection(Enum):
     """Enumeration of MCDA preference directions."""
 
-    MIN = auto()
-    MAX = auto()
+    MIN = "MIN"
+    MAX = "MAX"
 
     @classmethod
     def has_value(cls, x: "PreferenceDirection") -> bool:
         """Check if value is in enumeration.
 
         :param x:
         :return:
@@ -61,15 +61,15 @@
 
         :param nb: number of values to return
         :return:
         """
         pass
 
     @abstractmethod
-    def transform_to(
+    def transform(
         self, x: Any, target_scale: "Scale" = None
     ) -> Any:  # pragma: nocover
         """Transform value from this scale to target scale.
 
         :param x:
         :param target_scale:
         :return:
@@ -78,36 +78,43 @@
 
     def normalize(self, x: Any) -> float:
         """Normalize value.
 
         :param x:
         :return: normalized value
         """
-        return cast(float, self.transform_to(x, QuantitativeScale.normal()))
+        return cast(float, self.transform(x, QuantitativeScale.normal()))
 
     def denormalize(self, x: float) -> Any:
         """Denormalize value.
 
         :param x: normalized value
         :return: denormalized value
         """
-        return QuantitativeScale.normal().transform_to(x, self)
+        return QuantitativeScale.normal().transform(x, self)
 
 
 class NominalScale(Scale):
     """This class implements a MCDA nominal scale.
 
     :param labels:
     """
 
     def __init__(self, labels: List[Any]):
         """Constructor method"""
         Scale.__init__(self)
         self.labels = labels
 
+    def __repr__(self) -> str:  # pragma: nocover
+        """Return string representation of scale.
+
+        :return:
+        """
+        return f"{self.__class__.__name__}(labels={str(self.labels)})"
+
     def __eq__(self, other) -> bool:
         """Test equality of nominal scales.
 
         Equality is defined as being the same scale types, and having
         the same set of :attr:`labels`.
 
         :param other:
@@ -129,15 +136,15 @@
         """Return range of value from scale.
 
         :param nb: number of values to return (always ignored here)
         :return:
         """
         return self.labels
 
-    def transform_to(self, x: Any, target_scale: Scale = None) -> Any:
+    def transform(self, x: Any, target_scale: Scale = None) -> Any:
         """Transform value from this scale to target scale.
 
         :param x:
         :param target_scale:
         :return:
         :raise ValueError:
             * if value `x` is outside this scale
@@ -146,14 +153,16 @@
             if `target_scale` is neither :class:`QualitativeScale` nor
             :class:`NominalScale`
         """
         if x not in self:
             raise ValueError(f"label outside scale: {x}")
         if target_scale is None:
             raise ValueError("non-specified target scale")
+        if target_scale == self:
+            return x
         if isinstance(target_scale, NominalScale):
             return target_scale.labels[target_scale.labels.index(x)]
         raise TypeError("cannot transform from nominal to quantitative scale")
 
 
 class QuantitativeScale(Scale, Interval):
     """Class for quantitative scale.
@@ -182,14 +191,24 @@
     def normal(cls) -> "QuantitativeScale":
         """Retuen normal scale.
 
         :return:
         """
         return QuantitativeScale(0, 1)
 
+    def __repr__(self) -> str:  # pragma: nocover
+        """Return string representation of interval.
+
+        :return:
+        """
+        return (
+            f"{self.__class__.__name__}(dmin={self.dmin}, dmax={self.dmax},"
+            f"preference_direction={self.preference_direction})"
+        )
+
     def __eq__(self, other) -> bool:
         """Test equality of quantitative scales.
 
         Equality is defined as being the same scale types, having the same
         interval and :attr:`preference_direction`.
 
         :param other:
@@ -243,15 +262,15 @@
             `preference_direction` is taken into account, so preferred
             normalized value must always be bigger.
         """
         if self.preference_direction == PreferenceDirection.MIN:
             return cast(float, Interval.denormalize(self, 1 - x))
         return cast(float, Interval.denormalize(self, x))
 
-    def transform_to(self, x: Any, target_scale: Scale = None) -> Any:
+    def transform(self, x: Any, target_scale: Scale = None) -> Any:
         """Transform value from this scale to target scale.
 
         :param x:
         :param target_scale:
         :return:
         :raise ValueError:
             * if value `x` is outside this scale
@@ -262,14 +281,16 @@
 
         .. note:: `preference_direction` attributes are taken into account
         """
         if x not in self:
             raise ValueError(f"value outside scale: {x}")
         if target_scale is None:
             raise ValueError("non-specified target scale")
+        if target_scale == self:
+            return x
         _x = cast(float, x)
         if isinstance(target_scale, QualitativeScale):
             return target_scale.label_from_value(
                 target_scale._denormalize_value(self._normalize_value(_x))
             )
         if isinstance(target_scale, QuantitativeScale):
             return target_scale._denormalize_value(self._normalize_value(_x))
@@ -309,22 +330,19 @@
             else _x < _y
         )
 
 
 class QualitativeScale(QuantitativeScale, NominalScale):
     """This class implements a MCDA qualitative scale.
 
-    :param labels:
-    :param values:
+    :param values: numeric series with labels as index
     :param preference_direction: scale preference direction
     :param dmin: min boundary of scale (inferred from `values` if not set)
     :param dmax: max boundary of scale (inferred from `values` if not set)
     :raises ValueError:
-        * if number of `labels` and `values` differs
-        * if `preference_direction` is unknown
         * if at least one value is outside the bounds
     :raises TypeError:
         * if `values` contains non-numeric values
 
     .. warning::
         This scale contains `labels` not `values`. `values` are only here to
         define a corresponding quantitative scale for default scale
@@ -375,14 +393,25 @@
     @property
     def quantitative(
         self,
     ) -> QuantitativeScale:  # Property used to hide setter
         """Quantitative scale extracted from current qualitative scale."""
         return self.__quantitative
 
+    def __repr__(self) -> str:  # pragma: nocover
+        """Return string representation of interval.
+
+        :return:
+        """
+        return (
+            f"{self.__class__.__name__}(values={self.values},"
+            f"preference_direction={self.preference_direction},"
+            f"dmin={self.dmin}, dmax={self.dmax})"
+        )
+
     def __eq__(self, other) -> bool:
         """Test equality of qualitative scales.
 
         Equality is defined as having the same types, having the same set of
         :attr`labels` and corresponding :attr:`values`, and having the same
         interval and :attr:`preference_direction`.
 
@@ -412,29 +441,31 @@
         """Return range of value from scale.
 
         :param nb: number of values to return (always ignored here)
         :return:
         """
         return NominalScale.range(self, nb)
 
-    def transform_to(self, x: Any, target_scale: Scale = None) -> Any:
+    def transform(self, x: Any, target_scale: Scale = None) -> Any:
         """Transform value from this scale to target scale.
 
         :param x:
         :param target_scale:
         :return:
         :raise ValueError: if value `x` is outside this scale
         :raise TypeError: if `target_scale` has unknown type
 
         .. note::
             `preference_direction` attributes are taken into account when
             rescaling to a :class:`QuantitativeScale`
         """
         if x not in self:
             raise ValueError(f"label outside scale: {x}")
+        if target_scale == self:
+            return x
         target_scale = (
             self.quantitative if target_scale is None else target_scale
         )
         if isinstance(target_scale, NominalScale):
             return target_scale.labels[target_scale.labels.index(x)]
         if isinstance(target_scale, QuantitativeScale):
             value = self.values[x]
@@ -606,15 +637,15 @@
         :param a:
         :param b:
         :return:
         :raises ValueError: if `a` or `b` is not inside the scale
         """
         if a not in self or b not in self:
             raise ValueError("both labels must be inside the fuzzy scale")
-        labels = sorted(self.labels, key=lambda v: self.transform_to(v))
+        labels = sorted(self.labels, key=lambda v: self.transform(v))
         return abs(labels.index(a) - labels.index(b))
 
 
 def is_better(x: Any, y: Any, scale: QuantitativeScale) -> bool:
     """Check if x is better than y according to this scale
 
     :param x:
```

### Comparing `mcda-0.4.1/mcda/core/set_functions.py` & `mcda-0.5.0/mcda/core/set_functions.py`

 * *Files identical despite different names*

### Comparing `mcda-0.4.1/mcda/mavt/aggregators.py` & `mcda-0.5.0/mcda/mavt/aggregators.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,121 +1,169 @@
 """This module gathers aggregators
 """
+from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from math import log
 from typing import Any, Dict, List, Union, cast
 
 from pandas import DataFrame, Series
 
-from mcda.core.performance_table import PerformanceTable, ScaleValues
-from mcda.core.set_functions import Capacity, MobiusCapacity
-
-from ..core.aliases import NumericFunction
+from ..core.aliases import Function, NumericFunction
+from ..core.criteria_functions import CriteriaFunctions
 from ..core.functions import FuzzyNumber
-from ..core.scales import FuzzyScale, QuantitativeScale, Scale
-from ..plot.plot import Figure, LinePlot
+from ..core.interfaces import Ranker
+from ..core.performance_table import PerformanceTable
+from ..core.scales import (
+    FuzzyScale,
+    PreferenceDirection,
+    QuantitativeScale,
+    Scale,
+)
+from ..core.set_functions import Capacity, MobiusCapacity
+from ..core.values import Ranking, ScaleValues
+
+
+class Aggregator(Ranker, ABC):
+    """This abstract class represents a typical aggregator.
 
+    :param preference_direction:
+        preference direction used to order aggregation results
+    """
 
-class Aggregator(ABC):
-    """This abstract class represents a typical aggregator."""
+    def __init__(
+        self,
+        preference_direction: PreferenceDirection = PreferenceDirection.MAX,
+        **kwargs,
+    ):
+        self.preference_direction = preference_direction
 
     @abstractmethod
-    def _apply_series(
+    def _aggregate_series(
         self, series: Series, *args, **kwargs
     ) -> Any:  # pragma: nocover
         """Apply aggregation method to a pandas Series.
 
         :param series:
         """
         pass
 
-    def _apply_scale_values(
+    def _aggregate_scale_values(
         self, scale_values: ScaleValues, *args, **kwargs
     ) -> Any:
         """Apply aggregation method to a scale values object.
 
         :param scale_values:
         """
-        return self._apply_series(scale_values.data)
+        return self._aggregate_series(scale_values.data)
 
-    def _apply_dataframe(self, df: DataFrame, *args, **kwargs) -> Series:
+    def _aggregate_dataframe(self, df: DataFrame, *args, **kwargs) -> Series:
         """Apply aggregation method to a pandas DataFrame.
 
         :param df:
         :return: aggregated rows
         """
         return Series(
             {
-                alternative: self._apply_series(
+                alternative: self._aggregate_series(
                     df.loc[alternative], *args, **kwargs
                 )
                 for alternative in df.index.tolist()
             }
         )
 
-    def _apply_performance_table(
+    def _aggregate_performance_table(
         self, performance_table: PerformanceTable, *args, **kwargs
     ) -> Series:
         """Apply aggregation method to a performance table object.
 
         :param performance_table:
         :return: aggregated criteria values per alternative
         """
-        return self._apply_dataframe(performance_table.df, *args, **kwargs)
+        return self._aggregate_dataframe(
+            performance_table.data, *args, **kwargs
+        )
 
-    def __call__(
-        self, data: Union[PerformanceTable, DataFrame, Series], *args, **kwargs
+    def aggregate(
+        self,
+        data: PerformanceTable | DataFrame | Series | ScaleValues,
+        *args,
+        **kwargs,
     ) -> Any:
         """Apply aggregation method to input data.
 
         :param data:
         :return: aggregation result
 
         .. note:: aggregation is applied for each row in case of tabular data
         """
         if isinstance(data, PerformanceTable):
-            return self._apply_performance_table(data, *args, **kwargs)
+            return self._aggregate_performance_table(data, *args, **kwargs)
         if isinstance(data, DataFrame):
-            return self._apply_dataframe(data, *args, **kwargs)
+            return self._aggregate_dataframe(data, *args, **kwargs)
         if isinstance(data, ScaleValues):
-            return self._apply_scale_values(data, *args, **kwargs)
-        return self._apply_series(data, *args, **kwargs)
+            return self._aggregate_scale_values(data, *args, **kwargs)
+        return self._aggregate_series(data, *args, **kwargs)
+
+    def rank(self, performance_table: PerformanceTable, **kwargs) -> Ranking:
+        """Rank alternatives using aggregation results.
+
+        :param performance_table:
+        :return: ranking of alternatives
+        """
+        return Ranking(
+            self.aggregate(performance_table),
+            preference_direction=self.preference_direction,
+        )
 
 
 class WeightedSum(Aggregator):
     """This class represents a weighted sum aggregator.
 
     :param criteria_weights:
+        :param preference_direction:
+        preference direction used to order aggregation results
     """
 
-    def __init__(self, criteria_weights: Union[Dict[Any, float], Series]):
+    def __init__(
+        self,
+        criteria_weights: Union[Dict[Any, float], Series],
+        preference_direction: PreferenceDirection = PreferenceDirection.MAX,
+    ):
         self.criteria_weights = Series(criteria_weights)
+        super().__init__(preference_direction=preference_direction)
 
-    def _apply_series(self, series: Series, *args, **kwargs) -> float:
+    def _aggregate_series(self, series: Series, *args, **kwargs) -> float:
         """Return weighted sum of the input.
 
         :param series:
         :return:
         """
         return (series * self.criteria_weights).sum()
 
 
 class ChoquetIntegral(Aggregator):
     """This class represents a Choquet integral aggregator.
 
     :param capacity:
         capacity used for aggregation (either in regular or Möbius
         representation)
+    :param preference_direction:
+        preference direction used to order aggregation results
 
     .. note:: Implementation is based on :cite:p:`grabisch2008review`.
     """
 
-    def __init__(self, capacity: Union[Capacity, MobiusCapacity]):
+    def __init__(
+        self,
+        capacity: Union[Capacity, MobiusCapacity],
+        preference_direction: PreferenceDirection = PreferenceDirection.MAX,
+    ):
         self.capacity = capacity
+        super().__init__(preference_direction=preference_direction)
 
     def _choquet_integral_capacity(self, series: Series) -> float:
         """Return Choquet integral using a capacity.
 
         :param series:
         :return:
 
@@ -142,35 +190,42 @@
         """
         return sum(
             m * series[list(t)].min()
             for t, m in self.capacity.values.items()
             if len(t) > 0
         )
 
-    def _apply_series(self, series: Series, *args, **kwargs) -> float:
+    def _aggregate_series(self, series: Series, *args, **kwargs) -> float:
         """Return Choquet integral of the pandas Series.
 
         :param series:
         :return:
         """
         if isinstance(self.capacity, MobiusCapacity):
             return self._choquet_integral_mobius(series)
         return self._choquet_integral_capacity(series)
 
 
 class OWA(Aggregator):
     """This class represents an Ordered Weighted Aggregator (OWA).
 
     :param weights:
+    :param preference_direction:
+        preference direction used to order aggregation results
 
     .. note:: Implementation is based on :cite:p:`grabisch2008review`.
     """
 
-    def __init__(self, weights: List[float]):
+    def __init__(
+        self,
+        weights: List[float],
+        preference_direction: PreferenceDirection = PreferenceDirection.MAX,
+    ):
         self.weights = weights
+        super().__init__(preference_direction=preference_direction)
 
     @property
     def orness(self) -> float:
         """Return *orness* measure of OWA weights.
 
         :return:
 
@@ -244,15 +299,15 @@
         .. note:: quantifier as defined in :cite:p:`yager1988owa`
         """
         return [
             sum(w for w in self.weights[:i])
             for i in range(len(self.weights) + 1)
         ]
 
-    def _apply_series(self, series: Series, *args, **kwargs) -> float:
+    def _aggregate_series(self, series: Series, *args, **kwargs) -> float:
         """Return Ordered Weighted Aggregation of values.
 
         :param series:
         :return:
 
         .. note:: Implementation is based on :cite:p:`yager1988owa`
         """
@@ -303,27 +358,28 @@
 
     .. note:: implementation based on :cite:p:`isern2010ulowa`
     """
 
     def __init__(self, weights: List[float], scale: FuzzyScale):
         self.weights = weights
         self.scale = scale
+        super().__init__(preference_direction=self.scale.preference_direction)
 
     @staticmethod
     def delta(a: Any, b: Any, weight: float, scale: FuzzyScale) -> float:
         """Returns ULOWA delta value.
 
         :param a: worst value
         :param b: best value
         :param weight: ULOWA weight
         :param scale: fuzzy scale
         :return:
         """
-        xa = cast(float, scale.transform_to(a))
-        xb = cast(float, scale.transform_to(b))
+        xa = cast(float, scale.transform(a))
+        xb = cast(float, scale.transform(b))
         return xa + weight * (xb - xa)
 
     @staticmethod
     def most_similar(
         a: Any, b: Any, ref_fuzzy: FuzzyNumber, scale: FuzzyScale
     ) -> Any:
         """Returns label which fuzzy number is the most similar to the
@@ -335,26 +391,26 @@
         :param scale: fuzzy scale
         :return:
         """
         if scale.ordinal_distance(a, b) == 1:
             _labels = [a, b]
         else:
             _labels = sorted(
-                scale.labels, key=lambda v: scale.transform_to(v), reverse=True
+                scale.labels, key=lambda v: scale.transform(v), reverse=True
             )
             lmin = min(_labels.index(a), _labels.index(b))
             lmax = max(_labels.index(a), _labels.index(b))
             _labels = _labels[lmin : lmax + 1]
         sims = [
             scale.similarity(scale.fuzzy[scale.labels.index(v)], ref_fuzzy)
             for v in _labels
         ]
         return _labels[max(range(len(_labels)), key=lambda i: sims[i])]
 
-    def _apply_series(
+    def _aggregate_series(
         self, series: Series, *args, weights=None, **kwargs
     ) -> Any:
         """Returns Unbalanced Linguistic Weighted Average of values.
 
         :param values:
         :param weights:
         :return:
@@ -364,126 +420,150 @@
 
         .. warning::
             this function is intended for use with a fuzzy scale defining a
             fuzzy partition
         """
         values = sorted(
             series.tolist(),
-            key=lambda v: self.scale.transform_to(v),
+            key=lambda v: self.scale.transform(v),
             reverse=True,
         )
         weights = self.weights.copy() if weights is None else weights
         if len(values) == 0:
             raise ValueError("ULOWA needs at least one value")
         if len(values) == 1:
             return values[0]
         denominator = weights[-2] + weights[-1]
         weight = 0 if denominator == 0 else weights[-2] / denominator
         delta = self.delta(values[-1], values[-2], weight, self.scale)
         values[-2] = self.most_similar(
             values[-1], values[-2], FuzzyNumber([delta] * 4), self.scale
         )
         weights[-2] += weights[-1]
-        return self._apply_series(Series(values[:-1]), weights=weights[:-1])
+        return self._aggregate_series(
+            Series(values[:-1]), weights=weights[:-1]
+        )
 
+    def rank(self, performance_table: PerformanceTable, **kwargs) -> Ranking:
+        """Rank alternatives using aggregation results.
 
-class UtilityFunction(Aggregator):
-    """This class represents a multi-attribute utility functions aggregator.
+        :param performance_table:
+        :return: ranking of alternatives
+
+        .. note::
+            :attr:`scale` is used to transform the aggregation results to
+            numerical results
+        """
+        values = ScaleValues(
+            self.aggregate(performance_table), scales=self.scale
+        )
+        ranks = values.transform(self.scale.quantitative)
+        return Ranking(
+            ranks.data,
+            preference_direction=self.preference_direction,
+        )
+
+
+class AdditiveValueFunctions(CriteriaFunctions, Aggregator):
+    """This class represents a multi-attribute value functions aggregator.
 
     :param criteria_functions:
-    :param scales: normalized scales are used if not provided
+    :param in_scales:
+        scales used for inputs (if not provided, it will be inferred from
+        inputs)
+    :param out_scales:
+        scales used for outputs (if not provided, it will be inferred from
+        outputs)
+    :param preference_direction:
+        preference direction used to order aggregation results
 
     .. note::
         `criteria_functions` are defined for the provided scales, so when
         applying aggregation you must provide correctly scaled values (only
         :class:`mcda.api.core/performance_table.PerformanceTable`
         and :class:`mcda.api.core.performance_table.ScaleValues` are
         automatically transformed)
     """
 
     def __init__(
         self,
-        criteria_functions: Dict[Any, NumericFunction],
-        scales: Dict[Any, QuantitativeScale] = None,
+        criteria_functions: Dict[Any, NumericFunction] | CriteriaFunctions,
+        in_scales: Dict[Any, QuantitativeScale] = None,
+        out_scales: Dict[Any, QuantitativeScale] = None,
+        preference_direction: PreferenceDirection = PreferenceDirection.MAX,
     ):
-        self.criteria_functions = criteria_functions
-        self.scales = (
-            scales
-            if scales is not None
-            else {
-                c: QuantitativeScale.normal()
-                for c in criteria_functions.keys()
-            }
-        )
+        if isinstance(criteria_functions, CriteriaFunctions):
+            super().__init__(
+                criteria_functions=criteria_functions.criteria_functions,
+                in_scales=criteria_functions.in_scales,
+                out_scales=criteria_functions.out_scales,
+                preference_direction=preference_direction,
+            )
+        else:
+            super().__init__(
+                criteria_functions=cast(
+                    Dict[Any, Function], criteria_functions
+                ),
+                in_scales=cast(Dict[Any, Scale], in_scales),
+                out_scales=cast(Dict[Any, Scale], out_scales),
+                preference_direction=preference_direction,
+            )
 
-    def _apply_series(self, series: Series, *args, **kwargs) -> float:
+    def _aggregate_series(self, series: Series, *args, **kwargs) -> float:
         """Apply aggregation method to a pandas Series.
 
         :param series:
         """
-        res = Series(
-            {
-                criterion: self.criteria_functions[criterion](value)
-                for criterion, value in dict(series).items()
-            }
-        )
+        res = cast(Series, self(series))
         return res.sum()
 
-    def _apply_scale_values(
+    def _aggregate_scale_values(
         self, scale_values: ScaleValues, *args, **kwargs
     ) -> float:
         """Apply aggregation method to a scale values object.
 
         :param scale_values:
         :return: aggregated criteria values
 
         .. note::
-            `scale_values` values are transformed to utility functions `scales`
+            `scale_values` values are transformed to value functions `scales`
         """
-        return self._apply_series(
-            scale_values.transform_to(cast(Dict[Any, Scale], self.scales)).data
-        )
+        res = cast(ScaleValues, self(scale_values))
+        return res.sum()
 
-    def _apply_dataframe(self, df: DataFrame, *args, **kwargs) -> Series:
+    def _aggregate_dataframe(self, df: DataFrame, *args, **kwargs) -> Series:
         """Apply aggregation method to a pandas DataFrame.
 
         :param df:
         :return: aggregated rows
         """
-        res = cast(
-            DataFrame,
-            df.apply(
-                lambda col: col.apply(self.criteria_functions.get(col.name))
-            ),
-        )
+        res = cast(DataFrame, self(df))
         return res.sum(axis=1)
 
-    def _apply_performance_table(
+    def _aggregate_performance_table(
         self, performance_table: PerformanceTable, *args, **kwargs
     ) -> Series:
         """Apply aggregation method to a performance table object.
 
         :param performance_table:
         :return: aggregated criteria values per alternative
 
         .. note::
             `performance_table` values are transformed to utility functions
             `scales`
         """
-        return self._apply_dataframe(
-            performance_table.transform(cast(Dict[str, Scale], self.scales)).df
-        )
+        res = cast(PerformanceTable, self(performance_table))
+        return cast(Series, res.sum(axis=1))
 
-    def plot(self, nb_points=500) -> Figure:  # pragma: nocover
-        """Plot each criterion function on its respective scale.
+    @classmethod
+    def normal(
+        cls, criteria_functions: Dict[Any, NumericFunction]
+    ) -> "AdditiveValueFunctions":
+        """Return a normalized additive value functions.
 
-        :return: created figure
+        :param criteria_functions:
+        :return:
         """
-        fig = Figure(ncols=2)
-        for c, scale in self.scales.items():
-            x = cast(List[float], scale.range(nb_points))
-            y = [self.criteria_functions[c](xx) for xx in x]
-            ax = fig.create_add_axis()
-            ax.title = c
-            ax.add_plot(LinePlot(x, y))
-        fig.draw()
-        return fig
+        scales = {c: QuantitativeScale.normal() for c in criteria_functions}
+        return AdditiveValueFunctions(
+            criteria_functions, in_scales=scales, out_scales=scales
+        )
```

### Comparing `mcda-0.4.1/mcda/mavt/uta.py` & `mcda-0.5.0/mcda/mavt/uta.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,28 +9,27 @@
 from typing import Any, Dict, List, cast
 
 import numpy as np
 from pandas import Series
 from pulp import LpMaximize, LpMinimize, LpProblem, LpVariable, lpSum
 from pulp import value as pulp_value
 
-from mcda.core.performance_table import PerformanceTable, ScaleValues
-from mcda.core.relations import (
+from ..core.aliases import NumericFunction
+from ..core.functions import PieceWiseFunction
+from ..core.interfaces import Learner
+from ..core.performance_table import PerformanceTable, ScaleValues
+from ..core.relations import (
     IncomparableRelation,
     PreferenceRelation,
     PreferenceStructure,
 )
-
-from ..core.aliases import NumericFunction
-from ..core.functions import PieceWiseFunction
-from ..core.interfaces import Trainer
-from .aggregators import UtilityFunction
+from .aggregators import AdditiveValueFunctions
 
 
-class UTA(Trainer[UtilityFunction]):
+class UTA(Learner[AdditiveValueFunctions]):
     """This class represents the UTA disaggregator.
 
     :param performance_table:
     :param criteria_segments: number of segments per criteria
     :param relations: pairwise relations between alternatives
     :param delta: discrimination threshold for preference relations
     :param post_optimality: if ``True``, post-optimality is applied
@@ -95,25 +94,18 @@
 
         Objective taken from base `problem` or `post_optimality_problem`.
         """
         if self.post_optimality:
             return pulp_value(self.post_optimality_problem.objective)
         return pulp_value(self.problem.objective)
 
-    def disaggregate(self) -> UtilityFunction:
+    def disaggregate(self) -> AdditiveValueFunctions:
         """Perform disaggregation and return result.
 
-        :return: utility functions
-        """
-        return self.train()
-
-    def train(self) -> UtilityFunction:
-        """Perform disaggregation using UTA and return result.
-
-        :return: utility functions
+        :return: basic ranker with additive value functions
         """
         # Create all UTA variables
         g = self._generate_criteria_values_matrix(self.criteria_segments)
         u_var = self._generate_marginal_utility_variables(
             self.criteria_segments
         )
         sigma_var = self._generate_alternatives_errors_variables(
@@ -157,15 +149,15 @@
                 ]
                 segments = [
                     [p1, p2] for p1, p2 in zip(points[:-1], points[1:])
                 ]
                 criteria_functions[criterion] = PieceWiseFunction(
                     segments=segments
                 )
-            return UtilityFunction(criteria_functions)
+            return AdditiveValueFunctions.normal(criteria_functions)
 
         # Compute post-optimal utility functions
         max_cost = F_star * (1 + self.post_optimality_coeff)
 
         u = {
             criterion: [0.0 for _ in range(n + 1)]
             for criterion, n in self.criteria_segments.items()
@@ -223,17 +215,17 @@
             )
 
         # Compute post-optimality cost
         self.post_optimality_problem = LpProblem("Post-Optimality", LpMinimize)
         self.post_optimality_problem += lpSum(sigma_var.values())
         u_a = cast(
             Series,
-            self.performance_table.normalize()
-            .apply_criteria_functions(criteria_functions)  # type: ignore
-            .sum(axis=1),
+            AdditiveValueFunctions.normal(criteria_functions).aggregate(
+                self.performance_table
+            ),
         )
         for relation in self.relations:
             if isinstance(relation, PreferenceRelation):
                 self.post_optimality_problem += (
                     u_a[relation.a]
                     + sigma_var[relation.a]
                     - u_a[relation.b]
@@ -246,15 +238,22 @@
                     + sigma_var[relation.a]
                     - u_a[relation.b]
                     - sigma_var[relation.b]
                     == 0
                 )
         self.post_optimality_problem.solve(**self.solver_args)
 
-        return UtilityFunction(criteria_functions)
+        return AdditiveValueFunctions.normal(criteria_functions)
+
+    def learn(self) -> AdditiveValueFunctions:
+        """Perform disaggregation using UTA and return result.
+
+        :return: basic ranker with additive value functions
+        """
+        return self.disaggregate()
 
     @staticmethod
     def _generate_criteria_values_matrix(
         criteria_segments: Dict[str, int],
     ) -> Dict[Any, List[float]]:
         """Compute criteria values matrix.
 
@@ -315,23 +314,23 @@
 
         .. note:: Used by UTA algorithm
         """
         u_i_var = []
         for criterion, val in alternative_values.data.items():
             g_i = g_matrix[criterion]
             u_i = u_var[criterion]
-            for j, g_ij in enumerate(g_i[1:]):
-                if val <= g_ij:
-                    u_i_var.append(
-                        u_i[j]
-                        + (val - g_i[j])
-                        * (u_i[j + 1] - u_i[j])
-                        / (g_i[j + 1] - g_i[j])
-                    )
-                    break
+            j = 0
+            while val > g_i[j + 1]:
+                j += 1
+            u_i_var.append(
+                u_i[j]
+                + (val - g_i[j])
+                * (u_i[j + 1] - u_i[j])
+                / (g_i[j + 1] - g_i[j])
+            )
         return lpSum(u_i_var)
 
     @staticmethod
     def _add_uta_constraints(
         problem: LpProblem,
         performance_table: PerformanceTable,
         u_var: Dict[Any, List[LpVariable]],
@@ -353,15 +352,15 @@
         """
         # Preference constraints
         u_a = {}
         for relation in relations:
             for k in relation.elements:
                 if k not in u_a:
                     u_a[k] = UTA._generate_utility_variable(
-                        performance_table.get_alternative_values(k),
+                        performance_table.alternatives_values[k],
                         u_var,
                         g_matrix,
                     )
             if isinstance(relation, PreferenceRelation):
                 problem += (
                     u_a[relation.a]
                     + sigma_var[relation.a]
@@ -417,15 +416,15 @@
     .. note::
         `criteria_functions` are computed for normal scales, so when
         applying aggregation you must provide normalized values (
         :class:`mcda.api.core.PerformanceTable` alone are automatically
         normalized)
     """
 
-    def disaggregate(self) -> UtilityFunction:
+    def disaggregate(self) -> AdditiveValueFunctions:
         """Perform disaggregation using UTA\\* and return result.
 
         :return: utility functions
         """
         # Create all UTA variables
         g = self._generate_criteria_values_matrix(self.criteria_segments)
         w_var = self._generate_marginal_utility_variables(
@@ -478,15 +477,15 @@
                 ]
                 segments = [
                     [p1, p2] for p1, p2 in zip(points[:-1], points[1:])
                 ]
                 criteria_functions[criterion] = PieceWiseFunction(
                     segments=segments
                 )
-            return UtilityFunction(criteria_functions)
+            return AdditiveValueFunctions.normal(criteria_functions)
 
         # Compute post-optimal utility functions
         max_cost = F_star * (1 + self.post_optimality_coeff)
 
         w = {
             criterion: [0.0 for _ in range(n + 1)]
             for criterion, n in self.criteria_segments.items()
@@ -555,17 +554,17 @@
         # Compute post optimality cost
         self.post_optimality_problem = LpProblem("Post-Optimality", LpMinimize)
         self.post_optimality_problem += lpSum(sigma_p_var.values()) + lpSum(
             sigma_n_var.values()
         )
         u_a = cast(
             Series,
-            self.performance_table.normalize()
-            .apply_criteria_functions(criteria_functions)  # type: ignore
-            .sum(axis=1),
+            AdditiveValueFunctions.normal(criteria_functions).aggregate(
+                self.performance_table
+            ),
         )
         for relation in self.relations:
             if isinstance(relation, PreferenceRelation):
                 self.post_optimality_problem += (
                     u_a[relation.a]
                     + sigma_n_var[relation.a]
                     + sigma_p_var[relation.b]
@@ -582,15 +581,15 @@
                     - u_a[relation.b]
                     - sigma_n_var[relation.b]
                     - sigma_p_var[relation.a]
                     == 0
                 )
         self.post_optimality_problem.solve(**self.solver_args)
 
-        return UtilityFunction(criteria_functions)
+        return AdditiveValueFunctions.normal(criteria_functions)
 
     @staticmethod
     def _generate_utility_variable_star(
         alternative_values: ScaleValues,
         w_var: Dict[Any, List[LpVariable]],
         g_matrix: Dict[Any, List[float]],
     ) -> Any:
@@ -645,15 +644,15 @@
 
         # Preference constraints
         u_a = {}
         for relation in relations:
             for k in relation.elements:
                 if k not in u_a:
                     u_a[k] = UTAstar._generate_utility_variable_star(
-                        performance_table.get_alternative_values(k),
+                        performance_table.alternatives_values[k],
                         w_var,
                         g_matrix,
                     )
             if isinstance(relation, PreferenceRelation):
                 problem += (
                     u_a[relation.a]
                     + sigma_n_var[relation.a]
```

### Comparing `mcda-0.4.1/mcda/outranking/electre.py` & `mcda-0.5.0/mcda/outranking/electre.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,83 @@
 """This module implements the Electre algorithms.
 
 Implementation and naming conventions are taken from
 :cite:p:`vincke1998electre`.
 """
 from abc import ABC, abstractmethod
-from collections import defaultdict
-from typing import Any, Dict, List, Tuple, cast
+from typing import Any, Dict, Generic, List, Set, Tuple, TypeVar, cast
 
 from pandas import DataFrame, Series
 
-from mcda.core.performance_table import PerformanceTable, ScaleValues
-from mcda.core.relations import (
+from ..core.categories import BoundedCategoryProfile
+from ..core.interfaces import Assignator, Ranker, Selector
+from ..core.matrices import AdjacencyMatrix, ProfileAlternativeMatrix
+from ..core.performance_table import PerformanceTable
+from ..core.relations import (
     IncomparableRelation,
     IndifferenceRelation,
     OutrankingMatrix,
     PreferenceRelation,
     Relation,
 )
-from mcda.core.scales import PreferenceDirection, QuantitativeScale
+from ..core.scales import PreferenceDirection, QuantitativeScale
+from ..core.values import ScaleValues
 
+T = TypeVar("T")
 
-class Electre(ABC):
-    """This class represents the interface for Electre algorithms.
+
+class IElectre(Generic[T], ABC):
+    """This class represents the common interface between all Electre
+    algorithms
+    """
+
+    @abstractmethod
+    def concordance(
+        self,
+        performance_table: PerformanceTable,
+    ) -> AdjacencyMatrix:  # pragma: nocover
+        """Compute the concordance matrix.
+
+        :param performance_table:
+        :return: concordance matrix
+        """
+        pass
+
+    @abstractmethod
+    def discordance(
+        self,
+        performance_table: PerformanceTable,
+    ) -> AdjacencyMatrix:  # pragma: nocover
+        """Compute the discordance matrix.
+
+        :param performance_table:
+        :return: discordance matrix
+        """
+        pass
+
+    @abstractmethod
+    def construct(
+        self, performance_table: PerformanceTable
+    ) -> T:  # pragma: nocover
+        """Construct the outranking structure.
+
+        :param performance_table:
+        :return: outranking structure
+        """
+        pass
+
+    @abstractmethod
+    def exploit(
+        self, outranking_structure: T, **kwargs
+    ) -> Any:  # pragma: nocover
+        pass
+
+
+class BaseElectre1(ABC):
+    """This class implements common methods for Electre I and II.
 
     :param criteria_weights:
     """
 
     def __init__(self, criteria_weights: Dict[Any, float]):
         self.criteria_weights = criteria_weights
 
@@ -34,15 +86,14 @@
         alternative_values1: ScaleValues,
         alternative_values2: ScaleValues,
     ) -> float:
         """Compute the concordance comparison of 2 alternatives.
 
         :param alternative_values1:
         :param alternative_values2:
-        :param scales:
         :return: concordance index
 
         .. warning::
             this method assumes that alternatives values have the same scales
         """
         scales = cast(Dict[str, QuantitativeScale], alternative_values1.scales)
         concordance_value = 0.0
@@ -66,87 +117,93 @@
         )
         assert concordance_value >= 0
         return concordance_value
 
     def concordance(
         self,
         performance_table: PerformanceTable,
-    ) -> DataFrame:
+    ) -> AdjacencyMatrix:
         """Compute the concordance matrix.
 
         :param performance_table:
         :return: concordance matrix
         """
-        return DataFrame(
+        return AdjacencyMatrix(
             [
                 [
                     self._pairwise_concordance(
-                        performance_table.get_alternative_values(ai),
-                        performance_table.get_alternative_values(aj),
+                        performance_table.alternatives_values[ai],
+                        performance_table.alternatives_values[aj],
                     )
                     for aj in performance_table.alternatives
                 ]
                 for ai in performance_table.alternatives
             ],
-            index=performance_table.alternatives,
-            columns=performance_table.alternatives,
+            vertices=performance_table.alternatives,
         )
 
-    def discordance(
+    def _pairwise_disconcordance(
         self,
-        performance_table: PerformanceTable,
-    ) -> DataFrame:
-        """Compute the discordance matrix.
+        alternative_values1: ScaleValues,
+        alternative_values2: ScaleValues,
+    ) -> float:
+        """Compute the discordance comparison of 2 alternatives.
 
-        :param performance_table:
-        :return: discordance matrix
+        :param alternative_values1:
+        :param alternative_values2:
+        :return: discordance index
+
+        .. warning::
+            this method assumes that alternatives values have the same scales
         """
         pref_factor = Series(
             {
                 c: (
                     1
                     if scale.preference_direction == PreferenceDirection.MAX
                     else -1
                 )
                 for c, scale in cast(
-                    Dict[Any, QuantitativeScale], performance_table.scales
+                    Dict[Any, QuantitativeScale], alternative_values1.scales
                 ).items()
             }
         )
-        return DataFrame(
-            [
-                [
-                    max(
-                        (
-                            performance_table.get_alternative_values(aj).data
-                            - performance_table.get_alternative_values(ai).data
-                        )
-                        * pref_factor
-                    )
-                    for aj in performance_table.alternatives
-                ]
-                for ai in performance_table.alternatives
-            ],
-            index=performance_table.alternatives,
-            columns=performance_table.alternatives,
-        ) / max(performance_table.df.apply(lambda x: max(x) - min(x)))
+        return max(
+            (alternative_values2.data - alternative_values1.data) * pref_factor
+        )
 
-    @abstractmethod
-    def __call__(
-        self, performance_table: PerformanceTable, **kwargs
-    ) -> Any:  # pragma: nocover
-        """Apply the chosen Electre algorithm.
+    def discordance(
+        self,
+        performance_table: PerformanceTable,
+    ) -> AdjacencyMatrix:
+        """Compute the discordance matrix.
 
         :param performance_table:
-        :return: outranking matrix
+        :return: discordance matrix
         """
-        pass
+        return AdjacencyMatrix(
+            DataFrame(
+                [
+                    [
+                        self._pairwise_disconcordance(
+                            performance_table.alternatives_values[ai],
+                            performance_table.alternatives_values[aj],
+                        )
+                        for aj in performance_table.alternatives
+                    ]
+                    for ai in performance_table.alternatives
+                ],
+                index=performance_table.alternatives,
+                columns=performance_table.alternatives,
+            )
+            / max(performance_table.data.apply(lambda x: max(x) - min(x)))
+        )
 
 
-class Electre1(Electre):
+class Electre1(BaseElectre1, IElectre[OutrankingMatrix], Selector):
     """This class implements the Electre I algorithm.
 
     :param criteria_weights:
     :param c_hat: concordance threshold
     :param d_hat: discordance threshold
     """
 
@@ -155,32 +212,32 @@
     ):
         super().__init__(criteria_weights)
         self.c_hat = c_hat
         self.d_hat = d_hat
 
     def outranking(
         self,
-        concordance_matrix: DataFrame,
-        discordance_matrix: DataFrame,
+        concordance_matrix: AdjacencyMatrix,
+        discordance_matrix: AdjacencyMatrix,
     ) -> OutrankingMatrix:
         """Compute the outranking matrix using Electre I method.
 
         :param concordance_matrix: concordance matrix
         :param discordance_matrix: discordance matrix
         :return: the outranking matrix
         """
         ones = DataFrame(
             1,
-            index=concordance_matrix.index,
-            columns=concordance_matrix.columns,
+            index=concordance_matrix.vertices,
+            columns=concordance_matrix.vertices,
         )
         return OutrankingMatrix(
             ones[
-                (concordance_matrix >= self.c_hat)
-                & (discordance_matrix <= self.d_hat)
+                (concordance_matrix.data >= self.c_hat)
+                & (discordance_matrix.data <= self.d_hat)
             ].fillna(0)
         )
 
     def construct(
         self, performance_table: PerformanceTable
     ) -> OutrankingMatrix:
         """Construct the outranking matrix using Electre I method.
@@ -191,45 +248,46 @@
         return self.outranking(
             self.concordance(performance_table),
             self.discordance(performance_table),
         )
 
     def exploit(
         self,
-        outranking_matrix: OutrankingMatrix,
+        outranking_structure: OutrankingMatrix,
         cycle_reduction: bool = False,
         transitivity: bool = False,
+        **kwargs,
     ) -> List:
         """Choose best alternative candidates from outranking matrix.
 
         It uses :meth:`OutrankingMatrix.kernel` to find the best candidates.
 
-        :param outranking_matrix:
+        :param outranking_structure:
         :param cycle_reduction:
             if ``True``, apply :attr:`.AdjacencyMatrix.cycle_reduction_matrix`
             to outranking matrix
         :param transitivity:
             if ``True``, apply :attr:`.AdjacencyMatrix.transitive_closure` to
             outranking matrix
         :return: best alternative candidates
 
         .. warning::
             if `outranking_matrix` kernel does not exist, it returns all
             alternatives
         """
         matrix = (
-            outranking_matrix.cycle_reduction_matrix
+            outranking_structure.cycle_reduction_matrix
             if cycle_reduction
-            else outranking_matrix
+            else outranking_structure
         )
         matrix = matrix.transitive_closure if transitivity else matrix
         kernel = matrix.kernel
-        return kernel if len(kernel) > 0 else outranking_matrix.vertices
+        return kernel if len(kernel) > 0 else outranking_structure.vertices
 
-    def __call__(
+    def select(
         self,
         performance_table: PerformanceTable,
         cycle_reduction: bool = False,
         transitivity: bool = False,
         **kwargs,
     ) -> List:
         """Compute the outranking matrix using Electre I method.
@@ -249,185 +307,179 @@
         """
         matrix = self.construct(performance_table)
         return self.exploit(
             matrix, cycle_reduction=cycle_reduction, transitivity=transitivity
         )
 
 
-class Electre2(Electre):
+class Electre2(
+    BaseElectre1, IElectre[Tuple[OutrankingMatrix, OutrankingMatrix]], Ranker
+):
     """This class implements the Electre II algorithm.
 
     :param criteria_weights:
     :param c_hat: concordance thresholds (min, max)
     :param d_hat: discordance threshold (min, max)
     """
 
     def __init__(
         self,
         criteria_weights: Dict[Any, float],
         c_hat: Tuple[float, float],
         d_hat: Tuple[float, float],
     ):
-        Electre.__init__(self, criteria_weights)
+        super().__init__(criteria_weights)
         self.c_hat: Tuple[float, float] = c_hat
         self.d_hat: Tuple[float, float] = d_hat
 
     def outranking(
         self,
-        concordance_matrix: DataFrame,
-        discordance_matrix: DataFrame,
-        c_hat: float = None,
-        d_hat: float = None,
+        concordance_matrix: AdjacencyMatrix,
+        discordance_matrix: AdjacencyMatrix,
+        strong: bool = True,
     ) -> OutrankingMatrix:
         """Calculate the outranking matrix according to given thresholds.
 
         :param concordance_matrix: concordance matrix
         :param discordance_matrix: discordance matrix
-        :param c_hat: concordance threshold
-        :param d_hat: discordance threshold
+        :param strong:
+            return strong outranking matrix if ``True``, weak otherwise
         :return: outranking matrix
         """
-        c_hat = self.c_hat[1] if c_hat is None else c_hat
-        d_hat = self.d_hat[0] if d_hat is None else d_hat
+        c_hat = self.c_hat[1] if strong else self.c_hat[0]
+        d_hat = self.d_hat[0] if strong else self.d_hat[1]
         ones = DataFrame(
             1,
-            index=concordance_matrix.index,
-            columns=concordance_matrix.columns,
+            index=concordance_matrix.vertices,
+            columns=concordance_matrix.vertices,
         )
         return OutrankingMatrix(
             ones[
-                (concordance_matrix >= concordance_matrix.T)
-                & (concordance_matrix >= c_hat)
-                & (discordance_matrix <= d_hat)
+                (concordance_matrix.data >= concordance_matrix.data.T)
+                & (concordance_matrix.data >= c_hat)
+                & (discordance_matrix.data <= d_hat)
             ].fillna(0)
         )
 
     @staticmethod
     def distillation(
         strong_outranking_matrix: OutrankingMatrix,
         weak_outranking_matrix: OutrankingMatrix,
         ascending: bool = False,
-    ) -> List[List[Any]]:
+    ) -> OutrankingMatrix:
         """Compute distillation using outranking matrices.
 
         :param strong_outranking_matrix:
         :param weak_outranking_matrix:
         :param ascending:
             if ``True`` distillation is done in ascending direction
-        :return: ranking of categories
+        :return: resulting ranking as an outranking matrix
         """
         axis = 1 if ascending else 0
         distillate = []
         rest = weak_outranking_matrix.vertices
         strong_outranking_matrix = cast(
             OutrankingMatrix, strong_outranking_matrix.cycle_reduction_matrix
         )
         weak_outranking_matrix = cast(
             OutrankingMatrix, weak_outranking_matrix.cycle_reduction_matrix
         )
         while len(rest) > 0:
-            outranked = strong_outranking_matrix.df.loc[rest, rest].apply(
+            outranked = strong_outranking_matrix.data.loc[rest, rest].apply(
                 sum, axis=axis
             )
             B = outranked[outranked == 0].index.tolist()
-            outranked = weak_outranking_matrix.df.loc[B, B].apply(
+            outranked = weak_outranking_matrix.data.loc[B, B].apply(
                 sum, axis=axis
             )
             A = outranked[outranked == 0].index.tolist()
             for i in A:
                 rest.remove(i)
             distillate.append(A)
-        return distillate[::-1] if ascending else distillate
+        # Build resulting OutrankingMatrix
+        order = distillate[::-1] if ascending else distillate
+        return OutrankingMatrix.from_ordered_alternatives_groups(order)
 
     def construct(
         self, performance_table: PerformanceTable
     ) -> Tuple[OutrankingMatrix, OutrankingMatrix]:
         """Compute strong and weak dominance outranking matrices.
 
         :param performance_table:
-        :return: strong outranking matrix, weak outranking matric
+        :return: strong outranking matrix, weak outranking matrix
         """
         concordance_matrix = self.concordance(performance_table)
         discordance_matrix = self.discordance(performance_table)
         s_dominance_matrix = self.outranking(
             concordance_matrix,
             discordance_matrix,
-            c_hat=self.c_hat[1],
-            d_hat=self.d_hat[0],
         )
         w_dominance_matrix = self.outranking(
             concordance_matrix,
             discordance_matrix,
-            c_hat=self.c_hat[0],
-            d_hat=self.d_hat[1],
+            strong=False,
         )
         return s_dominance_matrix, w_dominance_matrix
 
     def exploit(
         self,
-        strong_outranking_matrix: OutrankingMatrix,
-        weak_outranking_matrix: OutrankingMatrix,
+        outranking_structure: Tuple[OutrankingMatrix, OutrankingMatrix],
+        **kwargs,
     ) -> OutrankingMatrix:
         """Compute distillations and merge results.
 
-        :param strong_outranking_matrix:
-        :param weak_outranking_matrix:
+        :param outranking_structure: strong and weak outranking matrices
         :return: result outranking matrix
         """
-        return OutrankingMatrix.from_ranked_categories(
+        strong_outranking_matrix, weak_outranking_matrix = outranking_structure
+        return cast(
+            OutrankingMatrix,
             self.distillation(
                 strong_outranking_matrix,
                 weak_outranking_matrix,
                 ascending=True,
             )
-        ) * OutrankingMatrix.from_ranked_categories(
-            self.distillation(
+            * self.distillation(
                 strong_outranking_matrix,
                 weak_outranking_matrix,
                 ascending=False,
-            )
+            ),
         )
 
-    def __call__(
+    def rank(
         self, performance_table: PerformanceTable, **kwargs
     ) -> OutrankingMatrix:
         """Compute final outranking matrix for Electre II.
 
         :param performance_table:
         :return: result outranking matrix
         """
-        return self.exploit(*self.construct(performance_table))
+        return self.exploit(self.construct(performance_table))
 
 
-class Electre3(Electre):
-    """This class implements the Electre III algorithm.
+class BaseElectre3(ABC):
+    """This class implements basic Electre III methods shared to other classes.
 
     :param criteria_weights:
     :param preference_thresholds:
     :param indifference_thresholds:
     :param veto_thresholds:
-    :param alpha:  preset up values of distillation coefficients
-    :param beta: preset up values of distillation coefficients
     """
 
     def __init__(
         self,
         criteria_weights: Dict[Any, float],
         preference_thresholds: Dict[Any, float],
         indifference_thresholds: Dict[Any, float],
         veto_thresholds: Dict[Any, float],
-        alpha: float = 0.30,
-        beta: float = -0.15,
     ):
-        Electre.__init__(self, criteria_weights)
+        self.criteria_weights = criteria_weights
         self.preference_thresholds = preference_thresholds
         self.indifference_thresholds = indifference_thresholds
         self.veto_thresholds = veto_thresholds
-        self.alpha = alpha
-        self.beta = beta
 
     @staticmethod
     def _concordance_index(
         ga: float,
         gb: float,
         pga: float,
         qga: float,
@@ -471,15 +523,14 @@
         alternative_values1: ScaleValues,
         alternative_values2: ScaleValues,
     ) -> float:
         """Compute the pairwise concordance between two alternatives.
 
         :param alternative_values1:
         :param alternative_values2:
-        :param scales:
         :return: pairwise concordance value
 
         .. warning::
             this method assumes that alternatives values have the same scales
         """
 
         scales = cast(Dict[str, QuantitativeScale], alternative_values1.scales)
@@ -491,14 +542,37 @@
                 self.preference_thresholds[i],
                 self.indifference_thresholds[i],
                 scales[i].preference_direction,
             )
             for i in self.criteria_weights
         ) / sum(self.criteria_weights.values())
 
+    def concordance(
+        self,
+        performance_table: PerformanceTable,
+    ) -> AdjacencyMatrix:
+        """Compute the concordance matrix.
+
+        :param performance_table:
+        :return: concordance matrix
+        """
+        return AdjacencyMatrix(
+            [
+                [
+                    self._pairwise_concordance(
+                        performance_table.alternatives_values[ai],
+                        performance_table.alternatives_values[aj],
+                    )
+                    for aj in performance_table.alternatives
+                ]
+                for ai in performance_table.alternatives
+            ],
+            vertices=performance_table.alternatives,
+        )
+
     @staticmethod
     def _discordance_index(
         ga: float,
         gb: float,
         pga: float,
         vga: float,
         preference_direction: PreferenceDirection,
@@ -538,47 +612,65 @@
         else:
             return (
                 (gb - pga - ga) / (vga - pga)
                 if preference_direction == PreferenceDirection.MAX
                 else (-gb - pga + ga) / (vga - pga)
             )
 
+    def _pairwise_disconcordance(
+        self,
+        alternative_values1: ScaleValues,
+        alternative_values2: ScaleValues,
+    ) -> Series:
+        """Compute the discordance comparison of 2 alternatives.
+
+        :param alternative_values1:
+        :param alternative_values2:
+        :return: discordance indexes
+
+        .. warning::
+            this method assumes that alternatives values have the same scales
+        """
+        return Series(
+            {
+                j: self._discordance_index(
+                    alternative_values1.data[j],
+                    alternative_values2.data[j],
+                    self.preference_thresholds[j],
+                    self.veto_thresholds[j],
+                    cast(
+                        QuantitativeScale,
+                        alternative_values1.scales[j],
+                    ).preference_direction,
+                )
+                for j in alternative_values1.labels
+            }
+        )
+
     def discordance(
         self,
         performance_table: PerformanceTable,
-    ) -> DataFrame:
+    ) -> AdjacencyMatrix:
         """Compute the discordance matrix.
 
         :param performance_table:
         :return: discordance matrix
         """
-        return DataFrame(
+        return AdjacencyMatrix(
             [
                 [
-                    Series(
-                        {
-                            j: self._discordance_index(
-                                performance_table.df.loc[k, j],
-                                performance_table.df.loc[i, j],
-                                self.preference_thresholds[j],
-                                self.veto_thresholds[j],
-                                cast(
-                                    QuantitativeScale,
-                                    performance_table.scales[j],
-                                ).preference_direction,
-                            )
-                            for j in performance_table.criteria
-                        }
+                    self._pairwise_disconcordance(
+                        performance_table.alternatives_values[ai],
+                        performance_table.alternatives_values[aj],
                     )
-                    for i in performance_table.alternatives
+                    for aj in performance_table.alternatives
                 ]
-                for k in performance_table.alternatives
+                for ai in performance_table.alternatives
             ],
-            index=performance_table.alternatives,
-            columns=performance_table.alternatives,
+            vertices=performance_table.alternatives,
         )
 
     @staticmethod
     def _pairwise_credibility_index(
         pairwise_concordance_: float,
         pairwise_discordance_: Series,
     ) -> float:
@@ -595,353 +687,411 @@
         ]
         S_ab = pairwise_concordance_
         if len(sup_discordance) > 0:
             for Di_ab in sup_discordance:
                 S_ab = S_ab * (1 - Di_ab) / (1 - pairwise_concordance_)
         return S_ab
 
-    def construct(self, performance_table: PerformanceTable) -> DataFrame:
+    def credibility(
+        self, performance_table: PerformanceTable
+    ) -> AdjacencyMatrix:
         """Compute the credibility matrix.
 
         :param performance_table:
         :return: credibility matrix
         """
         concordance_matrix = self.concordance(
             performance_table,
         )
         discordance_matrix = self.discordance(
             performance_table,
         )
-        return DataFrame(
+        return AdjacencyMatrix(
             [
                 [
                     self._pairwise_credibility_index(
-                        concordance_matrix.loc[i, j],
-                        discordance_matrix.loc[i, j],
+                        concordance_matrix.data.loc[i, j],
+                        discordance_matrix.data.loc[i, j],
                     )
                     for j in performance_table.alternatives
                 ]
                 for i in performance_table.alternatives
             ],
-            index=performance_table.alternatives,
-            columns=performance_table.alternatives,
+            vertices=performance_table.alternatives,
+        )
+
+
+class Electre3(BaseElectre3, IElectre[AdjacencyMatrix], Ranker):
+    """This class implements the Electre III algorithm.
+
+    :param criteria_weights:
+    :param preference_thresholds:
+    :param indifference_thresholds:
+    :param veto_thresholds:
+    :param alpha:  preset up values of distillation coefficients
+    :param beta: preset up values of distillation coefficients
+    """
+
+    def __init__(
+        self,
+        criteria_weights: Dict[Any, float],
+        preference_thresholds: Dict[Any, float],
+        indifference_thresholds: Dict[Any, float],
+        veto_thresholds: Dict[Any, float],
+        alpha: float = 0.30,
+        beta: float = -0.15,
+    ):
+        super().__init__(
+            criteria_weights,
+            preference_thresholds,
+            indifference_thresholds,
+            veto_thresholds,
         )
+        self.alpha = alpha
+        self.beta = beta
+
+    def construct(
+        self, performance_table: PerformanceTable
+    ) -> AdjacencyMatrix:
+        """Construct outranking structure which is the credibility matrix.
+
+        :param performance_table:
+        :return: credibility matrix
+        """
+        return self.credibility(performance_table)
 
-    def qualification(self, credibility_mat: DataFrame) -> Series:
+    def qualification(self, credibility_mat: AdjacencyMatrix) -> Series:
         """Compute the qualification for each pair of alternatives a and b.
 
         :param credibility_mat:
         :return: qualifications
         """
-        lambda_max = max(credibility_mat.apply(max))
+        lambda_max = max(credibility_mat.data.apply(max))
         lambda_ = lambda_max - (self.alpha + self.beta * lambda_max)
 
         lambda_strengths = Series(
             {
                 i: sum(
                     (
-                        credibility_mat.loc[i, j] > lambda_
-                        and credibility_mat.loc[i, j]
-                        > credibility_mat.loc[j, i]
+                        credibility_mat.data.loc[i, j] > lambda_
+                        and credibility_mat.data.loc[i, j]
+                        > credibility_mat.data.loc[j, i]
                     )
-                    for j in credibility_mat.index.tolist()
+                    for j in credibility_mat.vertices
                 )
-                for i in credibility_mat.index.tolist()
+                for i in credibility_mat.vertices
             }
         )
 
         lambda_weakness = Series(
             {
                 j: sum(
                     (
-                        credibility_mat.loc[i, j] > lambda_
-                        and credibility_mat.loc[i, j]
-                        > credibility_mat.loc[j, i]
+                        credibility_mat.data.loc[i, j] > lambda_
+                        and credibility_mat.data.loc[i, j]
+                        > credibility_mat.data.loc[j, i]
                     )
-                    for i in credibility_mat.index.tolist()
+                    for i in credibility_mat.vertices
                 )
-                for j in credibility_mat.index.tolist()
+                for j in credibility_mat.vertices
             }
         )
 
         return lambda_strengths - lambda_weakness
 
     def distillation(
         self,
-        credibility_matrix: DataFrame,
+        credibility_matrix: AdjacencyMatrix,
         ascending: bool = False,
-    ) -> List[List[Any]]:
+    ) -> OutrankingMatrix:
         """Compute distillation.
 
         :param credibility_matrix:
         :param ascending: if ``True`` distillation is performed in ascension
         :return: ranking of categories
         """
         comp = min if ascending else max
 
-        rest = credibility_matrix.index.tolist()
+        rest = credibility_matrix.vertices
         distillate = []
         while len(rest) > 0:
-            updated_credibility_mat = credibility_matrix.loc[rest]
+            updated_credibility_mat = AdjacencyMatrix(
+                credibility_matrix.data.loc[rest, rest]
+            )
             qualifications = self.qualification(
                 updated_credibility_mat,
             )
 
             maxes = qualifications[qualifications == comp(qualifications)]
             if len(maxes) > 1:
-                updated_credibility_mat = updated_credibility_mat.loc[
-                    maxes.index
-                ]
+                updated_credibility_mat = AdjacencyMatrix(
+                    updated_credibility_mat.data.loc[maxes.index, maxes.index]
+                )
                 qualifications = self.qualification(
                     updated_credibility_mat,
                 )
                 maxes = qualifications[qualifications == comp(qualifications)]
             distillate.append(maxes.index.tolist())
             for i in maxes.index.tolist():
                 rest.remove(i)
-        return distillate[::-1] if ascending else distillate
+        order = distillate[::-1] if ascending else distillate
+        return OutrankingMatrix.from_ordered_alternatives_groups(order)
 
-    def exploit(self, credibility_matrix: DataFrame) -> OutrankingMatrix:
+    def exploit(
+        self, outranking_structure: AdjacencyMatrix, **kwargs
+    ) -> OutrankingMatrix:
         """Compute the complete Electre III exploitation phase.
 
-        :param credibility_matrix:
+        :param outranking_structure: credibility matrix
         :return: final outranking matrix
         """
-        return OutrankingMatrix.from_ranked_categories(
-            self.distillation(credibility_matrix, ascending=True)
-        ) * OutrankingMatrix.from_ranked_categories(
-            self.distillation(credibility_matrix, ascending=False)
+        return cast(
+            OutrankingMatrix,
+            self.distillation(outranking_structure, ascending=True)
+            * self.distillation(outranking_structure, ascending=False),
         )
 
-    def __call__(
+    def rank(
         self, performance_table: PerformanceTable, **kwargs
     ) -> OutrankingMatrix:
         """Compute the complete Electre III algorithm
 
         :param performance_table:
         :return: final outranking matrix
         """
         return self.exploit(self.construct(performance_table))
 
 
-class ElectreTri(Electre):
+class ElectreTri(BaseElectre3, IElectre[ProfileAlternativeMatrix], Assignator):
     """This class implements the Electre-Tri B algorithm.
 
     :param criteria_weights:
-    :param category_profiles:
+    :param profiles: profiles in ascending dominance order
     :param preference_thresholds:
     :param indifference_thresholds:
     :param veto_thresholds:
     :param lambda_: cut level
+    :param categories: categories in ascending ranking order
+    :raise ValueError:
+        * if length of `categories` is not length of `profiles` + 1
+        * if the profiles are not in ascending dominance order
+
+    :attr category_profiles:
+        category profiles formed using `categories` and `profiles`
 
     .. note::
         Implementation and naming conventions are taken from
         :cite:p:`vincke1998electreTRI`.
     """
 
     def __init__(
         self,
         criteria_weights: Dict[Any, float],
-        category_profiles: PerformanceTable,
+        profiles: PerformanceTable,
         preference_thresholds: Dict[Any, float],
         indifference_thresholds: Dict[Any, float],
         veto_thresholds: Dict[Any, float],
         lambda_: float,
+        categories: List = None,
     ):
-        Electre.__init__(self, criteria_weights)
-        self.category_profiles = category_profiles
-        self.preference_thresholds = preference_thresholds
-        self.indifference_thresholds = indifference_thresholds
-        self.veto_thresholds = veto_thresholds
-        self.lambda_ = lambda_
-
-    @property
-    def _electre3(self) -> Electre3:
-        """Return the equivalent Electre3 object.
-
-        :return:
-        """
-        return Electre3(
-            self.criteria_weights,
-            self.preference_thresholds,
-            self.indifference_thresholds,
-            self.veto_thresholds,
+        super().__init__(
+            criteria_weights,
+            preference_thresholds,
+            indifference_thresholds,
+            veto_thresholds,
+        )
+        categories = (
+            list(range(len(profiles.alternatives) + 1))
+            if categories is None
+            else categories
         )
+        if len(categories) != len(profiles.alternatives) + 1:
+            raise ValueError(
+                "there must be exactly one more category than profiles"
+            )
+        self.profiles = profiles
+        self.category_profiles: Dict[Any, BoundedCategoryProfile] = dict(
+            zip(
+                categories,
+                BoundedCategoryProfile.profiles_partition(self.profiles),
+            )
+        )
+        self.lambda_ = lambda_
 
-    def concordance(
-        self,
-        performance_table: PerformanceTable,
-    ) -> DataFrame:
-        """Compute the concordance matrix.
-
-        :param performance_table:
-        :return: concordance matrix
-
-        .. note:: uses :meth:`Electre3.concordance` implementation
-        """
-        return self._electre3.concordance(performance_table)
-
-    def discordance(
-        self,
-        performance_table: PerformanceTable,
-    ) -> DataFrame:
-        """Compute the discordance matrix.
-
-        :param performance_table:
-        :return: discordance matrix
-
-        .. note:: uses :meth:`Electre3.discordance` implementation
-        """
-        return self._electre3.discordance(performance_table)
-
-    def construct(self, performance_table: PerformanceTable) -> DataFrame:
+    def credibility(
+        self, performance_table: PerformanceTable
+    ) -> ProfileAlternativeMatrix:
         """Return credibility matrix.
 
         Returned credibility matrix concatenates `performance_table`
-        and :attr:`category_profiles` (in that order) and replaces labels with
-        indexes to avoid duplicated indexes.
+        and :attr:`profiles` (in that order).
 
         :param performance_table:
         :return:
 
         .. note::
             uses :meth:`Electre3.construct` implementation
         """
         # Concatenate performance table and category profile
         # Replace indexes so no chance of same id category profile alternative
         altered_performance_table = PerformanceTable(
-            performance_table.df.values.tolist()
-            + self.category_profiles.df[
-                performance_table.criteria
-            ].values.tolist(),
+            performance_table.data.values.tolist()
+            + self.profiles.data[performance_table.criteria].values.tolist(),
             criteria=performance_table.criteria,
         )
-        return DataFrame(
-            self._electre3.construct(altered_performance_table),
+        matrix = BaseElectre3.credibility(self, altered_performance_table)
+        return ProfileAlternativeMatrix(
+            matrix.data.values,
+            alternatives=performance_table.alternatives,
+            profiles=self.profiles.alternatives,
         )
 
+    def construct(
+        self, performance_table: PerformanceTable
+    ) -> ProfileAlternativeMatrix:
+        """Construct outranking structure which is the credibility matrix.
+
+        :param performance_table:
+        :return: credibility matrix
+        """
+        return self.credibility(performance_table)
+
     def _pairwise_outrank(
         self,
-        credibility_mat: DataFrame,
-        alternative1: int,
-        alternative2: int,
+        credibility_mat: ProfileAlternativeMatrix,
+        label1: Tuple[Any, Any],
+        label2: Tuple[Any, Any],
+    ) -> bool:
+        """Check whether first label outranks second.
+
+        :param credibility_mat:
+        :param label1:
+        :param label2:
+        :return: ``True`` if `label1` outranks `label2`, ``False`` otherwise
+        """
+        aSb = cast(float, credibility_mat.data.at[label1, label2])
+        return aSb >= self.lambda_
+
+    def _pairwise_relation(
+        self,
+        credibility_mat: ProfileAlternativeMatrix,
+        label1: Tuple[Any, Any],
+        label2: Tuple[Any, Any],
     ) -> Relation:
         """Compute relation between two actions based on credibility matrix.
 
         :param credibility_mat:
-            credibility matrix of concatenated performance table / category
-            profiles
-        :param alternative1:
-        :param alternative2:
+            credibility matrix of concatenated performance table / profiles
+        :param label1:
+        :param label2:
         :return: relationship between both alternatives
         """
-        aSb = cast(float, credibility_mat.loc[alternative1, alternative2])
-        bSa = cast(float, credibility_mat.loc[alternative2, alternative1])
+        aSb = cast(float, credibility_mat.data.at[label1, label2])
+        bSa = cast(float, credibility_mat.data.at[label2, label1])
         if aSb >= self.lambda_ and bSa >= self.lambda_:
-            return IndifferenceRelation(alternative1, alternative2)
+            return IndifferenceRelation(label1, label2)
         elif aSb >= self.lambda_ > bSa:
-            return PreferenceRelation(alternative1, alternative2)
+            return PreferenceRelation(label1, label2)
         elif aSb < self.lambda_ <= bSa:
-            return PreferenceRelation(alternative2, alternative1)
-        return IncomparableRelation(alternative1, alternative2)
+            return PreferenceRelation(label2, label1)
+        return IncomparableRelation(label1, label2)
 
-    def _exploit(
-        self,
-        credibility_matrix: DataFrame,
-        performance_table: PerformanceTable,
-        pessimistic: bool = False,
-    ) -> Dict[int, List[Any]]:
-        """Compute the exploitation procedure (either optimistically or
-        pessimistically).
-
-        In the output ranking, class -1 means incomparable class
+    def _exploit_pessimistic(
+        self, outranking_structure: ProfileAlternativeMatrix
+    ) -> Dict[Any, Set]:
+        """Compute the exploitation procedure pessimistically.
 
-        :param credibility_matrix:
-        :param performance_table:
-        :param pessimistic: if ``True`` performs procedure pessimistically
+        :param outranking_structure: credibility matrix
         :return: categories
         """
-
-        # performance table and category profiles are concatenated
-        nb_classes = len(self.category_profiles.alternatives)
-        nb_actions = len(credibility_matrix.index.tolist()) - nb_classes
-
-        classes = defaultdict(list)
-        rest = [*range(nb_actions)]
-        for i in (
-            range(nb_classes - 1, -1, -1) if pessimistic else range(nb_classes)
+        rest = set(outranking_structure.alternatives)
+        categories = list(self.category_profiles.keys())
+        classes: Dict[Any, Set] = {category: set() for category in categories}
+        for cat, cat_profile in reversed(
+            list(self.category_profiles.items())[1:]
         ):
-            class_ = []
-            for action in rest:
-                relation = self._pairwise_outrank(
-                    credibility_matrix,
-                    action,
-                    i + nb_actions,
-                )
-                if isinstance(relation, PreferenceRelation):
-                    if relation.a == action and pessimistic:
-                        class_.append(action)
-                        classes[i + 1].append(
-                            performance_table.alternatives[action]
-                        )
-                    elif relation.b == action and not pessimistic:
-                        class_.append(action)
-                        classes[i].append(
-                            performance_table.alternatives[action]
-                        )
-            for a in class_:
-                rest.remove(a)
-        if len(rest) > 0:
-            for action in rest:
-                relation = self._pairwise_outrank(
-                    credibility_matrix,
-                    nb_actions if pessimistic else action,
-                    action if pessimistic else nb_actions + nb_classes - 1,
+            assigned = set()
+            for a in rest:
+                if self._pairwise_outrank(
+                    outranking_structure,
+                    outranking_structure.alternative_index(a),
+                    outranking_structure.profile_index(
+                        cast(ScaleValues, cat_profile.lower).name
+                    ),
+                ):
+                    classes[cat].add(a)
+                    assigned.add(a)
+            rest -= assigned
+        classes[categories[0]] = rest
+        return classes
+
+    def _exploit_optimistic(
+        self, outranking_structure: ProfileAlternativeMatrix
+    ) -> Dict[Any, Set]:
+        """Compute the exploitation procedure optimistically.
+
+        :param outranking_structure: credibility matrix
+        :return: categories
+        """
+        rest = set(outranking_structure.alternatives)
+        categories = list(self.category_profiles.keys())
+        classes: Dict[Any, Set] = {}
+        for cat, cat_profile in list(self.category_profiles.items())[:-1]:
+            assigned = set()
+            profile = cast(ScaleValues, cat_profile.upper).name
+            for a in rest:
+                pref = PreferenceRelation(
+                    outranking_structure.profile_index(profile),
+                    outranking_structure.alternative_index(a),
                 )
-                if isinstance(relation, IncomparableRelation):
-                    classes[-1].append(performance_table.alternatives[action])
-                elif relation.b == action and pessimistic:
-                    classes[0].append(performance_table.alternatives[action])
-                elif relation.a == action and not pessimistic:
-                    classes[nb_classes].append(
-                        performance_table.alternatives[action]
+                if (
+                    self._pairwise_relation(
+                        outranking_structure,
+                        outranking_structure.profile_index(profile),
+                        outranking_structure.alternative_index(a),
                     )
-                else:
-                    classes[-1].append(
-                        performance_table.alternatives[action]
-                    )  # pragma: nocover
+                    == pref
+                ):
+                    assigned.add(a)
+            classes[cat] = assigned
+            rest -= assigned
+        classes[categories[-1]] = rest
         return classes
 
     def exploit(
         self,
-        credibility_matrix: DataFrame,
-        performance_table: PerformanceTable,
-    ) -> Tuple[Dict[int, List[Any]], Dict[int, List[Any]]]:
-        """Compute the exploitation procedure of Electre Tri.
-
-        In the output ranking, class -1 means incomparable class
+        outranking_structure: ProfileAlternativeMatrix,
+        pessimistic: bool = False,
+        **kwargs,
+    ) -> Dict[Any, Set]:
+        """Compute the exploitation procedure (either optimistically or
+        pessimistically).
 
-        :param credibility_matrix:
-        :param performance_table:
-        :return: optimistic categories, pessimistic categories
+        :param outranking_structure: credibility matrix
+        :param pessimistic: if ``True`` performs procedure pessimistically
+        :return: categories
         """
-        return self._exploit(
-            credibility_matrix, performance_table
-        ), self._exploit(
-            credibility_matrix, performance_table, pessimistic=True
+        return (
+            self._exploit_pessimistic(outranking_structure)
+            if pessimistic
+            else self._exploit_optimistic(outranking_structure)
         )
 
-    def __call__(
-        self, performance_table: PerformanceTable, **kwargs
-    ) -> Tuple[Dict[int, List[Any]], Dict[int, List[Any]]]:
+    def assign(
+        self,
+        performance_table: PerformanceTable,
+        pessimistic: bool = False,
+        **kwargs,
+    ) -> Dict[Any, Set]:
         """Compute the exploitation procedure (either optimistically or
         pessimistically).
 
         In the output ranking, class -1 means incomparable class
 
         :param performance_table:
-        :return: optimistic categories, pessimistic categories
+        :param pessimistic:
+        :return: categories
         """
         return self.exploit(
             self.construct(performance_table=performance_table),
-            performance_table,
+            pessimistic=pessimistic,
         )
```

### Comparing `mcda-0.4.1/mcda/outranking/srmp.py` & `mcda-0.5.0/mcda/outranking/srmp.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,94 +15,97 @@
     LpMaximize,
     LpProblem,
     LpVariable,
     lpSum,
 )
 from pulp import value as pulp_value
 
-from mcda.core.performance_table import PerformanceTable, ScaleValues
-from mcda.core.relations import (
+from ..core.aliases import Function
+from ..core.criteria_functions import CriteriaFunctions
+from ..core.interfaces import Learner, Ranker
+from ..core.performance_table import PerformanceTable
+from ..core.relations import (
     IndifferenceRelation,
     OutrankingMatrix,
     PreferenceRelation,
     PreferenceStructure,
-    Ranking,
 )
-
-from ..core.aliases import Function
-from ..core.interfaces import Trainer
 from ..core.scales import (
     PreferenceDirection,
     QualitativeScale,
     QuantitativeScale,
     Scale,
     is_better_or_equal,
 )
+from ..core.values import Ranking, ScaleValues
 from ..plot.plot import (
     Annotation,
     AreaPlot,
     Axis,
     BarPlot,
     Figure,
     HorizontalStripes,
     LinePlot,
     ParallelCoordinatesPlot,
     StackedBarPlot,
     Text,
 )
 
 
-class SubSRMP:
-    """This class infers outranking relations related to a single category
-    profile.
+class ProfileWiseOutranking(Ranker):
+    """This class infers outranking relations related to a single profile.
 
     The relation compares each criterion of each alternative values with the
     category profile (``1`` if better or equal, ``0`` otherwise), apply
     the `criteria_weights` as a weighted sum for each alternative and compare
     those scores.
 
     :param criteria_weights:
-    :param category_profile:
+    :param profile:
 
     .. todo:: Find a better name
     """
 
     def __init__(
-        self, criteria_weights: Dict[Any, float], category_profile: ScaleValues
+        self, criteria_weights: Dict[Any, float], profile: ScaleValues
     ):
         self.criteria_weights = criteria_weights
-        self.category_profile = category_profile
+        self.profile = profile
 
     def construct(
         self, performance_table: PerformanceTable
     ) -> OutrankingMatrix:
         """Construct the outranking matrix.
 
         :param performance_table:
-        ;return:
+        :return:
         """
-        functions = {
-            criterion: (
-                cast(
-                    Function,
-                    lambda x, c=criterion: is_better_or_equal(
-                        x,
-                        self.category_profile.data[c],
-                        cast(QuantitativeScale, performance_table.scales[c]),
-                    ),
-                )
-            )  # https://bugs.python.org/issue13652
-            for criterion in performance_table.criteria
-        }
+        functions = CriteriaFunctions(
+            {
+                criterion: (
+                    cast(
+                        Function,
+                        lambda x, c=criterion: self.criteria_weights[c]
+                        if is_better_or_equal(
+                            x,
+                            self.profile.data[c],
+                            cast(
+                                QuantitativeScale, performance_table.scales[c]
+                            ),
+                        )
+                        else 0,
+                    )
+                )  # https://bugs.python.org/issue13652
+                for criterion in performance_table.criteria
+            }
+        )
 
         conditional_weighted_sum = cast(
             Series,
-            performance_table.apply_criteria_functions(functions)
-            .apply_criteria_weights(self.criteria_weights)
-            .sum(1),
+            performance_table.apply(functions).sum(1),
         )
 
         return OutrankingMatrix(
             DataFrame(
                 [
                     [
                         conditional_weighted_sum[ai]
@@ -113,128 +116,129 @@
                 ],
                 index=performance_table.alternatives,
                 columns=performance_table.alternatives,
                 dtype="int64",
             )
         )
 
-    def __call__(
-        self, performance_table: PerformanceTable
+    def rank(
+        self, performance_table: PerformanceTable, **kwargs
     ) -> OutrankingMatrix:
         """Construct an outranking matrix.
 
         :param performance_table:
-        ;return:
+        :return:
         """
         return self.construct(performance_table=performance_table)
 
 
-class SRMP:
+class SRMP(Ranker):
     """This class implements the SRMP algorithm.
 
     :param criteria_weights:
-    :param category_profiles:
+    :param profiles:
     :param lexicographic_order: profile indices used sequentially to rank
     """
 
     def __init__(
         self,
         criteria_weights: Dict[Any, float],
-        category_profiles: PerformanceTable,
+        profiles: PerformanceTable,
         lexicographic_order: List[int],
     ):
         self.criteria_weights = criteria_weights
-        self.category_profiles = category_profiles
+        self.profiles = profiles
         self.lexicographic_order = lexicographic_order
 
     @property
-    def sub_srmp(self) -> List[SubSRMP]:
+    def sub_srmp(self) -> List[ProfileWiseOutranking]:
         """Return list of sub SRMP problems (one per category profile).
 
         :return:
         """
         return [
-            SubSRMP(
+            ProfileWiseOutranking(
                 self.criteria_weights,
-                self.category_profiles.get_alternative_values(category),
+                self.profiles.alternatives_values[profile],
             )
-            for category in self.category_profiles.alternatives
+            for profile in self.profiles.alternatives
         ]
 
     def construct(
         self, performance_table: PerformanceTable
     ) -> List[OutrankingMatrix]:
         """Construct one outranking matrix per category profile.
 
         :param performance_table:
         :return:
         """
-        return [sub_srmp(performance_table) for sub_srmp in self.sub_srmp]
+        return [sub_srmp.rank(performance_table) for sub_srmp in self.sub_srmp]
 
     def exploit(
         self,
         outranking_matrices: List[OutrankingMatrix],
         lexicographic_order: List[int] = None,
     ) -> Ranking:
-        """Merge outranking matrices built by category profile in lexicographic
+        """Merge outranking matrices built by profiles in lexicographic
         order using SRMP exploitation method.
 
         :param outranking_matrices:
-            outranking matrix constructed in :attr:`category_profiles` order
+            outranking matrix constructed in :attr:`profiles` order
         :param lexicographic_order: (if not supplied, use attribute)
         :return:
             the outranking total order as a ranking
         """
         lexicographic_order = (
             self.lexicographic_order
             if lexicographic_order is None
             else lexicographic_order
         )
         relations_ordered = [
             outranking_matrices[i] for i in lexicographic_order
         ]
         n = len(relations_ordered)
         score = sum(
-            [relations_ordered[i].df * 2 ** (n - 1 - i) for i in range(n)],
+            [relations_ordered[i].data * 2 ** (n - 1 - i) for i in range(n)],
             DataFrame(
                 0,
                 index=relations_ordered[0].vertices,
                 columns=relations_ordered[0].vertices,
             ),
         )
         outranking_matrix = score - score.transpose() >= 0
         scores = outranking_matrix.sum(1)
         scores_ordered = sorted(set(scores.values), reverse=True)
         return Ranking(
             scores.apply(lambda x: scores_ordered.index(x) + 1),
+            PreferenceDirection.MIN,
         )
 
-    def __call__(self, performance_table: PerformanceTable) -> Ranking:
+    def rank(self, performance_table: PerformanceTable, **kwargs) -> Ranking:
         """Compute the SRMP algorithm
 
         :param performance_table:
         :return:
             the outranking total order as a ranking
         """
         return self.exploit(self.construct(performance_table))
 
     @classmethod
-    def train(
+    def learn(
         cls,
         performance_table: PerformanceTable,
         relations: PreferenceStructure,
         max_profiles_number: int = None,
         profiles_number: int = None,
         lexicographic_order: List[int] = None,
         inconsistencies: bool = True,
         gamma: float = 0.001,
         non_dictator: bool = False,
         solver_args: dict = None,
     ) -> Optional["SRMP"]:
-        """Train a SRMP instance
+        """Learn a SRMP instance
 
         :param performance_table:
         :param relations:
         :param max_profiles_number: highest number of reference profiles
         :param profiles_number: number of reference profiles
         :param lexicographic_order: profile indices used sequentially to rank
         :param inconsistencies:
@@ -249,32 +253,32 @@
             * if two or more of `max_profiles_number`, `profiles_number`
               and `lexicographic_order` are specified at the same time
 
         .. note::
             One and only one of `max_profiles_number`, `profiles_number`
             and `lexicographic_order` must be specified
         """
-        return SRMPTrainer(
+        return SRMPLearner(
             performance_table,
             relations,
             max_profiles_number,
             profiles_number,
             lexicographic_order,
             inconsistencies,
             gamma,
             non_dictator,
             solver_args,
-        ).train()
+        ).learn()
 
     @staticmethod
     def plot_input_data(
         performance_table: PerformanceTable,
         srmp: "SRMP" = None,
         criteria_weights: Dict[Any, float] = None,
-        category_profiles: PerformanceTable = None,
+        profiles: PerformanceTable = None,
         lexicographic_order: List[int] = None,
         annotations: bool = False,
         annotations_alpha: float = 0.5,
         scales_boundaries: bool = False,
         figsize: Tuple[float, float] = None,
         xticklabels_tilted: bool = False,
         **kwargs,
@@ -284,15 +288,15 @@
         For each criterion, the arrow indicates the preference direction.
         The criteria weights are displayed as a bar plot,
         and their values are written in parentheses
 
         :param performance_table:
         :param srmp: a SRMP object (if given, overrides SRMP parameters)
         :param criteria_weights:
-        :param category_profiles:
+        :param profiles:
         :param lexicographic_order: profile indices used sequentially to rank
         :param annotations:
             if ``True`` every point is annotated with its value
         :param annotations_alpha: annotations white box transparency
         :param scales_boundaries:
             if ``True`` the criteria boundaries are the scales boundaries,
             else they are computed from the data
@@ -304,15 +308,15 @@
         scales = {
             crit: performance_table.scales[crit]
             for crit in performance_table.criteria
         }
 
         if srmp is not None:
             criteria_weights = srmp.criteria_weights
-            category_profiles = srmp.category_profiles
+            profiles = srmp.profiles
             lexicographic_order = srmp.lexicographic_order
 
         if criteria_weights is not None:
             criteria_weights = {
                 crit: criteria_weights[crit]
                 for crit in performance_table.criteria
             }
@@ -321,34 +325,34 @@
         quantitative_scales = {}
         for key, scale in scales.items():
             if isinstance(scale, QualitativeScale):
                 quantitative_scales[key] = scale.quantitative
             else:
                 quantitative_scales[key] = cast(QuantitativeScale, scale)
 
-        # Concatenate category_profiles with performance_table
-        if category_profiles is not None:
-            df = concat([performance_table.df, category_profiles.df])
+        # Concatenate profiles with performance_table
+        if profiles is not None:
+            df = concat([performance_table.data, profiles.data])
         else:
-            df = performance_table.df.copy()
+            df = performance_table.data.copy()
         table = PerformanceTable(df, scales=scales)
         table = table.transform(cast(Dict[str, Scale], quantitative_scales))
         if not scales_boundaries:
             table.scales = table.bounds
             # Conserve preference direction
             for key, scale in quantitative_scales.items():
                 cast(
                     QuantitativeScale, table.scales[key]
                 ).preference_direction = scale.preference_direction
         table = table.normalize()
 
         # Create constants
         nb_alt = len(performance_table.alternatives)
-        if category_profiles is not None:
-            nb_profiles = len(category_profiles.alternatives)
+        if profiles is not None:
+            nb_profiles = len(profiles.alternatives)
 
         # Create figure and axis
         fig = Figure(figsize=figsize)
         ax = fig.create_add_axis()
 
         # Axis parameters
         x = cast(List[float], range(len(performance_table.criteria)))
@@ -378,44 +382,44 @@
                 )
             )
 
         # Plotted annotations' coordinates
         annotations_coord: List[Tuple[float, float]] = []
 
         # Profiles
-        if category_profiles is not None:
+        if profiles is not None:
             for profile in range(nb_alt, nb_alt + nb_profiles):
                 ax.add_plot(
                     AreaPlot(
                         x,
-                        table.df.iloc[profile],
+                        table.data.iloc[profile],
                         xticks=xticks,
                         yticks=[],
                         xticklabels=xticklabels,
                         xticklabels_tilted=xticklabels_tilted,
                         color="black",
                         alpha=0.1,
                         strongline=False,
                     )
                 )
                 ax.add_plot(
                     Annotation(
                         0,
-                        table.df.iloc[profile, 0],
+                        table.data.iloc[profile, 0],
                         f"$P^{profile - nb_alt}$",
                         -1,
                         0,
                         "right",
                         "center",
                     )
                 )
 
         # Alternatives
-        values = table.df[:nb_alt]
-        labels = table.df[:nb_alt].index
+        values = table.data[:nb_alt]
+        labels = table.data[:nb_alt].index
         ax.add_plot(
             ParallelCoordinatesPlot(
                 x,
                 values,
                 xticks=xticks,
                 yticks=[],
                 xticklabels=xticklabels,
@@ -428,18 +432,18 @@
         ax.add_legend(title="Alternatives :", location="right")
 
         fig.draw()
         assert ax.ax is not None  # to comply with mypy
 
         # Annotations
         if annotations:
-            if category_profiles is not None:
+            if profiles is not None:
                 for profile in range(nb_alt, nb_alt + nb_profiles):
                     for i in x:
-                        xy = (i, table.df.iloc[profile, i])
+                        xy = (i, table.data.iloc[profile, i])
                         overlap = False
                         for (xc, yc) in annotations_coord:
                             if (xc == i) and (
                                 abs(
                                     ax.ax.transData.transform(xy)[1]
                                     - ax.ax.transData.transform((xc, yc))[1]
                                 )
@@ -449,30 +453,30 @@
                                 # already plotted annotations
                                 overlap = True
                                 break
 
                         if not overlap:
                             annotation = Annotation(
                                 i,
-                                table.df.iloc[profile, i],
-                                category_profiles.df.iloc[profile - nb_alt, i],
+                                table.data.iloc[profile, i],
+                                profiles.data.iloc[profile - nb_alt, i],
                                 2,
                                 0,
                                 "left",
                                 "center",
                                 annotations_alpha,
                             )
                             ax.add_plot(annotation)
                             annotations_coord.append(
-                                (i, table.df.iloc[profile, i])
+                                (i, table.data.iloc[profile, i])
                             )
 
             for alt in range(nb_alt):
                 for i in x:
-                    xy = (i, table.df.iloc[alt, i])
+                    xy = (i, table.data.iloc[alt, i])
                     overlap = False
                     for (xc, yc) in annotations_coord:
                         if (xc == i) and (
                             abs(
                                 ax.ax.transData.transform(xy)[1]
                                 - ax.ax.transData.transform((xc, yc))[1]
                             )
@@ -482,24 +486,24 @@
                             # already plotted annotations
                             overlap = True
                             break
 
                     if not overlap:
                         annotation = Annotation(
                             i,
-                            table.df.iloc[alt, i],
-                            performance_table.df.iloc[alt, i],
+                            table.data.iloc[alt, i],
+                            performance_table.data.iloc[alt, i],
                             2,
                             0,
                             "left",
                             "center",
                             annotations_alpha,
                         )
                         ax.add_plot(annotation)
-                        annotations_coord.append((i, table.df.iloc[alt, i]))
+                        annotations_coord.append((i, table.data.iloc[alt, i]))
 
         # Lexicographic order
         if lexicographic_order is not None:
             text = Text(
                 0,
                 1.2,
                 "Lexicographic order : $"
@@ -526,23 +530,23 @@
         :param performance_table:
         :param figsize: figure size in inches as a tuple (`width`, `height`)
         :param xlabels_tilted:
             if ``True`` `xlabels` are tilted to better fit
         """
         # Create constants
         nb_alt = len(performance_table.alternatives)
-        nb_profiles = len(self.category_profiles.alternatives)
+        nb_profiles = len(self.profiles.alternatives)
         weights_sum = sum(self.criteria_weights.values())
 
         # Create figure and axes
         fig = Figure(figsize=figsize, ncols=ncols, nrows=nrows)
 
         for ind_alt in range(nb_alt):
             ax = Axis(
-                xlabel=f"{performance_table.df.index[ind_alt]}",
+                xlabel=f"{performance_table.data.index[ind_alt]}",
                 xlabel_tilted=xlabels_tilted,
             )
             # Axis properties
             x = cast(List[float], range(nb_profiles))
             xticks = cast(List[float], range(nb_profiles))
             xticklabels = [
                 f"$P^{profile}$" for profile in self.lexicographic_order
@@ -551,16 +555,16 @@
 
             values = []
             # Draw the stacked barplot
             for ind_crit, crit in enumerate(performance_table.criteria):
                 crit_values = [
                     self.criteria_weights[crit] / weights_sum
                     if is_better_or_equal(
-                        performance_table.df.iloc[ind_alt, ind_crit],
-                        self.category_profiles.df.iloc[profile, ind_crit],
+                        performance_table.data.iloc[ind_alt, ind_crit],
+                        self.profiles.data.iloc[profile, ind_crit],
                         cast(
                             QuantitativeScale,
                             performance_table.scales[crit],
                         ),
                     )
                     else 0
                     for profile in self.lexicographic_order
@@ -705,30 +709,30 @@
                     box=True,
                 )
             )
             previous_ranks = current_ranks
         fig.draw()
 
 
-class SRMPTrainer(Trainer[Optional[SRMP]]):
-    """This class gathers functions used to train a SRMP model.
+class SRMPLearner(Learner[Optional[SRMP]]):
+    """This class gathers functions used to learn a SRMP model.
 
     :param performance_table:
     :param relations:
     :param max_profiles_number: highest number of reference profiles
     :param profiles_number: number of reference profiles
     :param lexicographic_order: profile indices used sequentially to rank
     :param inconsistencies:
         if ``True`` inconsistent comparisons will be taken into account
     :param gamma: value used for modeling strict inequalities
     :param non_dictator: if ``True`` prevent dictator weights (> 0.5)
     :param solver_args: extra arguments supplied to the solver
     :raise TypeError:
-        * if `max_profiles_number`, `profiles_number`
-          and `lexicographic_order` are not specified
+        if `max_profiles_number`, `profiles_number`
+        and `lexicographic_order` are not specified
 
     .. note::
         If multiple arguments are supplied, only one will be used in the
         following priority: `lexicographic_order`, `profiles_number` then
         `max_profiles_number`
     """
 
@@ -769,15 +773,15 @@
     @staticmethod
     def compute_fitness(
         problem: LpProblem, nb_relations: int, inconsistencies: bool = True
     ) -> float:
         """Compute fitness of a SRMP solution.
 
         :param problem: LP problem (solved)
-        :param nb_relations: number of relations supplied for training
+        :param nb_relations: number of relations supplied for learning
         :param inconsistencies:
             if ``True`` inconsistent comparisons will be taken into account
         """
         return (
             0
             if problem.status != 1
             else (
@@ -785,23 +789,23 @@
                 if inconsistencies
                 else 1
             )
         )
 
     @property
     def fitness(self) -> float:
-        """Return fitness of last trained solution.
+        """Return fitness of last learned solution.
 
         :return:
         """
         return self.compute_fitness(
             self.problem, len(self.relations), self.inconsistencies
         )
 
-    def _train_lexicographic_order(
+    def _learn_lexicographic_order(
         self, lexicographic_order: List[int]
     ) -> Tuple[Optional[SRMP], LpProblem]:
         """Train a SRMP instance using lexicographic order
 
         :param lexicographic_order: profile indices used sequentially to rank
         :return: the inferred SRMP object, along its LP problem
         """
@@ -911,20 +915,20 @@
                 if h != k:
                     # Dominance between the reference profiles
                     prob += p[h + 1][j] >= p[h][j]
 
                 for a in A_star:
                     # Constraints on the local concordances
                     prob += (
-                        performance_table.df.loc[a, j] - p[h][j]
+                        performance_table.data.loc[a, j] - p[h][j]
                         >= delta[a][h][j] - 1
                     )
                     prob += (
                         delta[a][h][j]
-                        >= performance_table.df.loc[a, j]
+                        >= performance_table.data.loc[a, j]
                         - p[h][j]
                         + self.gamma
                     )
 
                     # Constraints on the weighted local concordances
                     prob += omega[a][h][j] <= w[j]
                     prob += omega[a][h][j] >= 0
@@ -986,30 +990,31 @@
             return None, prob
 
         # Compute optimum solution
         criteria_weights = {j: pulp_value(w[j]) for j in M}
         profiles = PerformanceTable(
             [[pulp_value(p[h][j]) for j in M] for h in profile_indices],
             criteria=M,
+            scales={c: QuantitativeScale.normal() for c in M},
         )
         # Denormalize profile values
-        profiles = self._denormalize(
+        profiles = self.denormalize(
             profiles,
             cast(Dict[Any, QuantitativeScale], self.performance_table.scales),
         )
 
         return SRMP(criteria_weights, profiles, lexicographic_order), prob
 
-    def _train(
+    def _learn(
         self,
         lexicographic_order: List[int] = None,
         profiles_number: int = None,
         max_profiles_number: int = None,
     ) -> Tuple[Optional[SRMP], LpProblem]:
-        """Train a SRMP instance
+        """Learn a SRMP instance
 
         :param lexicographic_order: profile indices used sequentially to rank
         :param profiles_number: number of reference profiles
         :param max_profiles_number: highest number of reference profiles
         :return: the inferred SRMP object, along with its fitness
         :raise TypeError:
             * if `max_profiles_number`, `profiles_number` and
@@ -1022,33 +1027,33 @@
         """
         # Check parameters provided
         provided = (
             (max_profiles_number is not None)
             + (profiles_number is not None)
             + (lexicographic_order is not None)
         )
-        if provided == 0:
+        if provided == 0:  # pragma: nocover
             raise ValueError(
                 "You must specify either 'max_profiles_number',\
                 'profiles_number' or 'lexicographic_order'"
             )
         if lexicographic_order is not None:
-            # Compute the training algorithm
-            result, prob = self._train_lexicographic_order(lexicographic_order)
+            # Compute the learning algorithm
+            result, prob = self._learn_lexicographic_order(lexicographic_order)
             return result, prob
         if profiles_number is not None:
             lexicographic_order_list = list(
                 permutations(range(profiles_number))
             )
             best_result = None
             best_prob = None
             best_fitness = -1.0
             for current_lexicographic_order in lexicographic_order_list:
-                # Compute the training algorithm for each lexicographic order
-                result, prob = self._train(
+                # Compute the learning algorithm for each lexicographic order
+                result, prob = self._learn(
                     lexicographic_order=list(current_lexicographic_order),
                 )
                 fitness = self.compute_fitness(
                     prob, len(self.relations), self.inconsistencies
                 )
 
                 if fitness > best_fitness:
@@ -1066,36 +1071,36 @@
             else []
         )
 
         best_result = None
         best_prob = None
         best_fitness = -1.0
         for profiles_number in profiles_number_list:
-            # Compute the training algorithm for each profiles number
-            result, prob = self._train(
+            # Compute the learning algorithm for each profiles number
+            result, prob = self._learn(
                 profiles_number=profiles_number,
             )
             fitness = self.compute_fitness(
                 prob, len(self.relations), self.inconsistencies
             )
             if fitness > best_fitness:
                 best_result = result
                 best_fitness = fitness
                 best_prob = prob
             if best_fitness == 1:
                 # Break recursion when a perfect solution is found
                 break
         return best_result, best_prob
 
-    def train(self) -> Optional[SRMP]:
-        """Train and return SRMP solution (if existing).
+    def learn(self) -> Optional[SRMP]:
+        """Learn and return SRMP solution (if existing).
 
         :return:
         """
-        result, self.problem = self._train(
+        result, self.problem = self._learn(
             self.lexicographic_order,
             self.profiles_number,
             self.max_profiles_number,
         )
         return result
 
     @staticmethod
@@ -1108,15 +1113,15 @@
         :param x:
         :param scale:
         :return:
         """
         if isinstance(scale, QualitativeScale):
             denormalized_x = cast(
                 float,
-                QuantitativeScale.normal().transform_to(x, scale.quantitative),
+                QuantitativeScale.normal().transform(x, scale.quantitative),
             )
             closest_prefered_value = (
                 min(
                     [
                         value
                         for value in scale.values
                         if value >= denormalized_x
@@ -1129,35 +1134,39 @@
                         for value in scale.values
                         if value <= denormalized_x
                     ]
                 )
             )
             return scale.label_from_value(closest_prefered_value)
         else:
-            return QuantitativeScale.normal().transform_to(x, scale)
+            return QuantitativeScale.normal().transform(x, scale)
 
     @staticmethod
-    def _denormalize(
+    def denormalize(
         performance_table: PerformanceTable,
-        scales: Dict[str, QuantitativeScale],
+        scales: Dict[Any, QuantitativeScale],
     ) -> PerformanceTable:
         """Denormalize performance table with the closest preferred values
         available
 
         :param performance_table:
         :param scales: target criteria scales
         :return: denormalized performance table
         """
-        functions = {
-            criterion: (
-                cast(
-                    Function,
-                    lambda x, c=criterion: SRMPTrainer._denormalize_value(
-                        x, scales[c]
-                    ),
-                )
-            )  # https://bugs.python.org/issue13652
-            for criterion in scales.keys()
-        }
-        res = performance_table.apply_criteria_functions(functions)
-        res.scales = cast(Dict[Any, Scale], scales)
-        return res
+        functions = CriteriaFunctions(
+            {
+                criterion: (
+                    cast(
+                        Function,
+                        lambda x, c=criterion: SRMPLearner._denormalize_value(
+                            x, scales[c]
+                        ),
+                    )
+                )  # https://bugs.python.org/issue13652
+                for criterion in scales.keys()
+            },
+            in_scales={
+                criterion: QuantitativeScale.normal() for criterion in scales
+            },
+            out_scales=cast(Dict[Any, Scale], scales),
+        )
+        return functions(performance_table)
```

### Comparing `mcda-0.4.1/mcda/plot/plot.py` & `mcda-0.5.0/mcda/plot/plot.py`

 * *Files identical despite different names*

### Comparing `mcda-0.4.1/mcda.egg-info/SOURCES.txt` & `mcda-0.5.0/mcda.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -10,35 +10,27 @@
 mcda.egg-info/SOURCES.txt
 mcda.egg-info/dependency_links.txt
 mcda.egg-info/not-zip-safe
 mcda.egg-info/requires.txt
 mcda.egg-info/top_level.txt
 mcda/core/__init__.py
 mcda/core/aliases.py
+mcda/core/categories.py
+mcda/core/criteria_functions.py
 mcda/core/functions.py
 mcda/core/interfaces.py
 mcda/core/matrices.py
 mcda/core/performance_table.py
 mcda/core/relations.py
 mcda/core/scales.py
 mcda/core/set_functions.py
+mcda/core/values.py
 mcda/dea/__init__.py
 mcda/mavt/__init__.py
 mcda/mavt/aggregators.py
 mcda/mavt/uta.py
 mcda/outranking/__init__.py
 mcda/outranking/electre.py
 mcda/outranking/promethee.py
 mcda/outranking/srmp.py
 mcda/plot/__init__.py
-mcda/plot/plot.py
-tests/test_aggregators.py
-tests/test_electre.py
-tests/test_functions.py
-tests/test_matrices.py
-tests/test_performance_table.py
-tests/test_promethee.py
-tests/test_relations.py
-tests/test_scales.py
-tests/test_set_functions.py
-tests/test_srmp.py
-tests/test_uta.py
+mcda/plot/plot.py
```

### Comparing `mcda-0.4.1/setup.py` & `mcda-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import find_packages, setup
 
 with open("README.PYPI.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 
 setup(
     name="mcda",
-    version="0.4.1",
+    version="0.5.0",
     author="Nicolas Duminy",
     author_email="nicolas.duminy@imt-atlantique.fr",
     description="Package for Multi Criteria Decision Analysis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "Source": "https://gitlab.com/decide.imt-atlantique/pymcda",
```


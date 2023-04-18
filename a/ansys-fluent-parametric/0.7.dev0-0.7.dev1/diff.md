# Comparing `tmp/ansys_fluent_parametric-0.7.dev0.tar.gz` & `tmp/ansys_fluent_parametric-0.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_fluent_parametric-0.7.dev0.tar", max compression
+gzip compressed data, was "ansys_fluent_parametric-0.7.dev1.tar", max compression
```

## Comparing `ansys_fluent_parametric-0.7.dev0.tar` & `ansys_fluent_parametric-0.7.dev1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1089 2023-01-12 18:25:51.803971 ansys_fluent_parametric-0.7.dev0/LICENSE
--rw-r--r--   0        0        0     4503 2023-01-12 18:25:51.803971 ansys_fluent_parametric-0.7.dev0/README.rst
--rw-r--r--   0        0        0     1202 2023-01-12 18:25:51.807971 ansys_fluent_parametric-0.7.dev0/pyproject.toml
--rw-r--r--   0        0        0    24824 2023-01-12 18:25:52.075983 ansys_fluent_parametric-0.7.dev0/src/ansys/fluent/parametric/__init__.py
--rw-r--r--   0        0        0     9627 2023-01-12 18:25:51.807971 ansys_fluent_parametric-0.7.dev0/src/ansys/fluent/parametric/local/__init__.py
--rw-r--r--   0        0        0    10653 2023-01-12 18:25:51.807971 ansys_fluent_parametric-0.7.dev0/src/ansys/fluent/parametric/parameters.py
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 ansys_fluent_parametric-0.7.dev0/setup.py
--rw-r--r--   0        0        0     5627 1970-01-01 00:00:00.000000 ansys_fluent_parametric-0.7.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-04-13 01:02:43.437745 ansys_fluent_parametric-0.7.dev1/LICENSE
+-rw-r--r--   0        0        0     4503 2023-04-13 01:02:43.437745 ansys_fluent_parametric-0.7.dev1/README.rst
+-rw-r--r--   0        0        0     1202 2023-04-13 01:02:43.441745 ansys_fluent_parametric-0.7.dev1/pyproject.toml
+-rw-r--r--   0        0        0    24957 2023-04-13 01:02:43.753766 ansys_fluent_parametric-0.7.dev1/src/ansys/fluent/parametric/__init__.py
+-rw-r--r--   0        0        0     9626 2023-04-13 01:02:43.441745 ansys_fluent_parametric-0.7.dev1/src/ansys/fluent/parametric/local/__init__.py
+-rw-r--r--   0        0        0    10653 2023-04-13 01:02:43.441745 ansys_fluent_parametric-0.7.dev1/src/ansys/fluent/parametric/parameters.py
+-rw-r--r--   0        0        0     5627 1970-01-01 00:00:00.000000 ansys_fluent_parametric-0.7.dev1/PKG-INFO
```

### Comparing `ansys_fluent_parametric-0.7.dev0/LICENSE` & `ansys_fluent_parametric-0.7.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_fluent_parametric-0.7.dev0/README.rst` & `ansys_fluent_parametric-0.7.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_fluent_parametric-0.7.dev0/pyproject.toml` & `ansys_fluent_parametric-0.7.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-fluent-parametric"
-version = "0.7.dev0"
+version = "0.7.dev1"
 description = "A python wrapper for Ansys Fluent parametric workflows"
 license = "MIT"
 authors = ["ANSYS, Inc. <ansys.support@ansys.com>"]
 maintainers = ["PyAnsys developers <pyansys.maintainers@ansys.com>"]
 readme = "README.rst"
 repository = "https://github.com/pyansys/pyfluent-parametric"
 classifiers = [
@@ -21,15 +21,15 @@
 packages = [
     { include = "ansys", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 importlib-metadata = {version = "^4.0", python = "<3.8"}
-ansys-fluent-core = "~=0.12.dev0"
+ansys-fluent-core = "~=0.13.dev0"
 h5py = ">=3.7.0"
 
 [tool.black]
 line-length = 88
 
 [tool.isort]
 profile = "black"
```

### Comparing `ansys_fluent_parametric-0.7.dev0/src/ansys/fluent/parametric/__init__.py` & `ansys_fluent_parametric-0.7.dev1/src/ansys/fluent/parametric/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,27 +48,29 @@
 
 >>> from ansys.fluent.parametric import ParametricSession
 >>> session1 = ParametricSession(case_filepath="elbow_params_2.cas.h5")
 >>> session1.studies['elbow_params_2-Solve'].design_points['Base DP'].input_parameters  # noqa: E501
 >>> study2 = session1.new_study()
 >>> session2 = ParametricSession(project_filepath="nozzle_para_named.flprj")
 """
+import logging
 from pathlib import Path
 import tempfile
 from typing import Any, Dict, List, Optional
 
 import ansys.fluent.core as pyfluent
-from ansys.fluent.core import LOG
+
+logger = logging.getLogger("ansys.fluent")
 
 try:
     import importlib.metadata as importlib_metadata
 except ModuleNotFoundError:
     import importlib_metadata
 
-_VERSION_INFO = "Build date: January 12, 2023 18:25 UTC ShaID: b85ca75"
+_VERSION_INFO = "Build date: April 13, 2023 01:02 UTC ShaID: 5a64f4e"
 __version__ = importlib_metadata.version(__name__.replace(".", "-"))
 
 
 def version_info() -> str:
     """Method returning the version of PyFluent being used.
 
     Returns
@@ -93,17 +95,18 @@
     ----------
     name : str
         Name of the design point.
     dp_settings
 
     """
 
-    def __init__(self, name: str, dp_settings: Any):
+    def __init__(self, name: str, study: Any):
         self.name = name
-        self._dp_settings = dp_settings
+        self._study = study
+        self._dp_settings = study.design_points[name]
 
     @property
     def input_parameters(self) -> Dict[str, float]:
         """Dictionary of input parameter values by name."""
         return self._dp_settings.input_parameters()
 
     @input_parameters.setter
@@ -129,14 +132,18 @@
         """Whether to capture simulation report data for the design point."""
         return self._dp_settings.capture_simulation_report_data()
 
     @capture_simulation_report_data_enabled.setter
     def capture_simulation_report_data_enabled(self, value: bool) -> None:
         self._dp_settings.capture_simulation_report_data = value
 
+    def set_as_current(self) -> None:
+        """Set the design point as the current design point."""
+        self._study.design_points.set_as_current(design_point=self.name)
+
 
 class ParametricStudy:
     """Provides for managing parametric studies and their respective design points.
 
     A parametric study is used to parametrize design points in a Fluent solver
     set up. This class provides the ability to run Fluent for a series of
     design points and access or modify input and output parameters.
@@ -197,34 +204,34 @@
             self._parametric_studies.initialize(
                 project_filename=self.project_filepath.stem
             )
             new_study_names = self._parametric_studies.get_object_names()
             self.name = set(new_study_names).difference(set(old_study_names)).pop()
             base_design_point = DesignPoint(
                 BASE_DP_NAME,
-                self._parametric_studies[self.name].design_points[BASE_DP_NAME],
+                self._parametric_studies[self.name],
             )
             self.design_points = {BASE_DP_NAME: base_design_point}
             self.session.current_study_name = self.name
             return self
         else:
-            LOG.error("Initialize is not available.")
+            logging.error("Initialize is not available.")
 
     def rename(self, new_name: str) -> None:
         """Rename the parametric study.
 
         Parameters
         ----------
         new_name : str
             New name.
         """
         self._parametric_studies.rename(new_name, self.name)
         self.name = new_name
         self.design_points = {
-            k: DesignPoint(k, self._parametric_studies[self.name].design_points[k])
+            k: DesignPoint(k, self._parametric_studies[self.name])
             for k, _ in self.design_points.items()
         }
 
     @property
     def is_current(self) -> bool:
         """Whether the parametric study is the current parametric study."""
         return self.session.current_study_name == self.name
@@ -252,33 +259,33 @@
         old_study_names = self._parametric_studies.get_object_names()
         self._parametric_studies.duplicate(copy_design_points=copy_design_points)
         new_study_names = self._parametric_studies.get_object_names()
         clone_name = set(new_study_names).difference(set(old_study_names)).pop()
         current_study = self.get_all_studies()[self.session.current_study_name]
         if copy_design_points:
             clone_design_points = {
-                k: DesignPoint(k, self._parametric_studies[clone_name].design_points[k])
+                k: DesignPoint(k, self._parametric_studies[clone_name])
                 for k, _ in current_study.design_points.items()
             }
         else:
             base_design_point = DesignPoint(
                 BASE_DP_NAME,
-                self._parametric_studies[clone_name].design_points[BASE_DP_NAME],
+                self._parametric_studies[clone_name],
             )
             clone_design_points = {BASE_DP_NAME: base_design_point}
         clone = ParametricStudy(
             self._parametric_studies, self.session, clone_name, clone_design_points
         )
         self.session.current_study_name = clone.name
         return clone
 
     def delete(self) -> None:
         """Delete the parametric study."""
         if self.is_current:
-            LOG.error("Cannot delete the current study %s", self.name)
+            logging.error("Cannot delete the current study %s", self.name)
         else:
             del self._parametric_studies[self.name]
             self.session._all_studies.pop(id(self))
             del self
 
     def use_base_data(self) -> None:
         """Use base data for the parametric study."""
@@ -342,29 +349,29 @@
             write_data=write_data,
             capture_simulation_report_data=capture_simulation_report_data,
         )
         dps_after = dp_settings.get_object_names()
         dp_name = set(dps_after).difference(set(dps_before)).pop()
         design_point = DesignPoint(
             dp_name,
-            self._parametric_studies[self.name].design_points[dp_name],
+            self._parametric_studies[self.name],
         )
         self.design_points[dp_name] = design_point
         return design_point
 
     def delete_design_points(self, design_points: List[DesignPoint]) -> None:
         """Delete a list of design points.
 
         Parameters
         ----------
         design_points : List[DesignPoint]
             List of design points to delete.
         """
         if self.current_design_point in design_points:
-            LOG.error(
+            logging.error(
                 "Cannot delete the current design point %s",
                 self.current_design_point.name,
             )
             design_points.remove(self.current_design_point)
         dp_settings = self._parametric_studies[self.name].design_points
         dp_settings.delete_design_points(
             design_points=[dp.name for dp in design_points]
@@ -389,15 +396,15 @@
         dp_settings = self._parametric_studies[self.name].design_points
         dps_before = dp_settings.get_object_names()
         dp_settings.duplicate(design_point=design_point.name)
         dps_after = dp_settings.get_object_names()
         new_dp_name = set(dps_after).difference(set(dps_before)).pop()
         new_dp = DesignPoint(
             new_dp_name,
-            self._parametric_studies[self.name].design_points[new_dp_name],
+            self._parametric_studies[self.name],
         )
         self.design_points[new_dp_name] = new_dp
         return new_dp
 
     def save_journals(self, separate_journals: bool) -> None:
         """Save journals.
 
@@ -506,15 +513,15 @@
         )
         self.project_filepath = project_filepath
         for study_name in self._parametric_studies.get_object_names():
             study = ParametricStudy(self._parametric_studies, self.session, study_name)
             dps_settings = self._parametric_studies[study_name].design_points
             for dp_name in dps_settings.get_object_names():
                 study.design_points[dp_name] = DesignPoint(
-                    dp_name, dps_settings[dp_name]
+                    dp_name, self._parametric_studies[study_name]
                 )
 
     def save(self) -> None:
         """Save the project."""
         self._parametric_project.save()
 
     def save_as(self, project_filepath: str) -> None:
@@ -657,15 +664,15 @@
             )
             studies_settings = self._session.parametric_studies
             for study_name in studies_settings.get_object_names():
                 study = ParametricStudy(studies_settings, self, study_name)
                 dps_settings = studies_settings[study_name].design_points
                 for dp_name in dps_settings.get_object_names():
                     study.design_points[dp_name] = DesignPoint(
-                        dp_name, dps_settings[dp_name]
+                        dp_name, studies_settings[study_name]
                     )
                 self.studies[study_name] = study
             self.current_study_name = self._session.current_parametric_study()
 
     def new_study(self) -> ParametricStudy:
         """Create a new study.
 
@@ -684,15 +691,15 @@
         Parameters
         ----------
         study_name : str
             Study name.
         """
         study = self.studies[study_name]
         if study.is_current:
-            LOG.error("Cannot delete the current study %s", study_name)
+            logging.error("Cannot delete the current study %s", study_name)
         else:
             study.delete()
             self.studies.pop(study_name)
 
     def rename_study(self, new_name: str, old_name: str) -> None:
         """Rename a study.
```

### Comparing `ansys_fluent_parametric-0.7.dev0/src/ansys/fluent/parametric/local/__init__.py` & `ansys_fluent_parametric-0.7.dev1/src/ansys/fluent/parametric/local/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,14 @@
 def _run_local_study_in_fluent(
     local_study,
     num_servers: int,
     launcher: Any,
     start_transcript: bool,
     capture_report_data: bool,
 ):
-
     source_table_size = len(local_study.design_point_table)
 
     def make_input_for_study(design_point_range) -> None:
         if design_point_range is None:
             design_point_range = range(0, source_table_size)
         study_input = []
         for idx in design_point_range:
```

### Comparing `ansys_fluent_parametric-0.7.dev0/src/ansys/fluent/parametric/parameters.py` & `ansys_fluent_parametric-0.7.dev1/src/ansys/fluent/parametric/parameters.py`

 * *Files identical despite different names*

### Comparing `ansys_fluent_parametric-0.7.dev0/setup.py` & `ansys_fluent_parametric-0.7.dev1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,138 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ansys-fluent-parametric
+Version: 0.7.dev1
+Summary: A python wrapper for Ansys Fluent parametric workflows
+Home-page: https://github.com/pyansys/pyfluent-parametric
+License: MIT
+Author: ANSYS, Inc.
+Author-email: ansys.support@ansys.com
+Maintainer: PyAnsys developers
+Maintainer-email: pyansys.maintainers@ansys.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: ansys-fluent-core (>=0.13.dev0,<1.0)
+Requires-Dist: h5py (>=3.7.0)
+Requires-Dist: importlib-metadata (>=4.0,<5.0) ; python_version < "3.8"
+Project-URL: Repository, https://github.com/pyansys/pyfluent-parametric
+Description-Content-Type: text/x-rst
+
+PyFluent-Parametric
+===================
+|pyansys| |pypi| |GH-CI| |MIT| |black| |pre-commit|
+
+.. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
+   :target: https://docs.pyansys.com/
+   :alt: PyAnsys
+
+.. |pypi| image:: https://img.shields.io/pypi/v/ansys-fluent-parametric.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/ansys-fluent-parametric
+   :alt: PyPI
+
+.. |GH-CI| image:: https://github.com/pyansys/pyfluent-parametric/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/pyansys/pyfluent-parametric/actions/workflows/ci_cd.yml
+   :alt: GH-CI
+
+.. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
+   :target: https://opensource.org/licenses/MIT
+   :alt: MIT
+
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
+   :target: https://github.com/psf/black
+   :alt: Black
+
+.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/pyansys/pyfluent-parametric/main.svg
+   :target: https://results.pre-commit.ci/latest/github/pyansys/pyfluent-parametric/main
+   :alt: pre-commit.ci status
+
+Overview
+--------
+PyFluent-Parametric provides Pythonic access to Ansys Fluent's parametric
+workflows.
+
+Documentation and issues
+------------------------
+For comprehensive information on PyFluent-Parametric, see the latest
+release `documentation <https://fluentparametric.docs.pyansys.com>`_.
+
+On the `PyFluent-Parametric Issues <https://github.com/pyansys/pyfluent-parametric/issues>`_,
+you can create issues to submit questions, report bugs, and request new features. To reach
+the PyAnsys support team, email `pyansys.support@ansys.com <pyansys.support@ansys.com>`_.
+
+Installation
+------------
+The ``ansys-fluent-parametric`` package currently supports Python 3.7 through Python
+3.10 on Windows and Linux.
+
+Install the latest release from `PyPI
+<https://pypi.org/project/ansys-fluent-parametric/>`_ with:
+
+.. code:: console
+
+   pip install ansys-fluent-parametric
+
+Alternatively, install the latest from `GitHub
+<https://github.com/pyansys/pyfluent-parametric>`_ with:
+
+.. code:: console
+
+   pip install git+https://github.com/pyansys/pyfluent-parametric.git
+
+If you plan on doing local *development* of PyFluent with Git, install
+with:
+
+.. code:: console
+
+   git clone https://github.com/pyansys/pyfluent-parametric.git
+   cd pyfluent-parametric
+   pip install pip -U
+   pip install -e .
+
+Dependencies
+------------
+You must have a locally-installed, licensed copy of Ansys to run Fluent. The
+first supported version is 2022 R2.
+
+Getting started
+---------------
+
+Basic usage
+~~~~~~~~~~~
+The following code assumes that a PyFluent session has already been created and a Fluent case
+with input parameters has been set up. For a full example, see `Defining Parametric Workflows
+<https://fluentparametric.docs.pyansys.com/users_guide/parametric_workflows.html>`_ in
+the PyFluent-Parametric documentation.
+
+.. code:: python
+
+   import ansys.fluent.core as pyfluent
+   from ansys.fluent.parametric import ParametricStudy
+   solver_session = pyfluent.launch_fluent(mode="solver")
+   study = ParametricStudy(solver_session.parametric_studies).initialize()
+   input_parameters_update = study.design_points["Base DP"].input_parameters
+   input_parameters_update["inlet1_vel"] = 0.5
+   study.design_points["Base DP"].input_parameters = input_parameters_update
+   study.update_current_design_point()
+   print(study.design_points["Base DP"].output_parameters)
+
+License and acknowledgments
+---------------------------
+PyFluent-Parametric is licensed under the MIT license.
+
+PyFluent-Parametric makes no commercial claim over Ansys whatsoever. This library
+extends the functionality of Fluent by adding a Python interface to Fluent without
+changing the core behavior or license of the original software. The use of the
+interactive Fluent control of PyFluent-Parametric requires a legally licensed
+local copy of Fluent.
 
-package_dir = \
-{'': 'src'}
+For more information, see the `Ansys Fluent <https://www.ansys.com/products/fluids/ansys-fluent>`
+page on the Ansys website.
 
-packages = \
-['ansys', 'ansys.fluent.parametric', 'ansys.fluent.parametric.local']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['ansys-fluent-core>=0.12.dev0,<1.0', 'h5py>=3.7.0']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata>=4.0,<5.0']}
-
-setup_kwargs = {
-    'name': 'ansys-fluent-parametric',
-    'version': '0.7.dev0',
-    'description': 'A python wrapper for Ansys Fluent parametric workflows',
-    'long_description': 'PyFluent-Parametric\n===================\n|pyansys| |pypi| |GH-CI| |MIT| |black| |pre-commit|\n\n.. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC\n   :target: https://docs.pyansys.com/\n   :alt: PyAnsys\n\n.. |pypi| image:: https://img.shields.io/pypi/v/ansys-fluent-parametric.svg?logo=python&logoColor=white\n   :target: https://pypi.org/project/ansys-fluent-parametric\n   :alt: PyPI\n\n.. |GH-CI| image:: https://github.com/pyansys/pyfluent-parametric/actions/workflows/ci_cd.yml/badge.svg\n   :target: https://github.com/pyansys/pyfluent-parametric/actions/workflows/ci_cd.yml\n   :alt: GH-CI\n\n.. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg\n   :target: https://opensource.org/licenses/MIT\n   :alt: MIT\n\n.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat\n   :target: https://github.com/psf/black\n   :alt: Black\n\n.. |pre-commit| image:: https://results.pre-commit.ci/badge/github/pyansys/pyfluent-parametric/main.svg\n   :target: https://results.pre-commit.ci/latest/github/pyansys/pyfluent-parametric/main\n   :alt: pre-commit.ci status\n\nOverview\n--------\nPyFluent-Parametric provides Pythonic access to Ansys Fluent\'s parametric\nworkflows.\n\nDocumentation and issues\n------------------------\nFor comprehensive information on PyFluent-Parametric, see the latest\nrelease `documentation <https://fluentparametric.docs.pyansys.com>`_.\n\nOn the `PyFluent-Parametric Issues <https://github.com/pyansys/pyfluent-parametric/issues>`_,\nyou can create issues to submit questions, report bugs, and request new features. To reach\nthe PyAnsys support team, email `pyansys.support@ansys.com <pyansys.support@ansys.com>`_.\n\nInstallation\n------------\nThe ``ansys-fluent-parametric`` package currently supports Python 3.7 through Python\n3.10 on Windows and Linux.\n\nInstall the latest release from `PyPI\n<https://pypi.org/project/ansys-fluent-parametric/>`_ with:\n\n.. code:: console\n\n   pip install ansys-fluent-parametric\n\nAlternatively, install the latest from `GitHub\n<https://github.com/pyansys/pyfluent-parametric>`_ with:\n\n.. code:: console\n\n   pip install git+https://github.com/pyansys/pyfluent-parametric.git\n\nIf you plan on doing local *development* of PyFluent with Git, install\nwith:\n\n.. code:: console\n\n   git clone https://github.com/pyansys/pyfluent-parametric.git\n   cd pyfluent-parametric\n   pip install pip -U\n   pip install -e .\n\nDependencies\n------------\nYou must have a locally-installed, licensed copy of Ansys to run Fluent. The\nfirst supported version is 2022 R2.\n\nGetting started\n---------------\n\nBasic usage\n~~~~~~~~~~~\nThe following code assumes that a PyFluent session has already been created and a Fluent case\nwith input parameters has been set up. For a full example, see `Defining Parametric Workflows\n<https://fluentparametric.docs.pyansys.com/users_guide/parametric_workflows.html>`_ in\nthe PyFluent-Parametric documentation.\n\n.. code:: python\n\n   import ansys.fluent.core as pyfluent\n   from ansys.fluent.parametric import ParametricStudy\n   solver_session = pyfluent.launch_fluent(mode="solver")\n   study = ParametricStudy(solver_session.parametric_studies).initialize()\n   input_parameters_update = study.design_points["Base DP"].input_parameters\n   input_parameters_update["inlet1_vel"] = 0.5\n   study.design_points["Base DP"].input_parameters = input_parameters_update\n   study.update_current_design_point()\n   print(study.design_points["Base DP"].output_parameters)\n\nLicense and acknowledgments\n---------------------------\nPyFluent-Parametric is licensed under the MIT license.\n\nPyFluent-Parametric makes no commercial claim over Ansys whatsoever. This library\nextends the functionality of Fluent by adding a Python interface to Fluent without\nchanging the core behavior or license of the original software. The use of the\ninteractive Fluent control of PyFluent-Parametric requires a legally licensed\nlocal copy of Fluent.\n\nFor more information, see the `Ansys Fluent <https://www.ansys.com/products/fluids/ansys-fluent>`\npage on the Ansys website.\n',
-    'author': 'ANSYS, Inc.',
-    'author_email': 'ansys.support@ansys.com',
-    'maintainer': 'PyAnsys developers',
-    'maintainer_email': 'pyansys.maintainers@ansys.com',
-    'url': 'https://github.com/pyansys/pyfluent-parametric',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```


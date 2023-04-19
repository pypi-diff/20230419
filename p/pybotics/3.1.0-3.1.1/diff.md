# Comparing `tmp/pybotics-3.1.0.tar.gz` & `tmp/pybotics-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybotics-3.1.0.tar", max compression
+gzip compressed data, was "pybotics-3.1.1.tar", max compression
```

## Comparing `pybotics-3.1.0.tar` & `pybotics-3.1.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1072 2022-09-26 15:06:19.249781 pybotics-3.1.0/LICENSE
--rw-r--r--   0        0        0    13486 2022-09-26 15:06:19.249781 pybotics-3.1.0/README.md
--rw-r--r--   0        0        0       24 2022-09-26 15:06:19.261781 pybotics-3.1.0/pybotics/__init__.py
--rw-r--r--   0        0        0      315 2022-09-26 15:06:19.261781 pybotics-3.1.0/pybotics/errors.py
--rw-r--r--   0        0        0     4996 2022-09-26 15:06:19.261781 pybotics-3.1.0/pybotics/geometry.py
--rw-r--r--   0        0        0      941 2022-09-26 15:06:19.261781 pybotics-3.1.0/pybotics/json_encoder.py
--rw-r--r--   0        0        0     5438 2022-09-26 15:06:19.261781 pybotics-3.1.0/pybotics/kinematic_chain.py
--rw-r--r--   0        0        0     4282 2022-09-26 15:06:19.261781 pybotics-3.1.0/pybotics/link.py
--rw-r--r--   0        0        0     5369 2022-09-26 15:06:19.261781 pybotics-3.1.0/pybotics/optimization.py
--rw-r--r--   0        0        0     2046 2022-09-26 15:06:19.261781 pybotics-3.1.0/pybotics/predefined_models.py
--rw-r--r--   0        0        0     9324 2022-09-26 15:06:19.261781 pybotics-3.1.0/pybotics/robot.py
--rw-r--r--   0        0        0     1101 2022-09-26 15:06:19.261781 pybotics-3.1.0/pybotics/tool.py
--rw-r--r--   0        0        0     3243 2022-09-26 15:06:32.157851 pybotics-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    14384 1970-01-01 00:00:00.000000 pybotics-3.1.0/setup.py
--rw-r--r--   0        0        0    16130 1970-01-01 00:00:00.000000 pybotics-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-19 15:36:49.545798 pybotics-3.1.1/LICENSE
+-rw-r--r--   0        0        0    13486 2023-04-19 15:36:49.545798 pybotics-3.1.1/README.md
+-rw-r--r--   0        0        0       24 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/__init__.py
+-rw-r--r--   0        0        0      315 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/errors.py
+-rw-r--r--   0        0        0     4996 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/geometry.py
+-rw-r--r--   0        0        0      941 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/json_encoder.py
+-rw-r--r--   0        0        0     5438 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/kinematic_chain.py
+-rw-r--r--   0        0        0     4282 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/link.py
+-rw-r--r--   0        0        0     5369 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/optimization.py
+-rw-r--r--   0        0        0     2046 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/predefined_models.py
+-rw-r--r--   0        0        0     9324 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/robot.py
+-rw-r--r--   0        0        0     1101 2023-04-19 15:36:49.557798 pybotics-3.1.1/pybotics/tool.py
+-rw-r--r--   0        0        0     3552 2023-04-19 15:37:03.405912 pybotics-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0    16180 1970-01-01 00:00:00.000000 pybotics-3.1.1/PKG-INFO
```

### Comparing `pybotics-3.1.0/LICENSE` & `pybotics-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.0/README.md` & `pybotics-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.0/pybotics/geometry.py` & `pybotics-3.1.1/pybotics/geometry.py`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.0/pybotics/json_encoder.py` & `pybotics-3.1.1/pybotics/json_encoder.py`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.0/pybotics/kinematic_chain.py` & `pybotics-3.1.1/pybotics/kinematic_chain.py`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.0/pybotics/link.py` & `pybotics-3.1.1/pybotics/link.py`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.0/pybotics/optimization.py` & `pybotics-3.1.1/pybotics/optimization.py`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.0/pybotics/predefined_models.py` & `pybotics-3.1.1/pybotics/predefined_models.py`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.0/pybotics/robot.py` & `pybotics-3.1.1/pybotics/robot.py`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.0/pybotics/tool.py` & `pybotics-3.1.1/pybotics/tool.py`

 * *Files identical despite different names*

### Comparing `pybotics-3.1.0/pyproject.toml` & `pybotics-3.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybotics"
-version = "3.1.0"
+version = "3.1.1"
 description = "Python Toolbox for Robotics"
 authors = ["Nicholas Nadeau <nicholas.nadeau@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/engnadeau/pybotics"
 repository = "https://github.com/engnadeau/pybotics"
 documentation = "https://github.com/engnadeau/pybotics"
 keywords = ["robot", "research", "automation", "kinematics", "geometry"]
@@ -47,46 +47,61 @@
   "Topic :: System :: Hardware",
   "Topic :: System",
   "Topic :: Utilities",
   "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8,<3.11"
+python = "^3.8"
 attrs = ">=19.0"
 numpy = "^1.22"
 scipy = "^1.6"
 
-[tool.poetry.dev-dependencies]
-black = { extras = ["jupyter"], version = "^22.6.0" }
+[tool.poetry.group.dev.dependencies]
+black = { extras = ["jupyter"], version = "^23.0.0" }
+isort = ">=5.5"
+rope = ">=1"
+
+[tool.poetry.group.test]
+optional = true
+[tool.poetry.group.test.dependencies]
 coverage = ">=6"
-flake8 = ">=4"
-flake8-bugbear = "*"
 hypothesis = ">=6"
-isort = ">=5.5"
-matplotlib = "*"
-mccabe = "*"
-mypy = ">=0.960"
-nbconvert = ">=6.5.1"
-notebook = ">=6.4.12"
-pandas = "*"
-pep8-naming = "*"
-Pillow = ">=9.0.1"
-pydocstyle = ">=6"
 pytest = ">=7"
 pytest-cov = "*"
 pytest-randomly = "*"
 pytest-runner = "*"
-rope = ">=1"
-scikit-learn = "*"
+
+[tool.poetry.group.lint]
+optional = true
+[tool.poetry.group.lint.dependencies]
+flake8 = ">=4"
+flake8-bugbear = "*"
+mccabe = "*"
+mypy = ">=0.981"
+pep8-naming = "*"
+vulture = ">=2.0"
+
+[tool.poetry.group.docs]
+optional = true
+[tool.poetry.group.docs.dependencies]
 sphinx = "*"
 sphinx-autobuild = "*"
 sphinx-rtd-theme = "*"
 sphinxcontrib-apidoc = "*"
-vulture = ">=2.0"
+
+[tool.poetry.group.examples]
+optional = true
+[tool.poetry.group.examples.dependencies]
+matplotlib = "*"
+nbconvert = ">=6.5.1"
+notebook = ">=6.4.12"
+pandas = "*"
+Pillow = ">=9.0.1"
+scikit-learn = "*"
 
 [tool.black]
 line-length = 88
 target_version = ['py37']
 include = '\.pyi?$'
 exclude = '''
 (
```

### Comparing `pybotics-3.1.0/setup.py` & `pybotics-3.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,269 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pybotics
+Version: 3.1.1
+Summary: Python Toolbox for Robotics
+Home-page: https://github.com/engnadeau/pybotics
+Keywords: robot,research,automation,kinematics,geometry
+Author: Nicholas Nadeau
+Author-email: nicholas.nadeau@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Robot Framework
+Classifier: Framework :: Robot Framework :: Library
+Classifier: Framework :: Robot Framework :: Tool
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Manufacturing
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Education
+Classifier: Topic :: Other/Nonlisted Topic
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Testing :: Mocking
+Classifier: Topic :: System
+Classifier: Topic :: System :: Hardware
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Dist: attrs (>=19.0)
+Requires-Dist: numpy (>=1.22,<2.0)
+Requires-Dist: scipy (>=1.6,<2.0)
+Project-URL: Documentation, https://github.com/engnadeau/pybotics
+Project-URL: Repository, https://github.com/engnadeau/pybotics
+Description-Content-Type: text/markdown
 
-packages = \
-['pybotics']
+# Pybotics
 
-package_data = \
-{'': ['*']}
+![Robot arm logo](media/robotic-arm.png)
 
-install_requires = \
-['attrs>=19.0', 'numpy>=1.22,<2.0', 'scipy>=1.6,<2.0']
-
-setup_kwargs = {
-    'name': 'pybotics',
-    'version': '3.1.0',
-    'description': 'Python Toolbox for Robotics',
-    'long_description': '# Pybotics\n\n![Robot arm logo](media/robotic-arm.png)\n\nThe Python Toolbox for Robotics\n\n- [Explore the docs](https://pybotics.readthedocs.io)\n- [View demos and examples](https://github.com/nnadeau/pybotics/tree/master/examples)\n- [Report a bug](https://github.com/nnadeau/pybotics/issues)\n- [Request a feature](https://github.com/nnadeau/pybotics/issues)\n\n| Item          | Badges                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |\n| ------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| Repo          | [![GitHub issues](https://img.shields.io/github/issues/nnadeau/pybotics.svg)](https://github.com/nnadeau/pybotics/issues) [![GitHub forks](https://img.shields.io/github/forks/nnadeau/pybotics.svg)](https://github.com/nnadeau/pybotics/network) [![GitHub stars](https://img.shields.io/github/stars/nnadeau/pybotics.svg)](https://github.com/nnadeau/pybotics/stargazers) ![GitHub repo size](https://img.shields.io/github/repo-size/engnadeau/pybotics)                                                                                                                                                                                                                                                 |\n| Releases      | [![GitHub tag](https://img.shields.io/github/tag/nnadeau/pybotics.svg?maxAge=2592000?style=flat-square)](https://github.com/nnadeau/pybotics/releases) [![PyPI Version](https://img.shields.io/pypi/v/pybotics.svg)](https://pypi.python.org/pypi/pybotics) [![PyPI Wheel](https://img.shields.io/pypi/wheel/pybotics.svg)](https://pypi.python.org/pypi/pybotics) [![PyPI Format](https://img.shields.io/pypi/format/pybotics.svg)](https://pypi.python.org/pypi/pybotics) [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release) [![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pybotics) |\n| Compatibility | [![PyPI Pythons](https://img.shields.io/pypi/pyversions/pybotics.svg)](https://pypi.python.org/pypi/pybotics) [![PyPI Implementation](https://img.shields.io/pypi/implementation/pybotics.svg)](https://pypi.python.org/pypi/pybotics)                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |\n| Workflows     | [![Test](https://github.com/nnadeau/pybotics/workflows/Test/badge.svg)](https://github.com/nnadeau/pybotics/actions) [![Release](https://github.com/nnadeau/pybotics/workflows/Release/badge.svg)](https://github.com/nnadeau/pybotics/actions) [![Publish](https://github.com/nnadeau/pybotics/workflows/Publish/badge.svg)](https://github.com/nnadeau/pybotics/actions)                                                                                                                                                                                                                                                                                                                                     |\n| Documentation | [![Documentation Status](https://readthedocs.org/projects/pybotics/badge/?version=latest)](https://pybotics.readthedocs.io/en/latest/?badge=latest)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |\n| Citations     | [![DOI](https://joss.theoj.org/papers/10.21105/joss.01738/status.svg)](https://doi.org/10.21105/joss.01738) [![DOI](https://zenodo.org/badge/66797360.svg)](https://zenodo.org/badge/latestdoi/66797360)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |\n| License       | [![PyPI License](https://img.shields.io/pypi/l/pybotics.svg)](https://pypi.python.org/pypi/pybotics)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |\n| Social        | ![Twitter Follow](https://img.shields.io/twitter/follow/engnadeau?style=social) [![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fnnadeau%2Fpybotics)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fnnadeau%2Fpybotics)                                                                                                                                                                                                                                                                                                                                                                                                                  |\n\n## Contents\n\n- [Pybotics](#pybotics)\n  - [Contents](#contents)\n  - [Overview](#overview)\n  - [Usage](#usage)\n    - [Documentation](#documentation)\n    - [Installation](#installation)\n    - [Applications & Examples](#applications--examples)\n  - [Featured In](#featured-in)\n  - [Citing](#citing)\n  - [Development and Community Guidelines](#development-and-community-guidelines)\n    - [Local Development](#local-development)\n    - [Docker Development](#docker-development)\n    - [Commits](#commits)\n    - [Dependency Management](#dependency-management)\n    - [Submit an Issue](#submit-an-issue)\n    - [Contributing](#contributing)\n    - [Testing](#testing)\n    - [GitHub Actions](#github-actions)\n\n## Overview\n\n`Pybotics` is an open-source Python toolbox for robot kinematics and calibration.\nIt was designed to provide a simple, clear, and concise interface to quickly simulate and evaluate common robot concepts, such as kinematics, dynamics, trajectory generations, and calibration.\nThe toolbox is specifically designed for use with the [Modified Denavit–Hartenberg parameters convention](https://en.wikipedia.org/wiki/Denavit%E2%80%93Hartenberg_parameters#Modified_DH_parameters).\n\n## Usage\n\n### Documentation\n\nPlease visit https://pybotics.readthedocs.io/\n\n### Installation\n\n```bash\n# python3 is mapped to pip or inside a venv\npip install pybotics\n\n# python3-pip\npip3 install pybotics\n\n# https://github.com/pypa/pipenv\npipenv install pybotics\n\n# https://github.com/sdispater/poetry\npoetry add pybotics\n```\n\n### Applications & Examples\n\n- [Basic Usage](examples/basic_usage.py)\n- [Kinematics](examples/kinematics.ipynb)\n- [Calibration](examples/calibration.ipynb)\n- [Trajectory and Path Planning](examples/trajectory_generation.ipynb)\n- [Machine Learning](examples/machine_learning.ipynb)\n- [Dynamics](examples/dynamics.ipynb)\n\n## Featured In\n\n- [Impedance Control Self-Calibration of a Collaborative Robot Using Kinematic Coupling](https://www.mdpi.com/2218-6581/8/2/33/htm)\n- [PyCon Canada 2017](https://2017.pycon.ca/schedule/53/)\n  - [Talk Photos](https://500px.com/nicholasnadeau/galleries/pycon-canada-2017)\n  - [Slides](https://github.com/nnadeau/pycon-canada-2017)\n- [Montreal-Python 2017](https://www.youtube.com/watch?v=wgKoGA69YXQ)\n\n## Citing\n\nPlease cite the following articles if you use `pybotics` in your research:\n\n> Nadeau, (2019). Pybotics: Python Toolbox for Robotics. Journal of Open Source Software, 4(41), 1738, https://doi.org/10.21105/joss.01738\n\n```\n@article{nadeau2019pybotics,\n  doi = {10.21105/joss.01738},\n  url = {https://doi.org/10.21105/joss.01738},\n  year = {2019},\n  month = sep,\n  publisher = {The Open Journal},\n  volume = {4},\n  number = {41},\n  pages = {1738},\n  author = {Nicholas Nadeau},\n  title = {Pybotics: Python Toolbox for Robotics},\n  journal = {Journal of Open Source Software}\n}\n```\n\n> Nadeau, Nicholas A., Ilian A. Bonev, and Ahmed Joubair. "Impedance Control Self-Calibration of a Collaborative Robot Using Kinematic Coupling." Robotics 8.2 (2019): 33.\n\n```\n@article{nadeau2019impedance,\n  title={Impedance Control Self-Calibration of a Collaborative Robot Using Kinematic Coupling},\n  volume={8},\n  ISSN={2218-6581},\n  url={http://dx.doi.org/10.3390/robotics8020033},\n  DOI={10.3390/robotics8020033},\n  number={2},\n  journal={Robotics},\n  publisher={MDPI AG},\n  author={Nadeau, Nicholas A. and Bonev, Ilian A. and Joubair, Ahmed},\n  year={2019},\n  month={Apr},\n  pages={33}\n}\n```\n\n## Development and Community Guidelines\n\n### Local Development\n\n- Use [poetry](https://python-poetry.org/) to install the dev virtual environment:\n\n```bash\npoetry install\n```\n\n### Docker Development\n\n- Docker is a great tool to test the package in an isolated environment\n- It is especially useful for debugging issues between python versions\n\n```bash\n# launch container attached to current directory\ndocker run -v $(pwd):/$(basename $(pwd)) -w /$(basename $(pwd)) -it python:3 bash\n\n# install deps\npip install poetry\npoetry install\n\n# run tests\nmake test\n```\n\n### Commits\n\n- The repo abides by [SemVer](https://semver.org/), [`semantic-release`](https://github.com/semantic-release/semantic-release), and [Angular commit message syntax](https://github.com/angular/angular/blob/main/CONTRIBUTING.md)\n- It is highly recommended to use the [`commitizen` CLI](https://github.com/commitizen/cz-cli)\n- See commit examples below:\n\n| Change                    | Commit Type |\n| ------------------------- | ----------- |\n| Bumped dependency version | `build`     |\n| Bumped Python requirement | `feat`      |\n\n### Dependency Management\n\n```bash\n# refresh lock file\npoetry lock --no-update\n```\n\n### Submit an Issue\n\n- Navigate to the repository\'s [issue tab](https://github.com/nnadeau/pybotics/issues)\n- Search for related existing issues\n- If necessary, create a new issue using the provided templates\n\n### Contributing\n\n- Please see [`CONTRIBUTING.md`](.github/CONTRIBUTING.md) and the [Code of Conduct](CODE_OF_CONDUCT.md) for how to contribute to the project\n\n### Testing\n\n- Please review the [`Makefile`](Makefile) for an overview of all available tests\n- The most important tests and `make` commands are highlighted below:\n\n```bash\n# auto-format code\nmake format\n\n# perform all static tests\nmake lint\n\n# run all python tests\nmake test\n```\n\n### GitHub Actions\n\n- This repo uses [`semantic-releases`](https://github.com/semantic-release/) to generate releases and release notes automatically from commits\n  - A [`PERSONAL_TOKEN` Actions secret](https://github.com/nnadeau/pybotics/settings/secrets/actions) from a [Personal Token](https://github.com/settings/tokens) with a [`public_repo` scope](https://github.com/semantic-release/github#github-authentication) is needed for CI releases\n\n---\n\nIcons made by <a href="https://icon54.com/" title="Pixel perfect">Pixel perfect</a> from <a href="https://www.flaticon.com/" title="Flaticon"> www.flaticon.com</a>\n',
-    'author': 'Nicholas Nadeau',
-    'author_email': 'nicholas.nadeau@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/engnadeau/pybotics',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
+The Python Toolbox for Robotics
+
+- [Explore the docs](https://pybotics.readthedocs.io)
+- [View demos and examples](https://github.com/nnadeau/pybotics/tree/master/examples)
+- [Report a bug](https://github.com/nnadeau/pybotics/issues)
+- [Request a feature](https://github.com/nnadeau/pybotics/issues)
+
+| Item          | Badges                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| ------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| Repo          | [![GitHub issues](https://img.shields.io/github/issues/nnadeau/pybotics.svg)](https://github.com/nnadeau/pybotics/issues) [![GitHub forks](https://img.shields.io/github/forks/nnadeau/pybotics.svg)](https://github.com/nnadeau/pybotics/network) [![GitHub stars](https://img.shields.io/github/stars/nnadeau/pybotics.svg)](https://github.com/nnadeau/pybotics/stargazers) ![GitHub repo size](https://img.shields.io/github/repo-size/engnadeau/pybotics)                                                                                                                                                                                                                                                 |
+| Releases      | [![GitHub tag](https://img.shields.io/github/tag/nnadeau/pybotics.svg?maxAge=2592000?style=flat-square)](https://github.com/nnadeau/pybotics/releases) [![PyPI Version](https://img.shields.io/pypi/v/pybotics.svg)](https://pypi.python.org/pypi/pybotics) [![PyPI Wheel](https://img.shields.io/pypi/wheel/pybotics.svg)](https://pypi.python.org/pypi/pybotics) [![PyPI Format](https://img.shields.io/pypi/format/pybotics.svg)](https://pypi.python.org/pypi/pybotics) [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release) [![semantic-release: angular](https://img.shields.io/badge/semantic--release-angular-e10079?logo=semantic-release)](https://github.com/semantic-release/semantic-release) ![PyPI - Downloads](https://img.shields.io/pypi/dm/pybotics) |
+| Compatibility | [![PyPI Pythons](https://img.shields.io/pypi/pyversions/pybotics.svg)](https://pypi.python.org/pypi/pybotics) [![PyPI Implementation](https://img.shields.io/pypi/implementation/pybotics.svg)](https://pypi.python.org/pypi/pybotics)                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| Workflows     | [![Test](https://github.com/nnadeau/pybotics/workflows/Test/badge.svg)](https://github.com/nnadeau/pybotics/actions) [![Release](https://github.com/nnadeau/pybotics/workflows/Release/badge.svg)](https://github.com/nnadeau/pybotics/actions) [![Publish](https://github.com/nnadeau/pybotics/workflows/Publish/badge.svg)](https://github.com/nnadeau/pybotics/actions)                                                                                                                                                                                                                                                                                                                                     |
+| Documentation | [![Documentation Status](https://readthedocs.org/projects/pybotics/badge/?version=latest)](https://pybotics.readthedocs.io/en/latest/?badge=latest)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+| Citations     | [![DOI](https://joss.theoj.org/papers/10.21105/joss.01738/status.svg)](https://doi.org/10.21105/joss.01738) [![DOI](https://zenodo.org/badge/66797360.svg)](https://zenodo.org/badge/latestdoi/66797360)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| License       | [![PyPI License](https://img.shields.io/pypi/l/pybotics.svg)](https://pypi.python.org/pypi/pybotics)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+| Social        | ![Twitter Follow](https://img.shields.io/twitter/follow/engnadeau?style=social) [![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fnnadeau%2Fpybotics)](https://twitter.com/intent/tweet?text=Wow:&url=https%3A%2F%2Fgithub.com%2Fnnadeau%2Fpybotics)                                                                                                                                                                                                                                                                                                                                                                                                                  |
+
+## Contents
+
+- [Pybotics](#pybotics)
+  - [Contents](#contents)
+  - [Overview](#overview)
+  - [Usage](#usage)
+    - [Documentation](#documentation)
+    - [Installation](#installation)
+    - [Applications & Examples](#applications--examples)
+  - [Featured In](#featured-in)
+  - [Citing](#citing)
+  - [Development and Community Guidelines](#development-and-community-guidelines)
+    - [Local Development](#local-development)
+    - [Docker Development](#docker-development)
+    - [Commits](#commits)
+    - [Dependency Management](#dependency-management)
+    - [Submit an Issue](#submit-an-issue)
+    - [Contributing](#contributing)
+    - [Testing](#testing)
+    - [GitHub Actions](#github-actions)
+
+## Overview
+
+`Pybotics` is an open-source Python toolbox for robot kinematics and calibration.
+It was designed to provide a simple, clear, and concise interface to quickly simulate and evaluate common robot concepts, such as kinematics, dynamics, trajectory generations, and calibration.
+The toolbox is specifically designed for use with the [Modified Denavit–Hartenberg parameters convention](https://en.wikipedia.org/wiki/Denavit%E2%80%93Hartenberg_parameters#Modified_DH_parameters).
+
+## Usage
+
+### Documentation
+
+Please visit https://pybotics.readthedocs.io/
+
+### Installation
+
+```bash
+# python3 is mapped to pip or inside a venv
+pip install pybotics
+
+# python3-pip
+pip3 install pybotics
+
+# https://github.com/pypa/pipenv
+pipenv install pybotics
+
+# https://github.com/sdispater/poetry
+poetry add pybotics
+```
+
+### Applications & Examples
+
+- [Basic Usage](examples/basic_usage.py)
+- [Kinematics](examples/kinematics.ipynb)
+- [Calibration](examples/calibration.ipynb)
+- [Trajectory and Path Planning](examples/trajectory_generation.ipynb)
+- [Machine Learning](examples/machine_learning.ipynb)
+- [Dynamics](examples/dynamics.ipynb)
+
+## Featured In
+
+- [Impedance Control Self-Calibration of a Collaborative Robot Using Kinematic Coupling](https://www.mdpi.com/2218-6581/8/2/33/htm)
+- [PyCon Canada 2017](https://2017.pycon.ca/schedule/53/)
+  - [Talk Photos](https://500px.com/nicholasnadeau/galleries/pycon-canada-2017)
+  - [Slides](https://github.com/nnadeau/pycon-canada-2017)
+- [Montreal-Python 2017](https://www.youtube.com/watch?v=wgKoGA69YXQ)
+
+## Citing
+
+Please cite the following articles if you use `pybotics` in your research:
+
+> Nadeau, (2019). Pybotics: Python Toolbox for Robotics. Journal of Open Source Software, 4(41), 1738, https://doi.org/10.21105/joss.01738
+
+```
+@article{nadeau2019pybotics,
+  doi = {10.21105/joss.01738},
+  url = {https://doi.org/10.21105/joss.01738},
+  year = {2019},
+  month = sep,
+  publisher = {The Open Journal},
+  volume = {4},
+  number = {41},
+  pages = {1738},
+  author = {Nicholas Nadeau},
+  title = {Pybotics: Python Toolbox for Robotics},
+  journal = {Journal of Open Source Software}
+}
+```
+
+> Nadeau, Nicholas A., Ilian A. Bonev, and Ahmed Joubair. "Impedance Control Self-Calibration of a Collaborative Robot Using Kinematic Coupling." Robotics 8.2 (2019): 33.
+
+```
+@article{nadeau2019impedance,
+  title={Impedance Control Self-Calibration of a Collaborative Robot Using Kinematic Coupling},
+  volume={8},
+  ISSN={2218-6581},
+  url={http://dx.doi.org/10.3390/robotics8020033},
+  DOI={10.3390/robotics8020033},
+  number={2},
+  journal={Robotics},
+  publisher={MDPI AG},
+  author={Nadeau, Nicholas A. and Bonev, Ilian A. and Joubair, Ahmed},
+  year={2019},
+  month={Apr},
+  pages={33}
 }
+```
+
+## Development and Community Guidelines
+
+### Local Development
+
+- Use [poetry](https://python-poetry.org/) to install the dev virtual environment:
+
+```bash
+poetry install
+```
+
+### Docker Development
+
+- Docker is a great tool to test the package in an isolated environment
+- It is especially useful for debugging issues between python versions
+
+```bash
+# launch container attached to current directory
+docker run -v $(pwd):/$(basename $(pwd)) -w /$(basename $(pwd)) -it python:3 bash
+
+# install deps
+pip install poetry
+poetry install
+
+# run tests
+make test
+```
+
+### Commits
+
+- The repo abides by [SemVer](https://semver.org/), [`semantic-release`](https://github.com/semantic-release/semantic-release), and [Angular commit message syntax](https://github.com/angular/angular/blob/main/CONTRIBUTING.md)
+- It is highly recommended to use the [`commitizen` CLI](https://github.com/commitizen/cz-cli)
+- See commit examples below:
+
+| Change                    | Commit Type |
+| ------------------------- | ----------- |
+| Bumped dependency version | `build`     |
+| Bumped Python requirement | `feat`      |
+
+### Dependency Management
+
+```bash
+# refresh lock file
+poetry lock --no-update
+```
+
+### Submit an Issue
+
+- Navigate to the repository's [issue tab](https://github.com/nnadeau/pybotics/issues)
+- Search for related existing issues
+- If necessary, create a new issue using the provided templates
+
+### Contributing
+
+- Please see [`CONTRIBUTING.md`](.github/CONTRIBUTING.md) and the [Code of Conduct](CODE_OF_CONDUCT.md) for how to contribute to the project
+
+### Testing
+
+- Please review the [`Makefile`](Makefile) for an overview of all available tests
+- The most important tests and `make` commands are highlighted below:
+
+```bash
+# auto-format code
+make format
+
+# perform all static tests
+make lint
+
+# run all python tests
+make test
+```
+
+### GitHub Actions
+
+- This repo uses [`semantic-releases`](https://github.com/semantic-release/) to generate releases and release notes automatically from commits
+  - A [`PERSONAL_TOKEN` Actions secret](https://github.com/nnadeau/pybotics/settings/secrets/actions) from a [Personal Token](https://github.com/settings/tokens) with a [`public_repo` scope](https://github.com/semantic-release/github#github-authentication) is needed for CI releases
+
+---
 
+Icons made by <a href="https://icon54.com/" title="Pixel perfect">Pixel perfect</a> from <a href="https://www.flaticon.com/" title="Flaticon"> www.flaticon.com</a>
 
-setup(**setup_kwargs)
```


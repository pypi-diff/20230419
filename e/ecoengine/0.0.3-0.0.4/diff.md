# Comparing `tmp/ecoengine-0.0.3.tar.gz` & `tmp/ecoengine-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoengine-0.0.3.tar", last modified: Thu Apr 13 18:51:18 2023, max compression
+gzip compressed data, was "ecoengine-0.0.4.tar", last modified: Wed Apr 19 19:39:24 2023, max compression
```

## Comparing `ecoengine-0.0.3.tar` & `ecoengine-0.0.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:51:18.924722 ecoengine-0.0.3/
--rw-rw-rw-   0        0        0       45 2023-04-13 18:49:37.000000 ecoengine-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3815 2023-04-13 18:51:18.954344 ecoengine-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3175 2023-04-11 19:29:37.000000 ecoengine-0.0.3/README.md
--rw-rw-rw-   0        0        0      108 2023-03-28 18:57:57.000000 ecoengine-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      767 2023-04-13 18:51:18.997104 ecoengine-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-04-11 19:29:37.000000 ecoengine-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:51:15.848715 ecoengine-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 18:51:16.292716 ecoengine-0.0.3/src/ecoengine/
--rw-rw-rw-   0        0        0      915 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:51:16.848717 ecoengine-0.0.3/src/ecoengine/constants/
--rw-rw-rw-   0        0        0      457 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/constants/Constants.py
--rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/constants/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:51:16.904718 ecoengine-0.0.3/src/ecoengine/data/
--rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:51:17.872720 ecoengine-0.0.3/src/ecoengine/data/load_shapes/
--rw-rw-rw-   0        0        0        0 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/__init__.py
--rw-rw-rw-   0        0        0     1295 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/apartment.json
--rw-rw-rw-   0        0        0      971 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/elementary_school.json
--rw-rw-rw-   0        0        0     1127 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/food_service_a.json
--rw-rw-rw-   0        0        0     1272 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/food_service_b.json
--rw-rw-rw-   0        0        0     1240 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/junior_high.json
--rw-rw-rw-   0        0        0     1259 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/mens_dorm.json
--rw-rw-rw-   0        0        0     1259 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/motel.json
--rw-rw-rw-   0        0        0    47218 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/multi_family.json
--rw-rw-rw-   0        0        0     1273 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/nursing_home.json
--rw-rw-rw-   0        0        0     1058 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/office_building.json
--rw-rw-rw-   0        0        0     1120 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/senior_high.json
--rw-rw-rw-   0        0        0     1219 2023-04-11 19:29:37.000000 ecoengine-0.0.3/src/ecoengine/data/load_shapes/womens_dorm.json
-drwxrwxrwx   0        0        0        0 2023-04-13 18:51:18.124720 ecoengine-0.0.3/src/ecoengine/engine/
--rw-rw-rw-   0        0        0     6879 2023-04-13 17:58:46.000000 ecoengine-0.0.3/src/ecoengine/engine/BuildingCreator.py
--rw-rw-rw-   0        0        0     7508 2023-04-13 17:57:47.000000 ecoengine-0.0.3/src/ecoengine/engine/EcosizerEngine.py
--rw-rw-rw-   0        0        0     2924 2023-04-11 19:29:38.000000 ecoengine-0.0.3/src/ecoengine/engine/SystemCreator.py
--rw-rw-rw-   0        0        0      894 2023-04-11 19:29:38.000000 ecoengine-0.0.3/src/ecoengine/engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:51:18.604722 ecoengine-0.0.3/src/ecoengine/objects/
--rw-rw-rw-   0        0        0     9746 2023-04-13 17:58:54.000000 ecoengine-0.0.3/src/ecoengine/objects/Building.py
--rw-rw-rw-   0        0        0    23618 2023-04-11 19:29:38.000000 ecoengine-0.0.3/src/ecoengine/objects/SystemConfig.py
--rw-rw-rw-   0        0        0      940 2023-04-11 19:29:38.000000 ecoengine-0.0.3/src/ecoengine/objects/__init__.py
--rw-rw-rw-   0        0        0     2948 2023-04-11 19:29:38.000000 ecoengine-0.0.3/src/ecoengine/objects/systemConfigUtils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:51:18.852722 ecoengine-0.0.3/src/ecoengine/objects/systems/
--rw-rw-rw-   0        0        0     3509 2023-04-11 19:29:38.000000 ecoengine-0.0.3/src/ecoengine/objects/systems/ParallelLoopTank.py
--rw-rw-rw-   0        0        0    16890 2023-04-11 19:29:38.000000 ecoengine-0.0.3/src/ecoengine/objects/systems/SwingTank.py
--rw-rw-rw-   0        0        0        0 2023-04-11 19:29:38.000000 ecoengine-0.0.3/src/ecoengine/objects/systems/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:51:16.684717 ecoengine-0.0.3/src/ecoengine.egg-info/
--rw-rw-rw-   0        0        0     3815 2023-04-13 18:51:15.000000 ecoengine-0.0.3/src/ecoengine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1430 2023-04-13 18:51:15.000000 ecoengine-0.0.3/src/ecoengine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:51:15.000000 ecoengine-0.0.3/src/ecoengine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-13 18:51:15.000000 ecoengine-0.0.3/src/ecoengine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 18:51:15.000000 ecoengine-0.0.3/src/ecoengine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.928132 ecoengine-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-19 19:38:51.000000 ecoengine-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-19 19:39:24.928132 ecoengine-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-19 19:38:51.000000 ecoengine-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 19:38:51.000000 ecoengine-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-19 19:39:24.932132 ecoengine-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-19 19:38:51.000000 ecoengine-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.916132 ecoengine-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.920132 ecoengine-0.0.4/src/ecoengine/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.920132 ecoengine-0.0.4/src/ecoengine/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/constants/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.920132 ecoengine-0.0.4/src/ecoengine/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.924131 ecoengine-0.0.4/src/ecoengine/data/load_shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/apartment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/elementary_school.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/food_service_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/food_service_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/junior_high.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/mens_dorm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/motel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47218 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/multi_family.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/nursing_home.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/office_building.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/senior_high.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/data/load_shapes/womens_dorm.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.928132 ecoengine-0.0.4/src/ecoengine/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/engine/BuildingCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/engine/EcosizerEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/engine/SystemCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.928132 ecoengine-0.0.4/src/ecoengine/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/objects/Building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23618 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/objects/SystemConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/objects/systemConfigUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.928132 ecoengine-0.0.4/src/ecoengine/objects/systems/
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/objects/systems/ParallelLoopTank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16890 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/objects/systems/SwingTank.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:38:51.000000 ecoengine-0.0.4/src/ecoengine/objects/systems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:24.920132 ecoengine-0.0.4/src/ecoengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-19 19:39:24.000000 ecoengine-0.0.4/src/ecoengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-19 19:39:24.000000 ecoengine-0.0.4/src/ecoengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:39:24.000000 ecoengine-0.0.4/src/ecoengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-19 19:39:24.000000 ecoengine-0.0.4/src/ecoengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 19:39:24.000000 ecoengine-0.0.4/src/ecoengine.egg-info/top_level.txt
```

### Comparing `ecoengine-0.0.3/PKG-INFO` & `ecoengine-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-Metadata-Version: 2.1
-Name: ecoengine
-Version: 0.0.3
-Summary: A software for sizing Heat Pump Water Heaters for buildings
-Home-page: https://ecosizer.ecotope.com/sizer/
-Author: Nolan
-Author-email: nolan@ecotope.com
-Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-
-# EcosizerEngine
-
-### Requirements:
-
-This software requires a python version greater than or equal to 3.11 to be installed in the environment it is running in.
-
-### Using the package in scripts:
-
-1. Install the package with pip
-
-	$ pip install ecosizer-engine
-
-2. To import and use the tools in this package, add the following import statement to your script:
-
-	from ecosizer_engine_package import *
-
-You should now be able to use the features of EcosizerEngine in your script
-
-### Running locally in a container:
-First, clone the EcosizerEngine repo from github
-
-    $ git clone https://github.com/EcotopeResearch/EcosizerEngine.git
-
-Depending on what type of environment you want to run the code in, please follow the appropriate steps.
-
-Steps for installing in a virtual environment:
-1. Navigate to the EcosizerEngine directory. This should be the same directory level as src/, setup.py, and this README document.
-2. Run the following command:
-
-	$ pip install -e .
-
-This will install the ecosizer-engine package locally in editable format, such that changes you make in the source code here will be reflected in implementation.
-This pip install should also install all dependencies for ecosizer-engine (i.e. numpy, scipy, pytest, and plotly)
-
-Steps for installing using docker container:
-1. Navigate to the EcosizerEngine directory.
-2. Build container with docker file
-
-	$ docker build -t ecosizerengine:latest .
-
-3. Run docker container
-
-	$  docker run -it ecosizerengine bash
-
-4. When you are done messing about in the docker image, just type the command
-
-	$ exit
-
-or press ctrl+c then ctrl+d
-
-Steps for installing conda environment from the Anaconda prompt:
-1. Navigate to the EcosizerEngine directory.
-2. Create new environment from .yml file.
-
-
-	$ conda env create --file EcosizerEngine.yml
-
-If the environment creation doesn't work, make sure Anaconda is up-to-date with
-
-    $ conda update --all
-
-If that doesn't work, you may need to force Anaconda to download and use python 3.11 (it defaults to 3.9) by making another environment
-
-    $ conda create -n py311 python=3.11
-    $ conda activate py311
-    $ conda env create --file EcosizerEngine.yml
-
-3. Check that the environment was created
-
-
-	$ conda env list
-
-4. Activate the new environment
-
-
-	$ conda activate EcosizerEngine
-
-If an environment already exits it can be removed with:
-
-	$ conda remove --name EcosizerEngine --all
-
-
-All the available environment can be found with:
-
-	$ conda env list
-
-### Testing:
-From the parent directory, type
-
-	$ python -m pytest
-
-This will run all unit tests for the package
-
-### Updating Documentation:
-1. If not installed in environment: pip install sphinx and numpydocs
-2. navigate to docs directory and run:
-
-
-	$ make html
-
-### Updating version on pypi
-
-1. If you haven't installed them before, pip install build and twine
-
-	$ python -m pip install --upgrade build
-
-
-	$ python -m pip install --user --upgrade twine
-
-2. Update the version number in setup.cfg
-3. Run the following commands from the project root directory:
-
-	$ python -m build
-
-	$ python -m twine upload dist/*
-
-### Contact Information
-To get in touch with Ecotope Inc. go here: http://ecotope.com/contact/
+Metadata-Version: 2.1
+Name: ecoengine
+Version: 0.0.4
+Summary: A software for sizing Heat Pump Water Heaters for buildings
+Home-page: https://ecosizer.ecotope.com/sizer/
+Author: Nolan
+Author-email: nolan@ecotope.com
+Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+
+# EcosizerEngine
+
+### Requirements:
+
+This software requires a python version greater than or equal to 3.11 to be installed in the environment it is running in.
+
+### Using the package in scripts:
+
+1. Install the package with pip
+
+	$ pip install ecosizer-engine
+
+2. To import and use the tools in this package, add the following import statement to your script:
+
+	from ecosizer_engine_package import *
+
+You should now be able to use the features of EcosizerEngine in your script
+
+### Running locally in a container:
+First, clone the EcosizerEngine repo from github
+
+    $ git clone https://github.com/EcotopeResearch/EcosizerEngine.git
+
+Depending on what type of environment you want to run the code in, please follow the appropriate steps.
+
+Steps for installing in a virtual environment:
+1. Navigate to the EcosizerEngine directory. This should be the same directory level as src/, setup.py, and this README document.
+2. Run the following command:
+
+	$ pip install -e .
+
+This will install the ecosizer-engine package locally in editable format, such that changes you make in the source code here will be reflected in implementation.
+This pip install should also install all dependencies for ecosizer-engine (i.e. numpy, scipy, pytest, and plotly)
+
+Steps for installing using docker container:
+1. Navigate to the EcosizerEngine directory.
+2. Build container with docker file
+
+	$ docker build -t ecosizerengine:latest .
+
+3. Run docker container
+
+	$  docker run -it ecosizerengine bash
+
+4. When you are done messing about in the docker image, just type the command
+
+	$ exit
+
+or press ctrl+c then ctrl+d
+
+Steps for installing conda environment from the Anaconda prompt:
+1. Navigate to the EcosizerEngine directory.
+2. Create new environment from .yml file.
+
+
+	$ conda env create --file EcosizerEngine.yml
+
+If the environment creation doesn't work, make sure Anaconda is up-to-date with
+
+    $ conda update --all
+
+If that doesn't work, you may need to force Anaconda to download and use python 3.11 (it defaults to 3.9) by making another environment
+
+    $ conda create -n py311 python=3.11
+    $ conda activate py311
+    $ conda env create --file EcosizerEngine.yml
+
+3. Check that the environment was created
+
+
+	$ conda env list
+
+4. Activate the new environment
+
+
+	$ conda activate EcosizerEngine
+
+If an environment already exits it can be removed with:
+
+	$ conda remove --name EcosizerEngine --all
+
+
+All the available environment can be found with:
+
+	$ conda env list
+
+### Testing:
+From the parent directory, type
+
+	$ python -m pytest
+
+This will run all unit tests for the package
+
+### Updating Documentation:
+1. If not installed in environment: pip install sphinx and numpydocs
+2. navigate to docs directory and run:
+
+
+	$ make html
+
+### Updating version on pypi
+
+1. If you haven't installed them before, pip install build and twine
+
+	$ python -m pip install --upgrade build
+
+
+	$ python -m pip install --user --upgrade twine
+
+2. Update the version number in setup.cfg
+3. Run the following commands from the project root directory:
+
+	$ python -m build
+
+	$ python -m twine upload dist/*
+
+### Contact Information
+To get in touch with Ecotope Inc. go here: http://ecotope.com/contact/
```

### Comparing `ecoengine-0.0.3/README.md` & `ecoengine-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/__init__.py` & `ecoengine-0.0.4/src/ecoengine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/data/load_shapes/apartment.json` & `ecoengine-0.0.4/src/ecoengine/data/load_shapes/apartment.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/data/load_shapes/elementary_school.json` & `ecoengine-0.0.4/src/ecoengine/data/load_shapes/elementary_school.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/data/load_shapes/food_service_a.json` & `ecoengine-0.0.4/src/ecoengine/data/load_shapes/food_service_a.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/data/load_shapes/food_service_b.json` & `ecoengine-0.0.4/src/ecoengine/data/load_shapes/food_service_b.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/data/load_shapes/junior_high.json` & `ecoengine-0.0.4/src/ecoengine/data/load_shapes/junior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/data/load_shapes/mens_dorm.json` & `ecoengine-0.0.4/src/ecoengine/data/load_shapes/mens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/data/load_shapes/motel.json` & `ecoengine-0.0.4/src/ecoengine/data/load_shapes/motel.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/data/load_shapes/multi_family.json` & `ecoengine-0.0.4/src/ecoengine/data/load_shapes/multi_family.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/data/load_shapes/nursing_home.json` & `ecoengine-0.0.4/src/ecoengine/data/load_shapes/nursing_home.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/data/load_shapes/office_building.json` & `ecoengine-0.0.4/src/ecoengine/data/load_shapes/office_building.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/data/load_shapes/senior_high.json` & `ecoengine-0.0.4/src/ecoengine/data/load_shapes/senior_high.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/data/load_shapes/womens_dorm.json` & `ecoengine-0.0.4/src/ecoengine/data/load_shapes/womens_dorm.json`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/engine/BuildingCreator.py` & `ecoengine-0.0.4/src/ecoengine/engine/BuildingCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/engine/EcosizerEngine.py` & `ecoengine-0.0.4/src/ecoengine/engine/EcosizerEngine.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/engine/SystemCreator.py` & `ecoengine-0.0.4/src/ecoengine/engine/SystemCreator.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/engine/__init__.py` & `ecoengine-0.0.4/src/ecoengine/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/objects/Building.py` & `ecoengine-0.0.4/src/ecoengine/objects/Building.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/objects/SystemConfig.py` & `ecoengine-0.0.4/src/ecoengine/objects/SystemConfig.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/objects/__init__.py` & `ecoengine-0.0.4/src/ecoengine/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/objects/systemConfigUtils.py` & `ecoengine-0.0.4/src/ecoengine/objects/systemConfigUtils.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/objects/systems/ParallelLoopTank.py` & `ecoengine-0.0.4/src/ecoengine/objects/systems/ParallelLoopTank.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine/objects/systems/SwingTank.py` & `ecoengine-0.0.4/src/ecoengine/objects/systems/SwingTank.py`

 * *Files identical despite different names*

### Comparing `ecoengine-0.0.3/src/ecoengine.egg-info/PKG-INFO` & `ecoengine-0.0.4/src/ecoengine.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-Metadata-Version: 2.1
-Name: ecoengine
-Version: 0.0.3
-Summary: A software for sizing Heat Pump Water Heaters for buildings
-Home-page: https://ecosizer.ecotope.com/sizer/
-Author: Nolan
-Author-email: nolan@ecotope.com
-Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-
-# EcosizerEngine
-
-### Requirements:
-
-This software requires a python version greater than or equal to 3.11 to be installed in the environment it is running in.
-
-### Using the package in scripts:
-
-1. Install the package with pip
-
-	$ pip install ecosizer-engine
-
-2. To import and use the tools in this package, add the following import statement to your script:
-
-	from ecosizer_engine_package import *
-
-You should now be able to use the features of EcosizerEngine in your script
-
-### Running locally in a container:
-First, clone the EcosizerEngine repo from github
-
-    $ git clone https://github.com/EcotopeResearch/EcosizerEngine.git
-
-Depending on what type of environment you want to run the code in, please follow the appropriate steps.
-
-Steps for installing in a virtual environment:
-1. Navigate to the EcosizerEngine directory. This should be the same directory level as src/, setup.py, and this README document.
-2. Run the following command:
-
-	$ pip install -e .
-
-This will install the ecosizer-engine package locally in editable format, such that changes you make in the source code here will be reflected in implementation.
-This pip install should also install all dependencies for ecosizer-engine (i.e. numpy, scipy, pytest, and plotly)
-
-Steps for installing using docker container:
-1. Navigate to the EcosizerEngine directory.
-2. Build container with docker file
-
-	$ docker build -t ecosizerengine:latest .
-
-3. Run docker container
-
-	$  docker run -it ecosizerengine bash
-
-4. When you are done messing about in the docker image, just type the command
-
-	$ exit
-
-or press ctrl+c then ctrl+d
-
-Steps for installing conda environment from the Anaconda prompt:
-1. Navigate to the EcosizerEngine directory.
-2. Create new environment from .yml file.
-
-
-	$ conda env create --file EcosizerEngine.yml
-
-If the environment creation doesn't work, make sure Anaconda is up-to-date with
-
-    $ conda update --all
-
-If that doesn't work, you may need to force Anaconda to download and use python 3.11 (it defaults to 3.9) by making another environment
-
-    $ conda create -n py311 python=3.11
-    $ conda activate py311
-    $ conda env create --file EcosizerEngine.yml
-
-3. Check that the environment was created
-
-
-	$ conda env list
-
-4. Activate the new environment
-
-
-	$ conda activate EcosizerEngine
-
-If an environment already exits it can be removed with:
-
-	$ conda remove --name EcosizerEngine --all
-
-
-All the available environment can be found with:
-
-	$ conda env list
-
-### Testing:
-From the parent directory, type
-
-	$ python -m pytest
-
-This will run all unit tests for the package
-
-### Updating Documentation:
-1. If not installed in environment: pip install sphinx and numpydocs
-2. navigate to docs directory and run:
-
-
-	$ make html
-
-### Updating version on pypi
-
-1. If you haven't installed them before, pip install build and twine
-
-	$ python -m pip install --upgrade build
-
-
-	$ python -m pip install --user --upgrade twine
-
-2. Update the version number in setup.cfg
-3. Run the following commands from the project root directory:
-
-	$ python -m build
-
-	$ python -m twine upload dist/*
-
-### Contact Information
-To get in touch with Ecotope Inc. go here: http://ecotope.com/contact/
+Metadata-Version: 2.1
+Name: ecoengine
+Version: 0.0.4
+Summary: A software for sizing Heat Pump Water Heaters for buildings
+Home-page: https://ecosizer.ecotope.com/sizer/
+Author: Nolan
+Author-email: nolan@ecotope.com
+Project-URL: Docs, https://ecosizer.ecotope.com/sizer/docs/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+
+# EcosizerEngine
+
+### Requirements:
+
+This software requires a python version greater than or equal to 3.11 to be installed in the environment it is running in.
+
+### Using the package in scripts:
+
+1. Install the package with pip
+
+	$ pip install ecosizer-engine
+
+2. To import and use the tools in this package, add the following import statement to your script:
+
+	from ecosizer_engine_package import *
+
+You should now be able to use the features of EcosizerEngine in your script
+
+### Running locally in a container:
+First, clone the EcosizerEngine repo from github
+
+    $ git clone https://github.com/EcotopeResearch/EcosizerEngine.git
+
+Depending on what type of environment you want to run the code in, please follow the appropriate steps.
+
+Steps for installing in a virtual environment:
+1. Navigate to the EcosizerEngine directory. This should be the same directory level as src/, setup.py, and this README document.
+2. Run the following command:
+
+	$ pip install -e .
+
+This will install the ecosizer-engine package locally in editable format, such that changes you make in the source code here will be reflected in implementation.
+This pip install should also install all dependencies for ecosizer-engine (i.e. numpy, scipy, pytest, and plotly)
+
+Steps for installing using docker container:
+1. Navigate to the EcosizerEngine directory.
+2. Build container with docker file
+
+	$ docker build -t ecosizerengine:latest .
+
+3. Run docker container
+
+	$  docker run -it ecosizerengine bash
+
+4. When you are done messing about in the docker image, just type the command
+
+	$ exit
+
+or press ctrl+c then ctrl+d
+
+Steps for installing conda environment from the Anaconda prompt:
+1. Navigate to the EcosizerEngine directory.
+2. Create new environment from .yml file.
+
+
+	$ conda env create --file EcosizerEngine.yml
+
+If the environment creation doesn't work, make sure Anaconda is up-to-date with
+
+    $ conda update --all
+
+If that doesn't work, you may need to force Anaconda to download and use python 3.11 (it defaults to 3.9) by making another environment
+
+    $ conda create -n py311 python=3.11
+    $ conda activate py311
+    $ conda env create --file EcosizerEngine.yml
+
+3. Check that the environment was created
+
+
+	$ conda env list
+
+4. Activate the new environment
+
+
+	$ conda activate EcosizerEngine
+
+If an environment already exits it can be removed with:
+
+	$ conda remove --name EcosizerEngine --all
+
+
+All the available environment can be found with:
+
+	$ conda env list
+
+### Testing:
+From the parent directory, type
+
+	$ python -m pytest
+
+This will run all unit tests for the package
+
+### Updating Documentation:
+1. If not installed in environment: pip install sphinx and numpydocs
+2. navigate to docs directory and run:
+
+
+	$ make html
+
+### Updating version on pypi
+
+1. If you haven't installed them before, pip install build and twine
+
+	$ python -m pip install --upgrade build
+
+
+	$ python -m pip install --user --upgrade twine
+
+2. Update the version number in setup.cfg
+3. Run the following commands from the project root directory:
+
+	$ python -m build
+
+	$ python -m twine upload dist/*
+
+### Contact Information
+To get in touch with Ecotope Inc. go here: http://ecotope.com/contact/
```

### Comparing `ecoengine-0.0.3/src/ecoengine.egg-info/SOURCES.txt` & `ecoengine-0.0.4/src/ecoengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*


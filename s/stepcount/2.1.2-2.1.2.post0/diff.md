# Comparing `tmp/stepcount-2.1.2.tar.gz` & `tmp/stepcount-2.1.2.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepcount-2.1.2.tar", last modified: Tue Mar 21 20:52:03 2023, max compression
+gzip compressed data, was "stepcount-2.1.2.post0.tar", last modified: Wed Apr 19 19:04:12 2023, max compression
```

## Comparing `stepcount-2.1.2.tar` & `stepcount-2.1.2.post0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-s---   0 vtx027   (37039) doherty  (30011)        0 2023-03-21 20:52:03.496127 stepcount-2.1.2/
--rw-r-----   0 vtx027   (37039) doherty  (30011)     8026 2023-02-23 16:01:09.000000 stepcount-2.1.2/LICENSE.md
--rw-r-----   0 vtx027   (37039) doherty  (30011)     5807 2023-03-21 20:52:03.496127 stepcount-2.1.2/PKG-INFO
--rw-r-----   0 vtx027   (37039) doherty  (30011)     5129 2023-03-21 20:46:25.000000 stepcount-2.1.2/README.md
--rw-r-----   0 vtx027   (37039) doherty  (30011)       38 2023-03-21 20:52:03.496127 stepcount-2.1.2/setup.cfg
--rw-r-----   0 vtx027   (37039) doherty  (30011)     2246 2023-03-21 20:46:35.000000 stepcount-2.1.2/setup.py
-drwxr-s---   0 vtx027   (37039) doherty  (30011)        0 2023-03-21 20:52:03.489127 stepcount-2.1.2/stepcount/
--rw-r-----   0 vtx027   (37039) doherty  (30011)      443 2023-03-21 20:46:41.000000 stepcount-2.1.2/stepcount/__init__.py
--rw-r-----   0 vtx027   (37039) doherty  (30011)     5378 2022-12-13 20:05:01.000000 stepcount-2.1.2/stepcount/features.py
--rw-r-----   0 vtx027   (37039) doherty  (30011)     9381 2022-12-13 10:18:42.000000 stepcount-2.1.2/stepcount/hmm_utils.py
--rw-r-----   0 vtx027   (37039) doherty  (30011)    21708 2023-02-10 21:28:22.000000 stepcount-2.1.2/stepcount/models.py
--rw-r-----   0 vtx027   (37039) doherty  (30011)    11956 2023-02-10 21:28:22.000000 stepcount-2.1.2/stepcount/sslmodel.py
--rw-r-----   0 vtx027   (37039) doherty  (30011)    12439 2023-03-21 19:01:40.000000 stepcount-2.1.2/stepcount/stepcount.py
-drwxr-s---   0 vtx027   (37039) doherty  (30011)        0 2023-03-21 20:52:03.495127 stepcount-2.1.2/stepcount/utils/
--rw-r-----   0 vtx027   (37039) doherty  (30011)       60 2023-03-21 19:01:46.000000 stepcount-2.1.2/stepcount/utils/__init__.py
--rw-r-----   0 vtx027   (37039) doherty  (30011)     1346 2023-03-21 19:01:46.000000 stepcount-2.1.2/stepcount/utils/collate_outputs.py
-drwxr-s---   0 vtx027   (37039) doherty  (30011)        0 2023-03-21 20:52:03.493127 stepcount-2.1.2/stepcount.egg-info/
--rw-r-----   0 vtx027   (37039) doherty  (30011)     5807 2023-03-21 20:52:03.000000 stepcount-2.1.2/stepcount.egg-info/PKG-INFO
--rw-r-----   0 vtx027   (37039) doherty  (30011)      424 2023-03-21 20:52:03.000000 stepcount-2.1.2/stepcount.egg-info/SOURCES.txt
--rw-r-----   0 vtx027   (37039) doherty  (30011)        1 2023-03-21 20:52:03.000000 stepcount-2.1.2/stepcount.egg-info/dependency_links.txt
--rw-r-----   0 vtx027   (37039) doherty  (30011)      120 2023-03-21 20:52:03.000000 stepcount-2.1.2/stepcount.egg-info/entry_points.txt
--rw-r-----   0 vtx027   (37039) doherty  (30011)      360 2023-03-21 20:52:03.000000 stepcount-2.1.2/stepcount.egg-info/requires.txt
--rw-r-----   0 vtx027   (37039) doherty  (30011)       10 2023-03-21 20:52:03.000000 stepcount-2.1.2/stepcount.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:12.279609 stepcount-2.1.2.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-19 19:04:12.279609 stepcount-2.1.2.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:04:12.279609 stepcount-2.1.2.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:12.275609 stepcount-2.1.2.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:12.283609 stepcount-2.1.2.post0/src/stepcount/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/src/stepcount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 19:04:12.283609 stepcount-2.1.2.post0/src/stepcount/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/src/stepcount/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/src/stepcount/hmm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21708 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/src/stepcount/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/src/stepcount/sslmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/src/stepcount/stepcount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:12.279609 stepcount-2.1.2.post0/src/stepcount/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/src/stepcount/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/src/stepcount/utils/collate_outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:04:12.279609 stepcount-2.1.2.post0/src/stepcount.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-19 19:04:12.000000 stepcount-2.1.2.post0/src/stepcount.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-19 19:04:12.000000 stepcount-2.1.2.post0/src/stepcount.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:04:12.000000 stepcount-2.1.2.post0/src/stepcount.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-19 19:04:12.000000 stepcount-2.1.2.post0/src/stepcount.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-19 19:04:12.000000 stepcount-2.1.2.post0/src/stepcount.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 19:04:12.000000 stepcount-2.1.2.post0/src/stepcount.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-19 19:04:01.000000 stepcount-2.1.2.post0/versioneer.py
```

### Comparing `stepcount-2.1.2/LICENSE.md` & `stepcount-2.1.2.post0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.2/PKG-INFO` & `stepcount-2.1.2.post0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: stepcount
-Version: 2.1.2
-Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
-Home-page: https://github.com/OxWearables/stepcount
-Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
-Author-email: shing.chan@ndph.ox.ac.uk, scott.small@ndph.ox.ac.uk, gert.mertes@ndph.ox.ac.uk, aiden.doherty@ndph.ox.ac.uk
-License: 2-Clause BSD
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Unix
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE.md
-
 # stepcount
 
 A Python package to estimate step counts from accelerometer data.
 
 The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649). 
 
 Check out the 5-minute video tutorial to get started: [https://www.youtube.com/watch?v=FPb7H-jyRVQ](https://www.youtube.com/watch?v=FPb7H-jyRVQ).
```

### Comparing `stepcount-2.1.2/setup.py` & `stepcount-2.1.2.post0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,57 @@
+import sys
+import os.path
+# https://github.com/python-versioneer/python-versioneer/issues/193
+sys.path.insert(0, os.path.dirname(__file__))
+
 import setuptools
 import codecs
-import os.path
+
+import versioneer
 
 
 def read(rel_path):
     here = os.path.abspath(os.path.dirname(__file__))
     with codecs.open(os.path.join(here, rel_path), 'r') as fp:
         return fp.read()
 
-def get_string(string, rel_path="stepcount/__init__.py"):
+def get_string(string, rel_path="src/stepcount/__init__.py"):
     for line in read(rel_path).splitlines():
         if line.startswith(string):
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     else:
         raise RuntimeError(f"Unable to find {string}.")
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="stepcount",
     python_requires=">=3.8",
-    version=get_string("__version__"),
+    version=versioneer.get_version(),
+    cmdclass=versioneer.get_cmdclass(),
     description="Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OxWearables/stepcount",
+    download_url="https://github.com/OxWearables/stepcount",
     author=get_string("__author__"),
-    author_email=get_string("__email__"),
+    maintainer=get_string("__maintainer__"),
+    maintainer_email=get_string("__maintainer_email__"),
     license=get_string("__license__"),
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Unix",
+        "Topic :: Scientific/Engineering",
+        "Topic :: Scientific/Engineering :: Bio-Informatics",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "Topic :: Scientific/Engineering :: Medical Science Apps.",
     ],
-    packages=setuptools.find_packages(exclude=("test", "tests")),
+    packages=setuptools.find_packages(where="src", exclude=("test", "tests")),
+    package_dir={"": "src"},
     include_package_data=False,
     install_requires=[
         "actipy==2.0.3",
         "numpy==1.24.*",
         "scipy==1.10.*",
         "pandas==1.5.*",
         "tqdm==4.64.*",
```

### Comparing `stepcount-2.1.2/stepcount/features.py` & `stepcount-2.1.2.post0/src/stepcount/features.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.2/stepcount/hmm_utils.py` & `stepcount-2.1.2.post0/src/stepcount/hmm_utils.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.2/stepcount/models.py` & `stepcount-2.1.2.post0/src/stepcount/models.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.2/stepcount/sslmodel.py` & `stepcount-2.1.2.post0/src/stepcount/sslmodel.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.2/stepcount/stepcount.py` & `stepcount-2.1.2.post0/src/stepcount/stepcount.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.2/stepcount/utils/collate_outputs.py` & `stepcount-2.1.2.post0/src/stepcount/utils/collate_outputs.py`

 * *Files identical despite different names*

### Comparing `stepcount-2.1.2/stepcount.egg-info/PKG-INFO` & `stepcount-2.1.2.post0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,199 +1,203 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 2.1.2
+Version: 2.1.2.post0
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
-Author-email: shing.chan@ndph.ox.ac.uk, scott.small@ndph.ox.ac.uk, gert.mertes@ndph.ox.ac.uk, aiden.doherty@ndph.ox.ac.uk
-License: 2-Clause BSD
+Maintainer: Shing Chan
+Maintainer-email: shing.chan@ndph.ox.ac.uk
+License: See LICENSE file.
+Download-URL: https://github.com/OxWearables/stepcount
+Description: # stepcount
+        
+        A Python package to estimate step counts from accelerometer data.
+        
+        The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649). 
+        
+        Check out the 5-minute video tutorial to get started: [https://www.youtube.com/watch?v=FPb7H-jyRVQ](https://www.youtube.com/watch?v=FPb7H-jyRVQ).
+        
+        ## Getting started
+        
+        ### Prerequisite
+        
+        - Python 3.8 or greater
+            ```console
+            $ python --version  # or python3 --version
+            ```
+        
+        - Java 8 (1.8.0) or greater
+            ```console
+            $ java -version
+            ```
+        
+        ### Install (Windows)
+        For Windows users, we recommend running stepcount using the **Anaconda Prompt** from **Miniconda** via the following steps:
+        
+        1. Download [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (light-weight version of Anaconda). Choose **Miniconda3 Windows 64-bit**.
+        2. Install. Use the default recommended settings.
+        3. From the Start menu, search and open the **Anaconda Prompt**.
+        
+        ```console
+        $ pip install stepcount
+        ```
+        
+        For further information running Anaconda on Windows using virtual environments, see [this guide](anaconda_on_windows.md).
+        
+        ### Install (Linux)
+        
+        <!-- ```console
+        $ pip install git+https://github.com/OxWearables/stepcount.git@master#egg=stepcount
+        ``` -->
+        
+        <!-- ```console
+        $ pip install git+ssh://git@github.com/OxWearables/stepcount.git@master#egg=stepcount
+        ``` -->
+        
+        ```console
+        $ pip install stepcount
+        ```
+        
+        
+        
+        ## Usage
+        
+        ```bash
+        # Process an AX3 file
+        $ stepcount sample.cwa
+        
+        # Or an ActiGraph file
+        $ stepcount sample.gt3x
+        
+        # Or a GENEActiv file
+        $ stepcount sample.bin
+        
+        # Or a CSV file (see data format below)
+        $ stepcount sample.csv
+        ```
+        
+        Output:
+        ```console
+        Summary
+        -------
+        {
+            "Filename": "sample.cwa",
+            "Filesize(MB)": 65.1,
+            "Device": "Axivity",
+            "DeviceID": 2278,
+            "ReadErrors": 0,
+            "SampleRate": 100.0,
+            "ReadOK": 1,
+            "StartTime": "2013-10-21 10:00:07",
+            "EndTime": "2013-10-28 10:00:01",
+            "TotalWalking(min)": 655.75,
+            "TotalSteps": 43132,
+            ...
+        }
+        
+        Estimated Daily Steps
+        ---------------------
+                      steps
+        time
+        2013-10-21     5368
+        2013-10-22     7634
+        2013-10-23    10009
+        ...
+        
+        Output: outputs/sample/
+        ```
+        
+        ### Output files
+        By default, output files will be stored in a folder named after the input file, `outputs/{filename}/`, created in the current working directory. You can change the output path with the `-o` flag:
+        
+        ```console
+        $ stepcount sample.cwa -o /path/to/some/folder/
+        ```
+        
+        The following output files are created:
+        
+        - *Info.json* Summary info, as shown above.
+        - *Steps.csv* Raw time-series of step counts
+        - *HourlySteps.csv* Hourly step counts
+        - *DailySteps.csv* Daily step counts
+        - *HourlyStepsAdjusted.csv* Like HourlySteps but accounting for missing data (see section below).
+        - *DailyStepsAdjusted.csv* Like DailySteps but accounting for missing data (see section below).
+        
+        
+        ### Crude vs. Adjusted Estimates
+        Adjusted estimates are provided that account for missing data.
+        Missing values in the time-series are imputed with the mean of the same timepoint of other available days.
+        For adjusted totals and daily statistics, 24h multiples are needed and will be imputed if necessary.
+        Estimates will be NaN where data is still missing after imputation.
+        
+        
+        ### Processing CSV files
+        If a CSV file is provided, it must have the following header: `time`, `x`, `y`, `z`. 
+        
+        Example:
+        ```console
+        time,x,y,z
+        2013-10-21 10:00:08.000,-0.078923,0.396706,0.917759
+        2013-10-21 10:00:08.010,-0.094370,0.381479,0.933580
+        2013-10-21 10:00:08.020,-0.094370,0.366252,0.901938
+        2013-10-21 10:00:08.030,-0.078923,0.411933,0.901938
+        ...
+        ```
+        
+        ### Processing multiple files
+        #### Windows
+        To process multiple files you can create a text file in Notepad which includes one line for each file you wish to process, as shown below for *file1.cwa*, *file2.cwa*, and *file2.cwa*.
+        
+        Example text file *commands.txt*: 
+        ```console
+        stepcount file1.cwa &
+        stepcount file2.cwa &
+        stepcount file3.cwa 
+        :END
+        ````
+        Once this file is created, run `cmd < commands.txt` from the terminal.
+        
+        #### Linux
+        Create a file *command.sh* with:
+        ```console
+        stepcount file1.cwa
+        stepcount file2.cwa
+        stepcount file3.cwa
+        ```
+        Then, run `bash command.sh` from the terminal.
+        
+        #### Collating outputs
+        
+        A utility script is provided to collate outputs from multiple runs:
+        
+        ```console
+        stepcount-collate-outputs outputs/
+        ```
+        This will collate all *-Info.json files found in outputs/ and generate a CSV file.
+        
+        ## Validation
+        
+        Validation for this algorithm is presented in a preprint on medRxiv at: [https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1](https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1). 
+        
+        
+        ## Citing our work
+        
+        When using this tool, please consider citing the works listed in [CITATION.md](CITATION.md).
+        
+        
+        ## Licence
+        See [LICENSE.md](LICENSE.md).
+        
+        
+        ## Acknowledgements
+        We would like to thank all our code contributors, manuscript co-authors, and research participants for their help in making this work possible.
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Unix
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
-License-File: LICENSE.md
-
-# stepcount
-
-A Python package to estimate step counts from accelerometer data.
-
-The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649). 
-
-Check out the 5-minute video tutorial to get started: [https://www.youtube.com/watch?v=FPb7H-jyRVQ](https://www.youtube.com/watch?v=FPb7H-jyRVQ).
-
-## Getting started
-
-### Prerequisite
-
-- Python 3.8 or greater
-    ```console
-    $ python --version  # or python3 --version
-    ```
-
-- Java 8 (1.8.0) or greater
-    ```console
-    $ java -version
-    ```
-
-### Install (Windows)
-For Windows users, we recommend running stepcount using the **Anaconda Prompt** from **Miniconda** via the following steps:
-
-1. Download [Miniconda](https://docs.conda.io/en/latest/miniconda.html) (light-weight version of Anaconda). Choose **Miniconda3 Windows 64-bit**.
-2. Install. Use the default recommended settings.
-3. From the Start menu, search and open the **Anaconda Prompt**.
-
-```console
-$ pip install stepcount
-```
-
-For further information running Anaconda on Windows using virtual environments, see [this guide](anaconda_on_windows.md).
-
-### Install (Linux)
-
-<!-- ```console
-$ pip install git+https://github.com/OxWearables/stepcount.git@master#egg=stepcount
-``` -->
-
-<!-- ```console
-$ pip install git+ssh://git@github.com/OxWearables/stepcount.git@master#egg=stepcount
-``` -->
-
-```console
-$ pip install stepcount
-```
-
-
-
-## Usage
-
-```bash
-# Process an AX3 file
-$ stepcount sample.cwa
-
-# Or an ActiGraph file
-$ stepcount sample.gt3x
-
-# Or a GENEActiv file
-$ stepcount sample.bin
-
-# Or a CSV file (see data format below)
-$ stepcount sample.csv
-```
-
-Output:
-```console
-Summary
--------
-{
-    "Filename": "sample.cwa",
-    "Filesize(MB)": 65.1,
-    "Device": "Axivity",
-    "DeviceID": 2278,
-    "ReadErrors": 0,
-    "SampleRate": 100.0,
-    "ReadOK": 1,
-    "StartTime": "2013-10-21 10:00:07",
-    "EndTime": "2013-10-28 10:00:01",
-    "TotalWalking(min)": 655.75,
-    "TotalSteps": 43132,
-    ...
-}
-
-Estimated Daily Steps
----------------------
-              steps
-time
-2013-10-21     5368
-2013-10-22     7634
-2013-10-23    10009
-...
-
-Output: outputs/sample/
-```
-
-### Output files
-By default, output files will be stored in a folder named after the input file, `outputs/{filename}/`, created in the current working directory. You can change the output path with the `-o` flag:
-
-```console
-$ stepcount sample.cwa -o /path/to/some/folder/
-```
-
-The following output files are created:
-
-- *Info.json* Summary info, as shown above.
-- *Steps.csv* Raw time-series of step counts
-- *HourlySteps.csv* Hourly step counts
-- *DailySteps.csv* Daily step counts
-- *HourlyStepsAdjusted.csv* Like HourlySteps but accounting for missing data (see section below).
-- *DailyStepsAdjusted.csv* Like DailySteps but accounting for missing data (see section below).
-
-
-### Crude vs. Adjusted Estimates
-Adjusted estimates are provided that account for missing data.
-Missing values in the time-series are imputed with the mean of the same timepoint of other available days.
-For adjusted totals and daily statistics, 24h multiples are needed and will be imputed if necessary.
-Estimates will be NaN where data is still missing after imputation.
-
-
-### Processing CSV files
-If a CSV file is provided, it must have the following header: `time`, `x`, `y`, `z`. 
-
-Example:
-```console
-time,x,y,z
-2013-10-21 10:00:08.000,-0.078923,0.396706,0.917759
-2013-10-21 10:00:08.010,-0.094370,0.381479,0.933580
-2013-10-21 10:00:08.020,-0.094370,0.366252,0.901938
-2013-10-21 10:00:08.030,-0.078923,0.411933,0.901938
-...
-```
-
-### Processing multiple files
-#### Windows
-To process multiple files you can create a text file in Notepad which includes one line for each file you wish to process, as shown below for *file1.cwa*, *file2.cwa*, and *file2.cwa*.
-
-Example text file *commands.txt*: 
-```console
-stepcount file1.cwa &
-stepcount file2.cwa &
-stepcount file3.cwa 
-:END
-````
-Once this file is created, run `cmd < commands.txt` from the terminal.
-
-#### Linux
-Create a file *command.sh* with:
-```console
-stepcount file1.cwa
-stepcount file2.cwa
-stepcount file3.cwa
-```
-Then, run `bash command.sh` from the terminal.
-
-#### Collating outputs
-
-A utility script is provided to collate outputs from multiple runs:
-
-```console
-stepcount-collate-outputs outputs/
-```
-This will collate all *-Info.json files found in outputs/ and generate a CSV file.
-
-## Validation
-
-Validation for this algorithm is presented in a preprint on medRxiv at: [https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1](https://www.medrxiv.org/content/10.1101/2023.02.20.23285750v1). 
-
-
-## Citing our work
-
-When using this tool, please consider citing the works listed in [CITATION.md](CITATION.md).
-
-
-## Licence
-See [LICENSE.md](LICENSE.md).
-
-
-## Acknowledgements
-We would like to thank all our code contributors, manuscript co-authors, and research participants for their help in making this work possible.
```


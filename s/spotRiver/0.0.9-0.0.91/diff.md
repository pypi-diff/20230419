# Comparing `tmp/spotRiver-0.0.9.tar.gz` & `tmp/spotRiver-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotRiver-0.0.9.tar", last modified: Sun Feb  5 11:57:55 2023, max compression
+gzip compressed data, was "spotRiver-0.0.91.tar", last modified: Wed Apr 19 20:56:29 2023, max compression
```

## Comparing `spotRiver-0.0.9.tar` & `spotRiver-0.0.91.tar`

### file list

```diff
@@ -1,34 +1,45 @@
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-02-05 11:57:55.137121 spotRiver-0.0.9/
--rw-r--r--   0 bartz      (501) staff       (20)     1520 2023-01-29 11:49:35.000000 spotRiver-0.0.9/LICENSE
--rw-r--r--   0 bartz      (501) staff       (20)      130 2023-01-29 16:41:52.000000 spotRiver-0.0.9/MANIFEST.in
--rw-r--r--   0 bartz      (501) staff       (20)     3382 2023-02-05 11:57:55.136954 spotRiver-0.0.9/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     2912 2023-01-29 16:41:52.000000 spotRiver-0.0.9/README.md
--rw-r--r--   0 bartz      (501) staff       (20)     1045 2023-02-05 11:57:26.000000 spotRiver-0.0.9/pyproject.toml
--rw-r--r--   0 bartz      (501) staff       (20)       38 2023-02-05 11:57:55.137168 spotRiver-0.0.9/setup.cfg
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-02-05 11:57:55.130191 spotRiver-0.0.9/src/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-02-05 11:57:55.130555 spotRiver-0.0.9/src/spotRiver/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-02-05 11:57:55.134412 spotRiver-0.0.9/src/spotRiver/data/
--rw-r--r--   0 bartz      (501) staff       (20)      413 2023-01-29 11:52:00.000000 spotRiver-0.0.9/src/spotRiver/data/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)     2182 2023-01-17 12:39:58.000000 spotRiver-0.0.9/src/spotRiver/data/airline-passengers.csv
--rw-r--r--   0 bartz      (501) staff       (20)     1023 2023-01-17 12:39:58.000000 spotRiver-0.0.9/src/spotRiver/data/airline_passengers.py
--rw-r--r--   0 bartz      (501) staff       (20)    12012 2023-02-01 17:37:08.000000 spotRiver-0.0.9/src/spotRiver/data/base.py
--rw-r--r--   0 bartz      (501) staff       (20)     1290 2023-02-05 00:56:40.000000 spotRiver-0.0.9/src/spotRiver/data/generic.py
--rw-r--r--   0 bartz      (501) staff       (20)     6121 2023-02-04 20:16:42.000000 spotRiver-0.0.9/src/spotRiver/data/opm.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-02-05 11:57:55.135215 spotRiver-0.0.9/src/spotRiver/data/synth/
--rw-r--r--   0 bartz      (501) staff       (20)      328 2023-01-18 17:25:51.000000 spotRiver-0.0.9/src/spotRiver/data/synth/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)     2445 2023-01-17 12:39:58.000000 spotRiver-0.0.9/src/spotRiver/data/synth/sea.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-02-05 11:57:55.135734 spotRiver-0.0.9/src/spotRiver/evaluation/
--rw-r--r--   0 bartz      (501) staff       (20)     3157 2023-02-04 23:14:24.000000 spotRiver-0.0.9/src/spotRiver/evaluation/eval_oml.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-02-05 11:57:55.135923 spotRiver-0.0.9/src/spotRiver/fun/
--rw-r--r--   0 bartz      (501) staff       (20)    20018 2023-02-05 10:58:38.000000 spotRiver-0.0.9/src/spotRiver/fun/hyperriver.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-02-05 11:57:55.136579 spotRiver-0.0.9/src/spotRiver/utils/
--rw-r--r--   0 bartz      (501) staff       (20)      641 2023-02-04 21:33:55.000000 spotRiver-0.0.9/src/spotRiver/utils/features.py
--rw-r--r--   0 bartz      (501) staff       (20)      826 2023-02-05 00:41:06.000000 spotRiver-0.0.9/src/spotRiver/utils/selectors.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-02-05 11:57:55.132545 spotRiver-0.0.9/src/spotRiver.egg-info/
--rw-r--r--   0 bartz      (501) staff       (20)     3382 2023-02-05 11:57:55.000000 spotRiver-0.0.9/src/spotRiver.egg-info/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)      650 2023-02-05 11:57:55.000000 spotRiver-0.0.9/src/spotRiver.egg-info/SOURCES.txt
--rw-r--r--   0 bartz      (501) staff       (20)        1 2023-02-05 11:57:55.000000 spotRiver-0.0.9/src/spotRiver.egg-info/dependency_links.txt
--rw-r--r--   0 bartz      (501) staff       (20)       20 2023-02-05 11:57:55.000000 spotRiver-0.0.9/src/spotRiver.egg-info/requires.txt
--rw-r--r--   0 bartz      (501) staff       (20)       10 2023-02-05 11:57:55.000000 spotRiver-0.0.9/src/spotRiver.egg-info/top_level.txt
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-02-05 11:57:55.136741 spotRiver-0.0.9/test/
--rw-r--r--   0 bartz      (501) staff       (20)      511 2023-01-29 16:42:44.000000 spotRiver-0.0.9/test/test_features.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.738029 spotRiver-0.0.91/
+-rw-r--r--   0 bartz      (501) staff       (20)     1520 2023-01-29 11:49:35.000000 spotRiver-0.0.91/LICENSE
+-rw-r--r--   0 bartz      (501) staff       (20)      164 2023-03-22 20:43:16.000000 spotRiver-0.0.91/MANIFEST.in
+-rw-r--r--   0 bartz      (501) staff       (20)     3383 2023-04-19 20:56:29.737903 spotRiver-0.0.91/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     2912 2023-01-29 16:41:52.000000 spotRiver-0.0.91/README.md
+-rw-r--r--   0 bartz      (501) staff       (20)     1046 2023-04-19 18:27:37.000000 spotRiver-0.0.91/pyproject.toml
+-rw-r--r--   0 bartz      (501) staff       (20)       38 2023-04-19 20:56:29.738063 spotRiver-0.0.91/setup.cfg
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.729949 spotRiver-0.0.91/src/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.730449 spotRiver-0.0.91/src/spotRiver/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.734688 spotRiver-0.0.91/src/spotRiver/data/
+-rw-r--r--   0 bartz      (501) staff       (20)      413 2023-01-29 11:52:00.000000 spotRiver-0.0.91/src/spotRiver/data/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2182 2023-01-17 12:39:58.000000 spotRiver-0.0.91/src/spotRiver/data/airline-passengers.csv
+-rw-r--r--   0 bartz      (501) staff       (20)     1023 2023-03-27 20:31:30.000000 spotRiver-0.0.91/src/spotRiver/data/airline_passengers.py
+-rw-r--r--   0 bartz      (501) staff       (20)    13646 2023-03-22 20:37:51.000000 spotRiver-0.0.91/src/spotRiver/data/base.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1113 2023-03-13 20:26:53.000000 spotRiver-0.0.91/src/spotRiver/data/bike_sharing.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1870 2023-03-07 16:50:39.000000 spotRiver-0.0.91/src/spotRiver/data/generic.py
+-rw-r--r--   0 bartz      (501) staff       (20)     7751 2023-03-07 16:50:39.000000 spotRiver-0.0.91/src/spotRiver/data/opm.py
+-rw-r--r--   0 bartz      (501) staff       (20)    17554 2023-04-08 14:44:16.000000 spotRiver-0.0.91/src/spotRiver/data/river_hyper_dict.json
+-rw-r--r--   0 bartz      (501) staff       (20)      329 2023-03-31 21:04:02.000000 spotRiver-0.0.91/src/spotRiver/data/river_hyper_dict.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.735282 spotRiver-0.0.91/src/spotRiver/data/synth/
+-rw-r--r--   0 bartz      (501) staff       (20)      328 2023-01-18 17:25:51.000000 spotRiver-0.0.91/src/spotRiver/data/synth/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2442 2023-02-20 15:46:37.000000 spotRiver-0.0.91/src/spotRiver/data/synth/sea.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.735467 spotRiver-0.0.91/src/spotRiver/drift/
+-rw-r--r--   0 bartz      (501) staff       (20)      767 2023-02-20 15:46:37.000000 spotRiver-0.0.91/src/spotRiver/drift/drift_generator.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.736260 spotRiver-0.0.91/src/spotRiver/evaluation/
+-rw-r--r--   0 bartz      (501) staff       (20)    29393 2023-04-06 12:46:27.000000 spotRiver-0.0.91/src/spotRiver/evaluation/eval_bml.py
+-rw-r--r--   0 bartz      (501) staff       (20)     3958 2023-02-26 22:39:12.000000 spotRiver-0.0.91/src/spotRiver/evaluation/eval_nowcast.py
+-rw-r--r--   0 bartz      (501) staff       (20)     6752 2023-04-06 12:44:54.000000 spotRiver-0.0.91/src/spotRiver/evaluation/eval_oml.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.736521 spotRiver-0.0.91/src/spotRiver/fun/
+-rw-r--r--   0 bartz      (501) staff       (20)    30535 2023-04-19 18:43:21.000000 spotRiver-0.0.91/src/spotRiver/fun/hyperriver.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.736843 spotRiver-0.0.91/src/spotRiver/plot/
+-rw-r--r--   0 bartz      (501) staff       (20)     1340 2023-03-11 14:52:45.000000 spotRiver-0.0.91/src/spotRiver/plot/stats.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.737051 spotRiver-0.0.91/src/spotRiver/preprocess/
+-rw-r--r--   0 bartz      (501) staff       (20)     2488 2023-03-07 16:50:39.000000 spotRiver-0.0.91/src/spotRiver/preprocess/impute.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.737442 spotRiver-0.0.91/src/spotRiver/utils/
+-rw-r--r--   0 bartz      (501) staff       (20)     2033 2023-04-04 17:58:20.000000 spotRiver-0.0.91/src/spotRiver/utils/data_conversion.py
+-rw-r--r--   0 bartz      (501) staff       (20)     5549 2023-04-13 20:07:21.000000 spotRiver-0.0.91/src/spotRiver/utils/features.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.731794 spotRiver-0.0.91/src/spotRiver.egg-info/
+-rw-r--r--   0 bartz      (501) staff       (20)     3383 2023-04-19 20:56:29.000000 spotRiver-0.0.91/src/spotRiver.egg-info/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)      951 2023-04-19 20:56:29.000000 spotRiver-0.0.91/src/spotRiver.egg-info/SOURCES.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        1 2023-04-19 20:56:29.000000 spotRiver-0.0.91/src/spotRiver.egg-info/dependency_links.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       20 2023-04-19 20:56:29.000000 spotRiver-0.0.91/src/spotRiver.egg-info/requires.txt
+-rw-r--r--   0 bartz      (501) staff       (20)       10 2023-04-19 20:56:29.000000 spotRiver-0.0.91/src/spotRiver.egg-info/top_level.txt
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2023-04-19 20:56:29.737715 spotRiver-0.0.91/test/
+-rw-r--r--   0 bartz      (501) staff       (20)      510 2023-02-25 09:55:05.000000 spotRiver-0.0.91/test/test_features.py
```

### Comparing `spotRiver-0.0.9/LICENSE` & `spotRiver-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.9/PKG-INFO` & `spotRiver-0.0.91/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotRiver
-Version: 0.0.9
+Version: 0.0.91
 Summary: spotRiver - Sequential Parameter Optimization Interface to River
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 Project-URL: Homepage, https://www.spotseven.de
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `spotRiver-0.0.9/README.md` & `spotRiver-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.9/pyproject.toml` & `spotRiver-0.0.91/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
             "numpy",
             "scikit-learn",
             "matplotlib"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spotRiver"
-version = "0.0.9"
+version = "0.0.91"
 authors = [
   { name="T. Bartz-Beielstein", email="tbb@bartzundbartz.de" }
 ]
 description = "spotRiver - Sequential Parameter Optimization Interface to River"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `spotRiver-0.0.9/src/spotRiver/data/airline-passengers.csv` & `spotRiver-0.0.91/src/spotRiver/data/airline-passengers.csv`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.9/src/spotRiver/data/airline_passengers.py` & `spotRiver-0.0.91/src/spotRiver/data/airline_passengers.py`

 * *Files identical despite different names*

### Comparing `spotRiver-0.0.9/src/spotRiver/data/base.py` & `spotRiver-0.0.91/src/spotRiver/data/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,44 @@
     # Ensure data_home is a Path() object pointing to an absolute path
     data_home = Path(data_home).absolute()
     # Create data directory if it does not exists.
     data_home.mkdir(parents=True, exist_ok=True)
     return data_home
 
 
+class Config(abc.ABC):
+    """Base class for all configurations.
+
+    All configurations inherit from this class, be they stored in a file or generated on the fly.
+    """
+
+    def __init__(
+        self,
+    ):
+        pass
+
+    @property
+    def desc(self):
+        """Return the description from the docstring."""
+        desc = re.split(pattern=r"\w+\n\s{4}\-{3,}", string=self.__doc__, maxsplit=0)[0]
+        return inspect.cleandoc(desc)
+
+    @property
+    def _repr_content(self):
+        """The items that are displayed in the __repr__ method.
+
+        This property can be overridden in order to modify the output of the __repr__ method.
+
+        """
+
+        content = {}
+        content["Name"] = self.__class__.__name__
+        return content
+
+
 class Dataset(abc.ABC):
     """Base class for all datasets.
 
     All datasets inherit from this class, be they stored in a file or generated on the fly.
 
     Parameters
     ----------
@@ -127,15 +157,14 @@
         if self.n_classes:
             content["Classes"] = f"{self.n_classes:,}"
         content["Sparse"] = str(self.sparse)
 
         return content
 
     def __repr__(self):
-
         l_len = max(map(len, self._repr_content.keys()))
         r_len = max(map(len, self._repr_content.values()))
 
         out = f"{self.desc}\n\n" + "\n".join(
             k.rjust(l_len) + "  " + v.ljust(r_len) for k, v in self._repr_content.items()
         )
 
@@ -195,14 +224,47 @@
         return {
             name: getattr(self, name)
             for name, param in inspect.signature(self.__init__).parameters.items()  # type: ignore
             if param.kind != param.VAR_KEYWORD
         }
 
 
+class FileConfig(Config):
+    """Base class for configurations that are stored in a local file.
+
+    Parameters
+    ----------
+    filename
+        The file's name.
+    directory
+        The directory where the file is contained. Defaults to the location of the `datasets`
+        module.
+    desc
+        Extra config parameters to pass as keyword arguments.
+
+    """
+
+    def __init__(self, filename, directory=None, **desc):
+        super().__init__(**desc)
+        self.filename = filename
+        self.directory = directory
+
+    @property
+    def path(self):
+        if self.directory:
+            return pathlib.Path(self.directory).joinpath(self.filename)
+        return pathlib.Path(__file__).parent.joinpath(self.filename)
+
+    @property
+    def _repr_content(self):
+        content = super()._repr_content
+        content["Path"] = str(self.path)
+        return content
+
+
 class FileDataset(Dataset):
     """Base class for datasets that are stored in a local file.
 
     Small datasets that are part of the spotRiver package inherit from this class.
 
     Parameters
     ----------
@@ -254,39 +316,36 @@
         An optional name to given to the file if the file is unpacked.
     desc
         Extra dataset parameters to pass as keyword arguments.
 
     """
 
     def __init__(self, url, size, unpack=True, filename=None, **desc):
-
         if filename is None:
             filename = path.basename(url)
 
         super().__init__(filename=filename, **desc)
         self.url = url
         self.size = size
         self.unpack = unpack
 
     @property
     def path(self):
         return pathlib.Path(get_data_home(), self.__class__.__name__, self.filename)
 
     def download(self, force=False, verbose=True):
-
         if not force and self.is_downloaded:
             return
 
         # Determine where to download the archive
         directory = self.path.parent
         directory.mkdir(parents=True, exist_ok=True)
         archive_path = directory.joinpath(path.basename(self.url))
 
         with request.urlopen(self.url) as r:
-
             # Notify the user
             if verbose:
                 meta = r.info()
                 try:
                     n_bytes = int(meta["Content-Length"])
                     msg = f"Downloading {self.url} ({utils.pretty.humanize_bytes(n_bytes)})"
                 except KeyError:
@@ -323,15 +382,14 @@
     def _iter(self):
         pass
 
     @property
     def is_downloaded(self):
         """Indicate whether or the data has been correctly downloaded."""
         if self.path.exists():
-
             if self.path.is_file():
                 return self.path.stat().st_size == self.size
             return sum(f.stat().st_size for f in self.path.glob("**/*") if f.is_file())
 
         return False
 
     def __iter__(self):
```

### Comparing `spotRiver-0.0.9/src/spotRiver/data/opm.py` & `spotRiver-0.0.91/src/spotRiver/data/opm.py`

 * *Files 23% similar despite different names*

```diff
@@ -43,34 +43,62 @@
     *,
     data_home: Union[str, Path] = None,
     download_if_missing: bool = True,
     return_X_y: bool = False,
     include_numeric: bool = True,
     include_categorical: bool = False,
 ) -> Union[Tuple[pd.DataFrame, pd.Series], pd.DataFrame, Bunch]:
-    """Load the Office of Planning and Managment dataset (regression).
+    """Fetch the OPM dataset from the Connecticut Open Data portal.
+
     Parameters
     ----------
-    data_home : str or Path, default=None
-        Specify another download and cache folder for the dataset.
+    data_home : str or pathlib.Path, default=None
+        Specify another download and cache folder for the datasets. By default
+        all spotRiver data is stored in '~/spotriver_data' subfolders.
     download_if_missing : bool, default=True
         If False, raise an IOError if the data is not locally available
-        instead of trying to download the data from the source site.
+        rather than trying to download the data from the source site.
     return_X_y : bool, default=False
-        If True, returns ``(data.data, data.target)`` instead of a
-        :class:`~sklearn.utils.Bunch`.
+        If True, return `(X, y)` instead of a `Bunch` object. See
+        `sklearn.utils.Bunch` for more information.
+    include_numeric : bool, default=True
+        If True, include numeric columns in the output. Numeric columns include
+        'List Year', 'Assessed Value', 'Sale Amount', 'Sales Ratio', 'lat', 'lon',
+        and 'timestamp_rec'.
+    include_categorical : bool, default=False
+        If True, include categorical columns in the output. Categorical columns
+        include 'Town', 'Address', 'Property Type', 'Residential Type',
+        'Non Use Code', 'Assessor Remarks', and 'OPM remarks'. Columns with fewer
+        than 200 unique values will be treated as categorical.
 
     Returns
     -------
-    dataset : :class:`~sklearn.utils.Bunch`
-        Dictionary-like object, with the following attributes.
-        data : DataFrame
-        target : Series
-    (data, target) : tuple if ``return_X_y`` is True
-        A tuple of a pandas DataFrame (the data) and a pandas Series (target).
+    Bunch or Tuple[pd.DataFrame, pd.Series] or pd.DataFrame
+        If `return_X_y` is False, return a `Bunch` object with the following
+        attributes:
+            * data : pd.DataFrame of shape (n_samples, n_features)
+                The feature matrix.
+            * target : pd.Series of shape (n_samples,)
+                The target vector.
+            * DESCR : str
+                A short description of the dataset.
+        If `return_X_y` is True, return a tuple `(X, y)` where `X` is the feature
+        matrix and `y` is the target vector. If only numeric or categorical
+        columns are included in the output, return a pd.DataFrame instead of a
+        Bunch.
+
+    Examples
+    --------
+    >>> from spotRiver.data import fetch_opm
+        # Fetch the OPM dataset and return a pandas DataFrame
+        opm_df = fetch_opm()
+        # Fetch the OPM dataset, include categorical columns, and return a Bunch object
+        opm_data = fetch_opm(include_numeric=False, include_categorical=True, return_X_y=False)
+        # Fetch the OPM dataset, include numeric and categorical columns, and return a tuple of pandas DataFrames
+        X, y = fetch_opm(include_categorical=True, return_X_y=True)
     """
     filename = get_data_home(data_home=data_home) / "opm_2001-2020.csv"
     if not filename.is_file():
         if not download_if_missing:
             raise IOError("Data not found and `download_if_missing` is False")
         logger.info(f"Downloading OPM dataset to '{filename}'.")
         urlretrieve(url=OPM_URL, filename=filename)
@@ -147,15 +175,16 @@
             if df[cat_col].nunique() < 200:
                 df[cat_col] = df[cat_col].astype("category")
 
     if len(cols) == 0:
         raise Exception("No columns selected. Did you set both `include_numeric` and `include_categorical` to False?")
 
     X = df[cols]
-    y = df["Sale Amount"]
+    # y = df["Sale Amount"]
+    y = X.pop("Sale Amount")
 
     if return_X_y:
         return (X, y)
     return Bunch(data=X, target=y)
 
 
 __all__ = ["fetch_opm"]
```

### Comparing `spotRiver-0.0.9/src/spotRiver/data/synth/sea.py` & `spotRiver-0.0.91/src/spotRiver/data/synth/sea.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,31 +47,28 @@
     References
     ----------
     [^1]: [A Streaming Ensemble Algorithm (SEA) for Large-Scale Classification](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.482.3991&rep=rep1&type=pdf)
 
     """
 
     def __init__(self, variant=0, noise=0.0, seed: int = None):
-
         super().__init__(n_features=3, task=datasets.base.BINARY_CLF)
 
         if variant not in (0, 1, 2, 3):
             raise ValueError("Unknown variant, possible choices are: 0, 1, 2, 3")
 
         self.variant = variant
         self.noise = noise
         self.seed = seed
         self._threshold = {0: 8, 1: 9, 2: 7, 3: 9.5}[variant]
 
     def __iter__(self):
-
         rng = random.Random(self.seed)
 
         while True:
-
             x = {i: rng.uniform(0, 10) for i in range(3)}
             y = x[0] + x[1] > self._threshold
 
             if self.noise and rng.random() < self.noise:
                 y = not y
 
             yield x, y
```

### Comparing `spotRiver-0.0.9/src/spotRiver.egg-info/PKG-INFO` & `spotRiver-0.0.91/src/spotRiver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotRiver
-Version: 0.0.9
+Version: 0.0.91
 Summary: spotRiver - Sequential Parameter Optimization Interface to River
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 Project-URL: Homepage, https://www.spotseven.de
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```


# Comparing `tmp/klassez-0.1a1.tar.gz` & `tmp/klassez-0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klassez-0.1a1.tar", last modified: Tue Feb 21 13:48:54 2023, max compression
+gzip compressed data, was "klassez-0.1a2.tar", last modified: Wed Apr 19 14:11:01 2023, max compression
```

## Comparing `klassez-0.1a1.tar` & `klassez-0.1a2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-02-21 13:48:54.374229 klassez-0.1a1/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1072 2023-01-23 10:50:18.000000 klassez-0.1a1/LICENSE.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       46 2022-10-07 15:29:16.000000 klassez-0.1a1/MANIFEST.in
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1146 2023-02-21 13:48:54.374229 klassez-0.1a1/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      586 2023-02-02 15:11:58.000000 klassez-0.1a1/README.md
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-02-21 13:48:54.370229 klassez-0.1a1/klassez/
--rwxr-xr-x   0 francesco  (1000) francesco  (1000)    57927 2023-02-21 13:16:34.000000 klassez-0.1a1/klassez/Spectra.py
--rwxr-xr-x   0 francesco  (1000) francesco  (1000)      656 2023-02-06 11:44:05.000000 klassez-0.1a1/klassez/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2356 2022-11-16 15:16:53.000000 klassez-0.1a1/klassez/config.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-02-21 13:48:54.370229 klassez-0.1a1/klassez/docs/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)  1106061 2023-02-21 13:14:09.000000 klassez-0.1a1/klassez/docs/klassez.pdf
--rwxr-xr-x   0 francesco  (1000) francesco  (1000)    52286 2023-02-20 11:19:00.000000 klassez-0.1a1/klassez/figures.py
--rwxr-xr-x   0 francesco  (1000) francesco  (1000)    84846 2023-02-15 13:43:18.000000 klassez-0.1a1/klassez/fit.py
--rwxr-xr-x   0 francesco  (1000) francesco  (1000)    46989 2023-02-20 14:08:29.000000 klassez-0.1a1/klassez/misc.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)   140125 2023-02-20 13:53:00.000000 klassez-0.1a1/klassez/processing.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)      380 2023-02-16 13:55:28.000000 klassez-0.1a1/klassez/qsin.py
--rwxr-xr-x   0 francesco  (1000) francesco  (1000)    28582 2023-02-14 09:46:20.000000 klassez-0.1a1/klassez/sim.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-02-21 13:48:54.370229 klassez-0.1a1/klassez/test/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      496 2022-12-07 10:52:08.000000 klassez-0.1a1/klassez/test/acqus_1D
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      864 2022-12-07 10:55:09.000000 klassez-0.1a1/klassez/test/acqus_2D
--rwxr-xr-x   0 francesco  (1000) francesco  (1000)      250 2023-01-23 14:40:44.000000 klassez-0.1a1/klassez/test/test.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-02-21 13:48:54.370229 klassez-0.1a1/klassez.egg-info/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1146 2023-02-21 13:48:54.000000 klassez-0.1a1/klassez.egg-info/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      461 2023-02-21 13:48:54.000000 klassez-0.1a1/klassez.egg-info/SOURCES.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2023-02-21 13:48:54.000000 klassez-0.1a1/klassez.egg-info/dependency_links.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       51 2023-02-21 13:48:54.000000 klassez-0.1a1/klassez.egg-info/requires.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        8 2023-02-21 13:48:54.000000 klassez-0.1a1/klassez.egg-info/top_level.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       85 2022-06-26 15:36:10.000000 klassez-0.1a1/pyproject.toml
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2023-02-21 13:48:54.374229 klassez-0.1a1/setup.cfg
--rwxr-xr-x   0 francesco  (1000) francesco  (1000)     1084 2023-02-21 13:48:49.000000 klassez-0.1a1/setup.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-19 14:11:01.603543 klassez-0.1a2/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1072 2023-01-23 10:50:18.000000 klassez-0.1a2/LICENSE.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       46 2022-10-07 15:29:16.000000 klassez-0.1a2/MANIFEST.in
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1147 2023-04-19 14:11:01.603543 klassez-0.1a2/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      586 2023-02-02 15:11:58.000000 klassez-0.1a2/README.md
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-19 14:11:01.603543 klassez-0.1a2/klassez/
+-rwxr-xr-x   0 francesco  (1000) francesco  (1000)    66185 2023-04-19 10:26:52.000000 klassez-0.1a2/klassez/Spectra.py
+-rwxr-xr-x   0 francesco  (1000) francesco  (1000)      662 2023-03-31 14:18:37.000000 klassez-0.1a2/klassez/__init__.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)     2833 2023-04-04 15:39:34.000000 klassez-0.1a2/klassez/config.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-19 14:11:01.603543 klassez-0.1a2/klassez/docs/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)  1170899 2023-04-19 14:10:58.000000 klassez-0.1a2/klassez/docs/klassez.pdf
+-rwxr-xr-x   0 francesco  (1000) francesco  (1000)    57660 2023-04-17 15:08:41.000000 klassez-0.1a2/klassez/figures.py
+-rwxr-xr-x   0 francesco  (1000) francesco  (1000)   138749 2023-04-18 14:21:11.000000 klassez-0.1a2/klassez/fit.py
+-rwxr-xr-x   0 francesco  (1000) francesco  (1000)    49289 2023-04-17 13:51:13.000000 klassez-0.1a2/klassez/misc.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)   146069 2023-04-17 15:53:36.000000 klassez-0.1a2/klassez/processing.py
+-rwxrwxr-x   0 francesco  (1000) francesco  (1000)      465 2023-04-06 12:51:03.000000 klassez-0.1a2/klassez/show_fcn.py
+-rwxr-xr-x   0 francesco  (1000) francesco  (1000)    28870 2023-04-19 13:41:18.000000 klassez-0.1a2/klassez/sim.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-19 14:11:01.603543 klassez-0.1a2/klassez/test/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      496 2022-12-07 10:52:08.000000 klassez-0.1a2/klassez/test/acqus_1D
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      864 2022-12-07 10:55:09.000000 klassez-0.1a2/klassez/test/acqus_2D
+-rwxr-xr-x   0 francesco  (1000) francesco  (1000)      250 2023-01-23 14:40:44.000000 klassez-0.1a2/klassez/test/test.py
+drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2023-04-19 14:11:01.603543 klassez-0.1a2/klassez.egg-info/
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)     1147 2023-04-19 14:11:01.000000 klassez-0.1a2/klassez.egg-info/PKG-INFO
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)      465 2023-04-19 14:11:01.000000 klassez-0.1a2/klassez.egg-info/SOURCES.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2023-04-19 14:11:01.000000 klassez-0.1a2/klassez.egg-info/dependency_links.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       51 2023-04-19 14:11:01.000000 klassez-0.1a2/klassez.egg-info/requires.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)        8 2023-04-19 14:11:01.000000 klassez-0.1a2/klassez.egg-info/top_level.txt
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       85 2022-06-26 15:36:10.000000 klassez-0.1a2/pyproject.toml
+-rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2023-04-19 14:11:01.603543 klassez-0.1a2/setup.cfg
+-rwxr-xr-x   0 francesco  (1000) francesco  (1000)     1085 2023-03-21 12:07:56.000000 klassez-0.1a2/setup.py
```

### Comparing `klassez-0.1a1/LICENSE.txt` & `klassez-0.1a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `klassez-0.1a1/PKG-INFO` & `klassez-0.1a2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: klassez
-Version: 0.1a1
+Version: 0.1a2
 Summary: A collection of functions for NMR data handling. Documentation: klassez.pdf in "docs" subfolder of your install dir.
-Home-page: https://test.pypi.org/legacy/klassez
+Home-page: https://github.com/MetallerTM/klassez
 Author: Francesco Bruno
 Author-email: bruno@cerm.unifi.it
 License: LICENSE.txt
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `klassez-0.1a1/README.md` & `klassez-0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `klassez-0.1a1/klassez/Spectra.py` & `klassez-0.1a2/klassez/Spectra.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,46 +15,82 @@
 import nmrglue as ng
 import lmfit as l
 from datetime import datetime
 import warnings
 
 from . import fit, misc, sim, figures, processing
 #from .__init__ import CM
-from .config import CM
+from .config import CM, COLORS, cron
 
 
-warnings.filterwarnings(action='ignore', category=UserWarning)
-
+# Suppress warnings that create alarmism
+warnings.filterwarnings(action='ignore', message='Error reading the pulse program')
+warnings.filterwarnings(action='ignore', message=r'[0-9]*cannot')
+
+# Declare interesting things
+proc_keys_1D = ['wf', 'zf', 'fcor', 'tdeff']
+wf0 = {
+        'mode':None,
+        'ssb':2,
+        'lb':5,
+        'gb':10,
+        'gc':0,
+        'sw':None
+        }
 """
 Classes for the management of NMR data.
 """
+
 class Spectrum_1D:
     """
     Class: 1D NMR spectrum
+    ---------
+    Attributes:
+    - datadir: str
+        Path to the input file/dataset directory
+    - fid: 1darray
+        FID
+    - acqus: dict
+        Dictionary of acqusition parameters
+    - ngdic: dict
+        Created only if it is an experimental spectrum. Generated by nmrglue.bruker.read, contains all the information on the spectrometer and on the spectrum.
+    - procs: dict
+        Dictionary of processing parameters
+    - S: 1darray
+        Complex spectrum
+    - r: 1darray
+        Real part of the spectrum
+    - i: 1darray
+        Imaginary part of the spectrum
+    - freq: 1darray
+        Frequency scale of the spectrum, in Hz
+    - ppm: 1darray
+        ppm scale of the spectrum
+    - F: fit.Voigt_Fit object
+        Used for deconvolution. See fit.Voigt_fit.
+    - baseline: 1darray
+        Baseline of the spectrum.
+    - integrals: dict
+        Dictionary where to save the regions and values of the integrals.
     """
     def __str__(self):
+        """ Prints info on the object """
         doc = '-'*64
         doc += '\nSpectrum_1D object.\n'
         if 'ngdic' in self.__dict__.keys():
             doc += f'Read from "{self.datadir}"\n'
         else:
             doc += f'Simulated from "{self.datadir}"\n'
         N = self.fid.shape[-1]
         doc += f'It is a {self.acqus["nuc"]} spectrum recorded over a\nsweep width of {self.acqus["SWp"]} ppm, centered at {self.acqus["o1p"]} ppm.\n'
         doc += f'The FID is {N} points long.\n'
         doc += '-'*64
 
         return doc
 
-    def __len__(self):
-        if 'S' in self.__dict__.keys():
-            return self.S.shape[-1]
-        else:
-            return self.fid.shape[-1]
-
     def __init__(self, in_file, pv=False, isexp=True):
         """
         Initialize the class. 
         Simulation of the dataset (i.e. isexp=False) employs sim.sim_1D.
         -------
         Parameters:
         - in_file: str
@@ -69,61 +105,50 @@
             self.acqus = sim.load_sim_1D(in_file)
             self.fid = sim.sim_1D(in_file, pv=pv)
         else:
             warnings.filterwarnings("ignore")   # Suppress errors due to CONVDTA in TopSpin
             dic, data = ng.bruker.read(in_file, cplex=True)
             self.fid = data
             self.acqus = misc.makeacqus_1D(dic)
-            self.BYTORDA = dic['acqus']['BYTORDA']
-            self.DTYPA = dic['acqus']['DTYPA']
+            self.acqus['BYTORDA'] = dic['acqus']['BYTORDA']
+            self.acqus['DTYPA'] = dic['acqus']['DTYPA']
             self.ngdic = dic        # NMRGLUE dictionary of parameters
             del dic
             del data
         # Look for group delay points: if there is not, put it to 0
         try:
-            self.grpdly = int(self.ngdic['acqus']['GRPDLY'])
+            self.acqus['GRPDLY'] = int(self.ngdic['acqus']['GRPDLY'])
         except:
-            self.grpdly = 0
+            self.acqus['GRPDLY'] = 0
 
         # Initalize the procs dictionary with default values
         #       DEFAULT VALUES
         # -----------------------------------------------
-        proc_keys_1D = ['wf', 'zf', 'fcor', 'tdeff']
-        wf0 = {
-                'mode':None,
-                'ssb':2,
-                'lb':5,
-                'gb':10,
-                'gc':0,
-                'sw':None
-                }
-        proc_init_1D = (wf0, None, 0.5, 0)
-        # -----------------------------------------------
+        proc_init_1D = (dict(wf0), None, 0.5, 0)
 
-        self.procs = {
-                }
+        self.procs = {}
         for k, key in enumerate(proc_keys_1D):
             self.procs[key] = proc_init_1D[k]         # Processing parameters
         self.procs['wf']['sw'] = round(self.acqus['SW'], 4)
         #   Then, phases
         self.procs['p0'] = 0
         self.procs['p1'] = 0
         self.procs['pv'] = round(self.acqus['o1p'], 2)
         
     def convdta(self, scaling=1):
-        """ Call processing.convdta using attribute self.grpdly """
-        self.fid = processing.convdta(self.fid, self.grpdly, scaling)
+        """ Call processing.convdta using self.acqus['GRPDLY'] """
+        self.fid = processing.convdta(self.fid, self.acqus['GRPDLY'], scaling)
 
     def process(self, interactive=False):
         """
         Performs the processing of the FID. The parameters are read from self.procs.
         Calls processing.interactive_fp or processing.fp using self.acqus and self.procs
         Writes the result is self.S, then unpacks it in self.r and self.i
         Calculates frequency and ppm scales.
-        Initializes self.F with fit.Voigt_Fit class using the current parameters
+        Also initializes self.F with fit.Voigt_Fit class using the current parameters
         --------
         Parameters:
         - interactive: bool
             True if you want to open the interactive panel, False to read the parameters from self.procs.
         """
         if interactive is True:
             self.S, self.procs = processing.interactive_fp(self.fid, self.acqus, self.procs)
@@ -222,26 +247,32 @@
         --------
         Parameters:
         - path: str
             Filename 
         """
         misc.write_acqus_1D(self.acqus, path=path)
 
-    def write_ser(self, path=None):
+    @staticmethod
+    def write_ser(ser, acqus, path=None):
         """
-        Writes the FID in binary format.
-        Calls misc.write_ser
+        Writes a real/complex array in binary format.
+        Calls misc.write_ser. Be sure that acqus contains the BYTORDA and DTYPA keys.
+        See misc.write_ser to understand the meaning of these values.
         --------
         Parameters:
-        - path: str or None
-            Path where to save the binary file. If it is None, the original binary file is overwritten, so BE CAREFUL!!!
+        - ser: ndarray
+            Array that you want to convert in binary format.
+        - acqus: dict
+            Dictionary of acquisition parameters. It must contain BYTORDA and DTYPA.
+        - path: str 
+            Path where to save the binary file.
         """
         if path is None:
-            path = self.datadir
-        misc.write_ser(path, self.fid, self.BYTORDA, self.DTYPA)
+            raise NameError('You must specify a filename!')
+        misc.write_ser(path, ser, acqus['BYTORDA'], acqus['DTYPA'])
 
     def plot(self):
         """
         Plots the real part of the spectrum.
         """
         n_xticks = 10
 
@@ -263,23 +294,23 @@
         X_label = '$\delta\ $'+misc.nuc_format(self.acqus['nuc'])+' /ppm'
         ax.set_xlabel(X_label)
 
         misc.mathformat(ax)
         misc.set_fontsizes(ax, 14)
         cursor = Cursor(ax, useblit=True, c='tab:red', lw=0.8, horizOn=False)
 
-
         plt.show()
         plt.close()
 
     def qfil(self, u=None, s=None):
         """
         Gaussian filter to suppress signals.
         Tries to read self.procs['qfil'], which is
             { 'u': u, 's': s }
+        Otherwise, these are set interactively by processing.interactive_qfil and then added to self.procs.
         Calls processing.qfil
         ---------
         Parameters:
         - u: float
             Position /ppm
         - s: float
             Width (standard deviation) /ppm
@@ -309,15 +340,19 @@
         if not os.path.exists(basl_file):
             processing.baseline_correction(self.ppm, self.r, basl_file=basl_file, winlim=winlim)
         self.baseline = processing.load_baseline(basl_file, self.ppm, self.r)
 
     def integrate(self, lims=None):
         """
         Integrate the spectrum with a dedicated GUI.
-        Calls fit.integrate and writes in self.integrals
+        Calls fit.integrate and writes in self.integrals with keys [ppm1:ppm2]
+        --------
+        Parameters:
+        - lims: tuple
+            Integrates from lims[0] to lims[1]. If it is None, calls for interactive integration.
         """
         X_label = '$\delta\,$'+misc.nuc_format(self.acqus['nuc'])+' /ppm'
         if lims is None:
             integrals = fit.integrate(self.ppm, self.r, X_label=X_label)
             for key, value in integrals.items():
                 self.integrals[key] = value
         else:
@@ -347,183 +382,217 @@
         f.close()
 
     
 class pSpectrum_1D(Spectrum_1D):
     """
     Subclass of Spectrum_1D that allows to handle processed 1D NMR spectra.
     Useful when dealing with traces of 2D spectra.
+    Shares the same attributes with Spectrum_1D.
+    -------------
+    Attributes:
+    - acqus: dict
+        Dictionary of acqusition parameters
+    - ngdic: dict
+        Created only if it is an experimental spectrum. Generated by nmrglue.bruker.read, contains all the information on the spectrometer and on the spectrum.
+    - procs: dict
+        Dictionary of processing parameters
+    - S: 1darray
+        Complex spectrum
+    - r: 1darray
+        Real part of the spectrum
+    - i: 1darray
+        Imaginary part of the spectrum
+    - freq: 1darray
+        Frequency scale of the spectrum, in Hz
+    - ppm: 1darray
+        ppm scale of the spectrum
+    - F: fit.Voigt_Fit object
+        Used for deconvolution. See fit.Voigt_fit.
+    - baseline: 1darray
+        Baseline of the spectrum.
+    - integrals: dict
+        Dictionary where to save the regions and values of the integrals.
     """
     def __init__(self, in_file, acqus=None, procs=None, istrace=False):
         """
         Initialize the class. 
         -------
         Parameters:
         - in_file: str or 1darray
-            If istrace is True, in_file is the NMR spectrum, real part. If istrace is False, in_file is the directory of the processed data.
+            If istrace is True, in_file is the NMR spectrum. Else, it is the directory of the processed data.
         - acqus: dict or None
-            If istrace is True, you must pass the associated 'acqus' dictionary. If istrace is False, it is not necessary as it is read from the input directory
+            If istrace is True, you must supply the associated 'acqus' dictionary. Else, it is not necessary as it is read from the input directory
         - procs: dict or None
-            You can pass the dictionary of processing parameters, if you want. Otherwise, it is initialized as empty.
+            You can pass the dictionary of processing parameters, if you want. Otherwise, it is initialized with standard values.
         - istrace: bool
-            Declare the object as trace extracted from a 2D (True) or true experimental spectrum (False)
+            Declare the object as trace extracted from a 2D (True) or as true experimental spectrum (False)
         """
         if istrace is True:
-            self.r = in_file
-            self.S = self.r
+            assert isinstance(in_file, np.ndarray), 'The first parameter must be an array if istrace=True!'
+            if np.iscomplexobj(in_file):
+                self.r = in_file.real
+                self.i = in_file.imag
+                self.S = self.r + 1j * self.i
+            else:
+                self.r = in_file
+                self.S = self.r
             self.acqus = acqus
-
         else:
-            warnings.filterwarnings("ignore")
             dic, data = ng.bruker.read_pdata(in_file)
             _, self.r = ng.bruker.read_pdata(in_file, bin_files=['1r'])
             _, self.i = ng.bruker.read_pdata(in_file, bin_files=['1i'])
             self.S = self.r + 1j * self.i
             self.acqus = misc.makeacqus_1D(dic)
-            self.BYTORDA = dic['acqus']['BYTORDA']
-            self.DTYPA = dic['acqus']['DTYPA']
+            self.acqus['BYTORDA'] = dic['acqus']['BYTORDA']
+            self.acqus['DTYPA'] = dic['acqus']['DTYPA']
             self.ngdic = dic
             del dic
             del data
         try:
-            self.grpdly = int(self.ngdic['acqus']['GRPDLY'])
+            self.acqus['GRPDLY'] = int(self.ngdic['acqus']['GRPDLY'])
         except:
-            self.grpdly = 0
-
-        if procs is None:
-            proc_keys_1D = ['wf', 'zf', 'fcor', 'tdeff']
-            wf0 = {
-                    'mode':None,
-                    'ssb':2,
-                    'lb':5,
-                    'gb':10,
-                    'gc':0,
-                    'sw':None
-                    }
-            proc_init_1D = (wf0, None, 0.5, 0)
+            self.acqus['GRPDLY'] = 0
 
-            self.procs = {
-                    }
+        if procs is None:   # Make it
+            proc_init_1D = (dict(wf0), None, 0.5, 0)
+            self.procs = {}
             for k, key in enumerate(proc_keys_1D):
                 self.procs[key] = proc_init_1D[k]         # Processing parameters
             self.procs['wf']['sw'] = round(self.acqus['SW'], 4)
             # Then, phases
             self.procs['p0'] = 0
             self.procs['p1'] = 0
             self.procs['pv'] = self.acqus['o1p']
-        else:
-            self.procs = procs
+        else:   # Copy it
+            self.procs = dict(procs)
         
         # Calculate frequency and ppm scales
         self.freq = processing.make_scale(self.r.shape[0], dw=self.acqus['dw'])
         if self.acqus['SFO1'] < 0:
             self.freq = self.freq[::-1]
         self.ppm = misc.freq2ppm(self.freq, B0=self.acqus['SFO1'], o1p=self.acqus['o1p'])
 
+        # Initialize fit object
         self.F = fit.Voigt_Fit(self.ppm, self.S, self.acqus['t1'], self.acqus['SFO1'], self.acqus['o1p'], self.acqus['nuc'])
 
-    def write_ser(self):
-        """Overwrite the original function to prevent writing of the binary file. It does nothing!"""
-        pass
-
 
 class Spectrum_2D:
     """
     Class: 2D NMR spectrum
+    ---------
+    Attributes:
+    - datadir: str
+        Path to the input file/dataset directory
+    - fid: 2darray
+        FID
+    - acqus: dict
+        Dictionary of acqusition parameters
+    - ngdic: dict
+        Created only if it is an experimental spectrum. Generated by nmrglue.bruker.read, contains all the information on the spectrometer and on the spectrum.
+    - procs: dict
+        Dictionary of processing parameters
+    - eaeflag: int
+        If FnMODE is Echo-Antiecho, keeps track of the manipulation of the data so to not repeat the same process twice
+    - S: 2darray
+        Complex (or hypercomplex, depending on FnMODE) spectrum
+    - rr: 2darray
+        Real part F2, real part F1
+    - ii: 2darray
+        Imaginary part F2, imaginary part F1
+    - ir: 2darray
+        Real part F2, imaginary part F1. Only exist if F1 is acquired in phase-sensitive mode
+    - ri: 2darray
+        Imaginary part F2, real part F1. Only exist if F1 is acquired in phase-sensitive mode
+    - freq_f1: 1darray
+        Frequency scale of the indirect dimension, in Hz
+    - freq_f2: 1darray
+        Frequency scale of the direct dimension, in Hz
+    - ppm_f1: 1darray
+        ppm scale of the indirect dimension
+    - ppm_f2: 1darray
+        ppm scale of the direct dimension
+    - trf1: dict
+        Projections of the indirect dimension, as 1darrays. Keys: 'ppm_f2' where they were taken
+    - trf2: dict
+        Projections of the direct dimension, as 1darrays. Keys: 'ppm_f1' where they were taken
+    - Trf1: dict
+        Projections of the indirect dimension, as pSpectrum_1D objects. Keys: 'ppm_f2' where they were taken
+    - Trf2: dict
+        Projections of the direct dimension, as pSpectrum_1D objects. Keys: 'ppm_f1' where they were taken
+    - integrals: dict
+        Dictionary where to save the regions and values of the integrals.
     """
     def __str__(self):
+        """ Prints info on the object """
         doc = '-'*64
         doc += '\nSpectrum_2D object.\n'
         if 'ngdic' in self.__dict__.keys():
             doc += f'Read from "{self.datadir}"\n'
         else:
             doc += f'Simulated from "{self.datadir}"\n'
         N = self.fid.shape
         doc += f'It is a {self.acqus["nuc1"]}-{self.acqus["nuc2"]} spectrum recorded over a \nsweep width of \n{self.acqus["SW1p"]} ppm centered at {self.acqus["o1p"]} ppm in F1, and\n{self.acqus["SW2p"]} ppm centered at {self.acqus["o2p"]} ppm in F2.\n'
         doc += f'The FID is {N[0]}x{N[1]} points long.\n'
         doc += '-'*64
 
         return doc
 
-    def __len__(self):
-        if 'S' in self.__dict__.keys():
-            return self.S.shape[-1]
-        else:
-            return self.fid.shape[-1]
-
     def __init__(self, in_file, pv=False, isexp=True, is_pseudo=False):
         """
         Initialize the class. 
         -------
         Parameters:
         - in_file: str
             path to file to read, or to the folder of the spectrum
-        - isexp: bool
-            True if this is an experimental dataset, False if it is simulated
         - pv: bool
             True if you want to use pseudo-voigt lineshapes for simulation, False for Voigt
+        - isexp: bool
+            True if this is an experimental dataset, False if it is simulated
         - is_pseudo: bool
             True if it is a pseudo-2D. 
         """
         self.datadir = in_file
         if isexp is False:
             self.acqus = sim.load_sim_2D(in_file)
             if is_pseudo:
                 self.acqus['FnMODE'] = 'No'
             else:
                 self.acqus['FnMODE'] = 'States-TPPI'
             self.fid = sim.sim_2D(in_file, pv=pv)
         else:
-            warnings.filterwarnings("ignore")
             dic, data = ng.bruker.read(in_file, cplex=True)
             self.ngdic = dic
             self.fid = data
             self.acqus = misc.makeacqus_2D(dic)
-            self.BYTORDA = dic['acqus']['BYTORDA']
-            self.DTYPA = dic['acqus']['DTYPA']
+            self.acqus['BYTORDA'] = dic['acqus']['BYTORDA']
+            self.acqus['DTYPA'] = dic['acqus']['DTYPA']
             FnMODE_flag = dic['acqu2s']['FnMODE']
             FnMODEs = ['Undefined', 'QF', 'QSEC', 'TPPI', 'States', 'States-TPPI', 'Echo-Antiecho']
             self.acqus['FnMODE'] = FnMODEs[FnMODE_flag]
             # put a flag to say "shuffle"
             if self.acqus['FnMODE'] == 'Echo-Antiecho':
                 self.eaeflag = 1
             else:
                 self.eaeflag = 0
             del dic
             del data
 
         try:
-            self.grpdly = int(self.ngdic['acqus']['GRPDLY'])
+            self.acqus['GRPDLY'] = int(self.ngdic['acqus']['GRPDLY'])
         except:
-            self.grpdly = 0
+            self.acqus['GRPDLY'] = 0
 
         # initialize the procs dictionary with default values
-        wf1 = {
-                'mode':None,
-                'ssb':2,
-                'lb':5,
-                'gb':10,
-                'gc':0,
-                'sw':None
-                }
-        wf2 = {
-                'mode':None,
-                'ssb':2,
-                'lb':5,
-                'gb':10,
-                'gc':0,
-                'sw':None
-                }
         proc_init_2D = (
-                [wf1, wf2],     # window function
+                [dict(wf0), dict(wf0)],     # window function
                 [None, None],   # zero-fill
                 [0.5, 0.5],     # fcor
                 [0,0]           # tdeff
                 )
 
-        proc_keys_1D = ['wf', 'zf', 'fcor', 'tdeff']
         self.procs = {}
         for k, key in enumerate(proc_keys_1D):
             self.procs[key] = proc_init_2D[k]         # Processing parameters
         self.procs['wf'][0]['sw'] = round(self.acqus['SW1'], 4)
         self.procs['wf'][1]['sw'] = round(self.acqus['SW2'], 4)
 
         # Then, phases
@@ -537,26 +606,37 @@
         # Create empty dictionary where to save the projections
         self.trf1 = {}
         self.trf2 = {}
         self.Trf1 = {}
         self.Trf2 = {}
 
     def convdta(self, scaling=1):
-        """ Calls processing.convdta """
-        self.fid = processing.convdta(self.fid, self.grpdly, scaling)
+        """
+        Calls processing.convdta to compensate for the group delay. 
+        It does not always work, depends on TopSpin version and planets alignment.
+        --------
+        Parameters:
+        - scaling: float
+            Scaling factor for processingconvdta.
+        """
+        self.fid = processing.convdta(self.fid, self.acqus['GRPDLY'], scaling)
 
     def eae(self):
-        """ Calls processing.EAE to shuffle the data. """
+        """
+        Calls processing.EAE to shuffle the data and make a States-like FID.
+        Sets self.eaeflag to 0.
+        """
         self.fid = processing.EAE(self.fid)
         self.eaeflag = 0
 
     def xf2(self):
         """
         Process only the direct dimension.
         Calls processing.fp using procs[keys][1]
+        The result is stored in self.S, then self.rr and self.ii are written.
         freq_f1 and ppm_f1 are assigned with the indexes of the transients.
         """
         if self.procs['zf'][1] is None:
             self.S = np.zeros_like(self.fid)
         else:
             self.S = np.zeros((self.fid.shape[0], self.procs['zf'][1]))
 
@@ -576,15 +656,18 @@
 
         self.freq_f1 = np.arange(self.S.shape[0])
         self.ppm_f1 = np.arange(self.S.shape[0])
 
     def xf1(self):
         """
         Process only the indirect dimension. 
-        Transposes the spectrum in hypermode or normally if FnMODE != QF, then calls for processing.fp using self.procs[keys][0], then transposes it back.
+        Transposes the spectrum in hypermode or normally if FnMODE != QF, 
+        then calls for processing.fp using self.procs[keys][0], finally transposes it back.
+        The result is stored in self.S, then self.rr and self.ii are written.
+        freq_f1 and ppm_f1 are assigned with the indexes of the transients.
         """
         if self.acqus['FnMODE']=='QF':
             self.fid = self.fid.T
         else:
             self.fid = processing.tp_hyper(self.fid)
 
         if self.procs['zf'][0] is None:
@@ -604,31 +687,31 @@
 
         self.freq_f1 = processing.make_scale(self.S.shape[0], dw=self.acqus['dw1'])
         if self.acqus['SFO1'] < 0:
             self.freq_f1 = self.freq_f1[::-1]
         self.ppm_f1 = misc.freq2ppm(self.freq_f1, B0=self.acqus['SFO1'], o1p=self.acqus['o1p'])
 
         self.rr = np.copy(self.S.real)
+        self.ii = np.copy(self.S.imag)
         self.ppm_f2 = np.arange(self.S.shape[1])
 
     def process(self, interactive=False, **int_kwargs):
         """
-        Performs the processing of the FID. The parameters are read from self.procs.
-        If interactive is True, calls processing.interactive_xfb with **int_kwargs, else calls processing.xfb
+        Performs the full processing of the FID on both dimensions. The parameters are read from self.procs.
+        If FnMODE is Echo-Antiecho and you did not call self.eae before, the FID is converted to States with processing.EAE before to start.
+        If interactive is True, calls processing.interactive_xfb with int_kwargs, else calls processing.xfb.
+        The complex/hypercomplex spectrum is stored in self.S, then unpacked into self.rr, self.ri, self.ir, self.ii.
+        If FnMODE is Echo-Antiecho, a phase correction of -90 degrees is applied on the indirect dimension.
         --------
         Parameters:
         - interactive: bool
             True if you want to open the interactive panel, False to read the parameters from self.procs.
-        - int_kwargs: 
-            - lvl0: float
-                For interactive processing. Set the starting contour values.
-            - show_cnt: bool
-                For interactive processing. If it is True shows the contours of the spectrum, if it is False shows the heatmap.
+        - int_kwargs: keyworded arguments
+            Additional parameters for processing.interactive_xfb, if interactive=True.
         """
-
         # If Echo-Antiecho, pre-process the FID to get the correct spectral arrangement
         if self.acqus['FnMODE'] == 'Echo-Antiecho' and self.eaeflag == 1:
             self.fid = processing.EAE(self.fid)
 
         if interactive is True:
             self.S, self.procs = processing.interactive_xfb(self.fid, self.acqus, self.procs, **int_kwargs)
         else:
@@ -676,15 +759,15 @@
         self.ppm_f2 = misc.freq2ppm(self.freq_f2, B0=self.acqus['SFO2'], o1p=self.acqus['o2p']) 
 
 
     def inv_process(self):
         """
         Performs the inverse processing of the spectrum according to the given parameters.
         Overwrites the S attribute!!
-        Calls inv_xfb
+        Calls inv_xfb.
         """
 
         # For EAE, correct the 90° phase shift in F1
         if self.acqus['FnMODE'] == 'Echo-Antiecho':
             self.S = processing.tp_hyper(self.S)
             self.S = processing.ps(self.S, p0=90)[0]
             self.S = processing.tp_hyper(self.S)
@@ -693,33 +776,39 @@
             self.S = self.S[:,::-1]
         if self.acqus['SFO1'] < 0:
             self.S = self.S[::-1,:]
             self.S = processing.tp_hyper(self.S)
             self.S = processing.ps(self.S, p0=-90)[0]
             self.S = processing.tp_hyper(self.S)
 
-        self.S = processing.inv_xfb(self.S, wf=self.procs['wf'], size=[self.acqus['TD1'], self.acqus['TD2']], fcor=self.procs['fcor'], FnMODE=self.acqus['FnMODE'])
+        self.S = processing.inv_xfb(self.S, wf=self.procs['wf'], size=(self.acqus['TD1'], self.acqus['TD2']), fcor=self.procs['fcor'], FnMODE=self.acqus['FnMODE'])
 
 
     def mc(self):
-        """ Compute the magnitude of the spectrum. """
+        """
+        Computes the magnitude of the spectrum on self.S.
+        Then, updates rr, ri, ir, ii.
+        """
         self.S = (self.S.real**2 + self.S.imag**2 )**0.5
         if self.acqus['FnMODE'] == 'QF':
             self.rr = self.S.real
             self.ii = self.S.imag
         else:
             rr, ir, ri, ii = processing.unpack_2D(self.S)
             self.rr = rr
             self.ri = ri
             self.ir = ir
             self.ii = ii
 
     def adjph(self, p01=None, p11=None, pv1=None, p02=None, p12=None, pv2=None):
         """
         Adjusts the phases of the spectrum according to the given parameters, or interactively if they are left as default.
+        The non-interactive workflow is to apply processing.ps on F2, transpose according to FnMODE, apply processing.ps on F1, transpose back.
+        If FnMODE is 'No', the phase correction is applied only on F2, as it should be done in a pseudo-2D experiment.
+        Once self.S was updated and unpacked, the phase values are added to the procs dictionary to keep track of multiple phase adjustments.
         -------
         Parameters:
         - p01: float or None
             0-th order phase correction /° of the indirect dimension
         - p11: float or None
             1-st order phase correction /° of the indirect dimension
         - pv1: float or None
@@ -785,29 +874,36 @@
         self.procs['p1_1'] += round(values_f1[1], 2)
         if values_f1[2] is not None:
             self.procs['pv_1'] = round(values_f1[2], 5)
 
 
     def qfil(self, which=None, u=None, s=None):
         """ 
-        Suppress signals using qfil. 
-        'Which' is the number of the trace to be used.
-        Edits only 'rr' if FnMODE is phase-sensitive
+        Gaussian filter to suppress signals.
+        Tries to read self.procs['qfil'], which is
+            { 'u': u, 's': s }
+        Otherwise, these are set interactively by processing.interactive_qfil and then added to self.procs.
         Calls processing.qfil
+        ---------
+        Parameters:
+        - which: int or None
+            Index of the F2 trace to be used for interactive_qfil. If None, a suitable trace can be selected using misc.select_traces.
+        - u: float
+            Position /ppm
+        - s: float
+            Width (standard deviation) /ppm
         """
         if 'qfil' not in self.procs.keys():
             self.procs['qfil'] = {'u': u, 's': s}
-        if which is None:
-            which_list = misc.select_traces(self.ppm_f1, self.ppm_f2, self.rr, Neg=False, grid=False)
-            print(which_list)
-            which, _ = misc.ppmfind(self.ppm_f1, which_list[0][1])
-        print(which, self.ppm_f1[which])
 
         for key, value in self.procs['qfil'].items():
             if value is None:
+                if which is None:
+                    which_list = misc.select_traces(self.ppm_f1, self.ppm_f2, self.rr, Neg=False, grid=False)
+                    which, _ = misc.ppmfind(self.ppm_f1, which_list[0][1])
                 self.procs['qfil']['u'], self.procs['qfil']['s'] = processing.interactive_qfil(self.ppm_f2, self.rr[which])
                 break
         self.S = processing.qfil(self.ppm_f2, self.S, self.procs['qfil']['u'], self.procs['qfil']['s'])
         if self.acqus['FnMODE'] == 'QF':
             self.rr = self.S.real
             self.ii = self.S.imag
         else:
@@ -821,14 +917,15 @@
         Parameters:
         - offset: tuple
             (scale shift F1, scale shift F2)
         - isHz: tuple of bool
             True if offset is in frequency units, False if offset is in ppm
         """
 
+        @staticmethod
         def _calibrate(ppm, trace, SFO1, o1p):
             offppm = processing.calibration(ppm, trace)
             offhz = misc.ppm2freq(offppm, SFO1, o1p)
             return offppm, offhz
 
         if offset[0] is None or offset[1] is None:
             coord = misc.select_traces(self.ppm_f1, self.ppm_f2, self.rr, Neg=False, grid=False)
@@ -888,86 +985,94 @@
             scale shift value
         - isHz: bool
             True if offset is in frequency units, False if offset is in ppm
         """
         offset = [value, 0]
         self.cal(offset, isHz)
 
-
-
     def save_acqus(self, path='sim_in_2D'):
         """
         Write the acqus dictionary in a file.
         Calls misc.write_acqus_2D
         --------
         Parameters:
         - path: str
             Filename 
         """
         misc.write_acqus_2D(self.acqus, path=path)
 
-    def write_ser(self, path=None):
+    @staticmethod
+    def write_ser(ser, acqus, path=None):
         """
-        Writes the FID in binary format.
-        Calls misc.write_ser
+        Writes a real/complex array in binary format.
+        Calls misc.write_ser. Be sure that acqus contains the BYTORDA and DTYPA keys.
+        See misc.write_ser to understand the meaning of these values.
         --------
         Parameters:
-        - path: str or None
-            Path where to save the binary file. If it is None, the original binary file is overwritten, so BE CAREFUL!!!
+        - ser: ndarray
+            Array that you want to convert in binary format.
+        - acqus: dict
+            Dictionary of acquisition parameters. It must contain BYTORDA and DTYPA.
+        - path: str 
+            Path where to save the binary file.
         """
         if path is None:
-            path = self.datadir
-        misc.write_ser(self.fid, path, self.BYTORDA, self.DTYPA)
+            raise NameError('You must specify a filename!')
+        misc.write_ser(path, ser, acqus['BYTORDA'], acqus['DTYPA'])
 
     def projf1(self, a, b=None):
         """
-        Calculates the sum trace of the indirect dimension, from a to b in F2.
+        Calculates the sum trace of the indirect dimension, from a ppm to b ppm in F2.
         Store the trace in the dictionary trf1 and as 1D spectrum in Trf1. The key is 'a' or 'a:b'
         Calls misc.get_trace on self.rr with column=True
         -------
         Parameters:
         - a: float
             ppm F2 value where to extract the trace.
         - b: float or None.
             If it is None, extract the trace in a. Else, sum from a to b in F2.
         """
         # make dictionary label
         if b is None:
-            label = str(a)
+            label = f'{a:.2f}'
         else:
-            label = str(a)+':'+str(b)
+            label = f'{a:.2f}:{b:.2f}'
         f1 = misc.get_trace(self.rr, self.ppm_f2, self.ppm_f1, a, b, column=True)
         self.trf1[label] = f1
         self.Trf1[label] = pSpectrum_1D(f1, acqus=misc.split_acqus_2D(self.acqus)[0], procs=misc.split_procs_2D(self.procs)[0], istrace=True)
 
     def projf2(self, a, b=None):
         """
-        Calculates the sum trace of the direct dimension, from a to b in F1.
+        Calculates the sum trace of the direct dimension, from a ppm to b ppm in F1.
         Store the trace in the dictionary trf2 and as 1D spectrum in Trf2. The key is 'a' or 'a:b'
         Calls misc.get_trace on self.rr with column=False
         -------
         Parameters:
         - a: float
             ppm F1 value where to extract the trace.
         - b: float or None.
             If it is None, extract the trace in a. Else, sum from a to b in F1.
         """
         # make dictionary label
         if b is None:
-            label = str(a)
+            label = f'{a:.2f}'
         else:
-            label = str(a)+':'+str(b)
+            label = f'{a:.2f}:{b:.2f}'
         f2 = misc.get_trace(self.rr, self.ppm_f2, self.ppm_f1, a, b, column=False)
         self.trf2[label] = f2
         self.Trf2[label] = pSpectrum_1D(f2, acqus=misc.split_acqus_2D(self.acqus)[1], procs=misc.split_procs_2D(self.procs)[1], istrace=True)
 
     def integrate(self, **kwargs):
         """
-        Integrate the spectrum with a dedicated GUI.
+        Integrates the spectrum with a dedicated GUI.
         Calls fit.integrate_2D 
+        --------
+        Parameters:
+        - kwargs: keyworded arguments
+            Additional parameters for fit.integrate_2D
         """
         self.integrals = fit.integrate_2D(self.ppm_f1, self.ppm_f2, self.rr, self.acqus['SFO1'], self.acqus['SFO2'], **kwargs)
 
     def write_integrals(self, filename='integrals.dat'):
         """
         Write the integrals in a file named filename.
         -------
@@ -987,15 +1092,15 @@
         """
         Plots the real part of the spectrum.
         -------
         Parameters:
         - Neg: bool
             Plot (True) or not (False) the negative contours.
         - lvl0: float
-            Starting contour value.
+            Starting contour value with respect to the maximum of the spectrum
         """
         warnings.filterwarnings("ignore", message="No contour levels were found within the data range.")
         # Plots data, set Neg=True to see negative contours
         S = self.rr
         n_xticks, n_yticks = 10, 10
 
         X_label = '$\delta\ $'+misc.nuc_format(self.acqus['nuc2'])+' /ppm'
@@ -1087,76 +1192,97 @@
         plt.close()
 
 
 class pSpectrum_2D(Spectrum_2D):
     """
     Subclass of Spectrum_2D that allows to handle processed 2D NMR spectra.
     Reads the processed spectrum from Bruker.
+    ---------
+    Attributes:
+    - datadir: str
+        Path to the input file/dataset directory
+    - acqus: dict
+        Dictionary of acqusition parameters
+    - ngdic: dict
+        Generated by nmrglue.bruker.read, contains all the information on the spectrometer and on the spectrum.
+    - procs: dict
+        Dictionary of processing parameters
+    - S: 2darray
+        Complex (or hypercomplex, depending on FnMODE) spectrum
+    - rr: 2darray
+        Real part F2, real part F1
+    - ii: 2darray
+        Imaginary part F2, imaginary part F1
+    - ir: 2darray
+        Real part F2, imaginary part F1. Only exist if F1 is acquired in phase-sensitive mode
+    - ri: 2darray
+        Imaginary part F2, real part F1. Only exist if F1 is acquired in phase-sensitive mode
+    - freq_f1: 1darray
+        Frequency scale of the indirect dimension, in Hz
+    - freq_f2: 1darray
+        Frequency scale of the direct dimension, in Hz
+    - ppm_f1: 1darray
+        ppm scale of the indirect dimension
+    - ppm_f2: 1darray
+        ppm scale of the direct dimension
+    - trf1: dict
+        Projections of the indirect dimension, as 1darrays. Keys: 'ppm_f2' where they were taken
+    - trf2: dict
+        Projections of the direct dimension, as 1darrays. Keys: 'ppm_f1' where they were taken
+    - Trf1: dict
+        Projections of the indirect dimension, as pSpectrum_1D objects. Keys: 'ppm_f2' where they were taken
+    - Trf2: dict
+        Projections of the direct dimension, as pSpectrum_1D objects. Keys: 'ppm_f1' where they were taken
+    - integrals: dict
+        Dictionary where to save the regions and values of the integrals.
     """
 
     def __init__(self, in_file):
         """
         Initialize the class. 
         -------
         Parameters:
         - in_file: str
             Path to the spectrum. Here, the 'pdata/#' folder must be specified.
         """
+        self.datadir = in_file
         if in_file[-1] != '/':
             in_file = in_file+'/'
-        warnings.filterwarnings("ignore")
         dic, data = ng.bruker.read(in_file.split('pdata')[0], cplex=True)
         _, self.rr = ng.bruker.read_pdata(in_file, bin_files=['2rr'])
         _, self.ii = ng.bruker.read_pdata(in_file, bin_files=['2ii'])
         if os.path.exists(in_file+'2ir') and os.path.exists(in_file+'2ri'):
             _, self.ir = ng.bruker.read_pdata(in_file, bin_files=['2ir'])
             _, self.ri = ng.bruker.read_pdata(in_file, bin_files=['2ri'])
             self.S = processing.repack_2D(self.rr, self.ir, self.ri, self.ii)
         else:
             self.ir = np.array(np.copy(self.rr))
             self.ri = np.copy(self.ii)
             self.S = self.rr + 1j*self.ii
 
         self.acqus = misc.makeacqus_2D(dic)
-        self.BYTORDA = dic['acqus']['BYTORDA']
-        self.DTYPA = dic['acqus']['DTYPA']
+        self.acqus['BYTORDA'] = dic['acqus']['BYTORDA']
+        self.acqus['DTYPA'] = dic['acqus']['DTYPA']
         self.ngdic = dic
         del dic
         del data
 
         try:
-            self.grpdly = int(self.ngdic['acqus']['GRPDLY'])
+            self.acqus['GRPDLY'] = int(self.ngdic['acqus']['GRPDLY'])
         except:
-            self.grpdly = 0
+            self.acqus['GRPDLY'] = 0
 
         # initialize the procs dictionary with default values
-        wf1 = {
-                'mode':None,
-                'ssb':2,
-                'lb':5,
-                'gb':10,
-                'gc':0,
-                'sw':None
-                }
-        wf2 = {
-                'mode':None,
-                'ssb':2,
-                'lb':5,
-                'gb':10,
-                'gc':0,
-                'sw':None
-                }
         proc_init_2D = (
-                [wf1, wf2],     # window function
+                [dict(wf0), dict(wf0)],     # window function
                 [None, None],   # zero-fill
                 [0.5, 0.5],     # fcor
                 [0,0]           # tdeff
                 )
 
-        proc_keys_1D = ['wf', 'zf', 'fcor', 'tdeff']
         self.procs = {}
         for k, key in enumerate(proc_keys_1D):
             self.procs[key] = proc_init_2D[k]         # Processing parameters
         self.procs['wf'][0]['sw'] = round(self.acqus['SW1'], 4)
         self.procs['wf'][1]['sw'] = round(self.acqus['SW2'], 4)
 
         # Then, phases
@@ -1180,20 +1306,19 @@
 
         # Create empty dictionary where to save the projections
         self.trf1 = {}
         self.trf2 = {}
         self.Trf1 = {}
         self.Trf2 = {}
 
-    def write_ser(self):
-        """Overwrite the original function to prevent writing of the binary file. It does nothing!"""
-        pass
-
 class Pseudo_2D(Spectrum_2D):
-    """ Pseudo_2D experiment """
+    """ 
+    Subclass of Spectrum_2D to simulate and handle pseudo-2D experiments.
+
+    """
 
     def __str__(self):
         doc = '-'*64
         doc += '\nPseudo_2D object.\n'
         if 'ngdic' in self.__dict__.keys():
             doc += f'Read from "{self.datadir}"\n'
         else:
@@ -1212,63 +1337,53 @@
         Initialize the class. 
         -------
         Parameters:
         - in_file: str
             path to file to read, or to the folder of the spectrum
         - fid: 2darray or None
             Array that replaces self.fid.
-        - isexp: bool
-            True if this is an experimental dataset, False if it is simulated
         - pv: bool
             True if you want to use pseudo-voigt lineshapes for simulation, False for Voigt
+        - isexp: bool
+            True if this is an experimental dataset, False if it is simulated
         """
         self.datadir = in_file
         if isexp is False:
             self.acqus = sim.load_sim_1D(in_file)
             self.fid = fid
         else:
             dic, data = ng.bruker.read(in_file, cplex=True)
             self.fid = data
             self.acqus = misc.makeacqus_1D(dic)
-            self.BYTORDA = dic['acqus']['BYTORDA']
-            self.DTYPA = dic['acqus']['DTYPA']
+            self.acqus['BYTORDA'] = dic['acqus']['BYTORDA']
+            self.acqus['DTYPA'] = dic['acqus']['DTYPA']
             self.ngdic = dic
             del dic
             del data
 
         try:
-            self.grpdly = int(self.ngdic['acqus']['GRPDLY'])
+            self.acqus['GRPDLY'] = int(self.ngdic['acqus']['GRPDLY'])
         except:
-            self.grpdly = 0
+            self.acqus['GRPDLY'] = 0
 
         # Initalize the procs dictionary with default values
-        proc_keys_1D = ['wf', 'zf', 'fcor', 'tdeff']
-        wf0 = {
-                'mode':None,
-                'ssb':2,
-                'lb':5,
-                'gb':10,
-                'gc':0,
-                'sw':None
-                }
-        proc_init_1D = (wf0, None, 0.5, 0)
+        proc_init_1D = (dict(wf0), None, 0.5, 0)
 
-        self.procs = {
-                }
+        self.procs = {}
         for k, key in enumerate(proc_keys_1D):
             self.procs[key] = proc_init_1D[k]         # Processing parameters
         self.procs['wf']['sw'] = round(self.acqus['SW'], 4)
         # Then, phases
         self.procs['p0'] = 0
         self.procs['p1'] = 0
         self.procs['pv'] = round(self.acqus['o1p'], 2)
 
     def convdta(self, scaling=1):
         """ Calls processing.convdta """
-        self.fid = processing.convdta(self.fid, self.grpdly, scaling)
+        self.fid = processing.convdta(self.fid, self.acqus['GRPDLY'], scaling)
         
     def process(self):
         """
         Process only the direct dimension.
         Calls processing.fp on each transient
         """
         if self.procs['zf'] is None:
@@ -1304,15 +1419,15 @@
 
     def adjph(self, expno=0, p0=None, p1=None, pv=None):
         """
         Adjusts the phases of the spectrum according to the given parameters, or interactively if they are left as default.
         -------
         Parameters:
         - expno: int
-            Number of the experiment (python numbering) to use in the interactive panel
+            Index of the experiment (python numbering) to use in the interactive panel
         - p0: float or None
             0-th order phase correction /°
         - p1: float or None
             1-st order phase correction /°
         - pv: float or None
             1-st order pivot /ppm
         """
@@ -1325,31 +1440,31 @@
         self.ii = self.S.imag
 
         self.procs['p0'] += round(values[0], 2)
         self.procs['p1'] += round(values[1], 2)
         if values[2] is not None:
             self.procs['pv'] = round(values[2], 5)
 
-
     def projf1(self, a, b=None):
         """
         Calculates the sum trace of the indirect dimension, from a to b in F2.
         Store the trace in the dictionary trf1 and as 1D spectrum in Trf1. The key is 'a' or 'a:b'
+        Updates the Trf1[label].freq and Trf1[label].ppm with self.freq_f1 and self.ppm_f1 respectively.
         -------
         Parameters:
         - a: float
             ppm F2 value where to extract the trace.
         - b: float or None.
             If it is None, extract the trace in a. Else, sum from a to b in F2.
         """
         # make dictionary label
         if b is None:
-            label = str(a)
+            label = f'{a:.2f}'
         else:
-            label = str(a)+':'+str(b)
+            label = f'{a:.2f}:{b:.2f}'
         f1 = misc.get_trace(self.rr, self.ppm_f2, self.ppm_f1, a, b, column=True)
         self.trf1[label] = f1
         self.Trf1[label] = pSpectrum_1D(f1, acqus=self.acqus, procs=self.procs, istrace=True)
         self.Trf1[label].freq = np.copy(self.freq_f1)
         self.Trf1[label].ppm = np.copy(self.ppm_f1)
 
     def projf2(self, a, b=None):
@@ -1361,30 +1476,32 @@
         - a: float
             ppm F1 value where to extract the trace.
         - b: float or None.
             If it is None, extract the trace in a. Else, sum from a to b in F1.
         """
         # make dictionary label
         if b is None:
-            label = str(a)
+            label = f'{a:.2f}'
         else:
-            label = str(a)+':'+str(b)
+            label = f'{a:.2f}:{b:.2f}'
         f2 = misc.get_trace(self.rr, self.ppm_f2, self.ppm_f1, a, b, column=False)
         self.trf2[label] = f2
         self.Trf2[label] = pSpectrum_1D(f2, acqus=self.acqus, procs=self.procs, istrace=True)
 
     def plot(self, Neg=True, lvl0=0.2, Y_label=''):
         """
         Plots the real part of the spectrum.
         -------
         Parameters:
         - Neg: bool
             Plot (True) or not (False) the negative contours.
         - lvl0: float
             Starting contour value.
+        - Y_label: str
+            Custom label for vertical axis.
         """
         warnings.filterwarnings("ignore", message="No contour levels were found within the data range.")
         # Plots data, set Neg=True to see negative contours
         S = np.copy(self.rr)
         n_xticks, n_yticks = 10, 10
 
         X_label = '$\delta\ $'+misc.nuc_format(self.acqus['nuc'])+' /ppm'
@@ -1528,15 +1645,16 @@
                 labels=[f'{w}' for w in which_exp])
 
 
     def integrate(self, which=0, lims=None):
         """
         Integrate the spectrum with a dedicated GUI.
         Calls processing.integral on each experiment, then saves the results in self.integrals.
-        If lims is not given, calls fit.integrate to select the regions to integrate.
+        Therefore, the entries of self.integrals are sequences!
+        If lims is not given, calls fit.integrate on the trace to select the regions to integrate.
         --------
         Parameters:
         - which: int
             Experiment index to show in interactive panel
         - lims: tuple
             Region of the spectrum to integrate (ppm1, ppm2)
         """
@@ -1549,14 +1667,53 @@
                     self.integrals[key] = [processing.integral(self.rr[k], self.ppm_f2, lims)[-1] for k in range(self.rr.shape[0])]
                 else:
                     self.integrals[key] = np.array(integrals[key])
 
         else:
             self.integrals[f'{lims[0]:.2f}:{lims[1]:.2f}'] = np.array(processing.integral(self.rr, self.ppm_f2, lims)[...,-1])
 
+    def write_integrals(self, filename='integrals.dat'):
+        """
+        Write the integrals in a file named filename.
+        -------
+        Parameters:
+        - filename: str
+            name of the file where to write the integrals.
+        """
+        @staticmethod
+        def arr2string(array):
+            if isinstance(array, (np.ndarray, list, tuple)):
+                string = [f'{w:.4e}' for w in array]
+            else: 
+                string = [f'{array:.4e}']
+            return string
+
+        @staticmethod
+        def write_arr(f, string):
+            for w in string:
+                f.write(f'{w}, ')
+
+        f = open(filename, 'w')
+        for key, value in self.integrals.items():
+            f.write('{:12}\t'.format(key))
+            if 'total' in key:
+                write_arr(f, [value])
+                f.write('\n')
+            elif 'ref' in key:
+                if 'pos' in key:
+                    f.write('{}\n'.format(value))
+                elif 'int' in key:
+                    f.write('{:.4e}\n'.format(value))
+                elif 'val' in key:
+                    f.write('{:.3f}\n'.format(value))
+            else:
+                write_arr(f, arr2string(value))
+                f.write('\n')
+        f.close()
+
```

### Comparing `klassez-0.1a1/klassez/__init__.py` & `klassez-0.1a2/klassez/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 import matplotlib.cm as cm
 import seaborn as sns
 from pprint import pprint as Print 
 
 from . import fit, misc, sim, figures, processing
 from .Spectra import Spectrum_1D, pSpectrum_1D, Spectrum_2D, pSpectrum_2D, Pseudo_2D
 
-__version__ = '0.1a.1'
+__version__ = '0.1a.2'
 
 # Use seaborn's colormaps and save it to a dictionary
-from .config import CM, COLORS
+from .config import CM, COLORS, cron
 
 def open_doc():
     """ Open the documentation .pdf file in the browser. """
     import webbrowser
     webbrowser.open_new(__doc__)
 
 __doc__ = f'{__path__[0]}/docs/klassez.pdf'
```

### Comparing `klassez-0.1a1/klassez/config.py` & `klassez-0.1a2/klassez/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 #! /usr/bin/env python3
 
 import seaborn as sns
+from datetime import datetime
+
+
+def cron(func, *args, **kwargs):
+    """ Decorator: use it to monitor the runtime of a function.  """
+    def new_func(*args, **kwargs):
+        #print(f'\nFunction "{func.__name__}" was called.')
+        start_time = datetime.now()
+
+        return_values = func(*args, **kwargs)
+
+        end_time = datetime.now()
+        run_time = end_time - start_time
+        print(f'Runtime: {run_time}\n')
+        return return_values
+    return new_func
 
 
 # Use seaborn's colormaps and save it to a dictionary
 CMapsNames = ['Accent', 'Accent_r', 'Blues', 'Blues_r', 'BrBG', 'BrBG_r', 'BuGn', 'BuGn_r', 'BuPu', 'BuPu_r', 'CMRmap', 'CMRmap_r', 'Dark2', 'Dark2_r', 'GnBu', 'GnBu_r', 'Greens', 'Greens_r', 'Greys', 'Greys_r', 'OrRd', 'OrRd_r', 'Oranges', 'Oranges_r', 'PRGn', 'PRGn_r', 'Paired', 'Paired_r', 'Pastel1', 'Pastel1_r', 'Pastel2', 'Pastel2_r', 'PiYG', 'PiYG_r', 'PuBu', 'PuBuGn', 'PuBuGn_r', 'PuBu_r', 'PuOr', 'PuOr_r', 'PuRd', 'PuRd_r', 'Purples', 'Purples_r', 'RdBu', 'RdBu_r', 'RdGy', 'RdGy_r', 'RdPu', 'RdPu_r', 'RdYlBu', 'RdYlBu_r', 'RdYlGn', 'RdYlGn_r', 'Reds', 'Reds_r', 'Set1', 'Set1_r', 'Set2', 'Set2_r', 'Set3', 'Set3_r', 'Spectral', 'Spectral_r', 'Wistia', 'Wistia_r', 'YlGn', 'YlGnBu', 'YlGnBu_r', 'YlGn_r', 'YlOrBr', 'YlOrBr_r', 'YlOrRd', 'YlOrRd_r', 'afmhot', 'afmhot_r', 'autumn', 'autumn_r', 'binary', 'binary_r', 'bone', 'bone_r', 'brg', 'brg_r', 'bwr', 'bwr_r', 'cividis', 'cividis_r', 'cool', 'cool_r', 'coolwarm', 'coolwarm_r', 'copper', 'copper_r', 'cubehelix', 'cubehelix_r', 'flag', 'flag_r', 'gist_earth', 'gist_earth_r', 'gist_gray', 'gist_gray_r', 'gist_heat', 'gist_heat_r', 'gist_ncar', 'gist_ncar_r', 'gist_rainbow', 'gist_rainbow_r', 'gist_stern', 'gist_stern_r', 'gist_yarg', 'gist_yarg_r', 'gnuplot', 'gnuplot2', 'gnuplot2_r', 'gnuplot_r', 'gray', 'gray_r', 'hot', 'hot_r', 'hsv', 'hsv_r', 'icefire', 'icefire_r', 'inferno', 'inferno_r', 'magma', 'magma_r', 'mako', 'mako_r', 'nipy_spectral', 'nipy_spectral_r', 'ocean', 'ocean_r', 'pink', 'pink_r', 'plasma', 'plasma_r', 'prism', 'prism_r', 'rainbow', 'rainbow_r', 'rocket', 'rocket_r', 'seismic', 'seismic_r', 'spring', 'spring_r', 'summer', 'summer_r', 'tab10', 'tab10_r', 'tab20', 'tab20_r', 'tab20b', 'tab20b_r', 'tab20c', 'tab20c_r', 'terrain', 'terrain_r', 'twilight', 'twilight_r', 'twilight_shifted', 'twilight_shifted_r', 'viridis', 'viridis_r', 'vlag', 'vlag_r', 'winter', 'winter_r']
 
 global CM, COLORS
 CM = {}
```

### Comparing `klassez-0.1a1/klassez/docs/klassez.pdf` & `klassez-0.1a2/klassez/docs/klassez.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 10% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,14 +1,14 @@
 Author:
 Francesco Bruno
 Major contributors:
 Letizia Fiorucci
-Version: 0.1a.1
+Version: 0.1a.2
 Documentation release date:
-February 21, 2023
+April 19, 2023
 
 i
 
 ii
 
 Contents
 1
@@ -42,19 +42,19 @@
 
 1
 2
 2
 2
 3
 5
-5
+6
 7
 8
 8
-9
+10
 11
 13
 
 MISC package . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 13
 
 3.1.1 misc.SNR . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.1.2 misc.SNR_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
@@ -65,26 +65,26 @@
 3.1.7 misc.edit_checkboxes . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.1.8 misc.find_nearest . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.1.9 misc.freq2ppm . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.1.10 misc.get_trace . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.1.11 misc.get_ylim . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.1.12 misc.hankel . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.1.13 misc.hz2pt . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.14 misc.makeacqus_1D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.15 misc.makeacqus_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.16 misc.mathformat . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.17 misc.molfrac . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.18 misc.noise_std . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.19 misc.nuc_format . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.20 misc.polyn . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.21 misc.ppm2freq . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.22 misc.ppmfind . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.23 misc.pretty_scale . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.24 misc.print_dict . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.25 misc.print_list . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.14 misc.in2px . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.15 misc.makeacqus_1D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.16 misc.makeacqus_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.17 misc.mathformat . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.18 misc.molfrac . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.19 misc.noise_std . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.20 misc.nuc_format . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.21 misc.polyn . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.22 misc.ppm2freq . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.23 misc.ppmfind . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.24 misc.pretty_scale . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.25 misc.print_dict . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 13
 14
 15
 16
 17
 18
@@ -108,29 +108,32 @@
 36
 37
 
 iii
 
 3.2
 
-3.1.26 misc.procpar . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.27 misc.readlistfile . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.28 misc.select_for_integration . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.29 misc.select_traces . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.30 misc.set_fontsizes . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.31 misc.set_ylim . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.32 misc.show_cmap . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.33 misc.split_acqus_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.34 misc.split_procs_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.35 misc.trim_data . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.36 misc.unhankel . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.37 misc.write_acqus_1D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.38 misc.write_acqus_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.39 misc.write_help . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.1.40 misc.write_ser . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.26 misc.print_list . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.27 misc.procpar . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.28 misc.px2in . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.29 misc.readlistfile . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.30 misc.select_for_integration . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.31 misc.select_traces . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.32 misc.set_fontsizes . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.33 misc.set_ylim . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.34 misc.show_cmap . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.35 misc.split_acqus_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.36 misc.split_procs_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.37 misc.trim_data . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.38 misc.trim_data_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.39 misc.unhankel . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.40 misc.write_acqus_1D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.41 misc.write_acqus_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.42 misc.write_help . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.1.43 misc.write_ser . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 38
 39
 40
 41
 42
 43
@@ -139,14 +142,17 @@
 46
 47
 48
 49
 50
 51
 52
+53
+54
+55
 
 . . . . . . . . . . . . . . . . . . . . . . . . .
 3.2.1 processing.Cadzow . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.2.2 processing.Cadzow_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.2.3 processing.EAE . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.2.4 processing.LRD . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.2.5 processing.MCR . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
@@ -162,33 +168,27 @@
 3.2.15 processing.ft . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.2.16 processing.gm . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.2.17 processing.gmb . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.2.18 processing.ift . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.2.19 processing.integral . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.2.20 processing.integral_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 3.2.21 processing.interactive_basl_windows . . . . . . . . . . . . . . . . . . . . . . .
-3.2.22 processing.interactive_fp . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.2.23 processing.interactive_phase_1D . . . . . . . . . . . . . . . . . . . . . . . . .
-3.2.24 processing.interactive_phase_2D . . . . . . . . . . . . . . . . . . . . . . . . .
-3.2.25 processing.interactive_qfil . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.2.26 processing.interactive_xfb . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.2.27 processing.inv_fp . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.2.28 processing.inv_xfb . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.2.29 processing.iterCadzow . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.2.30 processing.load_baseline . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.2.31 processing.make_polynomion_baseline . . . . . . . . . . . . . . . . . . . . . .
-3.2.32 processing.make_scale . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.2.33 processing.pknl . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.2.34 processing.ps . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-3.2.35 processing.qfil . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.2.22 processing.interactive_echo_param . . . . . . . . . . . . . . . . . . . . . . . .
+3.2.23 processing.interactive_fp . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.2.24 processing.interactive_phase_1D . . . . . . . . . . . . . . . . . . . . . . . . .
+3.2.25 processing.interactive_phase_2D . . . . . . . . . . . . . . . . . . . . . . . . .
+3.2.26 processing.interactive_qfil . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.2.27 processing.interactive_xfb . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.2.28 processing.inv_fp . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.2.29 processing.inv_xfb . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.2.30 processing.iterCadzow . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.2.31 processing.load_baseline . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.2.32 processing.make_polynomion_baseline . . . . . . . . . . . . . . . . . . . . . .
 
-53
-53
-54
-55
+56
 56
 57
 58
 59
 60
 61
 62
@@ -217,116 +217,130 @@
 85
 86
 87
 
 PROCESSING package
 
 iv
-3.2.36 processing.qpol . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 88
-3.2.37 processing.qsin . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 89
-3.2.38 processing.quad . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 90
-3.2.39 processing.repack_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 91
-3.2.40 processing.rev . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 92
-3.2.41 processing.sin . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 93
-3.2.42 processing.split_echo_train . . . . . . . . . . . . . . . . . . . . . . . . . . . . 94
-3.2.43 processing.stack_MCR . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 95
-3.2.44 processing.sum_echo_train . . . . . . . . . . . . . . . . . . . . . . . . . . . . 96
-3.2.45 processing.tabula_rasa . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 97
-3.2.46 processing.td_eff . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 98
-3.2.47 processing.tp_hyper . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 99
-3.2.48 processing.unpack_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 100
-3.2.49 processing.write_basl_info . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 101
-3.2.50 processing.xfb . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 102
-3.2.51 processing.zf . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 103
+3.2.33 processing.make_scale . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 88
+3.2.34 processing.new_MCR . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 89
+3.2.35 processing.new_MCR_ALS . . . . . . . . . . . . . . . . . . . . . . . . . . . . 90
+3.2.36 processing.pknl . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 91
+3.2.37 processing.ps . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 92
+3.2.38 processing.qfil . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 93
+3.2.39 processing.qpol . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 94
+3.2.40 processing.qsin . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 95
+3.2.41 processing.quad . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 96
+3.2.42 processing.repack_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 97
+3.2.43 processing.rev . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 98
+3.2.44 processing.sin . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 99
+3.2.45 processing.split_echo_train . . . . . . . . . . . . . . . . . . . . . . . . . . . . 100
+3.2.46 processing.stack_MCR . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 101
+3.2.47 processing.sum_echo_train . . . . . . . . . . . . . . . . . . . . . . . . . . . . 102
+3.2.48 processing.tabula_rasa . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 103
+3.2.49 processing.td_eff . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 104
+3.2.50 processing.tp_hyper . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 105
+3.2.51 processing.unpack_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 106
+3.2.52 processing.write_basl_info . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 107
+3.2.53 processing.xfb . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 108
+3.2.54 processing.zf . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 109
 3.3
 
 3.4
 
-FIGURES package . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 104
+FIGURES package . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 110
 
-3.3.1 figures.ax1D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 104
-3.3.2 figures.ax2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 106
-3.3.3 figures.ax_heatmap . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 108
-3.3.4 figures.dotmd . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 109
-3.3.5 figures.dotmd_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 110
-3.3.6 figures.figure1D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 111
-3.3.7 figures.figure1D_multi . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 112
-3.3.8 figures.figure2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 113
-3.3.9 figures.figure2D_multi . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 115
-3.3.10 figures.fitfigure . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 116
-3.3.11 figures.heatmap . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 117
-3.3.12 figures.plot_fid . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 118
-3.3.13 figures.plot_fid_re . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 119
-3.3.14 figures.redraw_contours . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 120
-3.3.15 figures.sns_heatmap . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 121
-3.3.16 figures.stacked_plot . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 122
-
-SIM package . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 123
-
-3.4.1 sim.calc_splitting . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 123
-3.4.2 sim.f_gaussian . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 124
-3.4.3 sim.f_lorentzian . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 125
-3.4.4 sim.f_pvoigt . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 126
-3.4.5 sim.gaussian_filter . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 127
-3.4.6 sim.load_sim_1D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 128
-3.4.7 sim.load_sim_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 129
-3.4.8 sim.multiplet . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 130
-3.4.9 sim.noisegen . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 131
-3.4.10 sim.sim_1D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 132
-3.4.11 sim.sim_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 133
-3.4.12 sim.t_2Dgaussian . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 134
-3.4.13 sim.t_2Dlorentzian . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 135
-3.4.14 sim.t_2Dpvoigt . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 137
-3.4.15 sim.t_2Dvoigt . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 138
-3.4.16 sim.t_gaussian . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 140
+3.3.1 figures.ax1D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 110
+3.3.2 figures.ax2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 112
+3.3.3 figures.ax_heatmap . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 114
+3.3.4 figures.dotmd . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 115
+3.3.5 figures.dotmd_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 116
+3.3.6 figures.figure1D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 117
+3.3.7 figures.figure1D_multi . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 118
+3.3.8 figures.figure2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 119
+3.3.9 figures.figure2D_multi . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 121
+3.3.10 figures.fitfigure . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 122
+3.3.11 figures.heatmap . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 123
+3.3.12 figures.plot_fid . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 124
+3.3.13 figures.plot_fid_re . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 125
+3.3.14 figures.redraw_contours . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 126
+3.3.15 figures.sns_heatmap . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 127
+3.3.16 figures.stacked_plot . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 128
+
+SIM package . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 129
+3.4.1 sim.calc_splitting . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 129
+3.4.2 sim.f_gaussian . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 130
+3.4.3 sim.f_lorentzian . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 131
+3.4.4 sim.f_pvoigt . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 132
+3.4.5 sim.gaussian_filter . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 133
+3.4.6 sim.load_sim_1D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 134
+3.4.7 sim.load_sim_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 135
+3.4.8 sim.mult_noise . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 136
+3.4.9 sim.multiplet . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 137
+3.4.10 sim.noisegen . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 138
 
 v
-3.4.17 sim.t_lorentzian . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 141
-3.4.18 sim.t_pvoigt . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 142
-3.4.19 sim.t_voigt . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 143
-3.4.20 sim.water7 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 144
+3.4.11 sim.sim_1D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 139
+3.4.12 sim.sim_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 140
+3.4.13 sim.t_2Dgaussian . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 141
+3.4.14 sim.t_2Dlorentzian . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 142
+3.4.15 sim.t_2Dpvoigt . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 144
+3.4.16 sim.t_2Dvoigt . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 145
+3.4.17 sim.t_gaussian . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 147
+3.4.18 sim.t_lorentzian . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 148
+3.4.19 sim.t_pvoigt . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 149
+3.4.20 sim.t_voigt . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 150
+3.4.21 sim.water7 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 151
 3.5
 
-FIT package . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 145
+FIT package . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 152
 
 3.6
 
-SPECTRA package . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 170
-
-3.5.1 fit.Voigt_Fit
-class . . . . . . . . . . . . . . . . 145
-3.5.2 fit.ax_histogram . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 147
-3.5.3 fit.bin_data . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 148
-3.5.4 fit.build_baseline . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 149
-3.5.5 fit.calc_fit_lines . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 150
-3.5.6 fit.dic2mat . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 151
-3.5.7 fit.fit_int . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 152
-3.5.8 fit.gaussian_fit . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 153
-3.5.9 fit.gen_iguess . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 154
-3.5.10 fit.get_region . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 155
-3.5.11 fit.histogram . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 156
-3.5.12 fit.integrate . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 157
-3.5.13 fit.integrate_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 158
-3.5.14 fit.interactive_smoothing . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 159
-3.5.15 fit.join_par . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 160
-3.5.16 fit.make_iguess . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 161
-3.5.17 fit.make_signal . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 162
-3.5.18 fit.print_par . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 163
-3.5.19 fit.read_par . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 164
-3.5.20 fit.smooth_spl . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 165
-3.5.21 fit.test_residuals . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 166
-3.5.22 fit.voigt_fit . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 167
-3.5.23 fit.write_log . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 168
-3.5.24 fit.write_par . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 169
+SPECTRA package . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 184
 
+3.5.1 fit.Voigt_Fit . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 152
+3.5.2 fit.ax_histogram . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 155
+3.5.3 fit.bin_data . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 156
+3.5.4 fit.build_2D_sgn . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 157
+3.5.5 fit.build_baseline . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 158
+3.5.6 fit.calc_fit_lines . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 159
+3.5.7 fit.dic2mat . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 160
+3.5.8 fit.fit_int . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 161
+3.5.9 fit.gaussian_fit . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 162
+3.5.10 fit.gen_iguess . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 163
+3.5.11 fit.gen_iguess_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 164
+3.5.12 fit.get_region . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 166
+3.5.13 fit.histogram . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 167
+3.5.14 fit.integrate . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 168
+3.5.15 fit.integrate_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 169
+3.5.16 fit.interactive_smoothing . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 170
+3.5.17 fit.join_par . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 171
+3.5.18 fit.make_iguess . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 172
+3.5.19 fit.make_signal . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 173
+3.5.20 fit.peak_pick . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 174
+3.5.21 fit.print_par . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 175
+3.5.22 fit.read_par . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 176
+3.5.23 fit.smooth_spl . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 177
+3.5.24 fit.test_residuals . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 178
+3.5.25 fit.voigt_fit . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 179
+3.5.26 fit.voigt_fit_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 180
+3.5.27 fit.write_log . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 182
+3.5.28 fit.write_par . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 183
 3.6.1
 3.6.2
-
-Spectrum_1D important attributes . . . . . . . . . . . . . . . . . . . . . . . . 170
-Spectrum_2D important attributes . . . . . . . . . . . . . . . . . . . . . . . . 171
+3.6.3
+3.6.4
+3.6.5
+
+Spectra.Pseudo_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 184
+Spectra.Spectrum_1D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 190
+Spectra.Spectrum_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 194
+Spectra.pSpectrum_1D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 200
+Spectra.pSpectrum_2D . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 204
 
 vi
 
 1
 
 1. Introduction
 KLASSEZ is a python package written to handle 1D and 2D NMR data. The aim of the project is
@@ -410,14 +424,20 @@
 best for GUIs and withstand font sizes of about 14 pt.
 For NMR: the variable sim.gamma is a dictionary containing the gyromagnetic ratio, in MHz/T,
 of all the magnetically-active nuclei. For instance:
 print(sim.gamma[’13C’])
 >>> 10.70611
 
 3
+A decorator function called cron is defined in the top-level script config, and imported by
+__init__, so that you can use it after writing:
+from klassez import cron
+
+This decorator allows to measure the runtime of a function, and print it on standard output once it
+ended.
 
 2.2
 
 Processing of a 'raw' 1D spectrum
 
 Let us say that your spectrum is saved in the folder /home/myself/spectra/mydataset/1/. Initialize
 the spectrum object through:
@@ -436,53 +456,45 @@
 on the version of TopSpin that the spectrometer ran and several other construction parameters.
 Therefore, if you see a residual of the digital filter in you spectrum, the easiest solution is to run
 CONVDTA inside TopSpin.
 A detailed description of acqus and procs is shown in table 2.1 and table 2.2.
 Table 2.1: Description of the acqus dictionary of a Spectrum_1D object.
 
 Key
-
-Explanation
-
 B0
+BYTORDA
+DTYPA
+GRPDLY
 nuc
 o1p
 o1
 SWp
 SW
 SFO1
 TD
 dw
 AQ
 t1
 
+Explanation
 Magnetic field strength /T
+Endianness of binary data: 0 little endian, 1 big endian
+Binary data type: 0 int32, 2 float64
+Number of points of the digital filter
 Observed nucleus
 Carrier frequency i.e. center of the spectrum, in ppm
 Same as o1p, but in Hz
 Sweep width, in ppm
 Sweep width, in Hz
 Larmor frequency of the observed nucleus at field B0
 Number of sampled complex points
 Dwell time, i.e. the sampling interval, in seconds
 Time duration of the FID
 Acquisition timescale
 
-To make the Fourier transform of the FID to obtain the spectrum, you must invoke the process
-method, which reads the procs dictionary to get the instructions on the processing you want to
-make on your spectrum. For instance, if you want to obtain a final spectrum of 8k points with an
-exponential broadening of 25 Hz:
-s.procs["wf"]["mode"] = "em"
-s.procs["wf"]["lb"] = 25
-s.procs["zf"] = 8192
-s.process()
-
-Calling the process method generates new attributes of the class:
-• freq: the frequency scale, in Hz;
-
 4
 Table 2.2: Description of the procs dictionary of a Spectrum_1D object.
 
 Key
 
 Explanation
 
@@ -515,33 +527,44 @@
 Zero-filling. Set the final number of points!
 Number of points to be used for processing
 Scaling factor for the first point of the FID before Fourier transform
 Frequency-independent phase correction /degrees
 First order phase correction /degrees
 Pivot point for the first order phase correction /ppm
 
+To make the Fourier transform of the FID to obtain the spectrum, you must invoke the process
+method, which reads the procs dictionary to get the instructions on the processing you want to
+make on your spectrum. For instance, if you want to obtain a final spectrum of 8k points with an
+exponential broadening of 25 Hz:
+s.procs["wf"]["mode"] = "em"
+s.procs["wf"]["lb"] = 25
+s.procs["zf"] = 8192
+s.process()
+
+Calling the process method generates new attributes of the class:
+• freq: the frequency scale, in Hz;
 • ppm: the ppm scale;
 • r: the real part of the spectrum;
 • i: the imaginary part of the spectrum;
 • S: the complex spectrum (S = r + ii).
 If the spectrum requires phase correction, you can perform it interactively:
+
+5
+
 s.adjph()
 
 or by passing the phase angles, in degrees, to adjph. Example, if you know you need to phase your
 spectrum with 30 degrees of ϕ(0) and −55 degrees of ϕ(1) with the pivot set at 7.32 ppm:
 s.adjph(p0=30, p1=-55, pv=7.32)
 
 In both cases, the phase angles are updated in the procs dictionary.
 The spectrum can be calibrated using a dedicated GUI:
 s.cal()
 
 or specifying the shift value in ppm or in Hz (in this case, be sure to set the isHz keyword to True).
-
-5
-
 s.cal(-3)
 # Shift of -3 ppm
 s.cal(1000, isHz=True) # Shift of +1 kHz
 
 Both ppm and freq are updated according to the given values.
 A tool for baseline correction and lineshape fitting are also provided:
 s.basl()
@@ -577,40 +600,36 @@
 
 The class Spectrum_1D does not work if you want to read the processed data directly from TopSpin
 (or whatever software you used to acquire and process them). Instead, you should use the class
 pSpectrum_1D, which is designed to perform exactly this task. It inherits most of the attributes and
 methods of the Spectrum_1D class, therefore its usage closely resembles the example reported in the
 previous section.
 
+6
+
 2.3
 
 Processing of a 'raw' 2D spectrum
 
 Let us say that your spectrum is saved in the folder /home/myself/spectra/mydataset/21/. Initialize
 the spectrum object through:
 Path = "/home/myself/spectra/mydataset/21/"
 s = Spectrum_2D(Path)
 
 The generated acqus and procs dictionaries include informations on both dimensions.
-Then, the sequence of commands resembles the ones of the 1D spectra.
-s.convdta()
-s.process()
-s.adjph()
-s.plot()
-
-# If there is the digital filter
-
-6
 Table 2.3: Description of the acqus dictionary of a Spectrum_2D object.
 
 Key
 
 Explanation
 
 B0
+BYTORDA
+DTYPA
+GRPDLY
 nuc1
 nuc2
 o1p
 o2p
 o1
 o2
 SW1p
@@ -625,14 +644,17 @@
 dw2
 AQ1
 AQ2
 t1
 t2
 
 Magnetic field strength /T
+Endianness of binary data: 0 little endian, 1 big endian
+Binary data type: 0 int32, 2 float64
+Number of points of the digital filter
 Observed nucleus in the indirect dimension
 Observed nucleus in the direct dimension
 Carrier frequency i.e. center of the indirect dimension, in ppm
 Carrier frequency i.e. center of the direct dimension, in ppm
 Same as o1p, but in Hz
 Same as o2p, but in Hz
 Sweep width of the indirect dimension, in ppm
@@ -646,25 +668,35 @@
 t1 increments, in seconds
 Dwell time, i.e. the sampling interval, in seconds
 Sampled timescale of the indirect dimension
 Time duration of the FID
 Evolution timescale
 Acquisition timescale
 
+Then, the sequence of commands resembles the ones of the 1D spectra.
+s.convdta()
+s.process()
+s.adjph()
+s.plot()
+
+# If there is the digital filter
+
 The keys for adjph are of the kind: pXY, where X is the order of the phase correction (0 or 1) and Y
 is the dimension on which to apply it (1 or 2). Explicative table below:
 F1
 
 F2
 
-ϕ(0) p01 p02
-ϕ(1) p11 p12
-pivot pv1 pv2
-For further information, rely on the help python builtin function.
-To read the processed data, use the pSpectrum_2D class instead.
+ϕ(0) p01
+ϕ(1) p11
+pivot pv1
+
+p02
+p12
+pv2
 
 7
 Table 2.4: Description of the procs dictionary of a Spectrum_2D object. Each of these dictionary entry is a list of
 two elements: the first one (index 0) is the processing to apply on the indirect dimension, the second (index 1) on the
 direct dimension. For instance, procs[tdeff] = [64, 1024] means to truncate the indirect evolutions to 64 points
 and the FIDs to 1024 points.
 
@@ -692,43 +724,48 @@
 zf
 tdeff
 fcor
 p0
 p1
 pv
 
-2.3.1
-
 Automatically set according to
 
 Zero-filling. Set the final number of points!
 Number of points to be used for processing
 Scaling factor for the first point of the FID before Fourier transform
 Frequency-independent phase correction /degrees
 First order phase correction /degrees
 Pivot point for the first order phase correction /ppm
 
+For further information, rely on the help python builtin function.
+To read the processed data, use the pSpectrum_2D class instead.
+
+2.3.1
+
 Computing projections
 
 While the 2D spectra give an overall look on the whole experiment, the user might want to extract
 projection of the direct or the indirect dimension, to focus onto particular features in the spectrum.
 In order to do so, klassez offers two commands: projf1 and projf2, which compute the sum
 projections on the indirect or on the direct dimension, respectively, and store the result in dictionaries
 called trf1 and trf2, whose keys are the ppm values correspondant to the projections. Actually, the
 capitalized versions of the two dictionaries (with the same keys), i.e. Trf1 and Trf2, can be more
 useful, as they are instances of the pSpectrum_1D class and therefore are initialized with ppm scales
 and other parameters.
 Example:
 # Supposed to have a 1H-15N HSQC spectrum
-# Extract the direct dimension trace at 115 ppm, 15N scale
+#
+
+Extract the direct dimension trace at 115 ppm, 15N scale
+
+8
 s.projf2(115)
 # Access to it through
 Proj_115 = s.Trf2[’115’]
-
-8
 # Extract the indirect dimension trace from 6 to 8 ppm, 1H scale
 s.projf1(6, 8)
 Proj_indim = s.Trf1[’6:8’]
 # You can plot them:
 Proj_115.plot()
 Proj_indim.plot()
 
@@ -758,25 +795,26 @@
 • phases: phases of the peaks /degrees. Default: all zeros;
 • mult: fine structures of the peaks (e.g. doublets of triplets: dt). Default: all singlets;
 • Jconst: coupling constants of the fine structures /Hz. If more of one coupling is expected,
 provide them as a sequence. Default: not used as the peaks are all singlets.
 Key and value must be separated by a tab character. You are allowed to leave empty rows to
 improve the readibility and to insert comments using the # character.
 Example:
+
+9
+
 B0 16.4
 nuc 1H
 o1p 4.7
 SWp 40
 TD 8192
 
 # 700 MHz 1H
 
 shifts 1, 3, 5, 7
-
-9
 fwhm
 [10 for k in range(4)]
 amplitudes 10, 20, 15, 10
 x_g 0, 0.4, 0.6, 1
 phases 5, 0, 10, 0
 mult
 s, t, dt, ddd
@@ -789,24 +827,24 @@
 s = Spectrum_1D(’sim_in_1D’, isexp=False)
 s.process()
 figures.figure1D(s.ppm, s.r, name=’test_1D’, X_label=’$\delta\, ^1$H /ppm’,
 Y_label=’Intensity /a.u.’)
 
 Figure 2.1: Example of a simulated 1D spectrum.
 
+10
+
 2.4.2
 
 Simulate 2D data
 
 The same procedure can be followed to simulate 2D spectra. The input file to write is very similar
 to the one for 1D data, except for the quantities that clearly span over two dimensions. As in NMR
 textbook, the direct and indirect dimensions will be named F2 and F2 respectively, and dimensionspecific quantities will feature the 1 or 2 labels accordingly.
 • B0: Magnetic field strength /T;
-
-10
 • nuc1: Observed nucleus in F1(e.g. 13C);
 • nuc2: Observed nucleus in F2(e.g. 1H);
 • o1p: Carrier frequency i.e. centre of F1 /ppm;
 • o2p: Carrier frequency i.e. centre of F2 /ppm;
 • SW1p: Sweep width /ppm. The indirect dimension will cover the range [o1p − SW1p/2, o1p +
 SW1p/2];
 • SW2p: Sweep width /ppm. The direct dimension will cover the range [o2p − SW2p/2, o2p +
@@ -839,19 +877,17 @@
 shifts_f1 130.0, 105.0, 120.0, 1.25e2, 130.0, 105.0
 shifts_f2 0.0, 0.0, 4.0, 7.0, 1.1e1, 10.5
 fwhm_f1 100, 100, 100, 100, 100, 100
 fwhm_f2 50, 50, 50, 50, 50, 50
 amplitudes 10, 20, 10, 20, 10, 10
 x_g 0.0, 0.2, 0.4, 0.6, 0.8, 1.0
 
+11
 This input file generates the spectrum in Figure 2.2.
 Code:
-
-11
-
 #! /usr/bin/env python3
 from klassez import *
 s = Spectrum_2D(’sim_in_2D’, isexp=False)
 s.process()
 figures.figure2D(s.ppm_f2, s.ppm_f1, s.rr, lvl=0.005, name=’test_2D’, X_label=’$\delta\,
 ^1$H /ppm’, Y_label=’$\delta\, ^{15}$N /ppm’)
 
@@ -869,18 +905,19 @@
 Pseudo_2D is a subclass of Spectrum_2D; however, many functions have been adapted to resemble
 the 1D version.
 Pseudo_2D does not encode for a routine to automatically simulate data. If you want to, you
 should give a 1D-like input file (just like the one in section 2.4.1), and replace the attribute fid
 with your FID, generated as you wish. With a real dataset this is not required, as it is able to read
 everything automatically.
 path_to_pseudo = "/home/myself/spectra/mydataset/899/"
+
+12
 s = Pseudo_2D(path_to_pseudo)
 s.convdta() # If there is the digital filter
 
-12
 The process() function applies apodization, zero-filling and Fourier transform only on the direct dimension, reading the parameters from a procs dictionary like the one of Spectrum_1D. The
 attributes freq_f1 and ppm_f1 are initialized with np.arange(N ), where N is the number of experiments that your FID comprises of.
 The phase adjustment is performed on a reference spectrum, then applied on the whole 2D matrix.
 By default, the chosen spectrum is the first one, but you can choose the one that fits the most your
 needs.
 s.process()
 s.adjph(expno = 10) # Calls interactive_phase_1D on the 10th experiment
@@ -1153,60 +1190,74 @@
 • pt : float
 The frequency value converted in points
 
 26
 
 3.1.14
 
+misc.in2px(*in_args)
+
+Converts a sequence of numbers from inches to pixels by multiplying ×96.
+Parameters:
+• in_args: sequence of floats
+Values in inches to convert
+Returns:
+• px_args: tuple of ints
+Values in pixels
+
+27
+
+3.1.15
+
 misc.makeacqus_1D(dic)
 
 Given a NMRGLUE dictionary from a 1D spectrum (generated by ng.bruker.read), this function
 builds the acqus file with only the 'important' parameters.
 Parameters
 • dic : dict
 NMRglue dictionary returned by ng.bruker.read
 Returns
 • acqus : dict
 Dictionary with only few parameters
 
-27
+28
 
-3.1.15
+3.1.16
 
 misc.makeacqus_2D(dic)
 
 Given a NMRGLUE dictionary from a 2D spectrum (generated by ng.bruker.read), this function
 builds the acqus file with only the 'important' parameters.
 Parameters
 • dic : dict
 NMRglue dictionary returned by ng.bruker.read
 Returns
 • acqus : dict
 Dictionary with only few parameters
 
-28
+29
 
-3.1.16
+3.1.17
 
 misc.mathformat(ax, axis=’y’, limits=(-2,2))
 
 Apply exponential formatting to the given axis of the given figure panel. The offset text size is
 uniformed to the tick labels’ size.
 Parameters:
 • ax: matplotlib.Subplot Object
 Panel of the figure to edit
 • axis: str
 ’x’, ’y’ or ’both’.
 • limits: tuple
 tuple of ints that indicate the order of magnitude range outside which the exponential format
 is applied.
 
-29
+30
 
-3.1.17
+3.1.18
 
 misc.molfrac(n)
 
 Computes the 'molar fraction' x of the array n. Returns also the total amount.
 X
 ni
 N=
@@ -1219,17 +1270,17 @@
 list of values
 Returns
 • x: list or 1darray
 molar fraction array
 • N: float
 sum of all the elements in n
 
-30
+31
 
-3.1.18
+3.1.19
 
 misc.noise_std(y)
 
 Calculates the standard deviation of the noise using the Bruker formula. Taken y as an array of N
 points, and yi its i-th entry:
 v
 u N
@@ -1260,48 +1311,48 @@
 Parameters
 • y : 1darray
 The spectral region you would like to use to calculate the standard deviation of the noise.
 Returns
 • noisestd : float
 The standard deviation of the noise.
 
-31
+32
 
-3.1.19
+3.1.20
 
 misc.nuc_format(nuc)
 
 Converts the nuc key you may find in acqus in the formatted label, e.g. ’13C’ → ’$ˆ
 {13}$C’
 Parameters:
 • nuc: str
 Unformatted string
 Returns:
 • fnuc: str
 Formatted string.
 
-32
+33
 
-3.1.20
+3.1.21
 
 misc.polyn(x, c)
 
 Computes p(x), polynomion of degree n − 1, where n is the number of provided coefficients.
 Parameters
 • x : 1darray
 Scale upon which to build the polynomion
 • c : list or 1darray
 Sequence of the polynomion coeffiecient, starting from the 0-th order coefficient
 Returns
 • px : 1darray
 Polynomion of degree n − 1.
 
-33
+34
 
-3.1.21
+3.1.22
 
 misc.ppm2freq(x, B0=701.125, o1p=0)
 
 Converts x from ppm to Hz.
 Parameters
 • x : float
 Value to be converted
@@ -1309,17 +1360,17 @@
 Field frequency, in MHz. Default: 700 MHz
 • o1p : float
 Carrier frequency, in ppm. Default: 0.
 Returns
 • y : float
 The converted value
 
-34
+35
 
-3.1.22
+3.1.23
 
 misc.ppmfind(ppm_scale, value)
 
 Finds the exact value in ppm scale.
 Parameters
 • ppm_scale : 1darray
 Self-explanatory
@@ -1327,17 +1378,17 @@
 The value to be found
 Returns
 • I : int
 The index correspondant to V in ppm_scale
 • V : float
 The closest value to value in ppm_scale
 
-35
+36
 
-3.1.23
+3.1.24
 
 misc.pretty_scale(ax, limits, axis=’x’, n_major_ticks=10)
 
 This function computes a pretty scale for your plot. Calculates and sets a scale made of n_major_ticks
 numbered ticks, spaced by 5 * n_major_ticks unnumbered ticks. After that, the plot borders are
 trimmed according to the given limits.
 Parameters
@@ -1346,80 +1397,94 @@
 • limits: tuple
 limits to apply of the given axis. (left, right)
 • axis: str
 ’x’ for x-axis, ’y’ for y-axis
 • n_major_ticks: int
 Number of numbered ticks in the final scale. An oculated choice gives very pleasant results.
 
-36
+37
 
-3.1.24
+3.1.25
 
 misc.print_dict(mydict)
 
 Prints a dictionary one entry per row, in the format key:
 with an indentation
 Parameters:
 • mydict: dict
 The dictionary you want to print
 Returns:
 • outstring: str
 The printed text formatted as single string
 
 value. Nested dictionaries are printed
 
-37
+38
 
-3.1.25
+3.1.26
 
 misc.print_list(mylist)
 
 Prints a list, one entry per row.
 Parameters:
 • mylist: list
 The list you want to print
 Returns:
 • outstring: str
 The printed text formatted as single string
 
-38
+39
 
-3.1.26
+3.1.27
 
 misc.procpar(txt)
 
 Takes as input the path of a file containing a 'key' in the first column and a 'value' in the second
 column. Returns a dictionary of shape key : value.
 Parameters
 • txt : str
 Path to a file that contains 'key' in first column and 'value' in the second
 Returns
 • procpars : dict
 Dictionary of shape key :
 
 value.
 
-39
+40
 
-3.1.27
+3.1.28
+
+misc.px2in(*px_args)
+
+Converts a sequence of numbers from inches to pixels by multiplying ×96.
+Parameters:
+• px_args: sequence of ints
+Values in pixels to convert
+Returns:
+• in_args: tuple of floats
+Values in inches
+
+41
+
+3.1.29
 
 misc.readlistfile(datafile)
 
 Takes as input the path of a file containing one entry for each row. Returns a list of the aforementioned
 entries.
 Parameters
 • datafile: str
 Path to a file that contains one entry for each row
 Returns
 • files : list
 List of the entries contained in the file
 
-40
+42
 
-3.1.28
+3.1.30
 
 misc.select_for_integration(ppm_f1, ppm_f2, data, Neg=True)
 
 Select the peaks of a 2D spectrum to integrate. First, select the area where your peak is located by
 dragging the red square. Then, select the center of the peak by right_clicking. Finally, click ’ADD’
 to store the peak. Repeat the procedure for as many peaks as you want.
 Parameters:
@@ -1433,17 +1498,17 @@
 Choose if to show the negative contours ( True) or not (False )
 Returns:
 • peaks: list of dict
 For each peak there are two keys, ’f1’ and ’f2’, whose meaning is obvious. For each of these
 keys, you have ’u’: center of the peak /ppm, and ’lim’: the limits of the square you drew
 before.
 
-41
+43
 
-3.1.29
+3.1.31
 
 misc.select_traces(ppm_f1, ppm_f2, data, Neg=True, grid=False)
 
 Select traces from a 2D spectrum, save the coordinates in a list. Left click to select a point, right
 click to remove it.
 Parameters
 • ppm_f1 : 1darray
@@ -1456,98 +1521,98 @@
 Choose if to show the negative contours (True) or not (False)
 • grid : bool
 Choose if to display the grid (True) or not (False)
 Returns
 • coord: list
 List containing the [x,y] coordinates of the selected points.
 
-42
+44
 
-3.1.30
+3.1.32
 
 misc.set_fontsizes(ax, fontsize=10)
 
 Automatically adjusts the fontsizes of all the figure elements. In particular:
 • title = fontsize
 • axis labels = fontsize −2
 • ticks labels = fontsize −3
 • legend entries = fontsize −4
 Parameters:
 • ax: matplotlib.Subplot Object
 Subplot of interest
 • fontsize: float
 Starting fontsize
 
-43
+45
 
-3.1.31
+3.1.33
 
 misc.set_ylim(ax, data_inp)
 
 Sets the y-limits of ax as follows:
 • Bottom: min(data) − 5% max(data)
 • Top: max(data) + 5% max(data)
 Parameters:
 • ax: matplotlib.Subplot Object
 Panel of the figure where to apply this scale
 • data_inp: ndarray or list
 Input data. If it is a list, data_inp is converted to array.
 
-44
+46
 
-3.1.32
+3.1.34
 
 misc.show_cmap(cmap, N=10, start=0, end=1)
 
 Plot the colors extracted from a colormap.
 Parameters:
 • cmap: matplotlib.Colormap Object
 The colormap from which you want to extract the list of colors
 • N: int
 Number of samples to extract
 • start: float
 Start point of the sampling. 0 = beginning of the cmap; 1 = end of the cmap.
 • end: float
 End point of the sampling. 0 = beginning of the cmap; 1 = end of the cmap.
 
-45
+47
 
-3.1.33
+3.1.35
 
 misc.split_acqus_2D(acqus)
 
 Split the acqus dictionary of a 2D spectrum into two separate 1D-like acqus dictionaries.
 Parameters:
 • acqus: dict
 acqus dictionary of a 2D spectrum
 Returns:
 • acqu1s: dict
 acqus dictionary of the indirect dimension
 • acqu2s: dict
 acqus dictionary of the direct dimension
 
-46
+48
 
-3.1.34
+3.1.36
 
 misc.split_procs_2D(procs)
 
 Split the procs dictionary of a 2D spectrum into two separate 1D-like procs dictionaries.
 Parameters
 • procs: dict
 procs dictionary of a 2D spectrum
 Returns
 • proc1s: dict
 procs dictionary of the indirect dimension
 • proc2s: dict
 procs dictionary of the direct dimension
 
-47
+49
 
-3.1.35
+3.1.37
 
 misc.trim_data(ppm_scale, y, sx, dx)
 
 Trims the frequency scale and correspondant 1D dataset y from sx (ppm) to dx (ppm).
 Parameters
 • ppm_scale : 1darray
 ppm scale of the spectrum
@@ -1559,87 +1624,118 @@
 ppm value where to finish trimming
 Returns
 • xtrim : 1darray
 Trimmed ppm scale
 • ytrim : 1darray
 Trimmed spectrum
 
-48
+50
 
-3.1.36
+3.1.38
+
+misc.trim_data_2D(x_scale, y_scale, data, xlim=None, ylim=None)
+
+Trims data and scales according to xlim and ylim. Returns the trimmed data and the correspondant
+trimmed scales.
+Parameters:
+• x_scale: 1darray
+Scale for the rows of data
+• y_scale: 1darray
+Scale for the columns of data
+• data: 2darray
+Data to be trimmed
+• xlim: tuple
+Limits for x_scale (L, R)
+• ylim: tuple
+Limits for y_scale (L, R)
+Returns:
+• trimmed_x: 1darray
+Trimmed x-scale
+• trimmed_y: 1darray
+Trimmed y-scale
+• trimmed_data: 2darray
+Trimmed data
+
+51
+
+3.1.39
 
 misc.unhankel(H)
 
 Concatenates the first row and the last column of the matrix H, which should have Hankel-like
 structure, so to build the array of independent parameters.
 Parameters:
 • H: 2darray
 Hankel-like matrix
 Returns:
 • h: 1darray
 First row and last column of H, concatenated
 
-49
+52
 
-3.1.37
+3.1.40
 
 misc.write_acqus_1D(acqus, path=’./’, filename=None)
 
 Writes the input file for a simulated spectrum, basing on a dictionary of parameters.
 Parameters
 • acqus : dict
 The dictionary containing the parameters for the simulation
 • path : str, optional
 Directory where the file will be saved.
 • filename: str, optional
 Name of the file to be saved in path. The default name is sim_in_1D
 
-50
+53
 
-3.1.38
+3.1.41
 
 misc.write_acqus_2Dacqus, path=’sim_in_2D’)
 
 Writes the input file for a simulated spectrum, basing on a dictionary of parameters.
 Parameters
 • acqus : dict
 The dictionary containing the parameters for the simulation
 • path : str, optional
 Directory where the file will be saved. The default name is sim_in_1D.
 
-51
+54
 
-3.1.39
+3.1.42
 
 misc.write_help(request, file=None)
 
 Gets the documentation of request, and tries to save it in a text file.
 Parameters:
 • request: function or class or package
 Whatever you need documentation of
 • file: str or None or False
 Name of the output documentation file. If it is None, a default name is given. If it is False,
 the output is printed on screen.
 
-52
+55
 
-3.1.40
+3.1.43
 
-misc.write_ser(path, fid)
+misc.write_ser(fid, path=’./’, BYTORDA=0, DTYPA=0, overwrite=True)
 
-Writes the FID file in directory path, in a TopSpin-readable way (i.e. little endian, int32). The
-binary file is named 'fid' if 1D, 'ser' if multiD.
-Apparently, bidimensional spectra are not saved correctly.
-Parameters
-• path : str
-Directory where to save the file
+Writes the FID file in directory ’path’, in a TopSpin-readable way (i.e. little endian, int32). The
+binary file is named ’fid’ if 1D, ’ser’ if multiD. The parameters BYTORDA and DTYPA can be found
+in the acqus file.
+− BYTORDA = 1 ⇒ big endian ⇒ ’>’
+− BYTORDA = 0 ⇒ little endian ⇒ ’<’
+− DTYPA = 0 ⇒ int32 ⇒ ’i4’
+− DTYPA = 2 ⇒ float64 ⇒ ’f8’
+Parameters:
 • fid : ndarray
 FID array to be written
+• path : str
+Directory where to save the file
 
-53
+56
 
 3.2
 
 PROCESSING package
 
 This package contains functions for the processing of NMR spectra, either in time domain or in
 frequency domain, and the transition between the two domains.
@@ -1664,15 +1760,15 @@
 Number of singular values to keep.
 • print_head: bool
 Set it to True to display the fancy heading.
 Returns
 • datap: 1darray
 Denoised data
 
-54
+57
 
 3.2.2
 
 processing.Cadzow_2D(data, n, nc, i=True, itermax=100, f=0.005,
 print_time=True)
 
 Performs the Cadzow denoising method on a 2D spectrum, one transient at the time. This function
@@ -1692,15 +1788,15 @@
 Factor for the arrest criterion.
 • print_time: bool
 Set it to True to display the time spent.
 Returns
 • datap: 2darray
 Denoised data
 
-55
+58
 
 3.2.3
 
 processing.EAE(data)
 
 Shuffles data if the spectrum is acquired with 'FnMODE':'Echo-Antiecho'. NOTE: introduces -90°
 phase shift in F1, to be corrected after the processing.
@@ -1711,15 +1807,15 @@
 Parameters
 • data : ndarray
 Data to be shuffled.
 Returns
 • pdata : ndarray
 Shuffled data.
 
-56
+59
 
 3.2.4
 
 processing.LRD(data, nc)
 
 Denoising method based on Low-Rank Decomposition. The algorithm performs a singular value
 decomposition on data, then keeps only the first nc singular values while setting all the others to 0.
@@ -1729,15 +1825,15 @@
 Data to be denoised
 • nc: int
 Number of components, i.e. number of singular values to keep
 Returns:
 • data_out: 2darray
 Denoised data
 
-57
+60
 
 3.2.5
 
 processing.MCR(input_data, nc, f=10, tol=1e-5, itermax=1e4, H=True,
 oncols=True)
 
 This is an implementation of Multivariate Curve Resolution for the denoising of 2D NMR data.
@@ -1772,15 +1868,15 @@
 • CS_f: 2darray or 3darray
 Final denoised data matrix
 • C_f: 2darray or 3darray
 Final C matrix
 • S_f: 2darray or 3darray
 Final S matrix
 
-58
+61
 
 3.2.6
 
 processing.MCR_ALS(D, C, S, itermax=10000, tol=1e-5)
 
 Performs alternating least squares to get the final C and S matrices. Being the fundamental MCR
 equation:
@@ -1815,15 +1911,15 @@
 Threshold for the arrest criterion.
 Returns
 • C: 2darray
 Optimized C matrix, of dimensions m × nc.
 • S: 2darray
 Optimized S matrix, of dimensions nc × n.
 
-59
+62
 
 3.2.7
 
 processing.MCR_unpack(C, S, nds, H=True)
 
 Reverts matrix augmentation of stack_MCR. If H=True, converts C from dimensions (Y, nds) to
 (X, Y, nds) and S from dimensions (nds, X ∗Z) to (X, nds, Z); if H=False converts C from dimensions
@@ -1839,15 +1935,15 @@
 True for horizontal stacking, False for vertical stacking.
 Returns
 • C_f: 3darray
 Not-augmented C matrix.
 • S_f: 3darray
 Not-augmented S matrix.
 
-60
+63
 
 3.2.8
 
 processing.SIMPLISMA(D, nc, f=10, oncols=True)
 
 Finds the first nc purest components of matrix D using the SIMPLISMA algorithm, proposed by
 Windig and Guilment (DOI: 10.1021/ac00014a016 ). If oncols=True, this function estimates S
@@ -1864,15 +1960,15 @@
 If True, SIMPLISMA estimates the S matrix, otherwise estimates C.
 Returns
 • C: 2darray
 Estimation of the C matrix, of dimensions m × nc.
 • S: 2darray
 Estimation of the S matrix, of dimensions nc × n.
 
-61
+64
 
 3.2.9
 
 processing.baseline_correction(ppm, data, basl_file=’spectrum.basl’,
 winlim=None)
 
 Interactively corrects the baseline of a given spectrum and saves the parameters in a file. The program
@@ -1885,15 +1981,15 @@
 The spectrum of which to adjust the baseline
 • basl_file: str
 Name for the baseline parameters file
 • winlim: list or str or None
 List of the breakpoints for the window. If it is str, it points to a file to be read with np.loadtxt.
 If it is None, the partitioning is done interactively.
 
-62
+65
 
 3.2.10
 
 processing.calc_nc(data, s_n)
 
 Calculates the optimal number of components, given the standard deviation of the noise. The
 threshold value is calculated as stated in Theorem 1 of reference: https://arxiv.org/abs/1710.09787v2
@@ -1902,15 +1998,15 @@
 Input data
 • s_n: float
 Noise standard deviation
 Returns:
 • n_c: int
 Number of components
 
-63
+66
 
 3.2.11
 
 processing.calibration(ppmscale, S)
 
 Scroll the ppm scale of spectrum to make calibration. The interface offers two guidelines: the red
 one, labelled 'reference signal' remains fixed, whereas the green one ('calibration value') moves with
@@ -1924,15 +2020,15 @@
 • S: 1darray
 The spectrum to calibrate
 Returns
 • offset: float
 Difference between original scale and new scale. This must be summed up to the original ppm
 scale to calibrate the spectrum.
 
-64
+67
 
 3.2.12
 
 processing.convdta(data, grpdly=0, scaling=1)
 
 Removes the digital filtering to obtain a spectrum similar to the command CONVDTA performed
 by TopSpin. However, they will differ a little bit because of the digitization. These differences are
@@ -1944,15 +2040,15 @@
 Number of points that the digital filter consists of. Key $GRPDLY in acqus file
 • scaling: float
 Scaling factor of the resulting FID. Needed to match TopSpin’s intensities.
 Returns:
 • data_in: ndarray
 FID without the digital filter. It will have grpdly points less than data.
 
-65
+68
 
 3.2.13
 
 processing.em(data, lb, sw)
 
 Exponential apodization.
 Being the FID an array of N points in its last dimension, and taken x = np.arange(N)/N :
@@ -1969,15 +2065,15 @@
 Lorentzian broadening, in Hz. lb > 0
 • sw : float
 Spectral width in Hz, used for normalization.
 Returns
 • apod * data : ndarray
 Apodized FID.
 
-66
+69
 
 3.2.14
 
 processing.fp(data, wf=None, zf=None, fcor=0.5, tdeff=0)
 
 Performs the full processing of a 1D NMR FID.
 Parameters
@@ -1991,15 +2087,15 @@
 Weighting factor for the first point of the FID.
 • tdeff: int
 Number of FID points to be employed for the processing. tdeff = 0 means whole FID.
 Returns
 • data: ndarray
 Processed spectrum.
 
-67
+70
 
 3.2.15
 
 processing.ft(data, alt=False, fcor=0.5, Numpy=True)
 
 Fourier transform in NMR sense, i.e. with positive exponential. This means to perform IFT reverting
 the 1/N scaling.
@@ -2014,15 +2110,15 @@
 • Numpy: bool
 If True (***STRONGLY ADVISED***) performs the FT using the FFT algorithm encoded
 in Numpy. Otherwise, performs it manually using the definition of discrete FT.
 Returns
 • dataft : ndarray
 Transformed FID.
 
-68
+71
 
 3.2.16
 
 processing.gm(data, lb, gb, sw, gc=0)
 
 Gaussian apodization.
 Being the FID an array of N points in its last dimension, and taken x = np.arange(N):
@@ -2054,15 +2150,15 @@
 Spectral width in Hz, used for normalization.
 • gc: float
 Gaussian center, relatively to the FID length: 0 ≤ gc ≤ 1
 Returns
 • apod * data : ndarray
 Apodized FID.
 
-69
+72
 
 3.2.17
 
 processing.gmb(data, lb, gb, sw)
 
 Gaussian apodization, Bruker-like. It does not work very well.
 Being the FID an array of N points in its last dimension, and taken t = np.arange(N)/sw:
@@ -2088,15 +2184,15 @@
 Spectral width in Hz, used for normalization.
 • gc: float
 Gaussian center, relatively to the FID length: 0 ≤ gc ≤ 1
 Returns
 • apod * data : ndarray
 Apodized FID.
 
-70
+73
 
 3.2.18
 
 processing.ift(data, alt=False, fcor=0.5, Numpy=True)
 
 Inverse Fourier transform in NMR sense, i.e. with negative exponential. This means to perform FT
 multiplying by N afterwards.
@@ -2111,15 +2207,15 @@
 • Numpy: bool
 If True (***STRONGLY ADVISED***) performs the FT using the FFT algorithm encoded
 in Numpy. Otherwise, performs it manually using the definition of discrete FT.
 Returns
 • dataft : ndarray
 Inverse transformed FID.
 
-71
+74
 
 3.2.19
 
 processing.integral(fx, x=None, lims=None)
 
 Calculates the primitive of fx. If fx is a multidimensional array, the integrals are computed along
 the last dimension.
@@ -2130,15 +2226,15 @@
 Independent variable. Determines the integration step. If None, it is set as the point scale
 • lims: tuple or None
 Integration range. If None, the whole function is integrated
 Returns:
 • Fx: ndarray
 Integrated function.
 
-72
+75
 
 3.2.20
 
 processing.integral_2D(ppm_f1, t_f1, SFO1, ppm_f2, t_f2, SFO2,
 u_1=None, fwhm_1=200, utol_1=0.5, u_2=None, fwhm_2=200,
 utol_2=0.5, plot_result=False)
 
@@ -2173,15 +2269,15 @@
 Allowed tolerance for u_2 during the fit. (u_2-utol_2, u_2+utol_2)
 • plot_result: bool
 True to show how the program fitted the traces.
 Returns:
 • I_tot: float
 Computed integral.
 
-73
+76
 
 3.2.21
 
 processing.interactive_basl_windows(ppm, data)
 
 Allows for interactive partitioning of a spectrum in windows. Double left click to add a bar, double
 right click to remove it. Returns the location of the red bars as a list.
@@ -2190,18 +2286,41 @@
 PPM scale of the spectrum
 • data: 1darray
 Spectrum to be partitioned
 Returns:
 • coord: list
 List containing the coordinates of the windows, plus ppm[0] and ppm[-1]
 
-74
+77
 
 3.2.22
 
+processing.interactive_echo_param(data0)
+
+Interactive plot that allows to select the parameters needed to process a CPMG-like FID. Use the
+TextBox or the arrow keys to adjust the values. You can call processing.sum_echo_train or
+processing.split_echo_train by starring the return statement of this function, i.e.:
+processing.sum_echo_train(data0, *interactive_echo_train(data0))
+
+as they are in the correct order to be used in this way.
+Parameters:
+• data0: ndarray
+CPMG FID
+Returns:
+• n: int
+Distance between one echo and the next one
+• n_echoes: int
+Number of echoes to sum/split
+• i_p: int
+Offset points from the start of the FID
+
+78
+
+3.2.23
+
 processing.interactive_fp(fid0, acqus, procs)
 
 Perform the processing of a 1D NMR spectrum interactively. The GUI offers the opportunity to test
 different window functions, as well as different tdeff values and final sizes. The active parameters
 appear as blue text.
 Parameters:
 • fid0: 1darray
@@ -2212,17 +2331,17 @@
 Dictionary of processing parameters
 Returns:
 • pdata: 1darray
 Processed spectrum
 • procs: dict
 Updated dictionary of processing parameters
 
-75
+79
 
-3.2.23
+3.2.24
 
 processing.interactive_phase_1D(ppmscale, S)
 
 Allows for interactive phase adjustment of 1D NMR spectra. Employs processing.ps for the actual
 phase correction. Press the z key on the keyboard to toggle the automatic adjustment of vertical
 scale on or off.
 Parameters
@@ -2230,17 +2349,17 @@
 PPM scale of the spectrum
 • S: 1darray
 The spectrum to be phased
 Returns
 • phased_data: 1darray
 Phased spectrum.
 
-76
+80
 
-3.2.24
+3.2.25
 
 processing.interactive_phase_2D(ppm_f1, ppm_f2, S)
 
 Interactively adjust the phases of a 2D spectrum. S must be hypercomplex, therefore must be passed
 before to unpack it into the 4 real files. The phase correction is done using processing.ps as follows:
 1. S = processing.ps(S, p0=p0_f2, p1=p1_f2, pivot=pivot_f2)
 2. Transpose: normal if FnMODE='QF', hypercomplex otherwise
@@ -2253,17 +2372,17 @@
 Direct dimension ppm scale
 • S: 2darray
 Hypercomplex spectrum
 Returns
 • S:2darray
 Phased spectrum
 
-77
+81
 
-3.2.25
+3.2.26
 
 processing.interactive_qfil(ppm, data_in)
 
 Interactive function to design a gaussian filter with the aim of suppressing signals in the spectrum.
 You can adjust position and width of the filter scrolling with the mouse.
 Parameters:
 • ppm: 1darray
@@ -2272,17 +2391,17 @@
 Spectrum on which to apply the filter.
 Returns:
 • u: float
 Position of the gaussian filter
 • s: float
 Width of the gaussian filter (Standard deviation)
 
-78
+82
 
-3.2.26
+3.2.27
 
 processing.interactive_xfb(fid0, acqus, procs, lvl0=0.1, show_cnt=True)
 
 Perform the processing of a 2D NMR spectrum interactively. The GUI offers the opportunity to test
 different window functions, as well as different tdeff values and final sizes. The active parameters
 appear as blue text. When changing the parameters, give it some time to compute. The figure panel
 is quite heavy.
@@ -2299,17 +2418,17 @@
 Choose if to display data using contours (True) or heatmap (False)
 Returns:
 • pdata: 2darray
 Processed spectrum
 • procs: dict
 Updated dictionary of processing parameters
 
-79
+83
 
-3.2.27
+3.2.28
 
 processing.inv_fp(data, wf=None, size=None, fcor=0.5)
 
 Performs the full inverse processing of a 1D NMR spectrum (data). Required parameters are:
 Parameters
 • data: 1darray
 Input data
@@ -2319,17 +2438,17 @@
 initial size of the FID
 • fcor: float
 weighting factor for the FID first point
 Returns
 • data: 1darray
 Processed data
 
-80
+84
 
-3.2.28
+3.2.29
 
 processing.inv_xfb(data, wf=[None, None], size=[None, None],
 fcor=[0.5, 0.5], FnMODE=’States-TPPI’)
 
 Performs the full processing of a 2D NMR FID (data). Required parameters are:
 Parameters
 • data: 2darray
@@ -2344,17 +2463,17 @@
 If True, unpacks the hypercomplex spectrum and returns the 4 real files, using processing.unpack_2D
 • tdeff: list of int
 number of points of the FID to be used for the processing, [F1, F2]
 Returns
 • data: 2darray
 Processed data
 
-81
+85
 
-3.2.29
+3.2.30
 
 processing.iterCadzow(data, n, nc, itermax=100, f=0.005, print_head=T
 print_time=True)
 
 This functions performs Cadzow denoising on data, which is a 1D array of N points, in an iterative
 manner. The algorithm works as follows:
 1. Transform data in a Hankel matrix H of dimensions (N − n, n)
@@ -2389,17 +2508,17 @@
 Set it to True to display the fancy heading.
 • print_time: bool
 Set it to True to display the time spent.
 Returns
 • datap: 1darray
 Denoised data
 
-82
+86
 
-3.2.30
+3.2.31
 
 processing.load_baseline(filename, ppm, data)
 
 Read the baseline parameters from a file and builds the baseline itself.
 Parameters:
 • filename: str
 Location of the baseline file
@@ -2407,17 +2526,17 @@
 PPM scale of the spectrum
 • data: 1darray
 Spectrum of which to correct the baseline
 Returns:
 • baseline: 1darray
 Computed baseline
 
-83
+87
 
-3.2.31
+3.2.32
 
 processing.make_polynomion_baseline(ppm, data, limits)
 
 Interactive baseline correction with 4th degree polynomion.
 Parameters:
 • ppm: 1darray
 PPM scale of the spectrum
@@ -2427,17 +2546,17 @@
 Window limits (left, right).
 Returns:
 • mode: str
 Baseline correction mode: ’polynomion’ as default, ’spline’ if you press the button
 • C_f: 1darray or str
 Baseline polynomion coefficients, or ’callintsmooth’ if you press the spline button
 
-84
+88
 
-3.2.32
+3.2.33
 
 processing.make_scale(size, dw, rev=True)
 
 Computes the frequency scale of the NMR spectrum, given the number of points and the employed
 dwell time (the REAL one, not the TopSpin one!). rev=True is required for the correct frequency
 arrangement in the NMR sense.
 Parameters
@@ -2447,17 +2566,42 @@
 Time spacing in the time dimension
 • rev: bool
 Reverses the scale
 Returns
 • fqscale: 1darray
 The computed frequency scale.
 
-85
+89
 
-3.2.33
+3.2.34
+
+processing.new_MCR(input_data, nc, f=10, tol=1e-05, itermax=10000.
+H=True, oncols=True, our_function=None, fargs=[], our_function2=No
+f2args=[])
+
+# This is an implementation of Multivariate Curve Resolution # for the denoising of 2D NMR data.
+It requires: # - input_data: a tensor containing the set of 2D NMR datasets to be coprocessed
+# stacked along the first dimension; # - nc : number of purest components; # - f : percentage of
+allowed noise; # - tol : tolerance for the arrest criterion; # - itermax : maximum number of allowed
+iterations, default 10000 # - H : True for horizontal stacking of data (default), False for vertical; #
+- oncols : True to estimate S with purest components, False to estimate C # This function returns
+the denoised datasets, ’CS’, and the ’C’ and ’S’ matrices.
+
+90
+
+3.2.35
+
+processing.new_MCR_ALS(D, C, S, itermax=10000, tol=1e-05,
+reg_f=None, reg_fargs=[])
+
+Modified function to do ALS
+
+91
+
+3.2.36
 
 processing.pknl(data, grpdly=0, onfid=False)
 
 Compensate for the Bruker group delay at the beginning of FID through a first-order phase correction
 of
 ϕ(1) = 360 ∗ GRPDLY
 This should be applied after apodization and zero-filling.
@@ -2468,17 +2612,17 @@
 Number of points that make the group delay.
 • onfid: bool
 If it is True, performs FT before to apply the phase correction, and IFT after.
 Returns:
 • datap: ndarray
 Corrected data
 
-86
+92
 
-3.2.34
+3.2.37
 
 processing.ps(data, ppmscale=None, p0=None, p1=None, pivot=None,
 interactive=False)
 
 Applies phase correction on the last dimension of data. The pivot is set at the center of the spectrum
 by default. Missing parameters will be inserted interactively.
 Being data a 1D array of N points, as well as ppmscale, the following parameters are defined:
@@ -2507,17 +2651,17 @@
 opened.
 Returns:
 • datap: ndarray
 Phased data
 • final_values: tuple
 Employed values of the phase correction. (p0, p1, pivot)
 
-87
+93
 
-3.2.35
+3.2.38
 
 processing.qfil(ppm, data, u, s)
 
 Suppress signals in the spectrum using a gaussian filter.
 Parameters:
 • ppm: 1darray
 Scale on which to build the filter
@@ -2527,32 +2671,32 @@
 Position of the filter
 • s: float
 Width of the filter (standard deviation)
 Returns:
 • pdata: ndarray
 Filtered data
 
-88
+94
 
-3.2.36
+3.2.39
 
 processing.qpol(fid)
 
 Fits the FID with a 4-th degree polynomion, then subtracts it from the original FID. The real and
 imaginary channels are treated separately.
 Parameters
 • fid : ndarray
 Self-explanatory.
 Returns
 • fid : ndarray
 Processed FID.
 
-89
+95
 
-3.2.37
+3.2.40
 
 processing.qsin(data, ssb)
 
 Sine-squared apodization.
 Being data an array of N points in its last dimension, and taken x = np.arange(N)/N , if ssb = 0
 or ssb = 1:
  
@@ -2584,57 +2728,57 @@
 – ssb = 1 : same as ssb = 0
 – ssb = 2 : from π/2 to π
 – ssb = 3 : from π/3 to π
 Returns
 • apod * data : ndarray
 Apodized FID.
 
-90
+96
 
-3.2.38
+3.2.41
 
 processing.quad(fid)
 
 Subtracts from the FID the arithmetic mean of its last quarter. The real and imaginary channels
 are treated separately.
 Parameters
 • fid : ndarray
 Self-explanatory.
 Returns
 • fid : ndarray
 Processed FID.
 
-91
+97
 
-3.2.39
+3.2.42
 
 processing.repack_2D(rr, ir, ri, ii)
 
 Renconstruct hypercomplex 2D NMR data given the 4 real arrays. See processing.unpack_2D for
 details.
 Returns
 • data
 
-92
+98
 
-3.2.40
+3.2.43
 
 processing.rev(data)
 
 Reverses the last dimension of data.
 Parameters
 • data : ndarray
 matrix to be reverted
 Returns
 • data[...,::-1] : ndarray
 Self-explanatory
 
-93
+99
 
-3.2.41
+3.2.44
 
 processing.sin(data, ssb)
 
 Sine apodization.
 Being data an array of N points in its last dimension, and taken x = np.arange(N)/N , if ssb = 0
 or ssb = 1:
  
@@ -2658,40 +2802,40 @@
 – ssb = 1 : same as ssb = 0
 – ssb = 2 : from π/2 to π
 – ssb = 3 : from π/3 to π
 Returns
 • apod * data : ndarray
 Apodized FID.
 
-94
+100
 
-3.2.42
+3.2.45
 
 processing.split_echo_train(datao, n, n_echoes, i_p=0)
 
-datao is a 1D or 2D dataset whose direct dimension has been acquired with the CPMG sequence,
-i.e. the FID is made of echoes separated one from each other by n points. The first good point of
-the FID is i_p. This function separates the first n_echoes echoes and stores them in a 2D array of
-shape (n_echoes, datao.shape[0], n/2).
-Parameters
-• datao : ndarray
-1D or 2D CPMG FID
-• n : int
-Number of points that separate an echo from the next one
-• n_echoes : int
-Number of echoes to add together
-• i_p : int
-First point offset.
-Returns
-• data_p : ndarray
-Processed FID.
+Separate a CPMG echo-train FID into echoes so to be processed separately. The first decay, i.e.
+the native FID, is extracted, and corresponds to echo number 0. Then, for each echo, the left side
+(reversed) is summed up to its right part. You can use processing.interactive_echo_param to
+calculate the parameters interactively.
+Parameters:
+• datao: ndarray
+FID with an echo train on its last dimension
+• n: int
+number of points that separate one echo from the next
+• n_echoes: int
+number of echoes to extract. If it is 0, extracts only the first decay
+• i_p: int
+Number of offset points
+Returns:
+• data_p: (n+1)darray
+Separated echoes
 
-95
+101
 
-3.2.43
+3.2.46
 
 processing.stack_MCR(input_data, H=True)
 
 Performs matrix augmentation converting input_data from dimensions (X, Y, Z) to (Y, X ∗ Z) if
 H=True, or (X ∗ Y, Z) if H=False.
 Parameters
 • input_data: 3darray
@@ -2699,39 +2843,38 @@
 first one.
 • H: bool
 True for horizontal stacking, False for vertical stacking.
 Returns
 • data: 2darray
 Augmented data matrix.
 
-96
+102
 
-3.2.44
+3.2.47
 
 processing.sum_echo_train(datao, n, n_echoes, i_p=0)
 
-datao is a 1D or 2D dataset whose direct dimension has been acquired with the CPMG sequence,
-i.e. the FID is made of echoes separated one from each other by n points. The first good point of
-the FID is i_p. This function sums up the first n_echoes echoes and returns the resulting FID.
-Parameters
-• datao : ndarray
-1D or 2D CPMG FID
-• n : int
-Number of points that separate an echo from the next one
-• n_echoes : int
-Number of echoes to add together
-• i_p : int, optional
-First point offset.
-Returns
-• data_p : ndarray
-Processed FID.
+Sum up a CPMG echo-train FID into echoes so to enchance the SNR. This function calls processing.split_ec
+with the same parameters. You can use processing.interactive_echo_param to calculate the parameters interactively.
+Parameters:
+• datao: ndarray
+FID with an echo train on its last dimension
+• n: int
+number of points that separate one echo from the next
+• n_echoes: int
+number of echoes to sum
+• i_p: int
+Number of offset points
+Returns:
+• data_p: ndarray
+Summed echoes
 
-97
+103
 
-3.2.45
+3.2.48
 
 processing.tabula_rasa(data, lvl=0.05, cmap=cm.Blues_r)
 
 This function is to be used in SIFT algorithm. Allows interactive selection using a Lasso widget of
 the region of the spectrum which contain signal. Returns a masking matrix, of the same shape as
 data, whose entries are 1 inside the selection and 0 outside.
 Parameters
@@ -2741,17 +2884,17 @@
 Level of the contours, expressed as fraction of the maximum intensity
 • cmap : matplotlib.cm Object
 Color of the contours
 Returns
 • mask: 2darray
 Matrix that contains 1 inside the selection and 0 outside.
 
-98
+104
 
-3.2.46
+3.2.49
 
 processing.td_eff(data, tdeff)
 
 Uses only the first tdeff points of data. It is applied before any other processing. The length of the
 list tdeff must match the dimension of data, if data is multidimensional.
 Parameters
 • data: ndarray
@@ -2760,17 +2903,17 @@
 The number of points to be used. If data is 1D, tdeff can be passed as integer, otherwise
 it has to be: [F1, F2, ..., Fn]. A 0 entry in the list means to not trim the corresponding
 dimension.
 Returns
 • data: ndarray
 Trimmed data according to tdeff.
 
-99
+105
 
-3.2.47
+3.2.50
 
 processing.tp_hyper(data)
 
 Computes the hypercomplex transpose of data. Needed for the processing of data acquired in a
 phase-sensitive manner in the indirect dimension.
 To explain how a hypercomplex transposition works, we will focus on the simpler example of a
 4 × 6 matrix, A, with complex coefficients ai,j = xi,j + iyi,j .
@@ -2812,17 +2955,17 @@
 Parameters
 • data : 2darray
 Complex data matrix.
 Returns
 • datatp : 2darray
 Hypercomplex transpose of data.
 
-100
+106
 
-3.2.48
+3.2.51
 
 processing.unpack_2D(data)
 
 Separates fully processed 2D NMR data into 4 distinct ser files:
 rr = Re{data}[:: 2]
 ir = Im{data}[:: 2]
 ri = Re{data}[1 :: 2]
@@ -2830,34 +2973,34 @@
 Parameters
 • data : 2darray
 Complex data matrix.
 Returns
 • rr, ir, ri, ii: 2darray, 2darray, 2darray, 2darray
 See above.
 
-101
+107
 
-3.2.49
+3.2.52
 
 processing.write_basl_info(f, limits, mode, data)
 
 Writes the baseline parameters of a certain window in a file.
 Parameters:
 • f: TextIO object
 File where to write the parameters
 • limits: tuple
 Limits of the spectral window. (left, right)
 • mode: str
 Baseline correction mode: ’polynomion’ or ’spline’
 • data: float or 1darray
 It can be either the spline smoothing factor or the polynomion coefficients
 
-102
+108
 
-3.2.50
+3.2.53
 
 processing.xfb(data, wf=[None, None], zf=[None, None], fcor=[0.5,0.5],
 tdeff=[0,0], u=True, FnMODE=’States-TPPI’)
 
 Performs the full processing of a 2D NMR FID.
 Parameters
 • data: 2darray
@@ -2874,31 +3017,31 @@
 [F1, F2]
 • u : bool
 if True, unpacks the hypercomplex spectrum and returns the 4 files.
 Returns
 • data : 2darray
 Processed data.
 
-103
+109
 
-3.2.51
+3.2.54
 
 processing.zf(data, size)
 
 Zero-filling of data up to size.
 Parameters
 • data : ndarray
 FID / Spectrum to be zero-filled
 • size : int
 Final size of the FID / Spectrum
 Returns
 • datazf : ndarray
 Zero-filled FID / Spectrum
 
-104
+110
 
 3.3
 
 FIGURES package
 
 This package contains a series of functions to make plots of various nature.
 
@@ -2937,20 +3080,20 @@
 • n_yticks: int
 Number of numbered ticks on the x-axis of the figure
 • label: str
 label to be put in the legend.
 • fontsize: float
 Biggest font size in the figure.
 
-105
+111
 Returns:
 • line: Line2D Object
 Line object returned by plt.plot.
 
-106
+112
 
 3.3.2
 
 figures.ax2D(ax, ppm_f2, ppm_f1, datax, xlims=None, ylims=None,
 cmap=None, c_fac=1.4, lvl=0.1, lw=0.5, X_label='$\delta\,$ F2
 /ppm', Y_label='$\delta\,$ F1 /ppm', title=None, n_xticks=10,
 n_yticks=10), fontsize=10
@@ -2987,23 +3130,23 @@
 • Y_label: str
 text of the y-axis label;
 • lw: float
 linewidth of the contours
 • title: str
 Figure title.
 
-107
+113
 • n_xticks: int
 Number of numbered ticks on the x-axis of the figure
 • n_yticks: int
 Number of numbered ticks on the x-axis of the figure
 • fontsize: float
 Biggest font size in the figure.
 
-108
+114
 
 3.3.3
 
 figures.ax_heatmap(ax, data, zlim='auto', z_sym=True, cmap=None,
 xscale=None, yscale=None, rev=(False, False), n_xticks=10, n_yticks=1
 n_zticks=10, fontsize=10)
 
@@ -3036,15 +3179,15 @@
 Biggest font size to apply to the figure.
 Returns:
 • im: matplotlib.AxesImage
 The heatmap
 • cax: matplotlib.Subplot object
 figure panel where the colorbar is drawn
 
-109
+115
 
 3.3.4
 
 figures.dotmd(ppmscale, S, labels=None, n_xticks=10)
 
 Interactive display of multiple 1D spectra.
 Parameters
@@ -3055,15 +3198,15 @@
 • S: list
 spectra to be plotted
 • labels: list
 labels to be put in the legend.
 • n_xticks: int
 Number of numbered ticks on the x-axis of the figure
 
-110
+116
 
 3.3.5
 
 figures.dotmd_2D(ppm_f1, ppm_f2, S, labels=None, name='dotmd_2D'
 X_label='$\delta\, $ F2 /ppm', Y_label='$\delta\, $ F1 /ppm',
 n_xticks=10, n_yticks=10, Neg=True)
 
@@ -3089,15 +3232,15 @@
 • n_xticks: int
 Number of numbered ticks on the x-axis of the figure
 • n_yticks: int
 Number of numbered ticks on the x-axis of the figure
 • Neg: bool
 If True, show the negative contours.
 
-111
+117
 
 3.3.6
 
 figures.figure1D(ppm, data, norm=False, xlims=None, ylims=None,
 c='b', lw=0.5, name=None, X_label='$\delta\, $ F1 /ppm', Y_label='In
 /a.u.', n_xticks=10, n_yticks=10, hideylabels=False)
 
@@ -3128,15 +3271,15 @@
 • n_xticks: int
 Number of numbered ticks on the x-axis of the figure
 • n_yticks: int
 Number of numbered ticks on the x-axis of the figure
 • hideylabels: bool
 if True, does not show label and tick labels of the y axis.
 
-112
+118
 
 3.3.7
 
 figures.figure1D_multi(ppm0, data0, xlims=None, ylims=None, norm=Fa
 c=None, name=None, X_label='$\delta\$ F1 /ppm', Y_label='Intensity
 /a.u.', n_xticks=10, n_yticks=10, hideylabels=False, labels=None)
 
@@ -3168,15 +3311,15 @@
 Number of numbered ticks on the x-axis of the figure
 • hideylabels: bool
 if True, does not show label and tick labels of the y axis.
 • labels: list or None or False
 List of the labels to be shown in the legend. If it is None, the default entries are used (i.e., ’1,
 2, 3,...’). If it is False, the legend is not shown.
 
-113
+119
 
 3.3.8
 
 figures.figure2D(ppm_f2, ppm_f1, datax, xlims=None, ylims=None,
 cmap=None, c_fac=1.4, lvl=0.09, name=None, X_label='$\delta\,$
 F2 /ppm', Y_label='$\delta\,$ F1 /ppm', lw=0.5, Negatives=False,
 cmapneg=None, n_xticks=10, n_yticks=10)
@@ -3214,21 +3357,21 @@
 • lw: float
 linewidth of the contours
 • Negatives: bool
 set it to True if you want to see the negative part of the spectrum
 • cmapneg: matplotlib.cm Object
 Colour of the negative contours
 
-114
+120
 • n_xticks: int
 Number of numbered ticks on the x-axis of the figure
 • n_yticks: int
 Number of numbered ticks on the x-axis of the figure
 
-115
+121
 
 3.3.9
 
 figures.figure2D_multi(ppm_f2, ppm_f1, datax, xlims=None, ylims=Non
 lvl='default', name=None, X_label='$\delta\, $ F2 /ppm', Y_label='$\d
 $ F1 /ppm', lw=0.5, Negatives=False, n_xticks=10, n_yticks=10,
 labels=None)
@@ -3262,15 +3405,15 @@
 • n_xticks: int
 Number of numbered ticks on the x-axis of the figure
 • n_yticks: int
 Number of numbered ticks on the x-axis of the figure
 • labels: list
 entries of the legend. If None, the legend is not drawn.
 
-116
+122
 
 3.3.10
 
 figures.fitfigure(S, ppm_scale, t_AQ, V, C=False, SFO1=701.125,
 o1p=0, limits=None, s_labels=None, X_label='δ F1 /ppm', n_xticks=1
 name=None)
 
@@ -3297,15 +3440,15 @@
 label for the x-axis.
 • n_xticks: int
 number of numbered ticks that will appear in the ppm scale. An oculated choice can be very
 satisfying.
 • name: str or None
 Name with which to save the figure. If None, the picture is shown instead of being saved.
 
-117
+123
 
 3.3.11
 
 figures.heatmap(data, zlim='auto', z_sym=True, cmap=None, xscale=None, yscale=None, rev=(False, False), n_xticks=10, n_yticks=10
 n_zticks=10, fontsize=10, name=None)
 
 Computes a heatmap of data.
@@ -3332,29 +3475,29 @@
 • n_zticks: int
 Number of ticks of the color bar
 • fontsize: float
 Biggest font size to apply to the figure.
 • name: str or None
 Filename for the figure. Set to None to show the figure.
 
-118
+124
 
 3.3.12
 
 figures.plot_fid(fid, name=None)
 
 Makes a double-panel figure that shows the real and imaginary part of the FID. X-scale and Y-scale
 are automatically adjusted. If the FID is of a 2D spectrum, it is flattened before to be plot.
 Parameters
 • fid: ndarray
 The data to be plot. The entries can be complex numbers.
 • name: str
 If None, displays the figure. Otherwise, represents the filename/path where to save the figure.
 
-119
+125
 
 3.3.13
 
 figures.plot_fid_re(fid, scale=None, c='b', lims=None, name=None)
 
 Makes a single-panel figure that shows either the real or imaginary part of the FID. X-scale and
 Y-scale are automatically adjusted. If the FID is of a 2D spectrum, it is flattened before to be plot.
@@ -3366,15 +3509,15 @@
 • c: str
 Color of the line. Default blue (’b’)
 • lims: tuple
 Limits of the x-axis. Syntax: (left, right).
 • name: str
 If None, displays the figure. Otherwise, represents the filename/path where to save the figure.
 
-120
+126
 
 3.3.14
 
 figures.redraw_contours(ax, ppm_f2, ppm_f1, S, lvl, cnt, Neg=False,
 Ncnt=None, lw=0.5, cmap=[None, None])
 
 Redraws the contours in interactive 2D visualizations.
@@ -3401,29 +3544,29 @@
 Colour of the contours. Format: [cmap +, cmap -]
 Returns:
 • cnt: matplotlib.contour.QuadContourSet object
 Updated contours
 • Ncnt: matplotlib.contour.QuadContourSet object or None
 Updated negative contours if Neg is True, None otherwise
 
-121
+127
 
 3.3.15
 
 figures.sns_heatmap(data, name=None)
 
 Computes a heatmap of data, which is a matrix. This function employs the seaborn package.
 Specify name if you want to save the figure.
 Parameters:
 • data: 2darray
 Data of which to compute the heatmap. Make sure the entries are real numbers.
 • name: str or None
 Filename of the figure to be saved. If None, the figure is shown instead.
 
-122
+128
 
 3.3.16
 
 figures.stacked_plot(ppmscale, S, xlims=None, lw=0.5, name=None,
 X_label='$\delta\, $ F1 /ppm', Y_label='Normalized intensity
 /a.u.', n_xticks=10, labels=None)
 
@@ -3444,15 +3587,15 @@
 • Y_label: str
 text of the y-axis label;
 • n_xticks: int
 Number of numbered ticks on the x-axis of the figure
 • labels: list
 labels to be put in the legend.
 
-123
+129
 
 3.4
 
 SIM package
 
 This package contains function for the simulation of various features of NMR spectra, being them
 monodimensional or bidimensional. Functions for the simulation of whole spectra are also provided.
@@ -3473,15 +3616,15 @@
 Scalar coupling constant (Hz)
 Returns:
 • u_s: 1darray
 Frequencies of the splitted signal (Hz)
 • I_s: 1darray
 Intensities of the splitted signal
 
-124
+130
 
 3.4.2
 
 sim.f_gaussian(x, u, s, A=1)
 
 Gaussian function in the frequency domain:
 2 
@@ -3502,21 +3645,21 @@
 Standard deviation
 • A: float
 Intensity
 Returns
 • f: 1darray
 Gaussian function.
 
-125
+131
 
 3.4.3
 
 sim.f_lorentzian(x, u, fwhm, A=1)
 
-Lorentzian function in the time domain:
+Lorentzian function in the frequency domain:
 L(x) =
 
 γ
 A
 π (x − u)2 + γ 2
 
 Parameters
@@ -3528,15 +3671,15 @@
 Full-width at half-maximum, Γ = 2γ
 • A: float
 Intensity
 Returns
 • f: 1darray
 Lorentzian function.
 
-126
+132
 
 3.4.4
 
 sim.f_pvoigt(x, u, fwhm, A=1, x_g=0)
 
 Pseudo-Voigt function in the frequency domain:
 S(x) = xg G(x) + (1 − xg )L(x)
@@ -3555,15 +3698,15 @@
 Intensity
 • x_g: float
 Fraction of gaussianity
 Returns
 • S: 1darray
 Pseudo-Voigt function.
 
-127
+133
 
 3.4.5
 
 sim.gaussian_filter(ppm, u, s)
 
 Compute a gaussian filter to be used in order to suppress signals in the spectrum.
 Parameters:
@@ -3573,15 +3716,15 @@
 Position of the filter
 • s: float
 Width of the filter (standard deviation)
 Returns:
 • G: 1darray
 Computed gaussian filter
 
-128
+134
 
 3.4.6
 
 sim.load_sim_1D(File)
 
 Creates a dictionary from the spectral parameters listed in the input file.
 Template of the input file:
@@ -3616,15 +3759,15 @@
 Parameters
 • File: str
 Path to the input file location
 Returns
 • dic: dict
 Dictionary of the parameters, ready to be read from the simulation functions.
 
-129
+135
 
 3.4.7
 
 sim.load_sim_2D(File, states=True)
 
 Creates a dictionary from the spectral parameters listed in the input file.
 Template of the input file:
@@ -3677,18 +3820,26 @@
 Path to the input file location
 • states: bool
 If FnMODE is States or States-TPPI, set it to True to get the correct timescale.
 Returns
 • dic: dict
 Dictionary of the parameters, ready to be read from the simulation functions.
 
-130
+136
 
 3.4.8
 
+sim.mult_noise(data_size, mean, s_n)
+
+Multiplicative noise model.
+
+137
+
+3.4.9
+
 sim.multiplet(u, I, m=’s’, J=[])
 
 Split a given signal according to a scalar coupling pattern.
 Parameters:
 • u: float
 Frequency of the non-splitted signal (Hz)
 • I: float
@@ -3700,17 +3851,17 @@
 branches
 Returns:
 • u_in: list
 List of the splitted frequencies (Hz)
 • I_in: list
 Intensities of the splitted signal
 
-131
+138
 
-3.4.9
+3.4.10
 
 sim.noisegen(size, o2, t2, s_n=1)
 
 Simulates additive noise in the time domain, in the form of a matrix of dimensions size.
 This model for the noise depicts it as a white noise vector (i.e. random number that fit a gaussian
 distribution with 0 mean and standard deviation equal to s_n), modulated for the carrier frequency
 o2.
@@ -3740,34 +3891,34 @@
 Time scale of the last temporal dimension.
 • s_n: float
 Standard deviation of the noise.
 Returns
 • noise: 2darray
 Noise matrix, of dimensions size.
 
-132
+139
 
-3.4.10
+3.4.11
 
 sim.sim_1D(File, pv=False)
 
 Simulates a 1D NMR spectrum from the instructions written in File.
 The instructions on how to write the input file are reported in the caption of sim.load_sim_1D.
 Parameters
 • File: str
 Path to the input file location
 • pv: bool
 True for pseudo-Voigt model, False for Voigt model.
 Returns
 • fid: 1darray
 FID of the simulated spectrum.
 
-133
+140
 
-3.4.11
+3.4.12
 
 sim.sim_2D(File, states=True, alt=True, pv=False)
 
 Simulates a 2D NMR spectrum from the instructions written in File. The indirect dimension is
 sampled with FnMODE=States-TPPI as default.
 The instructions on how to write the input file are reported in the caption of sim.load_sim_2D.
 Parameters
@@ -3779,21 +3930,22 @@
 Set it to True to allow for correct spectral arrangement in the indirect dimension.
 • pv: bool
 True for pseudo-Voigt model, False for Voigt model.
 Returns
 • fid: 2darray
 FID of the simulated spectrum.
 
-134
+141
 
-3.4.12
+3.4.13
 
 sim.t_2Dgaussian(t1, t2, v1, v2, s1, s2, A=1, states=True, alt=True)
 
-Bidimensional gaussian peak. The working code requires states=True and alt=True.
+Bidimensional gaussian peak in the time domain. The working code requires states=True and
+alt=True.
 The signal is generated as follows:
 # States acquires twice the same point of the indirect dimension time domain
 t1[1::2] = t1[::2]
 # TPPI cycles the receiver phase of 90 degrees at each transient acquisition
 freq_1 = np.zeros(len(t1), dtype=’complex64’)
 for k in range(4):
 t1t = t1[k::4]
@@ -3807,34 +3959,34 @@
 
 Parameters
 • t1: 1darray
 Indirect evolution timescale
 • t2: 1darray
 Timescale of the direct dimension
 • v1: float
-Peak position in the indirect dimension
+Peak position in the indirect dimension, in Hz
 • v2: float
-Peak position in the direct dimension
+Peak position in the direct dimension, in Hz
 • s1: float
-Standard deviation in the indirect dimension
+Standard deviation in the indirect dimension, in rad/s
 • s2: float
-Standard deviation in the direct dimension
+Standard deviation in the direct dimension, in rad/s
 • A: float
 Intensity
 • states: bool
 Set to True for FnMODE = States-TPPI
 • alt: bool
 Set to True for FnMODE = States-TPPI
 Returns
 • S: 2darray
 2D Gaussian function.
 
-135
+142
 
-3.4.13
+3.4.14
 
 sim.t_2Dlorentzian(t1, t2, v1, v2, fwhm1, fwhm2, A=1, states=True,
 alt=True)
 
 Bidimensional Lorentzian peak. The working code requires states=True and alt=True.
 The signal is generated as follows:
 hwhm1 = fwhm1 / 2
@@ -3856,36 +4008,36 @@
 
 Parameters
 • t1: 1darray
 Indirect evolution timescale
 • t2: 1darray
 Timescale of the direct dimension
 • v1: float
-Peak position in the indirect dimension
+Peak position in the indirect dimension, in Hz
 • v2: float
-Peak position in the direct dimension
+Peak position in the direct dimension, in Hz
 • fwhm1: float
-Full-width at half maximum in the indirect dimension
+Full-width at half maximum in the indirect dimension, in rad/s
 • fwhm2: float
-Full-width at half maximum in the direct dimension
+Full-width at half maximum in the direct dimension, in rad/s
 • A: float
 Intensity
 • states: bool
 Set to True for 'FnMODE':'States-TPPI
 • alt: bool
 Set to True for 'FnMODE':'States-TPPI
 
-136
+143
 Returns
 • S: 2darray
 Lorentzian function.
 
-137
+144
 
-3.4.14
+3.4.15
 
 sim.t_2Dpvoigt(t1, t2, v1, v2, fwhm1, fwhm2, A=1, x_g=0.5,
 states=True, alt=True)
 
 Generates a 2D pseudo-voigt signal in the time domain. x_g states for the fraction of gaussianity,
 whereas A defines the overall amplitude of the total peak. Indexes '1' and '2' on the variables stand
 for 'F1' and 'F2', respectively.
@@ -3900,36 +4052,36 @@
 
 Parameters
 • t1: 1darray
 Indirect evolution timescale
 • t2: 1darray
 Timescale of the direct dimension
 • v1: float
-Peak position in the indirect dimension
+Peak position in the indirect dimension, in Hz
 • v2: float
-Peak position in the direct dimension
+Peak position in the direct dimension, in Hz
 • fwhm1: float
-Full-width at half maximum in the indirect dimension
+Full-width at half maximum in the indirect dimension, in rad/s
 • fwhm2: float
-Full-width at half maximum in the direct dimension
+Full-width at half maximum in the direct dimension, in rad/s
 • A: float
 Intensity
 • x_g: float
 Fraction of gaussianity
 • states: bool
 Set to True for FnMODE=States-TPPI
 • alt: bool
 Set to True for FnMODE=States-TPPI
 Returns
 • fid: 2darray
 2D Pseudo-Voigt function.
 
-138
+145
 
-3.4.15
+3.4.16
 
 sim.t_2Dvoigt(t1, t2, v1, v2, fwhm1, fwhm2, A=1, x_g=0.5, states=True
 alt=True)
 
 Generates a 2D Voigt signal in the time domain. x_g states for the fraction of gaussianity, whereas
 A defines the overall amplitude of the total peak. Indexes '1' and '2' on the variables stand for 'F1'
 and 'F2', respectively.
@@ -3968,144 +4120,144 @@
 
 Parameters
 • t1: 1darray
 Indirect evolution timescale
 • t2: 1darray
 Timescale of the direct dimension
 • v1: float
-Peak position in the indirect dimension
+Peak position in the indirect dimension, in Hz
 • v2: float
-Peak position in the direct dimension
+Peak position in the direct dimension, in Hz
 
-139
+146
 • fwhm1: float
-Full-width at half maximum in the indirect dimension
+Full-width at half maximum in the indirect dimension, in rad/s
 • fwhm2: float
-Full-width at half maximum in the direct dimension
+Full-width at half maximum in the direct dimension, in rad/s
 • A: float
 Intensity
 • x_g: float
 Fraction of gaussianity
 • states: bool
 Set to True for 'FnMODE':'States-TPPI
 • alt: bool
 Set to True for 'FnMODE':'States-TPPI
 Returns
 • S: 2darray
 Voigt function.
 
-140
+147
 
-3.4.16
+3.4.17
 
 sim.t_gaussian(t, u, s, A=1, phi=0)
 
 Gaussian function in the time domain.
 2 2
 
 g(x) = Aeiϕ ei2πut e−s t /2
 Parameters
 • t: 1darray
 Independent variable
 • u: float
-Peak position
+Peak position, in Hz
 • s: float
-Standard deviation
+Standard deviation, in rad/s
 • A: float
 Intensity
 • phi: float
 Phase, in radians
 Returns
 • S: 1darray
 Gaussian function.
 
-141
+148
 
-3.4.17
+3.4.18
 
 sim.t_lorentzian(t, u, fwhm, A=1, phi=0)
 
 Lorentzian function in the time domain.
 ℓ(x) = Aeiϕ ei2πut e−γt
 Parameters
 • t: 1darray
 Independent variable
 • u: float
-Peak position
+Peak position, in Hz
 • fwhm: float
-Full-width at half-maximum, Γ = 2γ
+Full-width at half-maximum, Γ = 2γ, in rad/s
 • A: float
 Intensity
 • phi: float
 Phase, in radians
 Returns
 • S: 1darray
 Lorentzian function.
 
-142
+149
 
-3.4.18
+3.4.19
 
 sim.t_pvoigt(t, u, fwhm, A=1, x_g=0, phi=0)
 
 Pseudo-Voigt function in the time domain:
 s(x) = xg g(x) + (1 − xg )ℓ(x)
 s = fwhm / 2.355
 S = A * (sim.t_gaussian(t, u, s, A=x_g, phi=phi) + sim.t_lorentzian(t, u, fwhm, A=1-x_g,
 phi=phi))
 
 Parameters
 • t: 1darray
 Independent variable
 • u: float
-Peak position
+Peak position, in Hz
 • fwhm: float
-Full-width at half-maximum
+Full-width at half-maximum, in rad/s
 • A: float
 Intensity
 • x_g: float
 Fraction of gaussianity
 • phi: float
 Phase, in radians
 Returns
 • S: 1darray
 Pseudo-Voigt function.
 
-143
+150
 
-3.4.19
+3.4.20
 
 sim.t_voigt(t, u, fwhm, A=1, x_g=0, phi=0)
 
 Voigt function in the time domain. The parameter x_g affects the linewidth of the lorentzian and
 gaussian contributions.
 s = fwhm / 2.355
 S = A * np.exp(1j*phi) * sim.t_gaussian(t, u/2, s*x_g) * sim.t_lorentzian(t, u/2,
 fwhm*(1-x_g))
 
 Parameters
 • t: 1darray
 Independent variable
 • u: float
-Peak position
+Peak position, in Hz
 • fwhm: float
-Full-width at half-maximum
+Full-width at half-maximum, in rad/s
 • A: float
 Intensity
 • x_g: float
 Fraction of gaussianity
 • phi: float
 Phase, in radians
 Returns
 • S: 1darray
 Voigt function.
 
-144
+151
 
-3.4.20
+3.4.21
 
 sim.water7(N, t2, vW, fwhm=300, A=1, spread=701.125)
 
 Simulates a feature like the water ridge in HSQC spectra, in the time domain.
 This signal is modelled as a gaussian signal which does not encode for any frequency in the
 indirect dimension, and whose chemical shift moves due to field drifts through the various transients
 according to a gaussian distribution. This signal is on-phase in the even transients and 90°-dephased
@@ -4114,24 +4266,24 @@
 • N: int
 Number of transients
 • t2: 1darray
 Time scale of the last temporal dimension.
 • vW: float
 Nominal peak position, in Hz.
 • fwhm: float
-Nominal full-width at half maximum of the peak.
+Nominal full-width at half maximum of the peak, in rad/s
 • A: float
 Signal intensity.
 • spread: float
 Standard deviation of the peak position distribution, in Hz.
 Returns
 • ridge: 2darray
 Matrix of the ridge.
 
-145
+152
 
 3.5
 
 FIT package
 
 Functions for performing fits.
 
@@ -4170,27 +4322,84 @@
 • Cf : 1darray
 coefficients of the baseline polynomion after the fit
 • s_labels : list
 legend entries for the single signals.
 
 class
 
-146
-Methods
-• __init__(self, ppm_scale, S, t_AQ, SFO1, o1p, nuc=None):
-Add common variables
-• iguess(self, input_file, limits=None):
-Create initial guess and writes the input file if not present
-• dofit(self, log_file=’fit.log’, output_file=’fit.out’, utol=0.5, vary_phi=False, vary_xg=False,
-res_hist_name=’histogram_of_residuals’, test_res=True):
-Fit the data, writes the output file and the log file
-• plot(self, what, name=None, s_labels=None, X_label=’δ F1 /ppm’, n_major_ticks=10):
-plot either the initial guess (what=’iguess’) or the fitted data (what=’fit’).
+153
+Methods:
+__init__(self, ppm_scale, S, t_AQ, SFO1, o1p, nuc=None)
+Initialize the class with common values.
+Parameters:
+• ppm_scale: 1darray
+ppm scale of the spectrum
+• S: 1darray
+Spectrum to be fitted
+• t_AQ: 1darray
+Acquisition timescale
+• SFO1: float
+Larmor frequency of the observed nucleus, in MHz
+• o1p: float
+Carrier position, in ppm
+• nuc: str
+Observed nucleus. Used to customize the x-scale of the figures.
+dofit(self, input_file=None, output_file=None, log_file=’fit.log’, on_cplex=True, **kwargs)
+Performs the fit using fit.voigt_fit with self.Vi and self.Ci as initial parameters.
+Parameters:
+• input_file: str
+Path to the input file. If None, self.input_file is used.
+• output_file: str
+Path to the output file. If None, self.output_file is used.
+• log_file: str
+Path to the log file.
+• on_cplex: bool
+Choose if to fit on the complex data (True) or on the real data (False).
+• kwargs: keyworded parameters
+See fit.voigt_fit.
+get_fit_lines(self, what=’fit’)
+Calculates the components, total fit curve and baseline used for iguess or fit. Calls fit.calc_fit_lines
+to do it.
 
-147
+154
+Parameters:
+• what: str
+’iguess’ or ’fit’. self.Vi and self.Ci or self.Vf and self.Cf are read, respectively.
+Returns:
+• signals: list of 1darray
+Components used for the fit
+• Total: 1darray
+Sum of all the signals
+• baseline: 1darray
+Baseline.
+iguess(self, input_file=None, limits=None)
+Reads, or computes, the initial guess for the fit. The window limits can be set interactively or
+specified through the parameter ’limits’.
+Parameters:
+• input_file: str or None
+Path to the input file. If None, the default name ’ppm1:ppm2.inp’ is set.
+• limits: tuple or None
+(lim_sx, lim_dx) in ppm. If None and input_file does not exist yet, they are set interactively.
+load_fit(self, output_file=None)
+Reads the output file of a fit and stores the values in self.Vf, self.Cf and self.limits. self.output_file
+is also replaced with output_file.
+Parameters:
+• output_file: str
+Path to the output file to be read
+plot(self, what=’fit’, s_labels=None, **kwargs)
+Makes a figure of either the initial guess or the fit. Calls figures.fitfigure.
+Parameters:
+• what: str
+’iguess’ or ’fit’. self.Vi and self.Ci or self.Vf and self.Cf are read, respectively.
+• s_labels: list
+Labels for the components that will appear in the legend of the figure.
+• kwargs: keyworded parameters
+See figures.fitfigure for the additional parameters.
+
+155
 
 3.5.2
 
 fit.ax_histogram(ax, data, nbins=100, density=True, f_lims=None,
 xlabel=None, x_symm=False, barcolor='tab:blue')
 
 Computes an histogram of data and tries to fit it with a gaussian lineshape. The parameters of the
@@ -4214,15 +4423,15 @@
 Color of the bars of the histogram
 Returns:
 • m : float
 Mean of data
 • s : float
 Standard deviation of data.
 
-148
+156
 
 3.5.3
 
 fit.bin_data(data0, nbins=100, density=True, x_symm=False)
 
 Computes the histogram of data, sampling it into nbins bins. If data is multidimensional, it is
 flattened.
@@ -4237,18 +4446,39 @@
 set it to True to make symmetric x-axis with respect to 0
 Returns:
 • hist: 1darray
 The bin intensity
 • bin_scale: 1darray
 Scale built with the mean value of the bin widths.
 
-149
+157
 
 3.5.4
 
+fit.build_2D_sgn(parameters, acqus, N=None, procs=None)
+
+Create a 2D signal according to the final parameters returned by fit.gen_iguess_2D. Process it
+according to procs.
+Parameters:
+• parameters: list or 2darray
+sequence of the parameters: u1, u2, fwhm1, fwhm2, I, x_g. Multiple components are allowed
+• acqus: dict
+2D-like acqus dictionary containing the acquisition timescales (keys: t1 and t2)
+• N: tuple of int
+Zero-filling values (F1, F2). Read only if procs is None
+• procs: dict
+2D-like procs dictionary.
+Returns:
+• peak: 2darray
+rr part of the generated signal
+
+158
+
+3.5.5
+
 fit.build_baseline(ppm_scale, C, L=None)
 
 Builds the baseline calculating the polynomion with the given coefficients, and summing up to the
 right position.
 Parameters:
 • ppm_scale: 1darray
 ppm scale of the spectrum
@@ -4256,17 +4486,17 @@
 Baseline coefficients. No baseline corresponds to False.
 • L: list
 List of window regions. If it is None, the baseline is built on the whole ppm_scale
 Returns:
 • baseline: 1darray
 Self-explanatory.
 
-150
+159
 
-3.5.5
+3.5.6
 
 fit.calc_fit_lines(ppm_scale, limits, t_AQ, SFO1, o1p, N, V, C=False)
 
 Given the values extracted from a fit input/output file, calculates the signals, the total fit function,
 and the baseline.
 Parameters:
 • ppm_scale: 1darray
@@ -4289,17 +4519,17 @@
 • sgn: list
 Voigt signals built using V
 • Total: 1darray
 sum of all the arrays in sgn
 • baseline: 1darray
 Polynomion built using C as coefficients. False if C is False.
 
-151
+160
 
-3.5.6
+3.5.7
 
 fit.dic2mat(dic, peak_names, ns, A=None)
 
 This is used to make the matrix of the parameters starting from a dictionary like the one produced
 by lmfit. The column of the total intensity is not added, unless the parameter A is passed. In this
 case, the third column (which is the one with the relative intesities) is corrected using the function
 misc.molfrac.
@@ -4312,17 +4542,17 @@
 number of signals to unpack
 • A : float or None
 Total intensity.
 Returns:
 • V : 2darray
 Matrix containing the parameters.
 
-152
+161
 
-3.5.7
+3.5.8
 
 fit.fit_int(y, y_c)
 
 Calculate the intensity according to the least square fit as:
 P
 obs · calc
 I= P
@@ -4332,17 +4562,17 @@
 Observed data.
 • y_c: ndarray
 Calculated data
 Returns:
 • I: float
 Calculated intensity
 
-153
+162
 
-3.5.8
+3.5.9
 
 fit.gaussian_fit(x, y)
 
 Fit y with a gaussian function, built using x as independent variable. The gaussian function is built
 with sim.f_gaussian.
 Parameters:
 • x : 1darray
@@ -4353,17 +4583,17 @@
 • u : float
 mean
 • s : float
 standard deviation
 • A : float
 Integral
 
-154
+163
 
-3.5.9
+3.5.10
 
 fit.gen_iguess(x, experimental, param, model, model_args=[])
 
 GUI for the interactive setup of a Parameters object to be used in a fitting procedure. Once you
 initialized the Parameters object with the name of the parameters and a dummy value, you are
 allowed to set the value, minimum, maximum and vary status through the textboxes given in the
 right column, and see their effects in real time. Upon closure of the figure, the Parameters object
@@ -4379,17 +4609,64 @@
 Function to be used for the generation of the fit model. param must be the first argument.
 • model_args: list
 List of args to be passed to model, after param
 Returns:
 • param: lmfit.Parameters Object
 Updated Parameters Object
 
-155
+164
 
-3.5.10
+3.5.11
+
+fit.gen_iguess_2D(ppm_f1, ppm_f2, tr1, tr2, u1, u2, acqus, fwhm0=100
+procs=None)
+
+Generate the initial guess for the fit of a 2D signal. The employes model is the one of a 2D Voigt
+signal, acquired with the States-TPPI scheme in the indirect dimension (i.e. sim.t_2DVoigt). The
+program allows for the inclusion of up to 10 components for the signal, in order to improve the fit.
+The acqus dictionary must contain the following keys:
+• t1: acquisition timescale in the indirect dimension (States)
+• t2: acquisition timescale in the direct dimension
+• SFO1: Larmor frequency of the nucleus in the indirect dimension
+• SFO2: Larmor frequency of the nucleus in the direct dimension
+• o1p: carrier position in the indirect dimension /ppm
+• o2p: carrier position in the direct dimension /ppm
+The signals will be processed according to the values in the procs dictionary, if given; otherwise,
+they will be just zero-filled up to the data size (i.e. (len(ppm_f1), len(ppm_f2)) ).
+Parameters:
+• ppm_f1: 1darray
+ppm scale for the indirect dimension
+• ppm_f2: 1darray
+ppm scale for the direct dimension
+• tr1: 1darray
+Trace of the original 2D peak in the indirect dimension
+• tr2: 1darray
+Trace of the original 2D peak in the direct dimension
+• u1: float
+Chemical shift of the original 2D peak in the indirect dimension /ppm
+• u2: float
+Chemical shift of the original 2D peak in the direct dimension /ppm
+• acqus: dict
+Dictionary of acquisition parameters
+• fwhm0: float
+Initial value for FWHM in both dimensions
+• procs: dict
+Dictionary of processing parameters
+
+165
+Returns:
+• final_parameters: 2darray
+Matrix of dimension (# signals, 6) that contains, for each row: ν1 (Hz), ν2 (Hz), Γ1 (Hz),
+Γ2 (Hz), A, xg
+• fit_interval: tuple of tuple
+Fitting window. ( (left_f1, right_f1), (left_f2, right_f2) )
+
+166
+
+3.5.12
 
 fit.get_region(ppmscale, S, rev=True)
 
 Interactively select the spectral region to be fitted. Returns the border ppm values.
 Parameters:
 • ppmscale: 1darray
 The ppm scale of the spectrum
@@ -4399,17 +4676,17 @@
 Choose if to reverse ppm scale and data (True) or not (False).
 Returns:
 • left: float
 Left border of the selected spectral window
 • right: float
 Right border of the selected spectral window
 
-156
+167
 
-3.5.11
+3.5.13
 
 fit.histogram(data, nbins=100, density=True, f_lims= None, xlabel=None, x_symm=False, name=None, barcolor='tab:blue')
 
 Computes an histogram of data and tries to fit it with a gaussian lineshape. The parameters of the
 gaussian function are calculated analytically directly from data.
 Parameters:
 • data : ndarray
@@ -4430,17 +4707,17 @@
 Color of the bars of the histogram
 Returns:
 • m : float
 Mean of data
 • s : float
 Standard deviation of data.
 
-157
+168
 
-3.5.12
+3.5.14
 
 fit.integrate(ppm0, data0, X_label=’$\delta\,$F1 /ppm’)
 
 Allows interactive integration of a NMR spectrum through a dedicated GUI. Returns the values as a
 dictionary, where the keys are the selected regions truncated to the 2nd decimal figure. The returned
 dictionary contains some predefined keys, as follows:
 • total: total integrated area
@@ -4463,17 +4740,17 @@
 Spectrum to be integrated.
 • X_label: str
 Label of the x-axis
 Returns:
 • f_vals: dict
 Dictionary containing the values of the integrated peaks.
 
-158
+169
 
-3.5.13
+3.5.15
 
 fit.integrate_2D(ppm_f1, ppm_f2, data, SFO1, SFO2, fwhm_1=200,
 fwhm_2=200, utol_1=0.5, utol_2=0.5, plot_result=False)
 
 Function to select and integrate 2D peaks of a spectrum, using dedicated GUIs. Calls integral_2D
 to do the dirty job.
 Parameters:
@@ -4497,17 +4774,17 @@
 Allowed tolerance for u_2 during the fit. (u_2-utol_2, u_2+utol_2)
 • plot_result: bool
 True to show how the program fitted the traces.
 Returns:
 • I: dict
 Computed integrals. The keys are ’<ppm f1>:<ppm f2>’ with 2 decimal figures.
 
-159
+170
 
-3.5.14
+3.5.16
 
 fit.interactive_smoothing(x, y, cmap=’RdBu’)
 
 Interpolate the given data with a 3rd-degree spline. Type the desired smoothing factor in the box
 and see the outcome directly on the figure. When the panel is closed, the smoothed function is
 returned.
 Parameters:
@@ -4523,17 +4800,17 @@
 • sy: 1darray
 Smoothed y
 • s_f: float
 Employed smoothing factor for the spline
 • weights: 1darray
 Weights vector
 
-160
+171
 
-3.5.15
+3.5.17
 
 fit.join_par(filenames, ppm_scale, joined_name=None)
 
 Load a series of parameters fit files. Join them together, returning a unique array of signal parameters,
 a list of coefficients for the baseline, and a list of tuples for the regions. Also, uses the coefficients
 and the regions to directly build the baseline according to the ppm windows.
 Parameters:
@@ -4550,17 +4827,17 @@
 • C: list
 Baseline polynomion coefficients. No baseline corresponds to False.
 • L: list
 List of window regions.
 • baseline: 1darray
 Baseline built from C and L.
 
-161
+172
 
-3.5.16
+3.5.18
 
 fit.make_iguess(S, ppm_scale, t_AQ, limits=None, SFO1=701.125,
 o1p=0, rev=True, name='i_guess.inp')
 
 Compute the initial guess for the quantitative fit of 1D NMR spectrum in an interactive manner.
 When the panel is closed, the values are saved in a file.
 Parameters:
@@ -4583,17 +4860,17 @@
 Returns:
 • V_f : 2darray
 matrix (# signals, parameters)
 • C_f : 1darray or False
 Coefficients of the polynomion to be used as baseline correction. If the 'baseline' checkbox in
 the interactive figure panel is not checked, C_f is False.
 
-162
+173
 
-3.5.17
+3.5.19
 
 fit.make_signal(t, u, s, k, x_g, phi, A, SFO1=701.125, o1p=0,
 N=None)
 
 Generates a Voigt signal using sim.t_voigt on the basis of the specified parameters. Then, makes
 the Fourier transform and returns it.
 Parameters:
@@ -4617,33 +4894,55 @@
 pulse carrier frequency, in ppm
 • N : int or None
 length of the final signal array. If None, the signal is not zero-filled before to be transformed.
 Returns:
 • sgn : 1darray
 generated signal in the frequency domain (just the real part).
 
-163
+174
 
-3.5.18
+3.5.20
+
+fit.peak_pick(ppm_f1, ppm_f2, data, coord_filename=’coord.tmp’)
+
+Make interactive peak-picking on 2D spectra. The position of the selected signals are saved in
+coord_filename. If coord_filename already exists, the new signals are appended at its bottom:
+nothing is overwritten. Calls misc.select_traces for the selection.
+Parameters:
+• ppm_f1: 1darray
+ppm scale for the indirect dimension
+• ppm_f2: 1darray
+ppm scale for the direct dimension
+• data: 2darray
+Spectrum to peak-pick. The dimension should match the scale sizes.
+• coord_filename: str
+Path to the file where to save the peak coordinates
+Returns:
+• coord: list
+List of (u2, u1) for each peak
+
+175
+
+3.5.21
 
 fit.print_par(V, C, limits=[None,None])
 
 Prints on screen the same thing that fit.write_par writes in a file.
 Parameters:
 • V : 2darray
 matrix (# signals, parameters)
 • C : 1darray or False
 Coefficients of the polynomion to be used as baseline correction. If it is False, they are not
 printed.
 • limits : tuple or None
 Trim limits for the spectrum (left, right).
 
-164
+176
 
-3.5.19
+3.5.22
 
 fit.read_par(filename)
 
 Reads the input file of the fit and returns the values.
 Parameters:
 • filename: str
 directory and name of the input file to be read
@@ -4652,17 +4951,17 @@
 matrix (# signals, parameters)
 • C : 1darray or False
 Coefficients of the polynomion to be used as baseline correction. If the corresponding flag is
 not found in the file, C_f is set to False.
 • limits : tuple
 Trim limits for the spectrum (left, right).
 
-165
+177
 
-3.5.20
+3.5.23
 
 fit.smooth_spl(x, y, s_f=1, size=0, weights=None)
 
 Fit the input data with a 3rd-order spline, given the smoothing factor to be applied.
 Parameters:
 • x: 1darray
 Location of the experimental points
@@ -4676,17 +4975,17 @@
 Array of weights of the spline points. None assign the same weight to all points in x.
 Returns:
 • x_s: 1darray
 Location of the spline data points.
 • y_s: 1darray
 Spline that fits the data.
 
-166
+178
 
-3.5.21
+3.5.24
 
 fit.test_residuals(R, nbins=100, density=False)
 
 Test the residuals of a fit to see if it was reliable. Returns two values: SYSDEV and Q_G.
 SYSDEV is inspired by Svergun’s Gnom, and it tells if there are systematic deviations basing on
 the number of sign changes in the residual. Optimal value must be 1. Values greater than 1 show
 positive bias, values lesser than 1 show negative bias.
@@ -4738,17 +5037,17 @@
 True to normalize the histogram, False otherwise.
 Returns:
 • SYSDEV : float
 Read full caption
 • Q_G : float
 Read full caption
 
-167
+179
 
-3.5.22
+3.5.25
 
 fit.voigt_fit(S, ppm_scale, V, C, t_AQ, limits=None, SFO1=701.125,
 o1p=0, utol=0.5, vary_phi=False, vary_xg=True, hist_name=None,
 write_out='fit.out', test_res=True)
 
 Fits an NMR spectrum with a set of signals, whose parameters are specifed in the V matrix. There
 is the possibility to use a baseline through the parameter C. The signals are computed in the time
@@ -4782,17 +5081,68 @@
 • C_f : 1darray or False
 Coefficients of the polynomion to be used as baseline correction, or just False if not used.
 • V_f : 2darray
 matrix (# signals, parameters) after the fit
 • result : lmfit.fit_result Object
 container of all information on the fit
 
-168
+180
 
-3.5.23
+3.5.26
+
+fit.voigt_fit_2D(x_scale, y_scale, data, parameters, lim_f1, lim_f2,
+acqus, N=None, procs=None, utol=(1,1), s1tol=(0,500), s2tol=(0,500),
+vary_xg=False, logfile=None)
+
+Function that performs the fit of a 2D peak using multiple components. The program reads a
+parameter matrix, that contains:
+u1 /ppm, u2 /ppm, fwhm1 /Hz, fwhm2 /Hz, I /a.u., x_g
+in each row. The number of rows corresponds to the number of components used for the computation
+of the final signal. The function returns the analogue version of the parameters matrix, but with the
+optimized values.
+Parameters:
+• x_scale: 1darray
+ppm_f2 of the spectrum, full
+• y_scale: 1darray
+ppm_f1 of the spectrum, full
+• data: 2darray
+spectrum, full
+• parameters: 1darray or 2darray
+Matrix (# signals, 6). Read main caption.
+• lim_f2: tuple
+Trimming limits for x_scale
+• lim_f1: tuple
+Trimming limits for y_scale
+• acqus: dict
+Dictionary of acquisition parameters.
+• N: tuple of ints
+len(y_scale), len(x_scale). Used only if procs is None
+• procs: dict
+Dictionary of processing parameters.
+• utol: tuple of floats
+Tolerance for the chemical shifts (utol_f1, utol_f2). Values will be set to u1 ±utol_f1, u2 ±
+utol_f2.
+• s1tol: tuple of floats
+Range of variations for the fwhm in f1, in Hz
+• s2tol: tuple of floats
+Range of variations for the fwhm in f2, in Hz
+• vary_xg: bool
+Choose if to fix the xg value or not
+• logfile: str or None
+Path to a file where to write the fit information. If it is None, they will be printed into standard
+output.
+
+181
+Returns:
+• out_parameters: 2darray
+parameters, but with the optimized values.
+
+182
+
+3.5.27
 
 fit.write_log(input_file, output_file, limits, V_i, C_i, V_f, C_f,
 result, runtime, test_res=True, log_file='fit.log')
 
 Write a log file with all the information of the fit.
 Parameters:
 • input_file: str
@@ -4815,17 +5165,17 @@
 • runtime: datetime.datetime Object
 Time taken for the fit
 • test_res: bool
 Choose if to test the residual with the fit.test_residual function (True) or not (False)
 • log_file: str
 Filename of the log file to be saved.
 
-169
+183
 
-3.5.24
+3.5.28
 
 fit.write_par(V, C, limits, filename='i_guess.inp')
 
 Write the parameters of the fit, whether they are input or output.
 Parameters:
 • V : 2darray
 matrix (# signals, parameters)
@@ -4834,95 +5184,874 @@
 appear in the written file.
 • limits : tuple
 Trim limits for the spectrum (left, right).
 • filename: str or TextIO Object
 directory and name of the file to be written, or directly a file opened with open and writing
 rights.
 
-170
+184
 
 3.6
 
 SPECTRA package
 
 All the classes in the Spectra module are automatically imported together with klassez itself.
-They are:
-• Spectrum_1D
-• pSpectrum_1D
-• Spectrum_2D
-• pSpectrum_2D
-• Pseudo_2D
-Classes of spectra with same dimensionality share more or less the same attributes. A list of them
-is reported in the following sections. Regarding the methods, please refer to the examples reported in
-the User guide section to understand how to use them, or use the functions help(), vars(), dir()
-to get detailed info on how they exactly work.
+Refer to the examples reported in the User guide section to understand how to use them, or use
+the functions help(), vars(), dir() to get detailed info on how they exactly work.
 
 3.6.1
 
-Spectrum_1D important attributes
+Spectra.Pseudo_2D
 
-Initialized attributes:
-• fid : 1darray
-FID of the experiment.
-• acqus : dict
-Dictionary containing the important acquisition parameters.
-• procs : dict
-Dictionary containing the important processing parameters.
-• ngdic : dict
-Dictionary containing all the information about your experiments, as returned by nmrglue.
-Available for non-simulated data only.
-Created after process():
-• freq : 1darray
-Frequency scale of the spectrum.
-• ppm : 1darray
-PPM scale of the spectrum.
-• S : 1darray
-Complex spectrum.
-• r : 1darray
-Real part of the spectrum.
-• i : 1darray
-Imaginary part of the spectrum.
-• F : fit.Voigt_Fit Object
-Fitting interface initialized with the current attributes of the class.
+class
 
-171
+Subclass of Spectrum_2D to simulate and handle pseudo-2D experiments.
+Methods:
+__init__(self, in_file, fid=None, pv=False, isexp=True)
+Initialize the class.
+Parameters:
+• in_file: str
+path to file to read, or to the folder of the spectrum
+• fid: 2darray or None
+Array that replaces self.fid.
+• pv: bool
+True if you want to use pseudo-voigt lineshapes for simulation, False for Voigt
+• isexp: bool
+True if this is an experimental dataset, False if it is simulated
+adjph(self, expno=0, p0=None, p1=None, pv=None)
+Adjusts the phases of the spectrum according to the given parameters, or interactively if they are
+left as default.
+Parameters:
+• expno: int
+Index of the experiment (python numbering) to use in the interactive panel
+• p0: float or None
+0-th order phase correction /°
+• p1: float or None
+1-st order phase correction /°
+• pv: float or None
+1-st order pivot /ppm
+cal(self, offset=[None, None], isHz=False)
+Calibration of the ppm and frequency scales according to a given value, or interactively. In this
+latter case, a reference peak must be chosen. Calls processing.calibration
+
+185
+Parameters:
+• offset: tuple
+(scale shift F1, scale shift F2)
+• isHz: tuple of bool
+True if offset is in frequency units, False if offset is in ppm
+calf1(self, value=None, isHz=False)
+Calibrates the ppm and frequency scale of the indirect dimension according to a given value, or
+interactively. Calls self.cal on F1 only.
+Parameters:
+• value: float or None
+scale shift value
+• isHz: bool
+True if offset is in frequency units, False if offset is in ppm
+calf2(self, value=None, isHz=False)
+Calibrates the ppm and frequency scale of the direct dimension according to a given value, or
+interactively. Calls self.cal on F2 only
+Parameters:
+• value: float or None
+scale shift value
+• isHz: bool
+True if offset is in frequency units, False if offset is in ppm
+convdta(self, scaling=1)
+Calls processing.convdta
+eae(self )
+Calls processing.EAE to shuffle the data and make a States-like FID. Sets self.eaeflag to 0.
+integrate(self, which=0, lims=None)
+Integrate the spectrum with a dedicated GUI. Calls processing.integral on each experiment, then
+saves the results in self.integrals. Therefore, the entries of self.integrals are sequences! If lims is not
+given, calls fit.integrate on the trace to select the regions to integrate.
+
+186
+Parameters:
+• which: int
+Experiment index to show in interactive panel
+• lims: tuple
+Region of the spectrum to integrate (ppm1, ppm2)
+inv_process(self )
+Performs the inverse processing of the spectrum according to the given parameters. Overwrites
+the S attribute!! Calls inv_xfb.
+mc(self )
+Computes the magnitude of the spectrum on self.S. Then, updates rr, ri, ir, ii.
+plot(self, Neg=True, lvl0=0.2, Y_label=”)
+Plots the real part of the spectrum.
+Parameters:
+• Neg: bool
+Plot (True) or not (False) the negative contours.
+• lvl0: float
+Starting contour value.
+• Y_label: str
+Custom label for vertical axis.
+plot_md(self, which=’all’, lims=None)
+Plot a number of experiments, superimposed.
+Parameters:
+• which: str
+List of experiment indexes, so that eval(which) is meaningful
+• lims: tuple
+Region of the spectrum to show (ppm1, ppm2)
+plot_stacked(self, which=’all’, lims=None)
+Plot a number of experiments, stacked.
+
+187
+Parameters:
+• which: str
+List of experiment indexes, so that eval(which) is meaningful
+• lims: tuple
+Region of the spectrum to show (ppm1, ppm2)
+process(self )
+Process only the direct dimension. Calls processing.fp on each transient
+projf1(self, a, b=None)
+Calculates the sum trace of the indirect dimension, from a to b in F2. Store the trace in the
+dictionary trf1 and as 1D spectrum in Trf1. The key is ’a’ or ’a:b’ Updates the Trf1[label].freq and
+Trf1[label].ppm with self.freq_f1 and self.ppm_f1 respectively.
+Parameters:
+• a: float
+ppm F2 value where to extract the trace.
+• b: float or None.
+If it is None, extract the trace in a. Else, sum from a to b in F2.
+projf2(self, a, b=None)
+Calculates the sum trace of the direct dimension, from a to b in F1. Store the trace in the
+dictionary trf2 and as 1D spectrum in Trf2. The key is ’a’ or ’a:b’
+Parameters:
+• a: float
+ppm F1 value where to extract the trace.
+• b: float or None.
+If it is None, extract the trace in a. Else, sum from a to b in F1.
+qfil(self, which=None, u=None, s=None)
+Gaussian filter to suppress signals. Tries to read self.procs[’qfil’], which is { ’u’: u, ’s’: s }
+Otherwise, these are set interactively by processing.interactive_qfil and then added to self.procs.
+Calls processing.qfil
+
+188
+Parameters:
+• which: int or None
+Index of the F2 trace to be used for interactive_qfil. If None, a suitable trace can be selected
+using misc.select_traces.
+• u: float
+Position /ppm
+• s: float
+Width (standard deviation) /ppm
+save_acqus(self, path=’sim_in_2D’)
+Write the acqus dictionary in a file. Calls misc.write_acqus_2D
+Parameters:
+• path: str
+Filename
+write_integrals(self, filename=’integrals.dat’)
+Write the integrals in a file named filename.
+Parameters:
+• filename: str
+name of the file where to write the integrals.
+write_ser(ser, acqus, path=None)
+Writes a real/complex array in binary format. Calls misc.write_ser. Be sure that acqus contains
+the BYTORDA and DTYPA keys. See misc.write_ser to understand the meaning of these values.
+Parameters:
+• ser: ndarray
+Array that you want to convert in binary format.
+• acqus: dict
+Dictionary of acquisition parameters. It must contain BYTORDA and DTYPA.
+• path: str
+Path where to save the binary file.
+xf1(self )
+Process only the indirect dimension. Transposes the spectrum in hypermode or normally if
+FnMODE != QF, then calls for processing.fp using self.procs[keys][0], finally transposes it back. The
+result is stored in self.S, then self.rr and self.ii are written. freq_f1 and ppm_f1 are assigned with
+the indexes of the transients.
+
+189
+xf2(self )
+Process only the direct dimension. Calls processing.fp using procs[keys][1] The result is stored in
+self.S, then self.rr and self.ii are written. freq_f1 and ppm_f1 are assigned with the indexes of the
+transients.
+
+190
 
 3.6.2
 
-Spectrum_2D important attributes
+Spectra.Spectrum_1D
 
-Initialized attributes:
-• fid : 2darray
-FID of the experiment.
-• acqus : dict
-Dictionary containing the important acquisition parameters.
-• procs : dict
-Dictionary containing the important processing parameters.
-• ngdic : dict
-Dictionary containing all the information about your experiments, as returned by nmrglue.
-Available for non-simulated data only.
-Created after process():
-• freq_f1 : 1darray
-Frequency scale of the indirect dimension of the spectrum.
-• freq_f2 : 1darray
-Frequency scale of the direct dimension of the spectrum.
-• ppm_f1 : 1darray
-PPM scale of the indirect dimension of the spectrum.
-• ppm_f2 : 1darray
-PPM scale of the direct dimension of the spectrum.
-• S : 2darray
-(Hyper)Complex spectrum, depending on the acquisition scheme of the indirect dimension.
-• rr : 2darray
-Real part of the spectrum.
-• ir : 2darray
-Imaginary part of the direct dimension, real part of the indirect dimension.
-• ri : 2darray
-Real part of the direct dimension, imaginary part of the indirect dimension.
-• ii : 2darray
-Imaginary part of the direct dimension, imaginary part of the indirect dimension.
-• Trf1: dict of pSpectrum_1D Objects
-Projection of the indirect dimension, obtained by invoking projf1(a,b). The keys of the
-dictionary are [f'{a}:{b}'].
-• Trf2: dict of pSpectrum_1D Objects
-Projection of the direct dimension, obtained by invoking projf2(a,b). The keys of the dictionary are [f'{a}:{b}'].
+class
+
+Class: 1D NMR spectrum
+Attributes:
+• datadir: str
+Path to the input file/dataset directory
+• fid: 1darray
+FID
+• acqus: dict
+Dictionary of acqusition parameters
+• ngdic: dict
+Created only if it is an experimental spectrum. Generated by nmrglue.bruker.read, contains
+all the information on the spectrometer and on the spectrum.
+• procs: dict
+Dictionary of processing parameters
+• S: 1darray
+Complex spectrum
+• r: 1darray
+Real part of the spectrum
+• i: 1darray
+Imaginary part of the spectrum
+• freq: 1darray
+Frequency scale of the spectrum, in Hz
+• ppm: 1darray
+ppm scale of the spectrum
+• F: fit.Voigt_Fit object
+Used for deconvolution. See fit.Voigt_fit.
+• baseline: 1darray
+Baseline of the spectrum.
+• integrals: dict
+Dictionary where to save the regions and values of the integrals.
+Methods:
+__init__(self, in_file, pv=False, isexp=True)
+Initialize the class. Simulation of the dataset (i.e. isexp=False) employs sim.sim_1D.
+
+191
+Parameters:
+• in_file: str
+path to file to read, or to the folder of the spectrum
+• pv: bool
+True if you want to use pseudo-voigt lineshapes for simulation, False for Voigt
+• isexp: bool
+True if this is an experimental dataset, False if it is simulated
+adjph(self, p0=None, p1=None, pv=None)
+Adjusts the phases of the spectrum according to the given parameters, or interactively if they are
+left as default. Calls for processing.ps
+Parameters:
+• p0: float or None
+0-th order phase correction /°
+• p1: float or None
+1-st order phase correction /°
+• pv: float or None
+1-st order pivot /ppm
+basl(self, basl_file=’spectrum.basl’, winlim=None)
+Correct the baseline of the spectrum, according to a pre-existing file or interactively. Calls
+processing.baseline_correction or processing.load_baseline
+Parameters:
+• basl_file: str
+Path to the baseline file. If it already exists, the baseline will be built according to this file;
+otherwise this will be the destination file of the baseline.
+• winlim: tuple or None
+Limits of the baseline. If it is None, it will be interactively set. If basl_file exists, it will be
+read from there. Else, (ppm1, ppm2).
+cal(self, offset=None, isHz=False)
+Calibrates the ppm and frequency scale according to a given value, or interactively. Calls processing.calibration
+Parameters:
+• offset: float or None
+scale shift value
+• isHz: bool
+True if offset is in frequency units, False if offset is in ppm
+
+192
+convdta(self, scaling=1)
+Call processing.convdta using self.acqus[’GRPDLY’]
+integrate(self, lims=None)
+Integrate the spectrum with a dedicated GUI. Calls fit.integrate and writes in self.integrals with
+keys [ppm1:ppm2]
+Parameters:
+• lims: tuple
+Integrates from lims[0] to lims[1]. If it is None, calls for interactive integration.
+inv_process(self )
+Performs the inverse processing of the spectrum according to the given parameters. Overwrites
+the S attribute!! Calls processing.inv_fp
+mc(self )
+Calculates the magnitude of the spectrum and overwrites self.S, self.r, self.i
+plot(self )
+Plots the real part of the spectrum.
+process(self, interactive=False)
+Performs the processing of the FID. The parameters are read from self.procs. Calls processing.interactive_fp or processing.fp using self.acqus and self.procs Writes the result is self.S, then
+unpacks it in self.r and self.i Calculates frequency and ppm scales. Also initializes self.F with
+fit.Voigt_Fit class using the current parameters
+Parameters:
+• interactive: bool
+True if you want to open the interactive panel, False to read the parameters from self.procs.
+qfil(self, u=None, s=None)
+Gaussian filter to suppress signals. Tries to read self.procs[’qfil’], which is { ’u’: u, ’s’: s }
+Otherwise, these are set interactively by processing.interactive_qfil and then added to self.procs.
+Calls processing.qfil
+Parameters:
+• u: float
+Position /ppm
+• s: float
+Width (standard deviation) /ppm
+
+193
+save_acqus(self, path=’sim_in_1D’)
+Write the acqus dictionary in a file. Calls misc.write_acqus_1D
+Parameters:
+• path: str
+Filename
+write_integrals(self, filename=’integrals.dat’)
+Write the integrals in a file named filename.
+Parameters:
+• filename: str
+name of the file where to write the integrals.
+write_ser(ser, acqus, path=None)
+Writes a real/complex array in binary format. Calls misc.write_ser. Be sure that acqus contains
+the BYTORDA and DTYPA keys. See misc.write_ser to understand the meaning of these values.
+Parameters:
+• ser: ndarray
+Array that you want to convert in binary format.
+• acqus: dict
+Dictionary of acquisition parameters. It must contain BYTORDA and DTYPA.
+• path: str
+Path where to save the binary file.
+
+194
+
+3.6.3
+
+Spectra.Spectrum_2D
+
+class
+
+Class: 2D NMR spectrum
+Attributes:
+• datadir: str
+Path to the input file/dataset directory
+• fid: 2darray
+FID
+• acqus: dict
+Dictionary of acqusition parameters
+• ngdic: dict
+Created only if it is an experimental spectrum. Generated by nmrglue.bruker.read, contains
+all the information on the spectrometer and on the spectrum.
+• procs: dict
+Dictionary of processing parameters
+• eaeflag: int
+If FnMODE is Echo-Antiecho, keeps track of the manipulation of the data so to not repeat the
+same process twice
+• S: 2darray
+Complex (or hypercomplex, depending on FnMODE) spectrum
+• rr: 2darray
+Real part F2, real part F1
+• ii: 2darray
+Imaginary part F2, imaginary part F1
+• ir: 2darray
+Real part F2, imaginary part F1. Only exist if F1 is acquired in phase-sensitive mode
+• ri: 2darray
+Imaginary part F2, real part F1. Only exist if F1 is acquired in phase-sensitive mode
+• freq_f1: 1darray
+Frequency scale of the indirect dimension, in Hz
+• freq_f2: 1darray
+Frequency scale of the direct dimension, in Hz
+• ppm_f1: 1darray
+ppm scale of the indirect dimension
+• ppm_f2: 1darray
+ppm scale of the direct dimension
+• trf1: dict
+Projections of the indirect dimension, as 1darrays. Keys: ’ppm_f2’ where they were taken
+• trf2: dict
+Projections of the direct dimension, as 1darrays. Keys: ’ppm_f1’ where they were taken
+
+195
+• Trf1: dict
+Projections of the indirect dimension, as pSpectrum_1D objects. Keys: ’ppm_f2’ where they
+were taken
+• Trf2: dict
+Projections of the direct dimension, as pSpectrum_1D objects. Keys: ’ppm_f1’ where they
+were taken
+• integrals: dict
+Dictionary where to save the regions and values of the integrals.
+Methods:
+__init__(self, in_file, pv=False, isexp=True, is_pseudo=False)
+Initialize the class.
+Parameters:
+• in_file: str
+path to file to read, or to the folder of the spectrum
+• pv: bool
+True if you want to use pseudo-voigt lineshapes for simulation, False for Voigt
+• isexp: bool
+True if this is an experimental dataset, False if it is simulated
+• is_pseudo: bool
+True if it is a pseudo-2D.
+adjph(self, p01=None, p11=None, pv1=None, p02=None, p12=None, pv2=None)
+Adjusts the phases of the spectrum according to the given parameters, or interactively if they are
+left as default. The non-interactive workflow is to apply processing.ps on F2, transpose according
+to FnMODE, apply processing.ps on F1, transpose back. If FnMODE is ’No’, the phase correction
+is applied only on F2, as it should be done in a pseudo-2D experiment. Once self.S was updated
+and unpacked, the phase values are added to the procs dictionary to keep track of multiple phase
+adjustments.
+Parameters:
+• p01: float or None
+0-th order phase correction /° of the indirect dimension
+• p11: float or None
+1-st order phase correction /° of the indirect dimension
+• pv1: float or None
+1-st order pivot /ppm of the indirect dimension
+• p02: float or None
+0-th order phase correction /° of the direct dimension
+
+196
+• p12: float or None
+1-st order phase correction /° of the direct dimension
+• pv2: float or None
+1-st order pivot /ppm of the direct dimension
+cal(self, offset=[None, None], isHz=False)
+Calibration of the ppm and frequency scales according to a given value, or interactively. In this
+latter case, a reference peak must be chosen. Calls processing.calibration
+Parameters:
+• offset: tuple
+(scale shift F1, scale shift F2)
+• isHz: tuple of bool
+True if offset is in frequency units, False if offset is in ppm
+calf1(self, value=None, isHz=False)
+Calibrates the ppm and frequency scale of the indirect dimension according to a given value, or
+interactively. Calls self.cal on F1 only.
+Parameters:
+• value: float or None
+scale shift value
+• isHz: bool
+True if offset is in frequency units, False if offset is in ppm
+calf2(self, value=None, isHz=False)
+Calibrates the ppm and frequency scale of the direct dimension according to a given value, or
+interactively. Calls self.cal on F2 only
+Parameters:
+• value: float or None
+scale shift value
+• isHz: bool
+True if offset is in frequency units, False if offset is in ppm
+convdta(self, scaling=1)
+Calls processing.convdta to compensate for the group delay. It does not always work, depends
+on TopSpin version and planets alignment.
+
+197
+Parameters:
+• scaling: float
+Scaling factor for processingconvdta.
+eae(self )
+Calls processing.EAE to shuffle the data and make a States-like FID. Sets self.eaeflag to 0.
+integrate(self, **kwargs)
+Integrates the spectrum with a dedicated GUI. Calls fit.integrate_2D
+Parameters:
+• kwargs: keyworded arguments
+Additional parameters for fit.integrate_2D
+inv_process(self )
+Performs the inverse processing of the spectrum according to the given parameters. Overwrites
+the S attribute!! Calls inv_xfb.
+mc(self )
+Computes the magnitude of the spectrum on self.S. Then, updates rr, ri, ir, ii.
+plot(self, Neg=True, lvl0=0.2)
+Plots the real part of the spectrum.
+Parameters:
+• Neg: bool
+Plot (True) or not (False) the negative contours.
+• lvl0: float
+Starting contour value with respect to the maximum of the spectrum
+process(self, interactive=False, **int_kwargs)
+Performs the full processing of the FID on both dimensions. The parameters are read from
+self.procs. If FnMODE is Echo-Antiecho and you did not call self.eae before, the FID is converted
+to States with processing.EAE before to start. If interactive is True, calls processing.interactive_xfb
+with int_kwargs, else calls processing.xfb. The complex/hypercomplex spectrum is stored in self.S,
+then unpacked into self.rr, self.ri, self.ir, self.ii. If FnMODE is Echo-Antiecho, a phase correction of
+-90 degrees is applied on the indirect dimension.
+
+198
+Parameters:
+• interactive: bool
+True if you want to open the interactive panel, False to read the parameters from self.procs.
+• int_kwargs: keyworded arguments
+Additional parameters for processing.interactive_xfb, if interactive=True.
+projf1(self, a, b=None)
+Calculates the sum trace of the indirect dimension, from a ppm to b ppm in F2. Store the trace
+in the dictionary trf1 and as 1D spectrum in Trf1. The key is ’a’ or ’a:b’ Calls misc.get_trace on
+self.rr with column=True
+Parameters:
+• a: float
+ppm F2 value where to extract the trace.
+• b: float or None.
+If it is None, extract the trace in a. Else, sum from a to b in F2.
+projf2(self, a, b=None)
+Calculates the sum trace of the direct dimension, from a ppm to b ppm in F1. Store the trace in
+the dictionary trf2 and as 1D spectrum in Trf2. The key is ’a’ or ’a:b’ Calls misc.get_trace on self.rr
+with column=False
+Parameters:
+• a: float
+ppm F1 value where to extract the trace.
+• b: float or None.
+If it is None, extract the trace in a. Else, sum from a to b in F1.
+qfil(self, which=None, u=None, s=None)
+Gaussian filter to suppress signals. Tries to read self.procs[’qfil’], which is { ’u’: u, ’s’: s }
+Otherwise, these are set interactively by processing.interactive_qfil and then added to self.procs.
+Calls processing.qfil
+Parameters:
+• which: int or None
+Index of the F2 trace to be used for interactive_qfil. If None, a suitable trace can be selected
+using misc.select_traces.
+• u: float
+Position /ppm
+• s: float
+Width (standard deviation) /ppm
+
+199
+save_acqus(self, path=’sim_in_2D’)
+Write the acqus dictionary in a file. Calls misc.write_acqus_2D
+Parameters:
+• path: str
+Filename
+write_integrals(self, filename=’integrals.dat’)
+Write the integrals in a file named filename.
+Parameters:
+• filename: str
+name of the file where to write the integrals.
+write_ser(ser, acqus, path=None)
+Writes a real/complex array in binary format. Calls misc.write_ser. Be sure that acqus contains
+the BYTORDA and DTYPA keys. See misc.write_ser to understand the meaning of these values.
+Parameters:
+• ser: ndarray
+Array that you want to convert in binary format.
+• acqus: dict
+Dictionary of acquisition parameters. It must contain BYTORDA and DTYPA.
+• path: str
+Path where to save the binary file.
+xf1(self )
+Process only the indirect dimension. Transposes the spectrum in hypermode or normally if
+FnMODE != QF, then calls for processing.fp using self.procs[keys][0], finally transposes it back. The
+result is stored in self.S, then self.rr and self.ii are written. freq_f1 and ppm_f1 are assigned with
+the indexes of the transients.
+xf2(self )
+Process only the direct dimension. Calls processing.fp using procs[keys][1] The result is stored in
+self.S, then self.rr and self.ii are written. freq_f1 and ppm_f1 are assigned with the indexes of the
+transients.
+
+200
+
+3.6.4
+
+Spectra.pSpectrum_1D
+
+class
+
+Subclass of Spectrum_1D that allows to handle processed 1D NMR spectra. Useful when dealing
+with traces of 2D spectra. Shares the same attributes with Spectrum_1D.
+Attributes:
+• acqus: dict
+Dictionary of acqusition parameters
+• ngdic: dict
+Created only if it is an experimental spectrum. Generated by nmrglue.bruker.read, contains
+all the information on the spectrometer and on the spectrum.
+• procs: dict
+Dictionary of processing parameters
+• S: 1darray
+Complex spectrum
+• r: 1darray
+Real part of the spectrum
+• i: 1darray
+Imaginary part of the spectrum
+• freq: 1darray
+Frequency scale of the spectrum, in Hz
+• ppm: 1darray
+ppm scale of the spectrum
+• F: fit.Voigt_Fit object
+Used for deconvolution. See fit.Voigt_fit.
+• baseline: 1darray
+Baseline of the spectrum.
+• integrals: dict
+Dictionary where to save the regions and values of the integrals.
+Methods:
+__init__(self, in_file, acqus=None, procs=None, istrace=False)
+Initialize the class.
+Parameters:
+• in_file: str or 1darray
+If istrace is True, in_file is the NMR spectrum. Else, it is the directory of the processed data.
+• acqus: dict or None
+If istrace is True, you must supply the associated ’acqus’ dictionary. Else, it is not necessary
+as it is read from the input directory
+
+201
+• procs: dict or None
+You can pass the dictionary of processing parameters, if you want. Otherwise, it is initialized
+with standard values.
+• istrace: bool
+Declare the object as trace extracted from a 2D (True) or as true experimental spectrum (False)
+adjph(self, p0=None, p1=None, pv=None)
+Adjusts the phases of the spectrum according to the given parameters, or interactively if they are
+left as default. Calls for processing.ps
+Parameters:
+• p0: float or None
+0-th order phase correction /°
+• p1: float or None
+1-st order phase correction /°
+• pv: float or None
+1-st order pivot /ppm
+basl(self, basl_file=’spectrum.basl’, winlim=None)
+Correct the baseline of the spectrum, according to a pre-existing file or interactively. Calls
+processing.baseline_correction or processing.load_baseline
+Parameters:
+• basl_file: str
+Path to the baseline file. If it already exists, the baseline will be built according to this file;
+otherwise this will be the destination file of the baseline.
+• winlim: tuple or None
+Limits of the baseline. If it is None, it will be interactively set. If basl_file exists, it will be
+read from there. Else, (ppm1, ppm2).
+cal(self, offset=None, isHz=False)
+Calibrates the ppm and frequency scale according to a given value, or interactively. Calls processing.calibration
+Parameters:
+• offset: float or None
+scale shift value
+• isHz: bool
+True if offset is in frequency units, False if offset is in ppm
+
+202
+convdta(self, scaling=1)
+Call processing.convdta using self.acqus[’GRPDLY’]
+integrate(self, lims=None)
+Integrate the spectrum with a dedicated GUI. Calls fit.integrate and writes in self.integrals with
+keys [ppm1:ppm2]
+Parameters:
+• lims: tuple
+Integrates from lims[0] to lims[1]. If it is None, calls for interactive integration.
+inv_process(self )
+Performs the inverse processing of the spectrum according to the given parameters. Overwrites
+the S attribute!! Calls processing.inv_fp
+mc(self )
+Calculates the magnitude of the spectrum and overwrites self.S, self.r, self.i
+plot(self )
+Plots the real part of the spectrum.
+process(self, interactive=False)
+Performs the processing of the FID. The parameters are read from self.procs. Calls processing.interactive_fp or processing.fp using self.acqus and self.procs Writes the result is self.S, then
+unpacks it in self.r and self.i Calculates frequency and ppm scales. Also initializes self.F with
+fit.Voigt_Fit class using the current parameters
+Parameters:
+• interactive: bool
+True if you want to open the interactive panel, False to read the parameters from self.procs.
+qfil(self, u=None, s=None)
+Gaussian filter to suppress signals. Tries to read self.procs[’qfil’], which is { ’u’: u, ’s’: s }
+Otherwise, these are set interactively by processing.interactive_qfil and then added to self.procs.
+Calls processing.qfil
+Parameters:
+• u: float
+Position /ppm
+• s: float
+Width (standard deviation) /ppm
+
+203
+save_acqus(self, path=’sim_in_1D’)
+Write the acqus dictionary in a file. Calls misc.write_acqus_1D
+Parameters:
+• path: str
+Filename
+write_integrals(self, filename=’integrals.dat’)
+Write the integrals in a file named filename.
+Parameters:
+• filename: str
+name of the file where to write the integrals.
+write_ser(ser, acqus, path=None)
+Writes a real/complex array in binary format. Calls misc.write_ser. Be sure that acqus contains
+the BYTORDA and DTYPA keys. See misc.write_ser to understand the meaning of these values.
+Parameters:
+• ser: ndarray
+Array that you want to convert in binary format.
+• acqus: dict
+Dictionary of acquisition parameters. It must contain BYTORDA and DTYPA.
+• path: str
+Path where to save the binary file.
+
+204
+
+3.6.5
+
+Spectra.pSpectrum_2D
+
+class
+
+Subclass of Spectrum_2D that allows to handle processed 2D NMR spectra. Reads the processed
+spectrum from Bruker.
+Attributes:
+• datadir: str
+Path to the input file/dataset directory
+• acqus: dict
+Dictionary of acqusition parameters
+• ngdic: dict
+Generated by nmrglue.bruker.read, contains all the information on the spectrometer and on
+the spectrum.
+• procs: dict
+Dictionary of processing parameters
+• S: 2darray
+Complex (or hypercomplex, depending on FnMODE) spectrum
+• rr: 2darray
+Real part F2, real part F1
+• ii: 2darray
+Imaginary part F2, imaginary part F1
+• ir: 2darray
+Real part F2, imaginary part F1. Only exist if F1 is acquired in phase-sensitive mode
+• ri: 2darray
+Imaginary part F2, real part F1. Only exist if F1 is acquired in phase-sensitive mode
+• freq_f1: 1darray
+Frequency scale of the indirect dimension, in Hz
+• freq_f2: 1darray
+Frequency scale of the direct dimension, in Hz
+• ppm_f1: 1darray
+ppm scale of the indirect dimension
+• ppm_f2: 1darray
+ppm scale of the direct dimension
+• trf1: dict
+Projections of the indirect dimension, as 1darrays. Keys: ’ppm_f2’ where they were taken
+• trf2: dict
+Projections of the direct dimension, as 1darrays. Keys: ’ppm_f1’ where they were taken
+• Trf1: dict
+Projections of the indirect dimension, as pSpectrum_1D objects. Keys: ’ppm_f2’ where they
+were taken
+
+205
+• Trf2: dict
+Projections of the direct dimension, as pSpectrum_1D objects. Keys: ’ppm_f1’ where they
+were taken
+• integrals: dict
+Dictionary where to save the regions and values of the integrals.
+Methods:
+__init__(self, in_file)
+Initialize the class.
+Parameters:
+• in_file: str
+Path to the spectrum. Here, the ’pdata/#’ folder must be specified.
+adjph(self, p01=None, p11=None, pv1=None, p02=None, p12=None, pv2=None)
+Adjusts the phases of the spectrum according to the given parameters, or interactively if they are
+left as default. The non-interactive workflow is to apply processing.ps on F2, transpose according
+to FnMODE, apply processing.ps on F1, transpose back. If FnMODE is ’No’, the phase correction
+is applied only on F2, as it should be done in a pseudo-2D experiment. Once self.S was updated
+and unpacked, the phase values are added to the procs dictionary to keep track of multiple phase
+adjustments.
+Parameters:
+• p01: float or None
+0-th order phase correction /° of the indirect dimension
+• p11: float or None
+1-st order phase correction /° of the indirect dimension
+• pv1: float or None
+1-st order pivot /ppm of the indirect dimension
+• p02: float or None
+0-th order phase correction /° of the direct dimension
+• p12: float or None
+1-st order phase correction /° of the direct dimension
+• pv2: float or None
+1-st order pivot /ppm of the direct dimension
+cal(self, offset=[None, None], isHz=False)
+Calibration of the ppm and frequency scales according to a given value, or interactively. In this
+latter case, a reference peak must be chosen. Calls processing.calibration
+
+206
+Parameters:
+• offset: tuple
+(scale shift F1, scale shift F2)
+• isHz: tuple of bool
+True if offset is in frequency units, False if offset is in ppm
+calf1(self, value=None, isHz=False)
+Calibrates the ppm and frequency scale of the indirect dimension according to a given value, or
+interactively. Calls self.cal on F1 only.
+Parameters:
+• value: float or None
+scale shift value
+• isHz: bool
+True if offset is in frequency units, False if offset is in ppm
+calf2(self, value=None, isHz=False)
+Calibrates the ppm and frequency scale of the direct dimension according to a given value, or
+interactively. Calls self.cal on F2 only
+Parameters:
+• value: float or None
+scale shift value
+• isHz: bool
+True if offset is in frequency units, False if offset is in ppm
+convdta(self, scaling=1)
+Calls processing.convdta to compensate for the group delay. It does not always work, depends
+on TopSpin version and planets alignment.
+Parameters:
+• scaling: float
+Scaling factor for processingconvdta.
+eae(self )
+Calls processing.EAE to shuffle the data and make a States-like FID. Sets self.eaeflag to 0.
+integrate(self, **kwargs)
+Integrates the spectrum with a dedicated GUI. Calls fit.integrate_2D
+
+207
+Parameters:
+• kwargs: keyworded arguments
+Additional parameters for fit.integrate_2D
+inv_process(self )
+Performs the inverse processing of the spectrum according to the given parameters. Overwrites
+the S attribute!! Calls inv_xfb.
+mc(self )
+Computes the magnitude of the spectrum on self.S. Then, updates rr, ri, ir, ii.
+plot(self, Neg=True, lvl0=0.2)
+Plots the real part of the spectrum.
+Parameters:
+• Neg: bool
+Plot (True) or not (False) the negative contours.
+• lvl0: float
+Starting contour value with respect to the maximum of the spectrum
+process(self, interactive=False, **int_kwargs)
+Performs the full processing of the FID on both dimensions. The parameters are read from
+self.procs. If FnMODE is Echo-Antiecho and you did not call self.eae before, the FID is converted
+to States with processing.EAE before to start. If interactive is True, calls processing.interactive_xfb
+with int_kwargs, else calls processing.xfb. The complex/hypercomplex spectrum is stored in self.S,
+then unpacked into self.rr, self.ri, self.ir, self.ii. If FnMODE is Echo-Antiecho, a phase correction of
+-90 degrees is applied on the indirect dimension.
+Parameters:
+• interactive: bool
+True if you want to open the interactive panel, False to read the parameters from self.procs.
+• int_kwargs: keyworded arguments
+Additional parameters for processing.interactive_xfb, if interactive=True.
+projf1(self, a, b=None)
+Calculates the sum trace of the indirect dimension, from a ppm to b ppm in F2. Store the trace
+in the dictionary trf1 and as 1D spectrum in Trf1. The key is ’a’ or ’a:b’ Calls misc.get_trace on
+self.rr with column=True
+
+208
+Parameters:
+• a: float
+ppm F2 value where to extract the trace.
+• b: float or None.
+If it is None, extract the trace in a. Else, sum from a to b in F2.
+projf2(self, a, b=None)
+Calculates the sum trace of the direct dimension, from a ppm to b ppm in F1. Store the trace in
+the dictionary trf2 and as 1D spectrum in Trf2. The key is ’a’ or ’a:b’ Calls misc.get_trace on self.rr
+with column=False
+Parameters:
+• a: float
+ppm F1 value where to extract the trace.
+• b: float or None.
+If it is None, extract the trace in a. Else, sum from a to b in F1.
+qfil(self, which=None, u=None, s=None)
+Gaussian filter to suppress signals. Tries to read self.procs[’qfil’], which is { ’u’: u, ’s’: s }
+Otherwise, these are set interactively by processing.interactive_qfil and then added to self.procs.
+Calls processing.qfil
+Parameters:
+• which: int or None
+Index of the F2 trace to be used for interactive_qfil. If None, a suitable trace can be selected
+using misc.select_traces.
+• u: float
+Position /ppm
+• s: float
+Width (standard deviation) /ppm
+save_acqus(self, path=’sim_in_2D’)
+Write the acqus dictionary in a file. Calls misc.write_acqus_2D
+Parameters:
+• path: str
+Filename
+write_integrals(self, filename=’integrals.dat’)
+Write the integrals in a file named filename.
+
+209
+Parameters:
+• filename: str
+name of the file where to write the integrals.
+write_ser(ser, acqus, path=None)
+Writes a real/complex array in binary format. Calls misc.write_ser. Be sure that acqus contains
+the BYTORDA and DTYPA keys. See misc.write_ser to understand the meaning of these values.
+Parameters:
+• ser: ndarray
+Array that you want to convert in binary format.
+• acqus: dict
+Dictionary of acquisition parameters. It must contain BYTORDA and DTYPA.
+• path: str
+Path where to save the binary file.
+xf1(self )
+Process only the indirect dimension. Transposes the spectrum in hypermode or normally if
+FnMODE != QF, then calls for processing.fp using self.procs[keys][0], finally transposes it back. The
+result is stored in self.S, then self.rr and self.ii are written. freq_f1 and ppm_f1 are assigned with
+the indexes of the transients.
+xf2(self )
+Process only the direct dimension. Calls processing.fp using procs[keys][1] The result is stored in
+self.S, then self.rr and self.ii are written. freq_f1 and ppm_f1 are assigned with the indexes of the
+transients.
```

### Comparing `klassez-0.1a1/klassez/figures.py` & `klassez-0.1a2/klassez/figures.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,18 +14,17 @@
 import seaborn as sns
 import nmrglue as ng
 import lmfit as l
 from datetime import datetime
 import warnings
 
 from . import fit, misc, sim, figures, processing
-#from .__init__ import CM
 s_colors=[ 'tab:cyan', 'tab:red', 'tab:green', 'tab:purple', 'tab:pink', 'tab:gray', 'tab:brown', 'tab:olive', 'salmon', 'indigo' ]
 
-from .config import CM, COLORS
+from .config import CM, COLORS, cron
 
 figsize_small = (3.59, 2.56)
 figsize_large = (15, 8)
 
 warnings.filterwarnings("ignore", message="No contour levels were found within the data range.")
 
 
@@ -238,16 +237,23 @@
     # Return the heatmap and the colorbar axis
     return im, cax
 
 
 
 def sns_heatmap(data, name=None):
     """
-    Computes a heatmap of "data", which is a matrix. 
-    Specify "name" if you want to save the figure.
+    Computes a heatmap of data, which is a matrix. 
+    This function employs the seaborn package.
+    Specify name if you want to save the figure.
+    ---------
+    Parameters:
+    - data: 2darray
+        Data of which to compute the heatmap. Make sure the entries are real numbers.
+    - name: str or None
+        Filename of the figure to be saved. If None, the figure is shown instead.
     """
     data = data.real
 
     fig = plt.figure()
     fig.set_size_inches(figsize_small)
     ax = fig.add_subplot(1,1,1)
     formatter = matplotlib.ticker.ScalarFormatter(useMathText=True)
@@ -365,26 +371,58 @@
         plt.savefig(name+'.png', format='png', dpi=600)
     else:
         fig.set_size_inches(figsize_large)
         misc.set_fontsizes(14)
         plt.show()
     plt.close()
 
-def figure2D(ppm_f2, ppm_f1, datax, xlims=None, ylims=None, cmap=None, c_fac=1.4, lvl=0.09, name=None, X_label='$\delta\ $ F2 /ppm', Y_label='$\delta\ $ F1 /ppm', lw=0.5, Negatives=False, cmapneg=None, n_xticks=10, n_yticks=10):
+def figure2D(ppm_f2, ppm_f1, datax, xlims=None, ylims=None, cmap=None, c_fac=1.4, lvl=0.09, name=None, X_label='$\delta\ $ F2 /ppm', Y_label='$\delta\ $ F1 /ppm', lw=0.5, Negatives=False, cmapneg=None, n_xticks=10, n_yticks=10, fontsize=10):
     """
-    Creates the contour plot of a 2D NMR spectrum. It requires:
-    - ppm_f2 and ppm_f1: ppm scales of the direct and indirect dimension, respectively;
-    - datax: the 2D NMR spectrum;
-    - xsx, xdx, ysx, ydx: axis limits;
-    - lvl: height respect to maximum at which the contour are computed;
-    - name: filename of the figure, if it has to be saved;
-    - X_label, Y_label: text of the X and Y axis;
-    - lw: linewidth of the contours
-    - Negatives: set it to "True" if you want to see the negative part of the spectrum, in red.
-    - spacex, spacey: spaces between the ticks for the axes
+    Makes a 2D contour plot. 
+    Allows for the buildup of modular figures. 
+    The contours are drawn according to the formula:
+        cl = contour_start * contour_factor ** np.arange(contour_num)
+    where contour_start = np.max(data) * lvl, contour_num = 16 and contour_factor = c_fac.
+    Increasing the value of c_fac will decrease the number of contour lines, whereas decreasing the value of c_fac will increase the number of contour lines.
+    -----------
+    Parameters:
+    - ppm_f2: 1darray
+        ppm scale of the direct dimension
+    - ppm_f1: 1darray
+        ppm scale of the indirect dimension
+    - datax: 2darray
+        the 2D NMR spectrum to be plotted
+    - xlims: tuple
+        limits for the x-axis (left, right). If None, the whole scale is used.
+    - ylims: tuple
+        limits for the y-axis (left, right). If None, the whole scale is used.
+    - cmap: matplotlib.cm Object
+        Colour for the contour
+    - c_fac: float
+        Contour factor parameter
+    - lvl: float
+        height with respect to maximum at which the contour are computed
+    - name: str
+        Filename for the figure.
+    - X_label: str
+        text of the x-axis label;
+    - Y_label: str
+        text of the y-axis label;
+    - lw: float
+        linewidth of the contours
+    - Negatives: bool
+        Choose if to plot the negative contours or not
+    - cmapneg: matplotlib.cm Object
+        Colour for the negative contours
+    - n_xticks: int
+        Number of numbered ticks on the x-axis of the figure
+    - n_yticks: int
+        Number of numbered ticks on the x-axis of the figure
+    - fontsize: float
+        Biggest font size in the figure.
     """
 
     swapped_scales = len(ppm_f2) == datax.shape[0] and len(ppm_f1) == datax.shape[1]
     if swapped_scales:
         raise AssertionError('Swapped scales!')
 
     if cmap is None:
@@ -422,29 +460,72 @@
 
     ax.set_xlabel(X_label)
     ax.set_ylabel(Y_label)
 
     misc.pretty_scale(ax, (xsx, xdx), axis='x', n_major_ticks=n_xticks)
     misc.pretty_scale(ax, (ysx, ydx), axis='y', n_major_ticks=n_yticks)
 
-    misc.set_fontsizes(ax, 10)
+    misc.set_fontsizes(ax, fontsize)
 
     if name:
         print( 'Saving '+name+'.png...')
         plt.savefig(name+'.png', format='png', dpi=600)
     else:
         fig.set_size_inches(figsize_large)
         misc.set_fontsizes(ax, 14)
         plt.show()
     plt.close()
     print( 'Done.')
 
 def ax2D(ax, ppm_f2, ppm_f1, datax, xlims=None, ylims=None, cmap=None, c_fac=1.4, lvl=0.1, lw=0.5, X_label='$\delta\,$F2 /ppm', Y_label='$\delta\,$F1 /ppm', title=None, n_xticks=10, n_yticks=10, fontsize=10):
     """
-    Adds a 2D plot in the 'ax' subplot. Allows for modular figures setup.
+    Makes a 2D contour plot like the one in figures.figure2D, but in a specified panel. 
+    Allows for the buildup of modular figures. 
+    The contours are drawn according to the formula:
+        cl = contour_start * contour_factor ** np.arange(contour_num)
+    where contour_start = np.max(data) * lvl, contour_num = 16 and contour_factor = c_fac.
+    Increasing the value of c_fac will decrease the number of contour lines, whereas decreasing the value of c_fac will increase the number of contour lines.
+    -----------
+    Parameters:
+    - ax: matplotlib.subplot Object
+        panel where to put the figure
+    - ppm_f2: 1darray
+        ppm scale of the direct dimension
+    - ppm_f1: 1darray
+        ppm scale of the indirect dimension
+    - datax: 2darray
+        the 2D NMR spectrum to be plotted
+    - xlims: tuple
+        limits for the x-axis (left, right). If None, the whole scale is used.
+    - ylims: tuple
+        limits for the y-axis (left, right). If None, the whole scale is used.
+    - cmap: matplotlib.cm Object
+        Colour for the contour
+    - c_fac: float
+        Contour factor parameter
+    - lvl: float
+        height with respect to maximum at which the contour are computed
+    - X_label: str
+        text of the x-axis label;
+    - Y_label: str
+        text of the y-axis label;
+    - lw: float
+        linewidth of the contours
+    - title: str
+        Figure title.
+    - n_xticks: int
+        Number of numbered ticks on the x-axis of the figure
+    - n_yticks: int
+        Number of numbered ticks on the x-axis of the figure
+    - fontsize: float
+        Biggest font size in the figure.
+    ---------
+    Returns:
+    - cnt: matplotlib.QuadContour object
+        Drawn contour lines
     """
 
     swapped_scales = len(ppm_f2) == datax.shape[0] and len(ppm_f1) == datax.shape[1]
     if swapped_scales:
         raise AssertionError('Swapped scales!')
 
     if cmap is None:
@@ -483,26 +564,46 @@
     return cnt
 
 
 
 
 def figure2D_multi(ppm_f2, ppm_f1, datax, xlims=None, ylims=None, lvl='default', name=None, X_label='$\delta\ $ F2 /ppm', Y_label='$\delta\ $ F1 /ppm', lw=0.5, Negatives=False, n_xticks=10, n_yticks=10, labels=None):
     """
-    Creates the contour plot of a 2D NMR spectrum. It requires:
-    - ppm_f2 and ppm_f1: ppm scales of the direct and indirect dimension, respectively;
-    - datax: the 2D NMR spectrum;
-    - xsx, xdx, ysx, ydx: axis limits;
-    - lvl: height respect to maximum at which the contour are computed;
-    - name: filename of the figure, if it has to be saved;
-    - X_label, Y_label: text of the X and Y axis;
-    - lw: linewidth of the contours
-    - Negatives: set it to "True" if you want to see the negative part of the spectrum, in red.
-    - spacex, spacey: spaces between the ticks for the axes
+    Generates the figure of multiple, superimposed spectra.
+    --------
+    Parameters:
+    - ppm_f2: 1darray
+        ppm scale of the direct dimension
+    - ppm_f1: 1darray
+        ppm scale of the indirect dimension
+    - datax: list
+        the 2D NMR spectra to be plotted
+    - xlims: tuple
+        limits for the x-axis (left, right). If None, the whole scale is used.
+    - ylims: tuple
+        limits for the y-axis (left, right). If None, the whole scale is used.
+    - lvl: "default" or list
+        height with respect to maximum at which the contour are computed. If "default", each spectrum is at 10% of maximum height. Otherwise, each entry of the list corresponds to the contour height of the respective spectrum.
+    - name: str
+        filename of the figure, if it has to be saved;
+    - X_label: str
+        text of the x-axis label;
+    - Y_label: str
+        text of the y-axis label;
+    - lw: float
+        linewidth of the contours
+    - Negatives: bool
+        set it to True if you want to see the negative part of the spectrum
+    - n_xticks: int
+        Number of numbered ticks on the x-axis of the figure
+    - n_yticks: int
+        Number of numbered ticks on the x-axis of the figure
+    - labels: list
+        entries of the legend. If None, the legend is not drawn.
     """
-
     nsp = len(datax)
     cmaps = [cm.Blues_r, cm.Reds_r, cm.Greens_r, cm.Greys_r, cm.Purples_r, cm.Oranges_r, cm.YlOrBr_r, cm.YlOrRd_r, cm.OrRd_r, cm.PuRd_r, cm.RdPu_r, cm.BuPu_r, cm.GnBu_r, cm.PuBu_r, cm.YlGnBu_r, cm.PuBuGn_r, cm.BuGn_r, cm.YlGn]
 
     # Labels of the spectra that appear in the legend
     if not labels:
         labels = []
         for k in range(nsp):
@@ -562,23 +663,49 @@
 
 
 
 
 
 def figure1D(ppm, data, norm=False, xlims=None, ylims=None, c='b', lw=0.5, name=None, X_label='$\delta\ $ F1 /ppm', Y_label='Intensity /a.u.', n_xticks=10, n_yticks=10, hideylabels=False):
     """
-    Creates the contour plot of a 2D NMR spectrum. It requires:
-    - ppm_f2 and ppm_f1: ppm scales of the direct and indirect dimension, respectively;
-    - datax: the 2D NMR spectrum;
-    - xlims, ylims: tuple of axis limits;
-    - lvl: height respect to maximum at which the contour are computed;
-    - name: filename of the figure, if it has to be saved;
-    - lw = linewith of the line
-    - X_label, Y_label: text of the X and Y axis;
-    - Negatives: set it to "True" if you want to see the negative part of the spectrum, in red.
+    Makes the figure of a 1D NMR spectrum.
+
+    The plot can be customized in a very flexible manner by setting the function keywords properly.
+    --------
+    Parameters:
+	- ppm: 1darray
+		ppm scale of the spectrum
+	- data: 1darray
+		spectrum to be plotted
+	- norm: bool
+		if True, normalizes the intensity to 1.
+	- xlims: list or tuple
+		Limits for the x-axis. If None, the whole scale is used.
+	- ylims: list or tuple
+		Limits for the y-axis. If None, the whole scale is used.
+	- c: str
+		Colour of the line.
+	- lw: float
+		 linewidth
+    - name: str or None
+        Filename for the figure to be saved. If None, the figure is shown instead.
+	- X_label: str
+		 text of the x-axis label;
+	- Y_label: str
+		 text of the y-axis label;
+	- n_xticks: int
+		 Number of numbered ticks on the x-axis of the figure
+	- n_yticks: int
+		 Number of numbered ticks on the x-axis of the figure
+	- fontsize: float
+		 Biggest font size in the figure.
+    --------
+    Returns:
+	- line: Line2D Object
+		Line object returned by plt.plot.
     """
     if np.iscomplexobj(data):
         data = np.copy(data.real)
 
     if xlims is None:
         xsx, xdx = max(ppm), min(ppm)
     else:
@@ -623,23 +750,52 @@
         plt.show()
     plt.close()
     print( 'Done.')
 
 
 def ax1D(ax, ppm, data, norm=False, xlims=None, ylims=None, c='b', lw=0.5, X_label='$\delta\ $ F1 /ppm', Y_label='Intensity /a.u.', n_xticks=10, n_yticks=10, label=None, fontsize=10):
     """
-    Creates the contour plot of a 2D NMR spectrum. It requires:
-    - ppm_f2 and ppm_f1: ppm scales of the direct and indirect dimension, respectively;
-    - datax: the 2D NMR spectrum;
-    - xlims, ylims: tuple of axis limits;
-    - lvl: height respect to maximum at which the contour are computed;
-    - name: filename of the figure, if it has to be saved;
-    - lw = linewith of the line
-    - X_label, Y_label: text of the X and Y axis;
-    - Negatives: set it to "True" if you want to see the negative part of the spectrum, in red.
+    Makes the figure of a 1D NMR spectrum, placing it in a given figure panel.
+    This allows the making of modular figures.
+
+    The plot can be customized in a very flexible manner by setting the function keywords properly.
+    --------
+    Parameters:
+    - ax: matplotlib.subplot Object
+        panel where to put the figure
+	- ppm: 1darray
+		ppm scale of the spectrum
+	- data: 1darray
+		spectrum to be plotted
+	- norm: bool
+		if True, normalizes the intensity to 1.
+	- xlims: list or tuple
+		Limits for the x-axis. If None, the whole scale is used.
+	- ylims: list or tuple
+		Limits for the y-axis. If None, the whole scale is used.
+	- c: str
+		Colour of the line.
+	- lw: float
+		 linewidth
+	- X_label: str
+		 text of the x-axis label;
+	- Y_label: str
+		 text of the y-axis label;
+	- n_xticks: int
+		 Number of numbered ticks on the x-axis of the figure
+	- n_yticks: int
+		 Number of numbered ticks on the x-axis of the figure
+	- label: str
+		 label to be put in the legend.
+	- fontsize: float
+		 Biggest font size in the figure.
+    --------
+    Returns:
+	- line: Line2D Object
+		Line object returned by plt.plot.
     """
     if np.iscomplexobj(data):
         data = np.copy(data.real)
 
     if xlims is None:
         xsx, xdx = max(ppm), min(ppm)
     else:
@@ -663,16 +819,14 @@
 
     misc.pretty_scale(ax, (xsx, xdx), axis='x', n_major_ticks=n_xticks)
     misc.pretty_scale(ax, (ysx, ydx), axis='y', n_major_ticks=n_yticks)
     misc.mathformat(ax, axis='y')
 
     ax.set_xlabel(X_label)
     misc.set_fontsizes(ax, fontsize)
-
-
     return line
 
 
 def figure1D_multi(ppm0, data0, xlims=None, ylims=None, norm=False, c=None, name=None, X_label='$\delta\ $ F1 /ppm', Y_label='Intensity /a.u.', n_xticks=10, n_yticks=10, hideylabels=False, labels=None):
     """
     Creates the superimposed plot of a series of 1D NMR spectra.
     -------
@@ -908,15 +1062,15 @@
 
     # Experimental and total
     ax.plot(ppm_scale[lim1:lim2], S[lim1:lim2], label='Experimental', lw=0.8, c='k')
     ax.plot(ppm_scale[lim1:lim2], y+Total, label = 'Fit', c='tab:blue', lw=0.7)
 
     # Single components
     for i in range(V.shape[0]):
-        s_plot, = ax.plot(ppm_scale[lim1:lim2], sgn[i][lim1:lim2].real, c=s_colors[i], lw=0.4, ls='--')
+        s_plot, = ax.plot(ppm_scale[lim1:lim2], sgn[i][lim1:lim2].real, c=COLORS[i], lw=0.4, ls='--')
         if bool(s_labels[i]):
             s_plot.set_label(s_labels[i])
 
     # Baseline
     if C is not False:
         ax.plot(ppm_scale[lim1:lim2], y, label = 'Baseline', lw=0.4, c='tab:orange', ls='-.')
 
@@ -924,30 +1078,50 @@
     misc.pretty_scale(ax, limits, axis='x', n_major_ticks=n_xticks)
 
     ax.set_xlabel(X_label)
     ax.set_ylabel('Intensity /a.u.')
 
     misc.mathformat(ax, axis='y')
 
-    ax.legend()
+    ax.legend(framealpha=0.2)
     # Save/show the figure
     if name:
-        misc.set_fontsizes(ax, 10)
+        misc.set_fontsizes(ax, 8)
         plt.savefig(name+'.png', dpi=600)
     else:
         fig.set_size_inches(figsize_large)
         misc.set_fontsizes(ax, 14)
         plt.show()
     plt.close()
 
 
 
 def stacked_plot(ppmscale, S, xlims=None, lw=0.5, name=None, X_label='$\delta\ $ F1 /ppm', Y_label='Normalized intensity /a.u.', n_xticks=10, labels=None):
     """
     Creates a stacked plot of all the spectra contained in the list S. Note that S MUST BE a list. All the spectra must share the same scale.
+    --------
+    Parameters:
+    - ppmscale: 1darray
+        ppm scale of the spectrum
+    - S: list
+        spectra to be plotted
+    - xlims: list or tuple
+        Limits for the x-axis. If None, the whole scale is used.
+    - lw: float
+        linewidth
+    - name: str
+        filename of the figure, if it has to be saved;
+    - X_label: str
+        text of the x-axis label;
+    - Y_label: str
+        text of the y-axis label;
+    - n_xticks: int
+        Number of numbered ticks on the x-axis of the figure
+    - labels: list
+        labels to be put in the legend.
     """
     nsp = len(S)                                # number of spectra in the lsit
     if not labels:                              # auto-builds the labels for the spectra if not specified
         labels=[]
         for k in range(nsp):
             labels.append(str(k+1))
     
@@ -995,27 +1169,26 @@
         plt.show()
     plt.close()
     print( 'Done.')
 
 
 def dotmd(ppmscale, S, labels=None, lw=0.8, n_xticks=10):
     """
-    Interactive display of multiple 1D spectra. They have to share the same scale.
-    -------
-    Parameters
-    - ppmscale: 1darray
-        ppm scale of the spectra
-    - S: list or 1darray or 2darray
-        spectra to be plotted. If it is a 2darray, the spectra to be plotted are the rows of S
+    Interactive display of multiple 1D spectra.
+    --------
+    Parameters:
+    - ppmscale: 1darray or list
+        ppm scale of the spectra. If only one scale is supplied, all the spectra are plotted using the same scale. Otherwise, each spectrum is plotted using its scale. 
+    - S: list
+        spectra to be plotted
     - labels: list
-        labels to be put in the legend. 
+        labels to be put in the legend.
     - n_xticks: int
         Number of numbered ticks on the x-axis of the figure
     """
-
     if isinstance(S, list):
         S = [S[w].real for w in range(len(S))]
     elif isinstance(S, np.ndarray):
         if len(S.shape) == 1:
             S = [S.real]
         elif len(S.shape) == 2:
             S = [S[w].real for w in range(S.shape[0])]
```

### Comparing `klassez-0.1a1/klassez/fit.py` & `klassez-0.1a2/klassez/fit.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,30 +17,36 @@
 import nmrglue as ng
 import lmfit as l
 from datetime import datetime
 import warnings
 
 from . import fit, misc, sim, figures, processing
 #from .__init__ import CM
-from .config import CM
+from .config import CM, COLORS, cron
 
 
 """
 Functions for performing fits.
 """
 
 s_colors=[ 'tab:cyan', 'tab:red', 'tab:green', 'tab:purple', 'tab:pink', 'tab:gray', 'tab:brown', 'tab:olive', 'salmon', 'indigo' ]
 
 def f_t1(t, A, B, T1):
-    # Function that models the buildup of magnetization due to T1 relaxation
+    """
+    Function that models the buildup of magnetization due to T1 relaxation:
+        $ f(t) = A (1 - e^{-t/T_1}) + B $
+    """
     f = A * (1 - np.exp(-t/T1) ) + B
     return f
 
 def f_t2(t, A, B, T2):
-    # Function that models the decay of magnetization due to T2 relaxation
+    """
+    Function that models the decay of magnetization due to T2 relaxation
+        $ f(t) = A e^{-t/T_2} + B $
+    """
     f = A * np.exp(-t/T2) + B
     return f
 
 def histogram(data, nbins=100, density=True, f_lims= None, xlabel=None, x_symm=False, name=None):
     """
     Computes an histogram of 'data' and tries to fit it with a gaussian lineshape.
     The parameters of the gaussian function are calculated analytically directly from 'data'
@@ -632,14 +638,206 @@
         print('{:<30} = {:+9.3e} | Optimal : 1'.format('Systematic deviation', SYSDEV)) 
         print('{:<30} = {:+9.3e} | Optimal : 1'.format('Gaussianity of residuals', Q_G)) 
         print('-' * 60)
 
     return V_f, C_f, result, runtime
 
 
+@cron
+def voigt_fit_2D(x_scale, y_scale, data, parameters, lim_f1, lim_f2, acqus, N=None, procs=None, utol=(1,1), s1tol=(0,500), s2tol=(0,500), vary_xg=False, logfile=None):
+    """
+    Function that performs the fit of a 2D peak using multiple components. 
+    The program reads a parameter matrix, that contains:
+        u1 /ppm, u2 /ppm, fwhm1 /Hz, fwhm2 /Hz, I /a.u., x_g
+    in each row. The number of rows corresponds to the number of components used for the computation of the final signal.
+    The function returns the analogue version of the parameters matrix, but with the optimized values.
+    --------
+    Parameters:
+    - x_scale: 1darray
+        ppm_f2 of the spectrum, full
+    - y_scale: 1darray
+        ppm_f1 of the spectrum, full
+    - data: 2darray
+        spectrum, full
+    - parameters: 1darray or 2darray
+        Matrix (# signals, 6). Read main caption.
+    - lim_f2: tuple
+        Trimming limits for x_scale
+    - lim_f1: tuple
+        Trimming limits for y_scale
+    - acqus: dict
+        Dictionary of acquisition parameters.
+    - N: tuple of ints
+        len(y_scale), len(x_scale). Used only if procs is None
+    - procs: dict
+        Dictionary of processing parameters.
+    - utol: tuple of floats
+        Tolerance for the chemical shifts (utol_f1, utol_f2). Values will be set to u1 +/- utol_f1, u2 +/- utol_f2
+    - s1tol: tuple of floats
+        Range of variations for the fwhm in f1, in Hz
+    - s2tol: tuple of floats
+        Range of variations for the fwhm in f2, in Hz
+    - vary_xg: bool
+        Choose if to fix the x_g value or not
+    - logfile: str or None
+        Path to a file where to write the fit information. If it is None, they will be printed into standard output.
+    -------
+    Returns:
+    - out_parameters: 2darray
+        parameters, but with the optimized values.
+    """
+
+    def f2min(param, n_sgn, x_scale, y_scale, data_exp, lim_f2, lim_f1):
+        """ 
+        Cost function.
+        --------
+        Parameters:
+        - param: lmfit.Parameters object
+            Fit parameters. See fit_2D caption.
+        - n_sgn: int
+            Number of signals
+        - x_scale: 1darray
+            ppm_f2 of the spectrum, full
+        - y_scale: 1darray
+            ppm_f1 of the spectrum, full
+        - data_exp: 2darray
+            spectrum trimmed around the peak of interest
+        - lim_f2: tuple
+            Trimming limits for x_scale
+        - lim_f1: tuple
+            Trimming limits for y_scale
+        --------
+        Returns:
+        - res: 2darray
+            Experimental -  calculated
+        """
+        # Extract dictionary of values from param
+        P = param.valuesdict()
+
+        # Organize the parameters into a matrix
+        in_parameters = np.array([[
+                P[f'u1_{i+1}'],
+                P[f'u2_{i+1}'],
+                P[f's1_{i+1}'],
+                P[f's2_{i+1}'],
+                P[f'k_{i+1}'] * P['A'],
+                P[f'xg_{i+1}'],
+                ] for i in range(n_sgn)])
+
+        # Feed the peaks to build_2D_sgn to make the calculated spectrum
+        calc_peak = fit.build_2D_sgn(in_parameters, acqus, N=N, procs=procs)
+        # Trim the calculated spectrum to the experimental one's sizes
+        xtrim, ytrim, data_calc = misc.trim_data_2D(x_scale, y_scale, calc_peak, lim_f2, lim_f1)
+        # Compute the residuals
+        res = data_exp - data_calc
+        return res
+
+    #---------------------------------------------------------------------------------------------
+
+    # Redirect the output to logfile, if logfile is given
+    if isinstance(logfile, str):    # Open the file in "append" mode
+        sys.stdout = open(logfile, 'a', buffering=1)
+    elif isinstance(logfile, io.TextIOWrapper): # Just redirect
+        sys.stdout = logfile
+
+    # Trim the spectrum according to the given limits
+    data_exp = misc.trim_data_2D(x_scale, y_scale, data, lim_f2, lim_f1)[-1]
+
+
+    # Organize parameters
+    parameters = np.array(parameters)
+    if len(parameters.shape) == 1:  # it means it is only one signal
+        parameters = parameters.reshape(1,-1)   # therefore transform in 1 x n matrix
+    n_sgn = parameters.shape[0]     # Number of signals: number of rows of parameters
+
+    # Express relative intensities in "molar fractions" and adjust the absolute intensity accordingly
+    k_values, A = misc.molfrac(parameters[...,4])   
+
+    # Initialize the Parameters object
+    param = l.Parameters()
+
+    param.add('A', value=A, vary=False)     # Absolute intensity
+    for i in range(n_sgn):
+        param.add(f'u1_{i+1}', value=parameters[i,0])   # chemical shift f1 /ppm
+        param.add(f'u2_{i+1}', value=parameters[i,1])   # chemical shift f2 /ppm
+        param.add(f's1_{i+1}', value=parameters[i,2])   # fwhm f1 /Hz
+        param.add(f's2_{i+1}', value=parameters[i,3])   # fwhm f2 /Hz
+        param.add(f'k_{i+1}', value=k_values[i])        # relative intensity
+        param.add(f'xg_{i+1}', value=parameters[i,5], min=0-1e-5, max=1+1e-5)   # Fraction of gaussianity
+    
+    # Set limits to u and s
+    u1tol, u2tol = utol # Unpack tolerances for chemical shifts
+    [param[f'u1_{i+1}'].set(min=param[f'u1_{i+1}'].value - u1tol) for i in range(n_sgn)]    # min u1
+    [param[f'u1_{i+1}'].set(max=param[f'u1_{i+1}'].value + u1tol) for i in range(n_sgn)]    # max u1
+    [param[f'u2_{i+1}'].set(min=param[f'u2_{i+1}'].value - u2tol) for i in range(n_sgn)]    # min u2
+    [param[f'u2_{i+1}'].set(max=param[f'u2_{i+1}'].value + u2tol) for i in range(n_sgn)]    # max u2
+    [param[f's1_{i+1}'].set(min=min(s1tol)) for i in range(n_sgn)]  # min fwhm1
+    [param[f's1_{i+1}'].set(max=max(s1tol)) for i in range(n_sgn)]  # max fwhm1
+    [param[f's2_{i+1}'].set(min=min(s2tol)) for i in range(n_sgn)]  # min fwhm2
+    [param[f's2_{i+1}'].set(max=max(s2tol)) for i in range(n_sgn)]  # max fwhm2
+    [param[f'k_{i+1}'].set(min=0) for i in range(n_sgn)]    # min rel int to 0
+    [param[f'k_{i+1}'].set(max=5) for i in range(n_sgn)]    # max rel int to 5
+    if vary_xg is False:    # fix it
+        [param[f'xg_{i+1}'].set(vary=False) for i in range(n_sgn)]
+        
+    # Initialize the fit
+    minner = l.Minimizer(f2min, param, fcn_args=(n_sgn, x_scale, y_scale, data_exp, lim_f2, lim_f1))
+    result = minner.minimize(method='leastsq', max_nfev=10000, xtol=1e-10, ftol=1e-10)
+
+    # Adjust relative and absolute intensities, then update the optimized Parameters object
+    k_opt, A_opt = misc.molfrac([result.params.valuesdict()[f'k_{i+1}'] * param['A'] for i in range(n_sgn)])
+    [result.params[f'k_{i+1}'].set(value=k_opt[i]) for i in range(n_sgn)]
+    result.params['A'].set(value=A_opt) 
+
+    def calc_uncert(param, n_sgn, keys_list=None):
+        """ Get the stderr from Parameters and organize them in a matrix. """
+        if keys_list is None:   # Take all of them
+            keys_list = list(set([f'{key.rsplit("_", 1)[0]}' for key in param.keys()]))
+
+        uncert = []
+        for i in range(n_sgn):
+            tmp_stderr = []
+            for key in keys_list:
+                tmp_key = f'{key}_{i+1}'
+                try:    # There might not be stderr (NaN)
+                    tmp_stderr.append(param[tmp_key].stderr)
+                except Exception as E: # Therefore append None instead of NaN
+                    print(E, tmp_key)
+                    tmp_stderr.append(None)
+            uncert.append(tmp_stderr)
+        uncert = np.array(uncert)
+        return uncert
+
+    # Parameters
+    keys_list = 'u1', 'u2', 's1', 's2', 'k', 'xg'
+    stderr = calc_uncert(result.params, n_sgn, keys_list)   # Uncertainties
+
+    # Get dictionary of parameters
+    popt = result.params.valuesdict()
+    # Organize them in a matrix
+    out_parameters = np.array([[
+        popt[f'u1_{i+1}'],
+        popt[f'u2_{i+1}'],
+        popt[f's1_{i+1}'],
+        popt[f's2_{i+1}'],
+        popt[f'k_{i+1}'] * popt['A'],   # Put absolute intensity of each component
+        popt[f'xg_{i+1}'],
+        ] for i in range(n_sgn)])
+
+    # Print the outcome of the fit
+    print(f'{result.message} Number of function evaluations: {result.nfev:5.0f}.\nEstimated uncertainties:')
+    print(f'{"#":<4s},', *[f'{key:>8s},' for key in keys_list]) 
+    for k in range(stderr.shape[0]):
+        print(f'{k+1:<4},', *[f'{value:8.3g},' if value is not None else f'{"None":>8s}' for value in stderr[k]]) 
+    print('')
+
+    return out_parameters
+
+# ----------------------------------------------------------------------------------------------------------
+
 
 def smooth_spl(x, y, s_f=1, size=0, weights=None):
     """
     Fit the input data with a 3rd-order spline, given the smoothing factor to be applied.
     -------
     Parameters:
     - x: 1darray
@@ -1813,15 +2011,15 @@
 
 # --------------------------------------------------------------------
 
 
 def test_residuals(R, nbins=100, density=False):
     """
     Test the residuals of a fit to see if it was reliable.
-    Returns two values: SYSDEV and Q_G.
+    Returns two values, SYSDEV and Q_G.
     SYSDEV is inspired by Svergun's Gnom, and it tells if there are systematic deviations basing on the number of sign changes in the residual. Optimal value must be 1.
     Q_G is to see the discrepancy between a gaussian function built with the mean and standard deviation of the residuals and the gaussian built fitting the histogram of the residuals. Values go from 0 (worst case) to 1 (best case).
     -------
     Parameters:
     - R : 1darray
         Array of the residuals
     - nbins : int
@@ -2009,39 +2207,56 @@
         coefficients of the baseline polynomion as initial guess
     - Vf : 2darray
         array with the values of the signals after the fit
     - Cf : 1darray
         coefficients of the baseline polynomion after the fit
     - s_labels : list
         legend entries for the single signals.
-    --------
-    Methods:
-    - __init__(self, ppm_scale, S, t_AQ, SFO1, o1p, nuc=None): 
-        Add common variables
-    - iguess(self, input_file, limits=None):
-        Create initial guess and writes the input file if not present
-    - dofit(self, log_file='fit.log', output_file='fit.out', utol=0.5, vary_phi=False, vary_xg=False, res_hist_name='histogram_of_residuals', test_res=True):
-        Fit the data, writes the output and log file
-    - plot(self, what, name=None, s_labels=None, X_label='$\delta\, $F1 /ppm', n_major_ticks=10):
-        plot either the initial guess or the fitted data
     """
 
     def __init__(self, ppm_scale, S, t_AQ, SFO1, o1p, nuc=None):
+        """
+        Initialize the class with common values.
+        --------
+        Parameters:
+        - ppm_scale: 1darray
+            ppm scale of the spectrum
+        - S: 1darray
+            Spectrum to be fitted
+        - t_AQ: 1darray
+            Acquisition timescale
+        - SFO1: float
+            Larmor frequency of the observed nucleus, in MHz
+        - o1p: float
+            Carrier position, in ppm
+        - nuc: str
+            Observed nucleus. Used to customize the x-scale of the figures.
+        """
         self.ppm_scale = ppm_scale
         self.S = S
         self.t_AQ = t_AQ
         self.SFO1 = SFO1
         self.o1p = o1p
         if nuc is None:
             self.X_label = '$\delta\,$ /ppm'
         elif isinstance(nuc, str):
             fnuc = misc.nuc_format(nuc)
             self.X_label = '$\delta$ ' + fnuc +' /ppm'
 
     def iguess(self, input_file=None, limits=None):
+        """
+        Reads, or computes, the initial guess for the fit.
+        The window limits can be set interactively or specified through the parameter 'limits'.
+        --------
+        Parameters:
+        - input_file: str or None
+            Path to the input file. If None, the default name 'ppm1:ppm2.inp' is set.
+        - limits: tuple or None
+            (lim_sx, lim_dx) in ppm. If None and input_file does not exist yet, they are set interactively.
+        """
         # If input_file is not given, set in_file_exist to False.
         # If input_file is passed as argument, check if there is already, and set in_file_exist accordingly.
         if input_file is None:
             in_file_exist = False
         else:
             in_file_exist = os.path.exists(input_file)
 
@@ -2051,38 +2266,54 @@
         else:                           # Make the initial guess interactively and save the file.
             # Get the limits interactively if they are not given, and the input file is to be created
             if limits is None:
                 self.limits = fit.get_region(self.ppm_scale, self.S)
             else:
                 self.limits = limits
             if input_file is None:      # If the input file name was not passed, set a default name
-                input_file = f'inp_{self.limits[0]:.2f}:{self.limits[1]:.2f}'
+                input_file = f'{self.limits[0]:.2f}:{self.limits[1]:.2f}.inp'
             self.Vi, self.Ci = fit.make_iguess(self.S, self.ppm_scale, self.t_AQ, self.limits, self.SFO1, self.o1p, name=input_file)
 
         self.input_file = input_file
         print(f'{input_file} loaded as input file.')
 
     def load_fit(self, output_file=None):
+        """
+        Reads the output file of a fit and stores the values in self.Vf, self.Cf and self.limits.
+        self.output_file is also replaced with output_file.
+        ---------
+        Parameters:
+        - output_file: str
+            Path to the output file to be read
+        """
         out_file_exist = os.path.exists(output_file)
         if out_file_exist is True:       # Read everything you need from the file
             self.Vf, self.Cf, self.limits = fit.read_par(output_file)
             self.output_file = output_file
             print(f'{output_file} loaded as output file.')
         else:
             raise NameError(f'{output_file} does not exist.')
 
     def dofit(self, input_file=None, output_file=None, log_file='fit.log', on_cplex=True, **kwargs):
         """
-        kwargs:
-        - utol
-        - vary_phi
-        - vary_xg
-        - test_res
-        - hist_name
+        Performs the fit using fit.voigt_fit with self.Vi and self.Ci as initial parameters.
+        --------
+        Parameters:
+        - input_file: str 
+            Path to the input file. If None, self.input_file is used.
+        - output_file: str 
+            Path to the output file. If None, self.output_file is used.
+        - log_file: str
+            Path to the log file.
+        - on_cplex: bool
+            Choose if to fit on the complex data (True) or on the real data (False).
+        - kwargs: keyworded parameters
+            See fit.voigt_fit. 
         """
+
         if input_file is None:
             input_file = self.input_file
         if output_file is None:
             output_file = f'out_{self.limits[0]:.2f}:{self.limits[1]:.2f}'
 
         self.output_file = output_file
         if np.iscomplexobj(self.S) and on_cplex:
@@ -2095,14 +2326,26 @@
                 write_out=self.output_file, **kwargs)
      
         fit.write_log(input_file=self.input_file, output_file=self.output_file,
                 limits=self.limits, V_i=self.Vi, C_i=self.Ci, V_f=self.Vf, C_f=self.Cf,
                 result=self._result, runtime=self._runtime, test_res=True, log_file=log_file)
 
     def plot(self, what='fit', s_labels=None, **kwargs):
+        """
+        Makes a figure of either the initial guess or the fit.
+        Calls figures.fitfigure.
+        --------
+        Parameters:
+        - what: str
+            'iguess' or 'fit'. self.Vi and self.Ci or self.Vf and self.Cf are read, respectively.
+        - s_labels: list
+            Labels for the components that will appear in the legend of the figure.
+        - kwargs: keyworded parameters
+            See figures.fitfigure for the additional parameters.
+        """
         if what == 'iguess':
             V = self.Vi
             C = self.Ci
         elif what == 'fit':
             V = self.Vf
             C = self.Cf
         limits = self.limits
@@ -2129,15 +2372,30 @@
             self.ibasl = joined[3]
         elif flag == 1:   #output
             self.Vf = joined[0]
             self.Cf = joined[1]
             self.fbasl = joined[3]
 
     def get_fit_lines(self, what='fit'):
-
+        """
+        Calculates the components, total fit curve and baseline used for iguess or fit.
+        Calls fit.calc_fit_lines to do it.
+        --------
+        Parameters:
+        - what: str
+            'iguess' or 'fit'. self.Vi and self.Ci or self.Vf and self.Cf are read, respectively.
+        --------
+        Returns:
+        - signals: list of 1darray
+            Components used for the fit
+        - Total: 1darray
+            Sum of all the signals
+        - baseline: 1darray
+            Baseline.
+        """
         if what == 'iguess':
             V = self.Vi
             C = self.Ci
         elif what == 'fit':
             V = self.Vf
             C = self.Cf
 
@@ -2261,7 +2519,1041 @@
     for cb in var_cb:
         cb.on_clicked(set_vary)
 
     plt.show()
 
     return param
 
+
+
+
+def peak_pick(ppm_f1, ppm_f2, data, coord_filename='coord.tmp'):
+    """
+    Make interactive peak_picking.
+    The position of the selected signals are saved in coord_filename.
+    If coord_filename already exists, the new signals are appended at its bottom: nothing is overwritten.
+    Calls misc.select_traces for the selection.
+    -------
+    Parameters:
+    - ppm_f1: 1darray
+        ppm scale for the indirect dimension
+    - ppm_f2: 1darray
+        ppm scale for the direct dimension
+    - data: 2darray
+        Spectrum to peak-pick. The dimension should match the scale sizes.
+    - coord_filename: str
+        Path to the file where to save the peak coordinates
+    -------
+    Returns:
+    - coord: list
+        List of (u2, u1) for each peak
+    """
+    # Check for the existence of coord_filename
+    if os.path.exists(coord_filename):
+        with open(coord_filename, 'r') as Q:
+            # number of already present signals: last linei, first value before tab
+            n_C = eval(Q.readlines()[-1].split('\t')[0])   
+        C = open(coord_filename, 'a', buffering=1)  
+    else:
+        C = open(coord_filename, 'w', buffering=1)
+        C.write(r'#'+'\t'+f'{"u2":^8s},{"u1":^8s}'+'\n')    # Header line
+        n_C = 0 
+
+    # Make peak_picking
+    coord = misc.select_traces(ppm_f1, ppm_f2, data)
+
+    # Update the fucking coord file
+    for k, obj in enumerate(coord):
+        C.write(f'{k+1+n_C}'+'\t'+f'{obj[0]:-8.3f},{obj[1]:-8.3f}'+'\n')
+    C.close()
+
+    return coord
+
+def gen_iguess_2D(ppm_f1, ppm_f2, tr1, tr2, u1, u2, acqus, fwhm0=100, procs=None):
+    """
+    Generate the initial guess for the fit of a 2D signal.
+    The employes model is the one of a 2D Voigt signal, acquired with the States-TPPI scheme in the indirect dimension (i.e. sim.t_2DVoigt).
+    The program allows for the inclusion of up to 10 components for the signal, in order to improve the fit.
+    The acqus dictionary must contain the following keys: 
+        > t1: acquisition timescale in the indirect dimension (States)
+        > t2: acquisition timescale in the direct dimension
+        > SFO1: Larmor frequency of the nucleus in the indirect dimension
+        > SFO2: Larmor frequency of the nucleus in the direct dimension
+        > o1p: carrier position in the indirect dimension /ppm
+        > o2p: carrier position in the direct dimension /ppm
+    The signals will be processed according to the values in the procs dictionary, if given; otherwise, they will be just zero-filled up to the data size (i.e. (len(ppm_f1), len(ppm_f2)) ). 
+    -------
+    Parameters:
+    - ppm_f1: 1darray
+        ppm scale for the indirect dimension
+    - ppm_f2: 1darray
+        ppm scale for the direct dimension
+    - tr1: 1darray
+        Trace of the original 2D peak in the indirect dimension
+    - tr2: 1darray
+        Trace of the original 2D peak in the direct dimension
+    - u1: float
+        Chemical shift of the original 2D peak in the indirect dimension /ppm
+    - u2: float
+        Chemical shift of the original 2D peak in the direct dimension /ppm
+    - acqus: dict
+        Dictionary of acquisition parameters
+    - fwhm0: float
+        Initial value for FWHM in both dimensions
+    - procs: dict
+        Dictionary of processing parameters
+    -------
+    Returns:
+    - final_parameters: 2darray
+        Matrix of dimension (# signals, 6) that contains, for each row: v1(Hz), v2(Hz), fwhm1(Hz), fwhm2(Hz), A, x_g
+    - fit_interval: tuple of tuple
+        Fitting window. ( (left_f1, right_f1), (left_f2, right_f2) )
+    """
+
+    ### FIRST OF ALL, THE FIGURE!
+    fig = plt.figure()
+    fig.set_size_inches(figures.figsize_large)
+    plt.subplots_adjust(left=0.05, right=0.65, top=0.90, bottom=0.10, wspace=0.2)
+    ax2, ax1 = [fig.add_subplot(1, 2, w+1) for w in range(2)]
+
+    ### INITIALIZE THE VALUES
+
+    # Values to be returned
+    final_parameters = []
+    fit_interval = None, None
+
+    #limits of the window
+    lim_f1 = u1 + 100/np.abs(acqus['SFO1']), u1 - 100/np.abs(acqus['SFO1'])
+    lim_f2 = u2 + 100/np.abs(acqus['SFO2']), u2 - 100/np.abs(acqus['SFO2'])
+
+    V = [{
+        'u1': u1,   # ppm
+        'u2': u2,   # ppm
+        'fwhm1': fwhm0, # Hz
+        'fwhm2': fwhm0, # Hz
+        #'k': 0.1,   # relative intensity
+        'k': 0.1,   # relative intensity
+        'x_g': 0.5, # fraction of gaussianity
+        } for w in range(10)]
+    I1 = processing.integral(tr1, x=ppm_f1, lims=lim_f1)[-1]
+    I2 = processing.integral(tr2, x=ppm_f2, lims=lim_f2)[-1]
+    A = (I1 + I2) / (2*np.pi*fwhm0)
+
+
+    # Sensitivity for mouse
+    sens = {
+        'u1': 0.25,   # ppm
+        'u2': 0.25,   # ppm
+        'fwhm1': 10, # Hz
+        'fwhm2': 10, # Hz
+        'k': 0.01,  # 1%
+        'x_g': 0.1, # 10%
+        'A': np.floor(np.log10(A)) - 1      # This goes according to order of magnitudes
+        }
+
+
+    # Copy initial values for reset
+    V_in = [dict(q) for q in V]
+    A_in = np.copy(A)
+    sens_in = dict(sens)
+
+    #conversion of the names from radio labels to dict keys
+    conv_r2d = {
+            r'$\delta$ /ppm': 'u',
+            r'$\Gamma$ /Hz': 'fwhm',
+            r'$k$': 'k',
+            r'$x_{g}$': 'x_g',
+            }
+
+    #--------------------------------------------------------------------------
+    ### SETUP OF THE INTERACTIVE FIGURE PANEL
+
+    # make boxes for widgets
+    tb2_boxes = [   # limits for the direct dimension
+            plt.axes([0.050, 0.025, 0.05, 0.03]),   # left
+            plt.axes([0.275, 0.025, 0.05, 0.03]),   # right
+            ]
+    tb1_boxes = [   # limits for the indirect dimension
+            plt.axes([0.370, 0.025, 0.05, 0.03]),   # left
+            plt.axes([0.600, 0.025, 0.05, 0.03]),   # right
+            ]
+
+    slider_box = plt.axes([0.68, 0.10, 0.01, 0.65])     # peak selector
+    peak_box = plt.axes([0.72, 0.45, 0.10, 0.3])        # radiobuttons
+    su_box = plt.axes([0.815, 0.825, 0.08, 0.075])      # increase sensitivity button
+    giu_box = plt.axes([0.894, 0.825, 0.08, 0.075])     # decrease sensitivity button
+    save_box = plt.axes([0.7, 0.825, 0.085, 0.04])      # SAVE button
+    reset_box = plt.axes([0.7, 0.865, 0.085, 0.04])     # RESET button
+    p_or_s_box = plt.axes([0.73, 0.78, 0.04, 0.03])     # F1 or F2 selector
+    check_box = plt.axes([0.85, 0.1, 0.1, 0.7])         # Peak checker
+    
+    # Make widgets
+    #   Buttons
+    up_button = Button(su_box, '$\\uparrow$', hovercolor = '0.975')         # increase sensitivity button
+    down_button = Button(giu_box, '$\\downarrow$', hovercolor = '0.975')    # decrease sensitivity button
+    save_button = Button(save_box, 'SAVE', hovercolor = '0.975')            # SAVE button
+    reset_button = Button(reset_box, 'RESET', hovercolor = '0.975')         # RESET button
+    
+    #   textboxes
+    TB1 = [TextBox(box, '', initial=f'{value:.2f}', textalignment='center') for box, value in zip(tb1_boxes, lim_f1)]   # set limits for F1
+    TB2 = [TextBox(box, '', initial=f'{value:.2f}', textalignment='center') for box, value in zip(tb2_boxes, lim_f2)]   # set limits for F2
+
+    #   Radiobuttons for parameter selection
+    peak_name = [r'$\delta$ /ppm', r'$\Gamma$ /Hz', r'$k$', r'$x_{g}$', r'$A$']         # Labels for the parameters
+    peak_radio = RadioButtons(peak_box, peak_name, active=2, activecolor='tab:blue')      # Actual radiobuttons
+    
+    #   Sliders
+    #       Peak selector
+    slider = Slider(ax = slider_box, label = 'Active\nSignal', valmin = 1, valmax = 10, valinit = 1, valstep = 1, orientation='vertical', color='tab:blue')
+    #       Ruler for slider
+    for i, H in enumerate(np.linspace(0.10, 0.75, 10)):
+        plt.text(0.685, H, '$-$', ha='center', va='center', fontsize=20, color=COLORS[i], transform=fig.transFigure)
+    #       Dimension selector
+    f1_or_f2 = Slider(p_or_s_box, 'F', valmin=1, valmax=2, valinit=2, valstep=1, track_color='tab:blue', color='tab:orange')
+
+    #   Checkbox: peak checker
+    check_name = [str(w+1) for w in range(10)]      # 1, 2, 3...
+    check_status = [False if w else True for w in range(10)]    # Only the first
+    check = CheckButtons(check_box, check_name, check_status)   # Make the checkbutton
+
+    #       Customize checkbox appearance
+    #       ... make boxes more squared
+    HBOX = check_box.dataLim.bounds[-1]
+    misc.edit_checkboxes(check, xadj=0, yadj=0.001, length=0.1, height=(HBOX-0.5*HBOX)/len(check_name), color=COLORS)
+
+    # Text that shows the current values of the parameters
+    head_print = plt.text(0.725, 0.4,
+            '{:9s}:'.format(r'$\delta$ F2') + f'{V[0]["u2"]:-9.2f}\n'+
+            '{:9s}:'.format(r'$\delta$ F1') + f'{V[0]["u1"]:-9.2f}\n'+
+            '{:9s}:'.format(r'$\Gamma$ F2') + f'{V[0]["fwhm2"]:-9.2f}\n'+
+            '{:9s}:'.format(r'$\Gamma$ F1') + f'{V[0]["fwhm1"]:-9.2f}\n'+
+            '{:9s}:'.format(r'$k$') + f'{V[0]["k"]:-9.2f}\n'+
+            '{:9s}:'.format(r'$x_g$') + f'{V[0]["x_g"]:-9.2f}\n'+
+            '{:9s}:'.format(r'$A$') + f'{A:-9.2e}\n',
+            ha='left', va='top', transform=fig.transFigure, fontsize=12, color=COLORS[0])
+
+    #--------------------------------------------------------------------------
+    # SLOTS
+    def reset(event):
+        """ Bring all parameters and sens to the starting values """
+        nonlocal V, A, sens
+        # Copy initial values for reset
+        V = [dict(q) for q in V_in]
+        A = np.copy(A_in)
+        sens = dict(sens_in)
+        [update(q) for q in range(10)]
+
+    def edit_lims(text):
+        """ Read the limits from the textboxes and change the scales accordingly.  """
+        nonlocal lim_f1, lim_f2
+        lim_f1 = [eval(TB.text) for TB in TB1]
+        lim_f2 = [eval(TB.text) for TB in TB2]
+        misc.pretty_scale(ax2, lim_f2, 'x')
+        misc.pretty_scale(ax1, lim_f1, 'x')
+        fig.canvas.draw()
+
+    def set_visibility(event):
+        """
+        Set the signals visible or invisible according to their status in the checkbutton.
+        Recomputes the total function considering only the active signals.
+        """
+        slider.set_val(eval(event))     # Moves the selector to the "new" peak for easier handling
+        for k, stat in enumerate(check.get_status()):
+            s1_plot[k].set_visible(stat)
+            s2_plot[k].set_visible(stat)
+
+        total_1 = np.sum([sgn_1[k] for k in range(len(V)) if check.get_status()[k]], axis=0)
+        t1_plot.set_ydata(total_1)
+        total_2 = np.sum([sgn_2[k] for k in range(len(V)) if check.get_status()[k]], axis=0)
+        t2_plot.set_ydata(total_2)
+        fig.canvas.draw()
+
+
+    def make_sgn_2D(values, acqus, N=None, procs=None):
+        """
+        Create a 2D signal according to the final parameters returned by make_iguess_2D.
+        -------
+        Parameters:
+        - final_parameters: list or 2darray
+            sequence of the parameters: u1, u2, fwhm1, fwhm2, I, x_g
+        - acqus: dict
+            2D-like acqus dictionary containing the acquisition timescales (keys t1 and t2)
+        - N: tuple of int
+            Zero-filling values (F1, F2). Not read if procs is not None
+        - procs: dict
+            2D-like procs dictionary.
+        -------
+        Returns:
+        - peaks: list of 2darray
+            rr part of the generated signals
+        """
+        # Shallow copy of acquisition timescales
+        t1 = np.copy(acqus['t1'])
+        t2 = np.copy(acqus['t2'])
+        # Organize the parameters
+        to_pass = [
+                misc.ppm2freq(values[0], acqus['SFO1'], acqus['o1p']),  # u1 from ppm to Hz
+                misc.ppm2freq(values[1], acqus['SFO2'], acqus['o2p']),  # u2 from ppm to Hz
+                values[2] * 2 * np.pi,    # fwhm1 from Hz to radians
+                values[3] * 2 * np.pi,    # fwhm2 from Hz to radians
+                values[4],  # Intensity
+                values[5],   # x_g
+                ]
+        signal = sim.t_2Dvoigt(t1, t2, *to_pass)    # Make the 2D signal
+
+        if procs is not None:   # Processing according to procs
+            peak, *_ = processing.xfb(signal, wf=procs['wf'], zf=procs['zf'])
+        else:   # just zero-fill before FT
+            peak, *_ = processing.xfb(signal, zf=N)     # Just zero-fill
+
+        # Extract the traces
+        tr_f1 = misc.get_trace(peak, ppm_f2, ppm_f1, a=values[1], column=True)  # F2 @ u1 ppm
+        tr_f2 = misc.get_trace(peak, ppm_f2, ppm_f1, a=values[0], column=False) # F1 @ u2 ppm
+
+        return tr_f1, tr_f2
+
+    def get_key2edit():
+        """ Makes the conversion between the radiobutton labels and the keys of V/ A """
+        F = f'{f1_or_f2.val}'   # F1 or F2
+        label = peak_radio.value_selected    # active parameter
+        if label in conv_r2d.keys():    # i.e. it is not A
+            key2edit = f'{conv_r2d[label]}'
+            if 'k' not in key2edit and 'x_g' not in key2edit:   # i.e. it is u or fwhm
+                key2edit += F   # add 1 for f1 or 2 for f2
+        else:
+            key2edit = 'A'
+        return key2edit
+
+    def update(s_idx):
+        """ 
+        Computes the s_idx-th 2D signal, extract the traces in F1 and F2, then redraws them.
+        Updates the total functions with the sum of the active signals.
+        """
+        nonlocal sgn_1, sgn_2
+        # Organize the parameters
+        values = [V[s_idx][f'{key}'] for key in ('u1', 'u2', 'fwhm1', 'fwhm2', 'k', 'x_g')]
+        values[-2] *= A
+        # Compute the 2D signal and extract the traces
+        sgn_1[s_idx], sgn_2[s_idx] = make_sgn_2D(values, acqus, N=(N1,N2), procs=procs)
+        
+        # Update the plots:
+        #   F1
+        s1_plot[s_idx].set_ydata(sgn_1[s_idx])  # update plot
+        total_1 = np.sum([sgn_1[k] for k in range(len(V)) if check.get_status()[k]], axis=0)
+        t1_plot.set_ydata(total_1.real)
+        #   F2
+        s2_plot[s_idx].set_ydata(sgn_2[s_idx])
+        total_2 = np.sum([sgn_2[k] for k in range(len(V)) if check.get_status()[k]], axis=0)
+        t2_plot.set_ydata(total_2.real)
+
+        redraw_text(0)      # Update the text with the new values
+        fig.canvas.draw()
+
+    def roll(event):
+        """ Slot for the mouse wheel """
+        nonlocal V, A
+        s_idx = slider.val - 1 # active signal
+        key2edit = get_key2edit()   # active parameter
+        if key2edit == 'A':     # move A
+            if event.button == 'up':
+                A += 10**sens['A']
+            elif event.button == 'down':
+                A -= 10**sens['A']
+        else:   # Move the selected parameter
+            if event.button == 'up':
+                V[s_idx][key2edit] += sens[key2edit]
+            elif event.button == 'down':
+                V[s_idx][key2edit] -= sens[key2edit]
+        # Safety check for FWHM
+        if V[s_idx]['fwhm1'] <= 1:
+            V[s_idx]['fwhm1'] = 1
+        if V[s_idx]['fwhm2'] <= 1:
+            V[s_idx]['fwhm2'] = 1
+        # Safety check for x_g
+        if V[s_idx]['x_g'] <= 0:
+            V[s_idx]['x_g'] = 0
+        elif V[s_idx]['x_g'] >= 1:
+            V[s_idx]['x_g'] = 1
+        update(s_idx)   # Redraw everything and update text
+
+    def up_sens(event):
+        """ Slot for the up-arrow button"""
+        nonlocal sens
+        key2edit = get_key2edit()
+        if key2edit == 'A': # increase it by one order of magnitude
+            sens['A'] += 1
+        else:    # double
+            sens[key2edit] *= 2
+
+    def down_sens(event):
+        """ Slot for the down-arrow button"""
+        nonlocal sens
+        key2edit = get_key2edit()
+        if key2edit == 'A':
+            sens['A'] -= 1  # decrease it by one order of magnitude
+        else:   # halve
+            sens[key2edit] /= 2
+
+    def redraw_text(event):
+        """ Updates the text according to the current values. Also changes its color. """
+        s_idx = slider.val - 1  # python numbering
+        value_string = '{:9s}:'.format(r'$\delta$ F2') + f'{V[s_idx]["u2"]:-9.2f}\n'+ '{:9s}:'.format(r'$\delta$ F1') + f'{V[s_idx]["u1"]:-9.2f}\n'+ '{:9s}:'.format(r'$\Gamma$ F2') + f'{V[s_idx]["fwhm2"]:-9.2f}\n'+ '{:9s}:'.format(r'$\Gamma$ F1') + f'{V[s_idx]["fwhm1"]:-9.2f}\n'+ '{:9s}:'.format(r'$k$') + f'{V[s_idx]["k"]:-9.2f}\n'+ '{:9s}:'.format(r'$x_g$') + f'{V[s_idx]["x_g"]:-9.2f}\n'+ '{:9s}:'.format(r'$A$') + f'{A:-9.2e}\n'
+        head_print.set_text(value_string)
+        head_print.set_color(COLORS[s_idx]) # color of the active signal
+        fig.canvas.draw()
+
+    def save(event):
+        """ Slot for the save button: store the current values into the final variables """
+        nonlocal final_parameters, fit_interval
+        final_parameters = [[   # u1, u2, fwhm1, fwhm2, k*A, x_g
+                    misc.ppm2freq(V[x]['u1'], acqus['SFO1'], acqus['o1p']),
+                    misc.ppm2freq(V[x]['u2'], acqus['SFO2'], acqus['o2p']),
+                    V[x]['fwhm1'],
+                    V[x]['fwhm2'],
+                    V[x]['k'] * A,
+                    V[x]['x_g'],
+                    ] for x in range(len(V)) if check.get_status()[x]]
+        # ( (L_F1, R_F1), (L_F2, R_F2) )
+        fit_interval = tuple([eval(x.text) for x in TB1]), tuple([eval(x.text) for x in TB2])
+
+    #--------------------------------------------------------------------------
+
+    N1, N2 = ppm_f1.shape[-1], ppm_f2.shape[-1]         # Zero-filling dimension
+    if procs is None:   # I do not care
+        proc1s, proc2s = None, None
+    else:   # Split it into two 1D-like procs dictionaries
+        proc1s, proc2s = misc.split_procs_2D(procs)
+
+    # Figure titles
+    ax2.set_title(f'F2 trace @ {u1:.1f} ppm')
+    ax1.set_title(f'F1 trace @ {u2:.1f} ppm')
+    
+    # red dashed line as marker for the initially selected chemical shifts
+    ax2.axvline(u2, c='r', lw=0.3, ls='--')
+    ax1.axvline(u1, c='r', lw=0.3, ls='--')
+
+    # Draw the experimental spectrum
+    ax2.plot(ppm_f2, tr2, c='k', lw=1.0, label='Exp.')
+    ax1.plot(ppm_f1, tr1, c='k', lw=1.0, label='Exp.')
+
+    # Initialize the simulated signals with the starting values
+    #   F1
+    sgn_1, sgn_2 = [], []
+    for k, Vline in enumerate(V_in):
+        # Organize parameters
+        values = [Vline[f'{key}'] for key in ('u1', 'u2', 'fwhm1', 'fwhm2', 'k', 'x_g')]
+        values[-2] *= A
+        # Build the 2D signal and extract the traces
+        tmp1, tmp2 = make_sgn_2D(values, acqus, N=(N1, N2), procs=procs)
+        sgn_1.append(tmp1)
+        sgn_2.append(tmp2)
+
+    s1_plot = []        # lines
+    for i in range(len(V)):
+        temp1, = ax1.plot(ppm_f1, sgn_1[i].real, c=COLORS[i], lw=1.0, ls='--')
+        s1_plot.append(temp1)
+        s1_plot[i].set_visible(check.get_status()[i])
+    total_1 = np.sum([sgn_1[k] for k in range(len(V)) if check.get_status()[k]], axis=0)    # spectrum
+    t1_plot, = ax1.plot(ppm_f1, total_1.real, label='Fit', c='blue', lw=1.0)    # line
+
+    s2_plot = []        # lines
+    for i in range(len(V)):
+        temp2, = ax2.plot(ppm_f2, sgn_2[i].real, c=COLORS[i], lw=1.0, ls='--')
+        s2_plot.append(temp2)
+        s2_plot[i].set_visible(check.get_status()[i])
+    total_2 = np.sum([sgn_2[k] for k in range(len(V)) if check.get_status()[k]], axis=0)    # spectrum
+    t2_plot, = ax2.plot(ppm_f2, total_2.real, label='Fit', c='blue', lw=1.0)    # line
+
+    # Fancy shit
+    #   x scales
+    ax2.set_xlabel(r'$\delta$ '+f'{misc.nuc_format(acqus["nuc2"])}'+r' /ppm')
+    ax1.set_xlabel(r'$\delta$ '+f'{misc.nuc_format(acqus["nuc1"])}'+r' /ppm')
+    misc.pretty_scale(ax2, lim_f2, 'x')
+    misc.pretty_scale(ax1, lim_f1, 'x')
+    for ax in (ax2, ax1):
+        # y scales
+        misc.pretty_scale(ax, ax.get_ylim(), 'y')
+        misc.mathformat(ax, 'y')
+        # Draw legend
+        ax.legend()
+        # Bigger fontsizes
+        misc.set_fontsizes(ax, 14)
+
+    # Connect widgets to the slots
+    #   Textboxes
+    [TB.on_submit(edit_lims) for TB in TB1]
+    [TB.on_submit(edit_lims) for TB in TB2]
+    #   Checkbox
+    check.on_clicked(set_visibility)
+    #   Slider
+    slider.on_changed(redraw_text)
+    #   Mouse scroll
+    fig.canvas.mpl_connect('scroll_event', roll)
+
+    #   up-down buttons
+    up_button.on_clicked(up_sens)
+    down_button.on_clicked(down_sens)
+
+    #   reset and save
+    reset_button.on_clicked(reset)
+    save_button.on_clicked(save)
+
+    # fill the return variables with the starting ones
+    save('initial values')
+
+    plt.show()
+    plt.close()
+
+    return final_parameters, fit_interval
+
+
+def build_2D_sgn(parameters, acqus, N=None, procs=None):
+    """
+    Create a 2D signal according to the final parameters returned by make_iguess_2D.
+    Process it according to procs.
+    -------
+    Parameters:
+    - parameters: list or 2darray
+        sequence of the parameters: u1, u2, fwhm1, fwhm2, I, x_g. Multiple components are allowed
+    - acqus: dict
+        2D-like acqus dictionary containing the acquisition timescales (keys t1 and t2)
+    - N: tuple of int
+        Zero-filling values (F1, F2). Read only if procs is None
+    - procs: dict
+        2D-like procs dictionary.
+    -------
+    Returns:
+    - peak: 2darray
+        rr part of the generated signal
+    """
+    parameters = np.array(parameters)
+    if len(parameters.shape) == 1:
+        parameters = parameters.reshape(1,-1)
+    # Get timescales from acqus
+    t1 = np.copy(acqus['t1'])
+    t2 = np.copy(acqus['t2'])
+    signals = []        # Time domain
+    for k, values in enumerate(parameters):
+        values[0] = misc.ppm2freq(values[0], acqus['SFO1'], acqus['o1p'])
+        values[1] = misc.ppm2freq(values[1], acqus['SFO2'], acqus['o2p'])
+        values[2] *= 2*np.pi    # fwhm1 from Hz to radians
+        values[3] *= 2*np.pi    # fwhm2 from Hz to radians
+        sgn = sim.t_2Dvoigt(t1, t2, *values)    # Make the signal in the time domain
+        signals.append(sgn)
+    signal = np.sum(signals, axis=0)    # Sum the components
+
+    if procs is not None: # Process the data according to procs
+        peak, *_ = processing.xfb(signal, wf=procs['wf'], zf=procs['zf'])
+    else:
+        peak, *_ = processing.xfb(signal, zf=N)     # Just zero-fill
+
+    return peak
+#----------------------------------------------------------------------------------------------------------------------
+
+class Voigt_Fit_2D:
+    """
+    Class that wraps methods for the fit of 2D spectra with a set of 2D Voigtian lines.
+    This is work in progress.
+    """
+    def __init__(self, ppm_f1, ppm_f2, data, acqus, procs=None, label_list=None):
+        """
+        Initialize the class with ppm scales, experimental spectrum, acqus and procs dictionaries.
+        -------
+        Parameters:
+        - ppm_f1: 1darray
+            ppm scale for the indirect dimension
+        - ppm_f2: 1darray
+            ppm scale for the direct dimension
+        - data: 2darray
+            Spectrum to fit. The dimension should match the scale sizes.
+        - acqus: dict
+            Dictionary of acquisition parameters
+        - procs: dict
+            Dictionary of processing parameters
+        - label_list: list
+            Labels for the peaks
+        """
+        self.ppm_f1 = np.copy(ppm_f1)
+        self.ppm_f2 = np.copy(ppm_f2)
+        self.data = np.copy(data)
+        self.acqus = dict(acqus)
+        if procs is None:
+            self.procs = None
+        else:
+            self.procs = dict(procs)
+        self.label_list = label_list
+
+    def plot(self, name=None, show_exp=True, dpi=600, **kwargs):
+        """ 
+        Draw a plot of the guessed/fitted peaks.
+        -------
+        Parameters:
+        - name: str or None
+            Filename for the figure. If it is None, the figure is shown.
+        - show_exp: bool
+            Choose if to plot the experimental spectrum or not
+        - dpi: int
+            Resolution of the saved image
+        - kwargs: keyworded arguments
+            Additional parameters to be passed to figures.ax2D.
+        """
+
+        # Generate the full spectrum to make the plot computationally less expensive
+        fitted_data = np.sum(self.peaks, axis=0)
+
+        # Make the figure
+        fig = plt.figure()
+        fig.set_size_inches(figures.figsize_large)
+        ax = fig.add_subplot(1,1,1)
+        if 'cmap' in kwargs.keys():
+            kwargs.pop('cmap')
+            
+        if show_exp:
+            if 'lvl' in kwargs.keys():
+                l_E = kwargs['lvl']
+                kwargs.pop('lvl')
+            else:
+                l_E = 0.1
+            # Plot experimental spectrum
+            figures.ax2D(ax, self.ppm_f2, self.ppm_f1, self.data, cmap=CM['Greys_r'], lvl=l_E, **kwargs)
+            m_E = np.max(self.data)
+            m_C = np.max(fitted_data)
+            l_C = l_E * m_E / m_C
+        else:
+            if 'lvl' in kwargs.keys():
+                l_C = kwargs['lvl']
+                kwargs.pop('lvl')
+            else:
+                l_C = 0.1
+
+        # Plot fitted spectrum
+        figures.ax2D(ax, self.ppm_f2, self.ppm_f1, fitted_data, cmap=CM['Greens_r'], lvl=l_C, **kwargs)
+        # Draw the labels of the fitted peaks according to coord and peak_labels
+        if 'fontsize' in kwargs.keys():
+            labelsize = kwargs['fontsize'] - 2
+        else:
+            labelsize = 8
+        self.draw_crossmarks(self.coord, ax, markersize=5, labelsize=labelsize, label_list=self.label_list)
+
+        # Visual shit
+        ax.set_xlabel(r'$\delta$ '+f'{misc.nuc_format(self.acqus["nuc2"])}'+r' /ppm')
+        ax.set_ylabel(r'$\delta$ '+f'{misc.nuc_format(self.acqus["nuc1"])}'+r' /ppm')
+        # Save/plot the figure
+        if name is None:
+            misc.set_fontsizes(ax, 14)
+            plt.show()
+        else:
+            plt.savefig(f'{name}.png', dpi=dpi)
+        plt.close()
+
+    @staticmethod
+    def draw_crossmarks(coord, ax, label_list=None, markersize=5, labelsize=8, markercolor='tab:blue', labelcolor='b'):
+        """
+        Draw crossmarks and peak labels on a figure.
+        -------
+        Parameters:
+        - ax: matplotlib.Subplot object
+            Subplot where to plot the crossmarks and the labels.
+        - label_list: list
+            Labels for the peaks. If None, they are computed as 1, 2, 3, ...
+        - markersize: int
+            Dimension of the crossmark
+        - labelsize: int
+            Fontsize for the labels
+        - markercolor: str
+            Color of the crossmark
+        - labelcolor: str
+            Color of the labels
+        """
+
+        for k, C in enumerate(coord):
+            x, y = C    # position of the crossmark
+            ax.plot(x, y, '+', c=markercolor, ms=markersize)    # Plot crossmark
+            # Draw the text on the top-right of the crossmark
+            if label_list is None:
+                ax.text(x, y, f'{k+1}', c=labelcolor, ha='left', va='bottom', fontsize=labelsize)
+            else:
+                ax.text(x, y, f'{label_list[k]}', c=labelcolor, ha='left', va='bottom', fontsize=labelsize)
+
+    def peak_pick(self, coord_filename='coord.tmp'):
+        """
+        Performs peak_picking by calling fit.peak_pick.
+        Saves the list of peak positions in the attribute coord
+        -------
+        Parameters:
+        - coord_filename: str
+            Path to the file where to save the peak coordinates
+        """
+        fit.peak_pick(self.ppm_f1, self.ppm_f2, self.data, coord_filename)
+
+    def load_coord(self, coord_filename='coord.tmp'):
+        """
+        Read the values from the coord filename and save them into the attribute "coord".
+        --------
+        Parameters:
+        - coord_filename: str
+            Path to the file to be read
+        """
+        f = open(coord_filename, 'r')
+        R = f.readlines()
+
+        coord = []
+        label_list = []
+        for k, line in enumerate(R):
+            if line[0] == '#' or line.isspace():    # Skip comments and empty lines
+                continue
+            else:   
+                x, y = eval(line.split('\t',2)[1].strip('\n'))  # second and third column
+                coord.append([x, y])
+                if len(line.split('\t',2)) > 2: # If there is the label
+                    label = line.split("\t",2)[-1].strip("\n")
+                    if not label.isspace():
+                        label_list.append(f'{label}')
+        # Store coord into the attribute coord
+        self.coord = coord
+        print(f'Loaded {coord_filename} as coord.')
+
+        # Update label_list, if there are labels in the coord file
+        if len(label_list) > 0:
+            self.label_list = label_list
+        if self.label_list is not None:
+            if len(self.label_list) < len(self.coord):
+                raise ValueError('The number of provided labels is not enough for the peaks.')
+
+    def draw_coord(self, filename=None, labelsize=8, dpi=600, **kwargs):
+        """
+        Makes a figure with the experimental dataset and the peak-picked signals as crosshairs.
+        --------
+        Parameters:
+        - filename: str or None
+            Filename for the figure to be saved. If None, it is shown instead.
+        - labelsize: float
+            Font size for the peak index
+        - dpi: int
+            Resolution of the saved image in dots per inches
+        - kwargs: keyworded arguments
+            Additional options for figures.ax2D
+        """
+
+        fig = plt.figure()
+        fig.set_size_inches(figures.figsize_large)
+        ax = fig.add_subplot(1,1,1)
+
+        figures.ax2D(ax, self.ppm_f2, self.ppm_f1, self.data, **kwargs)
+        self.draw_crossmarks(self.coord, ax, label_list=self.label_list, markersize=5, labelsize=labelsize, markercolor='tab:blue', labelcolor='b')
+        
+        ax.set_xlabel(r'$\delta$ '+f'{misc.nuc_format(self.acqus["nuc2"])}'+ r' /ppm')
+        ax.set_ylabel(r'$\delta$ '+f'{misc.nuc_format(self.acqus["nuc1"])}'+ r' /ppm')
+        misc.set_fontsizes(ax, 14)
+        if filename is None:
+            plt.show()
+        else:
+            plt.savefig(f'{filename}.png', dpi=dpi)
+        plt.close()
+
+
+    @cron
+    def make_peaks(self, idx, V):
+        """
+        Calculate the set of 2D peaks, given the matrix of their parameters and their index.
+        The array of indexes is required in order to recognize the different components that contribute to a single peak.
+        The attribute peaks of the class will be cleared and updated.
+        --------
+        Parameters:
+        - idx: 1darray
+            Array of indexes of the peaks.
+        - V: list or 2darray
+            List of parameters that describe the peaks.
+        """
+
+        self.peaks = []     # Clear peaks attribute
+        # Get the number of signals
+        if isinstance(V, np.ndarray):
+            n_sgn = V.shape[0]
+        elif isinstance(V, list):
+            n_sgn = len(V)
+
+        print('Calculation of the peaks from the input file.\nThis might take a while...')
+        for k in range(n_sgn):
+            peak_index = k + 1  # Peak index
+            # Read the whole file, append only the parameters labelled with peak_index 
+            tmp_par = [V[k] for k in range(n_sgn) if idx[k] == peak_index]
+            if len(tmp_par) == 0:   # No peaks found -> skip
+                del tmp_par
+                continue
+            # Compute the signal and put it into peaks
+            self.peaks.append(fit.build_2D_sgn(tmp_par, self.acqus, N=(len(self.ppm_f1), len(self.ppm_f2)), procs=self.procs))
+            del tmp_par # Clear memory
+        print('Done.', end=' ') # remove \n so that the runtime is shown in the same line
+
+
+    def load_iguess(self, filename='peaks.inp'):
+        """
+        Reads the initial guess file with the parameters of the peaks, separates the values and stores them into attributes.
+        In particular: 
+            > idx will contain the peak index (first column of the file), 
+            > Vi will contain [u1, u2, fwhm1, fwhm2, Im, x_g] for each peak,
+            > Wi will contain the fitting interval as ( (L_f1, R_f1), (L_f2, R_f2) )
+        --------
+        Parameters:
+        - filename: str
+            Path to the input file to be read
+        """
+
+        # Safety check: if filename does exist
+        if os.path.exists(filename): # open the file and reads the lines,
+            f = open(filename, 'r')
+            R = f.readlines()
+        else:   # raises error
+            raise NameError(f'{filename} does not exist.')
+
+        # Initialize empty attributes
+        self.idx = []
+        self.Vi = []
+        self.Wi = []
+
+        for k, line in enumerate(R):    # Loop on the lines of the file
+            if line[0] == r'#' or line.isspace():
+                continue    # Skip empty lines and comments
+            index, values, fit_interval = self._read_par_line(line)   
+            self.idx.append(index)
+            self.Vi.append(values)
+            self.Wi.append(fit_interval)
+        f.close()
+        self.make_peaks(self.idx, self.Vi)
+
+    def load_fit(self, filename='fit.out'):
+        """
+        Reads the file with the parameters of the fitted peaks, separates the values and stores them into attributes.
+        Then, uses these values to compute the peaks and save them into self.peaks.
+        In particular: 
+            > idx will contain the peak index (first column of the file), 
+            > Vf will contain [u1, u2, fwhm1, fwhm2, Im, x_g] for each peak,
+            > Wf will contain the fitting interval as ( (L_f1, R_f1), (L_f2, R_f2) )
+        --------
+        Parameters:
+        - filename: str
+            Path to the input file to be read
+        """
+
+        # Safety check: if filename does exist
+        if os.path.exists(filename): # open the file and reads the lines,
+            f = open(filename, 'r')
+            R = f.readlines()
+        else:   # raises error
+            raise NameError(f'{filename} does not exist.')
+
+        # Initialize empty attributes
+        self.idx = []
+        self.Vf = []
+        self.Wf = []
+
+        for k, line in enumerate(R):    # Loop on the lines of the file
+            if line[0] == r'#' or line.isspace():
+                continue    # Skip empty lines and comments
+            index, values, fit_interval = self._read_par_line(line)   
+            self.idx.append(index)
+            self.Vf.append(values)
+            self.Wf.append(fit_interval)
+        f.close()
+        self.make_peaks(self.idx, self.Vf)  # Update the peaks attribute
+
+    def iguess(self, filename='peaks.inp', start_index=1, only_edit=None, fwhm0=100, overwrite=False, auto=False):
+        """
+        Make the initial guess for all the peaks.
+        ---------
+        Parameters:
+        - filename: str
+            Path to the file where the peak parameters will be written
+        - start_index: int
+            Index of the first peak to be guessed. 
+        - only_edit: sequence of ints or None
+            Index of the peak that have to be guessed interactively. The ones that do not appear here are guessed automatically.
+        - fwhm0: float
+            Default value for fwhm in both dimension for automatic guess
+        - overwrite: bool
+            Choose if to overwrite the file or append the new peaks at the bottom
+        - auto: bool
+            Allow automatic guess for the peaks. To be used in conjunction with only_edit: if auto is False, all the peaks are guessed interactively!
+        ----------
+        """
+        def auto_val(ppm_f1, ppm_f2, tr1, tr2, u1, u2, fwhm0, acqus):
+            """ Compute initial guess automatically """
+            # Limits
+            lim_f1 = u1 + 100/np.abs(acqus['SFO1']), u1 - 100/np.abs(acqus['SFO1'])
+            lim_f2 = u2 + 100/np.abs(acqus['SFO2']), u2 - 100/np.abs(acqus['SFO2'])
+            interval = lim_f1, lim_f2
+            # Parameters
+            parameters = [[   # u1, u2, fwhm1, fwhm2, k*A, x_g
+                misc.ppm2freq(u1, acqus['SFO1'], acqus['o1p']), # v1 /Hz
+                misc.ppm2freq(u2, acqus['SFO2'], acqus['o2p']), # v2 /Hz
+                fwhm0,  # fwhm1 /Hz
+                fwhm0,  # fwhm2 /Hz
+                1,     # I
+                0.5,    # x_g
+                ]] 
+            # Integral
+            """
+            _, _, data_exp = misc.trim_data_2D(ppm_f2, ppm_f1, self.data, lim_f2, lim_f1)
+            data_calc = fit.build_2D_sgn(parameters, acqus, N=(len(tr1), len(tr2)), procs=self.procs)
+            _, _, data_calc = misc.trim_data_2D(ppm_f2, ppm_f1, data_calc, lim_f2, lim_f1)
+            #A0 = fit.fit_int(data_exp.flatten(), data_calc.flatten())
+            """
+            A0 = np.max(self.data) / np.prod(self.data.shape)**0.5
+            parameters[0][-2] = A0
+            
+            return parameters, interval
+        #-------------------------------------------------------------------------------
+
+        if os.path.exists(filename) and overwrite is False:    # append next peaks 
+            f = open(filename, 'a', buffering=1)
+        else:   # create a new file
+            f = open(filename, 'w', buffering=1)
+            self._write_head_line(f)
+
+        # Make the generator where to loop on peaks
+        def extract(coord):
+            """ Generator: yields the chemical shifts and the traces onto which to loop """
+            for x, y in coord:   # u2, u1
+                tr1 = misc.get_trace(self.data, self.ppm_f2, self.ppm_f1, x, column=True)  # F1 @ u2 ppm
+                tr2 = misc.get_trace(self.data, self.ppm_f2, self.ppm_f1, y, column=False) # F2 @ u1 ppm
+                yield (y, tr1), (x, tr2)    # (u1, f1), (u2, f2)
+        peaks_coord = extract(self.coord)   # Call the generator
+
+        # Start looping
+        peak_index = 1
+        for TR1, TR2 in peaks_coord:
+            if peak_index < start_index:    # Do not guess
+                peak_index += 1
+                continue
+            print(f'Preparing iguess for {peak_index:4.0f}/{len(self.coord):4.0f} peak', end='\r')
+            # Unpack TR1 and TR2
+            u1, tr1 = TR1
+            u2, tr2 = TR2
+
+            if auto is True and only_edit is None:  # All automatic
+                parameters, interval = auto_val(self.ppm_f1, self.ppm_f2, tr1, tr2, u1, u2, fwhm0, self.acqus)
+            elif auto is True and only_edit is not None:    # Interactively guess only the given peaks, all the others automatically
+                if peak_index in only_edit:
+                    parameters, interval = fit.gen_iguess_2D(self.ppm_f1, self.ppm_f2, tr1, tr2, u1, u2, self.acqus, fwhm0, self.procs)
+                else:
+                    parameters, interval = auto_val(self.ppm_f1, self.ppm_f2, tr1, tr2, u1, u2, fwhm0, self.acqus)
+            else:   # All interactively
+                parameters, interval = fit.gen_iguess_2D(self.ppm_f1, self.ppm_f2, tr1, tr2, u1, u2, self.acqus, fwhm0, self.procs)
+
+            for values in parameters:   # Write the parameters
+                self._write_par_line(f, self.acqus, peak_index, values, interval_f1=interval[0], interval_f2=interval[1])
+            peak_index += 1 # Increment the peak index
+        print('')
+
+    def fit(self, filename='fit.out', overwrite=False, start_index=1, **fit_kws):
+        """
+        Perform the fit of all the 2D peaks, one by one, by reading the starting values from Vi.
+        
+        """
+
+        # Flag: did you set a logfile?
+        if 'logfile' in fit_kws.keys():
+            use_logfile = True
+        else:
+            use_logfile = False
+
+        # Generator: group the parameters with the same index.
+        def values_loop(V, idx):
+            if isinstance(V, list):
+                n_sgn = len(V)
+            else:
+                n_sgn = V.shape[0]
+
+            for k in range(n_sgn):
+                peak_index = k + 1
+                if peak_index > max(idx):
+                    break
+                tmp_par = [V[k] for k in range(n_sgn) if idx[k] == peak_index]
+                yield peak_index, tmp_par
+        looped_values = values_loop(self.Vi, self.idx)  # Call the generator
+
+        if os.path.exists(filename) and overwrite is False:    # append next peaks 
+            f = open(filename, 'a', buffering=1)
+        else:   # create a new file
+            f = open(filename, 'w', buffering=1)
+            self._write_head_line(f)
+
+        # Loop for the fit
+        for peak_index, peak_values in looped_values:
+            if use_logfile: # Redirect the standard output to the logfile
+                sys.stdout = open(fit_kws['logfile'], 'a', buffering=1) 
+            print(f'Fitting peak {peak_index:4.0f} / {max(self.idx):4.0f}')
+            if peak_index < start_index:    # Skip
+                continue
+            if len(peak_values) == 0:   # Skip empty parameters
+                continue
+            lim_f1, lim_f2 = self.Wi[peak_index-1]  # Get the window for the fit
+            # Call the fit
+            fit_parameters = voigt_fit_2D(self.ppm_f2, self.ppm_f1, self.data, peak_values, lim_f1, lim_f2, self.acqus, N=(len(self.ppm_f1),len(self.ppm_f2)), procs=self.procs, **fit_kws)
+            # Write the output in the new file
+            for fit_values in fit_parameters:
+                self._write_par_line(f, self.acqus, peak_index, fit_values, interval_f1=lim_f1, interval_f2=lim_f2, conv_u=False)
+
+        # Revert standard output to default
+        if use_logfile:
+            sys.stdout = sys.__stdout__
+
+    ### PRIVATE METHODS
+    def _write_head_line(self, f):
+        """ 
+        Writes the header of the output file.
+        -------
+        Parameters:
+        - f: TextIOWrapper
+            writable file generated by open(filename, 'w'/'a')
+        """
+        f.write(f'{"#":<4s}\t{"u1":>8s}\t{"u2":>8s}\t{"fwhm1":>8s}\t{"fwhm2":>8s}\t{"I":>8s}\t{"x_g":>8s}\t{"Fit. interv.":>20s}\n')
+
+    def _write_par_line(self, f, acqus, index, values, interval_f1=None, interval_f2=None, conv_u=True):
+        """ 
+        Writes a line of parameters to the output file.
+        -------
+        Parameters:
+        - f: TextIOWrapper
+            writable file generated by open(filename, 'w'/'a')
+        - acqus: dict
+            2D-like acquisition parameters
+        - values: 1darray
+            u1, u2, fwhm1, fwhm2, I, xg
+        - interval_f1: tuple
+            left limit F1, right limit F1
+        - interval_f2: tuple
+            left limit F2, right limit F2
+        - conv_u: bool
+            Conversion of u1 and u2 from Hz to ppm
+        """
+        if interval_f1 is None:
+            interval_f1 = ('SW', 'SW')  # Whole SW
+        else:
+            interval_f1 = tuple([eval(f'{x:4.1f}') for x in interval_f1])
+        if interval_f2 is None:
+            interval_f2 = ('SW', 'SW')  # Whole SW
+        else:
+            interval_f2 = tuple([eval(f'{x:4.1f}') for x in interval_f2])
+        interval = f'{interval_f1},{interval_f2}'
+
+        v1, v2, fwhm1, fwhm2, I, x_g = values   # Unpack
+        if conv_u:
+            # Convert u1, u2 from Hz to ppm
+            u1, u2 = [misc.freq2ppm(x, acqus[f'SFO{y}'], acqus[f'o{y}p']) for x, y in zip([v1, v2], [1, 2])]
+        else:
+            u1, u2 = v1, v2
+
+        # Write the line
+        f.write(f'{index:4.0f}\t{u1:8.2f}\t{u2:8.2f}\t{fwhm1:8.1f}\t{fwhm2:8.1f}\t{I:8.3e}\t{x_g:8.4f}\t{interval}\n')
+
+    def _read_par_line(self, line):
+        """ Splits the line into the three attributes """
+        split = line.split('\t')
+        index = eval(split[0])
+        values = [eval(w) for w in split[1:-1]]
+        fit_interval = eval(split[-1])
+        return index, values, fit_interval
+
+
+
```

### Comparing `klassez-0.1a1/klassez/misc.py` & `klassez-0.1a2/klassez/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,29 +14,28 @@
 import seaborn as sns
 import nmrglue as ng
 import lmfit as l
 from datetime import datetime
 import warnings
 
 from . import fit, misc, sim, figures, processing
-#from .__init__ import CM
-from .config import CM
+from .config import CM, COLORS, cron
 """ 
 Collection of all-purpose functions
 """
 
 def noise_std(y):
     """
     Calculates the standard deviation of the noise using the Bruker formula. Taken y as an array of N points, and yi its i-th entry:
     -------
-    Parameters
+    Parameters:
     - y : 1darray
         The spectral region you would like to use to calculate the standard deviation of the noise.
     -------
-    Returns
+    Returns:
     - noisestd : float
         The standard deviation of the noise.
     """
     N = len(y)
     n = N//2 + 1
     # W
     W = 0
@@ -55,23 +54,23 @@
     return noisestd
 
 
 def SNR(data, signal=None, n_reg=None):
     """
     Computes the signal to noise ratio of a 1D spectrum.
     -------
-    Parameters
+    Parameters:
     - data : 1darray
         The spectrum of which you want to compute the SNR
     - signal : float, optional
         If provided, uses this value as maximum signal. Otherwise, it is selected as the maximum value in "data"
     - n_reg : list or tuple, optional
         If provided, contains the points that delimit the noise region. Otherwise, the whole spectrum is used.
     -------
-    Returns
+    Returns:
     - snr : float
         The SNR of the spectrum
     """
     # Computes the SNR of a 1D spectrum (or 2D projection).
     # n_reg is a list/tuple of 2 values that delimitates the noise region
     if signal is None:
         signal = np.max(data)
@@ -83,22 +82,22 @@
     snr = signal / (2 * misc.noise_std(y))
     return snr
 
 def SNR_2D(data, n_reg=None):
     """
     Computes the signal to noise ratio of a 2D spectrum.
     -------
-    Parameters
+    Parameters:
     - data : 1darray
         The spectrum of which you want to compute the SNR
     - n_reg : list or tuple
         If provided, the points of F1 scale and F2 scale, respectively, of which to extract the projections.
     Otherwise, opens the tool for interactive selection.
     --------
-    Returns
+    Returns:
     - snr_f1 : float
         The SNR of the indirect dimension
     - snr_f2 : float
         The SNR of the direct dimension
     """
     # Computes the SNR of a 2D spectrum.
     # n_reg is: (ppmf1 for f2 trace, ppmf2 for f1 trace)
@@ -117,19 +116,19 @@
 
     return snr_f1, snr_f2
 
 def makeacqus_1D(dic):
     """
     Given a NMRGLUE dictionary from a 1D spectrum (generated by ng.bruker.read), this function builds the acqus file with only the "important" parameters. 
     -------
-    Parameters
+    Parameters:
     - dic: dict
         NMRglue dictionary returned by ng.bruker.read
     -------
-    Returns
+    Returns:
     - acqus : dict
         Dictionary with only few parameters
     """
     acqus = {}
     acqus['nuc'] = dic['acqus']['NUC1']
     acqus['SFO1'] = dic['acqus']['SFO1']
     acqus['SWp'] = dic['acqus']['SW']
@@ -144,19 +143,19 @@
     acqus['AQ'] = acqus['t1'][-1]
     return acqus
 
 def makeacqus_2D(dic):
     """
     Given a NMRGLUE dictionary from a 2D spectrum (generated by ng.bruker.read ), this function builds the acqus file with only the "important" parameters.
     -------
-    Parameters
+    Parameters:
     - dic: dict
         NMRglue dictionary returned by ng.bruker.read
     -------
-    Returns
+    Returns:
     - acqus : dict
         Dictionary with only few parameters
     """
     acqus = {}
     acqus['nuc1'] = dic['acqu2s']['NUC1']
     acqus['nuc2'] = dic['acqus']['NUC1']
     acqus['SFO1'] = dic['acqu2s']['SFO1']
@@ -171,25 +170,28 @@
     acqus['B0'] = acqus['SFO2'] / sim.gamma[acqus['nuc2']]
     acqus['o1p'] = acqus['o1'] / acqus['SFO1']
     acqus['o2p'] = acqus['o2'] / acqus['SFO2']
     acqus['SW1'] = acqus['SW1p'] * np.abs(acqus['SFO1'])
     acqus['SW2'] = acqus['SW2p'] * np.abs(acqus['SFO2'])
     acqus['dw1'] = 1 / acqus['SW1']
     acqus['dw2'] = 1 / acqus['SW2']
-    acqus['t1'] = np.linspace(0, acqus['TD1']*acqus['dw1'], acqus['TD1'])
+    if dic['acqu2s']['FnMODE'] in (3, 4, 5):
+        acqus['t1'] = np.linspace(0, acqus['TD1']//2*acqus['dw1'], acqus['TD1'])
+    else:
+        acqus['t1'] = np.linspace(0, acqus['TD1']*acqus['dw1'], acqus['TD1'])
     acqus['t2'] = np.linspace(0, acqus['TD2']*acqus['dw2'], acqus['TD2'])
     acqus['AQ1'] = acqus['t1'][-1]
     acqus['AQ2'] = acqus['t2'][-1]
     return acqus
 
 def write_acqus_1D(acqus, path='sim_in_1D'):
     """
     Writes the input file for a simulated spectrum, basing on a dictionary of parameters.
     -------
-    Parameters
+    Parameters:
     - acqus : dict
         The dictionary containing the parameters for the simulation
     - path : str, optional
         Directory where the file will be saved.
     """
     f = open(path, 'w')
     keylist = acqus.keys()
@@ -208,15 +210,15 @@
         
     f.close()
 
 def write_acqus_2D(acqus, path='sim_in_2D'):
     """
     Writes the input file for a simulated spectrum, basing on a dictionary of parameters.
     -------
-    Parameters
+    Parameters:
     - acqus : dict
         The dictionary containing the parameters for the simulation
     - path : str, optional
         Directory where the file will be saved.
     """
     f = open(path, 'w')
     keylist = acqus.keys()
@@ -233,112 +235,190 @@
                 f.write('{}\t{}\n'.format(key, acqus[key]))
     f.close()
 
 def calcres(fqscale):
     """
     Calculates the frequency resolution of an axis scale, i.e. how many Hz is a "tick".
     --------
-    Parameters
+    Parameters:
     - fqscale : 1darray
         Scale to be processed
     -------
-	Returns
-    --------
+    Returns:
     - res: float
         The resolution of the scale
     """
     return np.abs(fqscale[1]-fqscale[0])
 
 def hz2pt(fqscale, hz):
     """
     Converts hzfrom frequency units to points, on the basis of its scale.
     --------
-    Parameters
+    Parameters:
     - fqscale : 1darray
         Scale to be processed
     - hz :float
         Value to be converted
     -------
-	Returns
+    Returns:
     - pt :float
         The frequency value converted in points
     """
     hzpt = misc.calcres(fqscale)
     pt = int(round(hz / hzpt))
     return pt
 
+def in2px(*in_args):
+    """
+    Converts a sequence of numbers from inches to pixels by multiplying times 96.
+    --------
+    Parameters:
+    - *in_args: sequence of floats
+        Values in inches to convert
+    -------
+    Returns:
+    - px_args: tuple of ints
+        Values in pixels
+    """
+    px_args = tuple([int(X * 96) for X in in_args])
+    return px_args
+
+def px2in(*px_args):
+    """
+    Converts a sequence of numbers from inches to pixels by multiplying times 96.
+    --------
+    Parameters:
+    - *px_args: sequence of ints 
+        Values in pixels to convert
+    -------
+    Returns:
+    - in_args: tuple of floats
+        Values in inches
+    """
+    in_args = tuple([X / 96 for X in px_args])
+    return in_args
 
 def find_nearest(array, value):
     """
     Finds the value in array which is the nearest to value .
     -------
-	Parameters
+    Parameters:
     - array : 1darray
         Self-explanatory
     - value : float
         Value to be found
     -------
-	Returns
+    Returns:
     - val :float
         The closest value in array tovalue
     """
     # Finds the value in 'array' which is the nearest to 'value'
     array = np.asarray(array)
     idx = (np.abs(array - value)).argmin()
     return array[idx]
 
-def trim_data(ppm_scale, y, sx, dx):
+def trim_data(ppm_scale, y, lims):
     """
     Trims the frequency scale and correspondant 1D dataset y from sx (ppm) to dx (ppm).
     -------
-	Parameters
+	Parameters:
     - ppm_scale : 1darray
         ppm scale of the spectrum
     - y :1darray
         spectrum
-    - sx :float
-        ppm value where to start trimming
-    - dx :float
-        ppm value where to finish trimming
+    - lims: tuple 
+        ppm values where to start and stop trimming
     -------
-	Returns
+    Returns:
     - xtrim : 1darray
         Trimmed ppm scale
     - ytrim : 1darray
         Trimmed spectrum
     """
-    SX = misc.ppmfind(ppm_scale, sx)[0]
-    DX = misc.ppmfind(ppm_scale, dx)[0]
-    xtrim = ppm_scale[min(SX,DX):max(SX,DX)]
+    lims_p = sorted([misc.ppmfind(ppm_scale, x)[0] for x in lims])
+    slice_x = slice(*lims_p)
+    xtrim = ppm_scale[slice_x]
     if np.iscomplexobj(y):
-        ytrim_re = y.real[...,min(SX,DX):max(SX,DX)]
-        ytrim_im = y.imag[...,min(SX,DX):max(SX,DX)]
+        ytrim_re = y.real[..., slice_x]
+        ytrim_im = y.imag[..., slice_x]
         ytrim = ytrim_re + 1j*ytrim_im
     else:
-        ytrim = y[...,min(SX,DX):max(SX,DX)]
+        ytrim = y[..., slice_x]
     return xtrim, ytrim
 
+def trim_data_2D(x_scale, y_scale, data, xlim=None, ylim=None):
+    """ 
+    Trims data and the scales according to xlim and ylim.
+    Returns the trimmed data and the correspondant trimmed scales.
+    --------
+    Parameters:
+    - x_scale: 1darray
+        Scale for the rows of data
+    - y_scale: 1darray
+        Scale for the columns of data
+    - data: 2darray
+        Data to be trimmed
+    - xlim: tuple
+        Limits for x_scale (L, R)
+    - ylim: tuple
+        Limits for y_scale (L, R)
+    --------
+    Returns:
+    - trimmed_x: 1darray
+        Trimmed x_scale
+    - trimmed_y: 1darray
+        Trimmed y_scale
+    - trimmed_data: 2darray
+        Trimmed data
+    """
+
+    # Shallow copy
+    trimmed_x = np.copy(x_scale)
+    trimmed_y = np.copy(y_scale)
+    datap = np.copy(data)
+
+    if xlim is None:    # Set whole scale
+        xlim = x_scale[0], x_scale[-1]
+    if ylim is None:    # Set whole scale
+        ylim = y_scale[0], y_scale[-1]
+    # Get the indexes of the limits on both scale and sort them
+    xlim_p = sorted([misc.ppmfind(x_scale, lim)[0] for lim in xlim])
+    ylim_p = sorted([misc.ppmfind(y_scale, lim)[0] for lim in ylim])
+    # Trim
+    slice_x = slice(*xlim_p)            # slice on X
+    slice_y = slice(*ylim_p)            # slice on Y
+    #   Scales
+    trimmed_x = trimmed_x[slice_x]
+    trimmed_y = trimmed_y[slice_y]
+    #   Data
+    trimmed_data = datap[..., slice_x]
+    trimmed_data = trimmed_data[slice_y, ...]
+
+    return trimmed_x, trimmed_y, trimmed_data
+
+
+
 def ppmfind(ppm_scale, value):
     """
     Finds the exact value in ppm_scale.
     -------
-	Parameters
+    Parameters:
     - ppm_scale : 1darray
         Self-explanatory
     - value : float
         The value to be found
     -------
-	Returns
+    Returns:
     - I :int
         The index correspondant to ’V’ in ’ppm_scale’
     - V :float
         The closest value to ’value’ in ’ppm_scale’
     """
     # Finds the exact 'value' in ppm scale 'ppm_1h'
-    # Returns the found value 'V' and its index 'I'
+    # Returns: the found value 'V' and its index 'I'
     avgstep = np.abs((ppm_scale[0]-ppm_scale[1])/2)
     I, V = None, None
     for i, delta in enumerate(ppm_scale):
         if value-avgstep <= delta and delta < value+avgstep:
             I = i
             V = ppm_scale[i]
             break
@@ -349,59 +429,59 @@
     else:
         return I, V
 
 def ppm2freq(x, B0=701.125, o1p=0):
     """
     Converts xfrom ppm to Hz.
     -------
-	Parameters
+    Parameters:
     - x :float
         Value to be converted
     - B0 :float
         Field frequency, in MHz. Default: 700 MHz
     - o1p : float
         Carrier frequency, in ppm. Default: 0.
     -------
-	Returns
+    Returns:
     - y :float
         The converted value
     """
     # Converts 'x' from ppm to Hz.
     # B0 is the frequency of the field in MHz.
     y = (x-o1p)*B0
     return y
 
 def freq2ppm(x, B0=701.125, o1p=0):
     """
     Converts xfrom Hz to ppm.
     -------
-	Parameters
+    Parameters:
     - x :float
         Value to be converted
     - B0 :float
         Field frequency, in MHz. Default: 700 MHz
     - o1p : float
         Carrier frequency, in ppm. Default: 0.
     -------
-	Returns
+    Returns:
     - y :float
         The converted value
     """
     y = x/B0 + o1p
     return y
 
 def readlistfile(datafile):
     """
     Takes as input the path of a file containing one entry for each row. Returns a list of the aforementioned entries.
     -------
-	Parameters
+    Parameters:
     - datafile: str
         Path to a file that contains one entry for each row
     -------
-	Returns
+    Returns:
     - files : list
         List of the entries contained in the file
     """
     with open(datafile) as F:
         names = F.readlines()
 
     files = []
@@ -409,21 +489,21 @@
         files.append(names[i].strip())
 
     return files
 
 def procpar(txt):
     """
     Takes as input the path of a file containing a "key" in the first column and a "value" in the second
-    column. Returns a dictionary of shape "key" : "value".
+    column. Returns the correspondant dictionary 
     -------
-	Parameters
+	Parameters:
     - txt :str
         Path to a file that contains "key" in first column and "value" in the second
     -------
-	Returns
+	Returns:
     - procpars : dict
         Dictionary of shape "key":"value"
     """
     fyle = open(txt).readlines()
     procpars = {}
     for line in fyle:
         if line[0] == '#':
@@ -431,33 +511,32 @@
         string = line.split('\t')
         procpars[string[0]] = float(string[1].strip())
     return procpars
 
 def get_trace(data, ppm_f2, ppm_f1, a, b=None, column=True):
     """
     Takes as input a 2D dataset and the ppm scales of direct and indirect dimensions respectively.
-    Calculates the projection on the given axis summing from a (ppm) to b(ppm). 
+    Calculates the projection on the given axis summing from a (ppm) to b (ppm). 
     Default: indirect dimension projection (i.e. column=True), change it to "False" for the direct dimension projection.
-    Returns the calculated 1D projection.
     -------
-	Parameters
+	Parameters:
     - data : 2darray
         Spectrum of which to extract the projections
     - ppm_f2 : 1darray
         ppm scale of the direct dimension
     - ppm_f1 : 1darray
         ppm scale of the indirect dimension
     - a :float
         The ppm value from which to start extracting the projection.
     - b :float, optional
         If provided, the ppm value at which to stop extracting the projection. Otherwise, returns only the 'a' trace.
     - column : bool
         If True, extracts the F1 projection. If False, extracts the F2 projection.
     -------
-	Returns
+	Returns:
     - y :1darray
         Computed projection
     """
     if not b:
         b = a
 
     if column:
@@ -478,27 +557,27 @@
 
 
 def select_traces(ppm_f1, ppm_f2, data, Neg=True, grid=False):
     """
     Select traces from a 2D spectrum, save the coordinates in a list. 
     Left click to select a point, right click to remove it.
     -------
-	Parameters
+	Parameters:
     - ppm_f1 : 1darray
         ppm scale of the indirect dimension
     - ppm_f2 : 1darray
         ppm scale of the direct dimension
     - data : 2darray
         Spectrum
     - Neg : bool
         Choose if to show the negative contours ( True) or not ( False )
     - grid : bool
         Choose if to display the grid ( True) or not ( False )
     -------
-	Returns
+	Returns:
     - coord: list
         List containing the ’[x,y]’ coordinates of the selected points.
     """
     cmaps = CM['Blues_r'], CM['Reds_r']
     # Select traces from a 2D spectrum, save the coordinates in a list
     lvlstep = 0.02                  # for mouse scroll
 
@@ -531,15 +610,15 @@
     ygrid = ppm_f1
     if grid:        # Set grid to visible
         for i in xgrid:
             ax.axvline(i, color='grey', lw=0.1)
         for j in ygrid:
             ax.axhline(j, color='grey', lw=0.1)
 
-    # Parameters to save coordinates
+    # Parameters: to save coordinates
     coord = []          # Final list of coordinates
     dot = []            # Bullets in figure
     dothline = []       # Horizontal lines
     dotvline = []       # Vertical lines
 
     def on_click(event):
         # What happens if you click?
@@ -606,37 +685,37 @@
 def select_for_integration(ppm_f1, ppm_f2, data, Neg=True):
     """
     Select the peaks of a 2D spectrum to integrate.
     First, select the area where your peak is located by dragging the red square.
     Then, select the center of the peak by right_clicking. 
     Finally, click 'ADD' to store the peak. Repeat the procedure for as many peaks as you want.
     -------
-	Parameters
+	Parameters:
     - ppm_f1 : 1darray
         ppm scale of the indirect dimension
     - ppm_f2 : 1darray
         ppm scale of the direct dimension
     - data : 2darray
         Spectrum
     - Neg : bool
         Choose if to show the negative contours ( True) or not ( False )
     -------
-	Returns
+	Returns:
     - peaks: list of dict
         For each peak there are two keys, 'f1' and 'f2', whose meaning is obvious. 
         For each of these keys, you have 'u': center of the peak /ppm, and 'lim': the limits of the square you drew before.
     """
 
     cmaps = CM['Blues_r'], CM['Reds_r']
     lvlstep = 0.02                  # Increase step for contours when scroll the mouse1
 
     # Make an underlying grid to snap the pointer
     xgrid = np.copy(ppm_f2)
     ygrid = np.copy(ppm_f1)
-    # Parameters to save coordinates
+    # Parameters: to save coordinates
     coord = []          # Final list of coordinates
     rekt = []           # Rectangles
     # Set figure borders
     xsx, xdx = max(ppm_f2), min(ppm_f2)
     ysx, ydx = max(ppm_f1), min(ppm_f1)
     # set base level for contour
     lvl0 = 0.2
@@ -799,25 +878,25 @@
                 },
             })
     return peaks
 
 
 def polyn(x, c):
     """
-    Computes p(x), polynomion of degree n−1, where nis the number of provided coefficients.
+    Computes p(x), polynomion of degree n-1, where nis the number of provided coefficients.
     -------
-	Parameters
+    Parameters:
     - x :1darray
         Scale upon which to build the polynomion
     - c :list or 1darray
         Sequence of the polynomion coeffiecient, starting from the 0-th order coefficient
     -------
-	Returns
+    Returns:
     - px :1darray
-        Polynomion of degree n−1.
+        Polynomion of degree n-1.
     """
     # Computes p(x) polynomion of degree n-1.
     # c is a list/array of the n coefficients, sorted starting 
     # from the 0th-order coefficient 
     degree = len(c)
     px = np.zeros_like(x)
     for i in range(degree):
@@ -827,20 +906,20 @@
 
 
 def write_ser(fid, path='./', BYTORDA=0, DTYPA=0, overwrite=True):
     """
     Writes the FID file in directory 'path', in a TopSpin-readable way (i.e. little endian, int32).
     The binary file is named 'fid' if 1D, 'ser' if multiD.
     The parameters BYTORDA and DTYPA can be found in the acqus file.
-    - BYTORDA = 1   =>  big endian      =>  '>'
-    - BYTORDA = 0   =>  little endian   =>  '<'
-    - DTYPA = 0     =>  int32           =>  'i4'
-    - DTYPA = 2     =>  float64         =>  'f8'
+    > BYTORDA = 1   =>  big endian      =>  '>'
+    > BYTORDA = 0   =>  little endian   =>  '<'
+    > DTYPA = 0     =>  int32           =>  'i4'
+    > DTYPA = 2     =>  float64         =>  'f8'
     -------
-	Parameters
+    Parameters:
     - fid :ndarray
         FID array to be written
     - path : str
         Directory where to save the file
     """
 
     if BYTORDA == 0:
@@ -954,21 +1033,21 @@
         ax.set_yticks(minorlocs, minor=True)
         ax.set_ylim(sx,dx)
 
 
 def molfrac(n):
     """
     Computes the "molar fraction" 'x' of the array 'n'.
-    Returns also the total amount.
+    Also computes the total amount.
     -------
     Parameters:
     - n: list or 1darray
         list of values
     -------
-    Returns:
+    Return:
     - x: list or 1darray
         molar fraction array
     - N: float
         sum of all the elements in 'n'
     """
     if isinstance(n, list):
         n = np.array(n)
@@ -982,15 +1061,15 @@
     """
     Split the acqus dictionary of a 2D spectrum into two separate 1D-like acqus dictionaries.
     --------
     Parameters:
     - acqus: dict
         acqus dictionary of a 2D spectrum
     --------
-    Returns:
+    Return:
     - acqu1s: dict
         acqus dictionary of the indirect dimension
     - acqu2s: dict
         acqus dictionary of the direct dimension
     """
     keys = ['B0', 'nuc', 'o1p', 'SWp', 'TD', 'SFO1', 'SW', 'dw', 't1', 'o1', 'AQ1']
     acqu1v = [
@@ -1028,15 +1107,15 @@
     """
     Split the procs dictionary of a 2D spectrum into two separate 1D-like procs dictionaries.
     --------
     Parameters:
     - procs: dict
         procs dictionary of a 2D spectrum
     --------
-    Returns:
+    Return:
     - proc1s: dict
         procs dictionary of the indirect dimension
     - proc2s: dict
         procs dictionary of the direct dimension
     """
     keys = ['wf', 'zf', 'fcor', 'tdeff', 'p0', 'p1', 'pv']
     proc1v = [
@@ -1066,15 +1145,15 @@
     """
     Converts the 'nuc' key you may find in acqus in the formatted label, e.g. '13C' -> '$^{13}$C'
     --------
     Parameters:
     - nuc: str
         Unformatted string
     --------
-    Returns:
+    Return:
     - fnuc: str
         Formatted string.
     """
     import re
     fnuc = re.split('(\D+)',nuc)
     f_nuc = '$^{' + str(fnuc[0]) + '}$'+str(fnuc[1])
     return f_nuc
@@ -1147,18 +1226,18 @@
         ax.xaxis.get_offset_text().set_size(fontsize)
 
         
 def set_fontsizes(ax, fontsize=10):
     """
     Automatically adjusts the fontsizes of all the figure elements.
     In particular:
-    - title = fontsize
-    - axis labels = fontsize - 2
-    - ticks labels = fontsize - 3
-    - legend entries = fontsize - 4
+    > title = fontsize
+    > axis labels = fontsize - 2
+    > ticks labels = fontsize - 3
+    > legend entries = fontsize - 4
     --------
     Parameters:
     - ax: matplotlib.Subplot Object
         Subplot of interest
     - fontsize: float
         Starting fontsize
     -------
@@ -1233,15 +1312,15 @@
     If data id a 2darray, computes the closest Hankel matrix in the Frobenius norm sense by averaging the values on the antidiagonals.
     -------
     Parameters:
     - data: 1darray
         Vector to be Hankel-ized, of length N
     - n: int
         Number of columns that the Hankel matrix will have
-    Returns:
+    Return:
     - H: 2darray
         Hankel matrix of dimensions (N-n+1, n)
     """
     if isinstance(data, np.ndarray):
         if len(data.shape) == 1:
             if n is None:
                 raise ValueError('You must specify the number of columns of the Hankel matrix.')
@@ -1258,15 +1337,15 @@
     """
     Concatenates the first row and the last column of the matrix H, which should have Hankel-like structure, so to build the array of independent parameters.
     ------
     Parameters:
     - H: 2darray
         Hankel-like matrix
     ------
-    Returns:
+    Return:
     - h: 1darray
         First row and last column, concatenated
     """
     h = np.concatenate((H[0,:], H[1:, -1]), axis=-1)
     return h
 
 
@@ -1274,15 +1353,15 @@
     """
     Given a matrix X without any specific structure, finds the closest Hankel matrix in the Frobenius norm sense by averaging the antidiagonals.
     ---------
     Parameters:
     - X: 2darray
         Input matrix
     --------
-    Returns:
+    Return:
     - Xp: 2darray
         Hankel matrix obtained from X
     """
     m, n = X.shape  # Get dimensions of X
     N = m + n - 1   # Degrees of freedom that Xp will have
     data = np.array([np.mean(np.diag(X[:, ::-1], w)) for w in range(-N+n, n)])[::-1]      # Mean on the antidiagonals
     Xp = misc.hankel(data, n)    # Transform the "data" array into a matrix
@@ -1314,15 +1393,15 @@
     """
     Prints a list, one entry per row.
     -------
     Parameters:
     - mylist: list
         The list you want to print
     -------
-    Returns:
+    Return:
     - outstring: str
         The printed text formatted as single string
     """
     outstring = ''
     for entry in mylist:
         outstring += '{}\n'.format(entry)
     print(outstring)
@@ -1332,15 +1411,15 @@
     """
     Prints a dictionary one entry per row, in the format key: value. Nested dictionaries are printed with an indentation
     -------
     Parameters:
     - mydict: dict
         The dictionary you want to print
     -------
-    Returns:
+    Return:
     - outstring: str
         The printed text formatted as single string
     """
     outstring = ''
     for key, value in mydict.items():
         if isinstance(value, dict):
             outstring += '{}:\n'.format(key)
@@ -1403,15 +1482,15 @@
     - N: int
         Number of samples to extract
     - start: float
         Start point of the sampling. 0 = beginning of the cmap; 1 = end of the cmap.
     - end: float
         End point of the sampling. 0 = beginning of the cmap; 1 = end of the cmap.
     -------
-    Returns:
+    Return:
     - colors: list
         List of the extracted colors.
     """
     x = np.linspace(start, end, N)
     colors = cmap(x)
     return colors
 
@@ -1461,19 +1540,19 @@
     """
     Calculates the n-th row of the binomial triangle. The first row is n=1, not 0.
     Example:
     In: > binomial_triangle(4)
         > 1 3 3 1
     --------
     Parameters:
-    n: int
+    - n: int
         Row index
     --------
-    Returns:
-    row: 1darray
+    Return:
+    - row: 1darray
         The n-th row of binomial triangle.
     """
     row = []
     n -= 1
     for k in range(n+1):
         row.append(
                 np.math.factorial(n) / ( np.math.factorial(k) * np.math.factorial(n-k) )
```

### Comparing `klassez-0.1a1/klassez/processing.py` & `klassez-0.1a2/klassez/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,132 +14,275 @@
 import seaborn as sns
 import nmrglue as ng
 import lmfit as l
 from datetime import datetime
 import warnings
 
 from . import fit, misc, sim, figures, processing
+from .config import CM, COLORS, cron
 
-#from .__init__ import CM
-#CM = __init__.CM
-from .config import CM
 """ 
 Contains a series of processing functions for different purposes
 """
 
 
+
 # CPMG processing
-def sum_echo_train(datao, n, n_echoes, i_p=0):
+
+def interactive_echo_param(data0):
+    """
+    Interactive plot that allows to select the parameters needed to process a CPMG-like FID.
+    Use the TextBox or the arrow keys to adjust the values.
+    You can call processing.sum_echo_train or processing.split_echo_train by starring the return statement of this function, i.e.:
+        processing.sum_echo_train(data0, *interactive_echo_train(data0))
+    as they are in the correct order to be used in this way.
+    -------
+    Parameters:
+    - data0: ndarray
+        CPMG FID
+    -------
+    Returns:
+    - n: int
+        Distance between one echo and the next one
+    - n_echoes: int
+        Number of echoes to sum/split
+    - i_p: int
+        Offset points from the start of the FID
     """
-    "datao" is a 1D or 2D dataset whose direct dimension
-    has been acquired with CPMG, i.e. it is made of 
-    echoes separated one from each other by "n" points.
-    The first good point of the FID is "i_p".
-    This function sums the first "n_echoes" echoes and 
-    returns the resulting FID.
-    """
-    try:
-        if len(datao[:,0])>1:
-            transients = len(datao[:,0])
-    except:
-        transients = 1
-        datao = np.reshape(datao, (1,-1))
 
-    data = datao[ 0:transients, i_p : n*n_echoes+i_p+1 ]
-    if np.mod(n,2) == 0:
-        nm = int(n/2)
+    # Check for data dimension and safety copy
+    if len(data0.shape) == 1:
+        data = np.copy(data0)
+    elif len(data0.shape) == 2:
+        data = np.copy(data0[0,:])
     else:
-        nm = int(n/2)+1
+        raise ValueError('Data shape not supported')
 
-    data_p = np.zeros((transients, nm), dtype='complex64')
-    datad = np.zeros_like(data_p)
-    datar = np.zeros_like(data_p)
+    # Make the figure
+    fig = plt.figure()
+    fig.set_size_inches(figures.figsize_large)
+    plt.subplots_adjust(left=0.25, right=0.95, top=0.90, bottom=0.15)
+    ax = fig.add_subplot(2,3,(1,5)) # Square plot
+    axs = fig.add_subplot(2,3,3)    # Right top
+    axt = fig.add_subplot(2,3,6)    # Right bottom
+
+    # Initialize the three values in a dictionary
+    param = {
+            'n' : 20,
+            'n_echoes' : 2,
+            'i_p' : 0,
+            }
 
-    for i in range(n_echoes):
-        a = i * n
-        b1 = i * n + nm
-        b2 = b1
-        if np.mod(n, 2) == 0:
-            b2 = b1 + 1
-        c = i * n + n + 1
+    # ---------------------------------------------------------
+    def update_axs():
+        """ Redraw the figure """
+        # Compute new data
+        newdata = processing.sum_echo_train(data, **param)
+        # Draw it in the top-right subplot
+        sum_sp.set_data(np.arange(len(newdata)), newdata)
+        # Make FT and draw it in bottom-right subplot
+        new_ft = processing.ft(newdata)
+        sum_ft.set_data(np.arange(len(new_ft)), new_ft)
+        # Make pretty scales
+        misc.pretty_scale(axs, (0, len(newdata)), 'x')
+        misc.set_ylim(axs, newdata)
+        misc.set_ylim(axt, new_ft)
+        misc.pretty_scale(axs, (0, len(newdata)-1), 'x')
+        misc.pretty_scale(axt, (0, len(new_ft)-1), 'x')
+        misc.pretty_scale(axs, axs.get_ylim(), 'y')
+        misc.pretty_scale(axt, axt.get_ylim(), 'y')
+        # Write the current values
+        for label in radio.labels:
+            T = label.get_text()
+            val_text[f'{T}'].set_text(f'{param[T]}')
+        plt.draw()
 
-        datad[:, 0:nm] += data[:, a:b1]             #dritto
-        datar[:,0:nm] += data[:, b2:c][:,::-1]      #rovescio
-        
-    datar = datar.real - 1j * datar.imag
-    data_p = datad + datar
+    def read_tb(text):
+        """ Eval() the input in the textbox, clear it """
+        val = eval(text)
+        input_tb.text_disp.set_text('')
+        return int(val)
+
+    def change_param(text):
+        """ Change parameters according to the TextBox """
+        nonlocal param
+        try:    # Avoid error due to the clear text
+            param[f'{radio.value_selected}'] = read_tb(text)
+        except SyntaxError:
+            pass
+        # Draw the red bars and set them visible
+        [X.set_xdata(k*param['n']+param['i_p']) for k, X in enumerate(sampling)]
+        change_nechoes()
+        # Redraw the plots
+        update_axs()
+
+    def change_nechoes():
+        """ Set a certain number of red bars as visible """
+        for k, X in enumerate(sampling):
+            if k < param['n_echoes']:
+                X.set_visible(True)
+            else:
+                X.set_visible(False)
+
+    def key_press(event):
+        """ Edit the param dictionary with uparrow and downarrow """
+        nonlocal param
+        if event.key == 'up':
+            param[f'{radio.value_selected}'] += 1
+        elif event.key == 'down':
+            param[f'{radio.value_selected}'] -= 1
+        else:
+            return
+        # Redraw the red bars and set them visible
+        [X.set_xdata(k*param['n']+param['i_p']) for k, X in enumerate(sampling)]
+        change_nechoes()
+        # Redraw the subplots
+        update_axs()
+
+    # ---------------------------------------------------------
+
+    # Make the widgets with their boxes
+    radio_box = plt.axes([0.025, 0.40, 0.15, 0.35])
+    input_box = plt.axes([0.025, 0.20, 0.15, 0.08])
+    input_box.set_title('Insert value here')
+    input_tb = TextBox(input_box, '')
+    radio = RadioButtons(radio_box, list(param.keys()), activecolor='tab:blue')
+
+    # Write the current values to be updated
+    val_text = {}
+    for k, label in enumerate(radio.labels):
+        val_text[f'{label.get_text()}'] = radio_box.text(0.95, label.get_position()[1]-0.025, 
+                f'{param[label.get_text()]:.0f}',
+                ha='right', va='bottom')
+
+    # Set a scale
+    x = np.arange(data.shape[-1])
+
+    ax.plot(x, data, lw=0.5)    # FID
+    # Top right plot
+    sum_sp, = axs.plot(np.arange(param['n']//2), processing.sum_echo_train(data, **param))
+    # Bottom right plot
+    sum_ft,  = axt.plot(np.arange(param['n']//2), processing.ft(processing.sum_echo_train(data, **param)))
+
+    # Red bars
+    sampling = [ax.axvline(k*param['n'], c='r', lw=0.5) for k in range(data.shape[-1]//param['n'])]
+    change_nechoes()    # Draw them
+
+    # Titles
+    ax.set_title('FID')
+    axs.set_title('Sum FID')
+    axt.set_title('Sum Spectrum')
+
+    # Scales
+    misc.pretty_scale(ax, (x[0], x[-1]), 'x')
+    misc.pretty_scale(ax, ax.get_ylim(), 'y')
+    misc.pretty_scale(axs, (0, param['n']//2-1), 'x')
+    misc.pretty_scale(axt, (0, param['n']//2-1), 'x')
+    misc.pretty_scale(axs, axs.get_ylim(), 'y')
+    misc.pretty_scale(axt, axt.get_ylim(), 'y')
 
-    if transients == 1:
-        data_p = np.reshape(data_p, -1)       
+    # Connect the widgets to the functions
+    input_tb.on_submit(change_param)        # Text box
+    fig.canvas.mpl_connect('key_press_event', key_press)    # Keys
+
+    plt.show()
+    plt.close()
+
+    return tuple([param[f'{label.get_text()}'] for label in radio.labels])
+
+
+def sum_echo_train(datao, n, n_echoes, i_p=0):
+    """
+    Sum up a CPMG echo-train FID into echoes so to be enchance the SNR.
+    This function calls processing.split_echo_train with the same parameters.
+    -------
+    Parameters:
+    - datao: ndarray
+        FID with an echo train on its last dimension
+    - n: int
+        number of points that separate one echo from the next
+    - n_echoes: int
+        number of echoes to sum
+    - i_p: int
+        Number of offset points
+    ------
+    Returns:
+    - data_p: ndarray
+        Summed echoes
+    """
+    # Separate the echoes
+    data = processing.split_echo_train(datao, n, n_echoes, i_p)
+    # Sum on the first dimension
+    data_p = np.sum(data, axis=0)
 
     return data_p
 
+
+
 def split_echo_train(datao, n, n_echoes, i_p=0):
     """
-    "datao" is a 1D or 2D dataset whose direct dimension
-    has been acquired with CPMG, i.e. it is made of 
-    echoes separated one from each other by "n" points.
-    The first good point of the FID is "i_p".
-    This function separates the first "n_echoes" echoes and 
-    store them in a tensor of shape 
-    (n_echoes, len(datao[:,0]), n/2).
-    """
-
-    try:
-        if len(datao[:,0])>1:
-            transients = len(datao[:,0])
-    except:
-        transients = 1
-        datao = np.reshape(datao, (1,-1))
-
-    data = datao[ 0:transients, i_p : n*n_echoes+i_p+1 ]
+    Separate a CPMG echo-train FID into echoes so to be processed separately.
+    The first decay, i.e. the native FID, is extracted, and corresponds to echo number 0. 
+    Then, for each echo, the left side (reversed) is summed up to its right part.
+    -------
+    Parameters:
+    - datao: ndarray
+        FID with an echo train on its last dimension
+    - n: int
+        number of points that separate one echo from the next
+    - n_echoes: int
+        number of echoes to extract. If it is 0, extracts only the first decay
+    - i_p: int
+        Number of offset points
+    ------
+    Returns:
+    - data_p: (n+1)darray
+        Separated echoes
+    """
+    # Take account of the offset points 
+    data = datao[..., i_p:]
+    # nm = middle point. +1 if n is odd
     if np.mod(n,2) == 0:
-        nm = int(n/2)
+        nm = n // 2
     else:
-        nm = int(n/2)+1
-
-    datad = np.zeros((transients, nm), dtype='complex64')
-    datar = np.zeros((transients, nm), dtype='complex64')
+        nm = n // 2 + 1
+    
+    # Where to save the echoes
+    datap = []
+    datap.append(datao[..., :nm])   # Add first decay
 
     for i in range(n_echoes):
-        a = i * n
-        b1 = i * n + nm
-        b2 = b1
-        if np.mod(n, 2) == 0:
-            b2 = b1 + 1
-        c = i * n + n + 1
+        c = (i+1)*n                         # Echo centre
+        A = slice(c-nm+1, c+1)              # Left part to echo centre
+        B = slice(c, c+nm)                  # Right part from echo centre
 
-        datad[:, 0:nm] = data[:, a:b1]             #dritto
-        datar[:,0:nm] = data[:, b2:c][:,::-1]      #rovescio
+        datal = data[..., A][...,::-1]      # Left part, reversed
+        datar = data[..., B]                # Right part
         
-        datar = datar.real - 1j * datar.imag
-        datap = datad + datar
-        datap = np.reshape(datap, (1, len(datap[:,0]), len(datap[0,:])))
-        if i==0:
-            data_p = datap
-        else:
-            data_p = np.vstack((data_p, datap))
-
-    if transients == 1:
-        data_p = np.reshape(data_p, (n_echoes,-1))
+        # Reversing in time means to change sign to the imaginary part
+        if np.iscomplexobj(data):
+            datal = np.conj(datal)
+        datap.append(datal + datar) # Sum up
+    # Create the output data by stacking the echoes. This adds a dimension
+    data_p = np.stack(datap)
 
     return data_p
 
 # -----------------------------------------------------------------------
 
 #   fid adjustment
 def quad(fid):
     """
     Subtracts from the FID the arithmetic mean of its last quarter. The real and imaginary channels are treated separately.
     -------
-    Parameters
+    Parameters:
     - fid : ndarray
         Self-explanatory.
     -------
-    Returns
+    Returns:
     - fid : ndarray
         Processed FID.
     """
     size = fid.shape[-1]
     qsize = size//4
     avg_re = np.average(fid[...,-qsize:].real)
     avg_im = np.average(fid[...,-qsize:].imag)
@@ -262,14 +405,15 @@
         Lorentzian broadening /Hz. It should be negative.
     - gb: float
         Gaussian broadening /Hz. It should be positive.
     - sw: float
         Spectral width /Hz
     - gc: float
         Gaussian center, relatively to the FID length: 0 <= gc <= 1
+    -------
     Returns:
     - pdata: ndarray
         Processed data
     """
     size = data.shape[-1]
     a = np.pi * lb / sw * np.arange(size)
     b = 0.6 * np.pi * (gb / sw) * (gc * (size-1) - np.arange(size) ) 
@@ -286,91 +430,104 @@
     a = np.pi * lb
     b = - a / (2 *  gb * aq)
     apod = np.exp(a * t - b**2 * t**2)
     return apod * data
 
 # zero-filling
 def zf(data, size):
-    # zero-filling of data up to size
+    """
+    Zero-filling of data up to size in its last dimension.
+    -------
+    Parameters:
+    - data: ndarray
+        Array to be zero-filled
+    - size: int
+        Number of points of the last dimension after zero-filling
+    -------
+    Returns:
+    - datazf: ndarray
+        Zero-filled data
+    """
     def zf_pad(data, pad):
         size = list(data.shape)
         size[-1] = int(pad)
         z = np.zeros(size, dtype=data.dtype)
         return np.concatenate((data, z), axis=-1)
     zpad = size - data.shape[-1]
     if zpad <= 0 :
         zpad = 0
     datazf = zf_pad(data, pad=zpad)
     return datazf
 
 # Fourier transform
-def ft(data0, alt=False, fcor=0.5, Numpy=True):
+def ft(data0, alt=False, fcor=0.5):
     """ 
     Fourier transform in NMR sense, i.e. with positive exponential.
     This means to perform IFT reverting the 1/N scaling.
     ------------
     Parameters:
-    -   alt: negates the sign of the odd points, then take the complex conjugate.
-            Required for States-TPPI processing.
-    -   fcor: weighting factor for FID 1st point. Default value (0.5) prevents baseline offset
-    -   Numpy: if True (STRONGLY ADVISED) performs the FT using the FFT algorithm encoded
-            in numpy. If False, performs it manually using the definition of discrete FT.
+    - data0: ndarray
+        Array to Fourier-transform
+    - alt: bool
+        negates the sign of the odd points, then take their complex conjugate. Required for States-TPPI processing.
+    - fcor: float
+        weighting factor for FID 1st point. Default value (0.5) prevents baseline offset
+    ---------
+    Returns:
+    - dataft: ndarray
+        Transformed data
     """
     data = np.copy(data0)
     if not np.iscomplexobj(data):
-        print('WARNING! The input array is not complex.')
+        warnings.warn('WARNING! The input array is not complex.')
     size = data.shape[-1]
     data[...,0] = data[...,0] * fcor
     if data.dtype != "complex64":
         data = data.astype("complex64")
     if alt:
         data[...,1::2] = data[...,1::2] * -1
         data.imag = data.imag * -1
-    if Numpy is True:
-        dataft = np.fft.fftshift(np.fft.ifft(data, axis=-1).astype(data.dtype), -1) * size
-    else:
-        dataft = np.zeros_like(data)
-        for k in range(size):
-            for n in range(size):
-                dataft[...,n] += np.exp( (1j/size) * 2 * np.pi * k * (n - (size/2)) ) * data[..., k]
+    dataft = np.fft.fftshift(np.fft.ifft(data, axis=-1).astype(data.dtype), -1) * size
     return dataft
 
-def ift(data0, alt=False, fcor=0.5, Numpy=True):
+def ift(data0, alt=False, fcor=0.5):
     """ 
     Inverse Fourier transform in NMR sense, i.e. with negative exponential.
     This means to perform FT adding the "times-N" scaling.
     ------------
     Parameters:
-    -   alt: negates the sign of the odd points, then take the complex conjugate.
-            Required for States-TPPI processing.
-    -   fcor: weighting factor for FID 1st point. Default value (0.5) prevents baseline offset
-    -   Numpy: if True (STRONGLY ADVISED) performs the IFT using the FFT algorithm encoded
-            in numpy. If False, performs it manually using the definition of discrete IFT.
+    - data0: ndarray
+        Array to Fourier-transform
+    - alt: bool
+        negates the sign of the odd points, then take their complex conjugate. Required for States-TPPI processing.
+    - fcor: float
+        weighting factor for FID 1st point. Default value (0.5) prevents baseline offset
+    -----------
+    Returns:
+    - dataft: ndarray
+        Transformed data
     """
     data = np.copy(data0)
     if not np.iscomplexobj(data):
-        print('WARNING! The input array is not complex.')
+        warnings.warn('WARNING! The input array is not complex.')
     size = data.shape[-1]
-    if Numpy:
-        s = 1 / size
-        dataft = np.fft.fft(np.fft.ifftshift(data, -1), axis=-1).astype(data.dtype) * s
-    else:
-        dataft = np.zeros_like(data)
-        for k in range(size):
-            for n in range(size):
-                dataft[...,n] += 1/size * np.exp( (-1j/size) * 2 * np.pi * n * (k - (size/2)) ) * data[..., k]
+    s = 1 / size
+    dataft = np.fft.fft(np.fft.ifftshift(data, -1), axis=-1).astype(data.dtype) * s
     if alt:
         dataft[...,1::2] = dataft[...,1::2] * -1
         dataft.imag = dataft.imag * -1
     dataft[...,0] = dataft[...,0] / fcor
     return dataft
     
 def rev(data):
-    # Reverse data
-    return data[...,::-1]
+    """
+    Reverse data over its last dimension
+    """
+    datarev = data[...,::-1]
+    return datarev
     
     # phase correction
 def ps(data, ppmscale=None, p0=None, p1=None, pivot=None, interactive=False):
     """
     Applies phase correction on the last dimension of data.
     The pivot is set at the center of the spectrum by default.
     Missing parameters will be inserted interactively.
@@ -422,14 +579,19 @@
     return datap, final_values
     
     
 def EAE(data):
     """
     Shuffles data if the spectrum is acquired with FnMODE = Echo-Antiecho.
     NOTE: introduces -90° phase shift in F1, to be corrected after the processing
+
+    pdata = np.zeros_like(data)
+    pdata[::2] = (data[::2].real - data[1::2].real) + 1j*(data[::2].imag - data[1::2].imag)
+    pdata[1::2] = -(data[::2].imag + data[1::2].imag) + 1j*(data[::2].real + data[1::2].real)
+
     """
     pdata = np.zeros_like(data)
     pdata[::2] = (data[::2].real - data[1::2].real) + 1j*(data[::2].imag - data[1::2].imag)
     pdata[1::2] = -(data[::2].imag + data[1::2].imag) + 1j*(data[::2].real + data[1::2].real)
     return pdata
     
     
@@ -455,90 +617,141 @@
         n.real = data.real[..., ::2]
         n.imag = data.real[..., 1::2]
         return n
     datatp = np.array(c2ri(ri2c(data).T), dtype='complex64')
     return datatp
         
 def unpack_2D(data):
-    # Separates fully processed 2D NMR data into 4 distinct ser files
+    """
+    Separates hypercomplex data into 4 distinct ser files
+    --------
+    Parameters:
+    - data: 2darray
+        Hypercomplex matrix
+    --------
+    Returns:
+    - rr: 2darray
+        Real F2, Real F1
+    - ir: 2darray
+        Imaginary F2, Real F1
+    - ri: 2darray
+        Real F2, Imaginary F1
+    - ii: 2darray
+        Imaginary F2, Imaginary F1
+    """
     rr = data.real[::2]
     ir = data.imag[::2]
     ri = data.real[1::2]
     ii = data.imag[1::2]
     return rr, ir, ri, ii
     
 def repack_2D(rr, ir, ri, ii):
-    # Renconstruct hypercomplex 2D NMR data given the 4 sers
+    """
+    Renconstruct hypercomplex 2D NMR data given the 4 ser files
+    -------
+    Parameters:
+    - rr: 2darray
+        Real F2, Real F1
+    - ir: 2darray
+        Imaginary F2, Real F1
+    - ri: 2darray
+        Real F2, Imaginary F1
+    - ii: 2darray
+        Imaginary F2, Imaginary F1
+    -------
+    Returns:
+    - data: 2darray
+        Hypecomplex matrix
+    """
     data = np.empty((2*rr.shape[0],rr.shape[1]), dtype='complex64')
     data.real[::2] = rr
     data.imag[::2] = ir
     data.real[1::2] = ri
     data.imag[1::2] = ii
     return data
     
 def td_eff(data, tdeff):
     """
     Uses only the first tdeff points of data. tdeff must be a list as long as the dimensions:
     tdeff = [F1, F2, ..., Fn]
+    --------
+    Parameters:
+    - data: ndarray
+        Data to be trimmed
+    - tdeff: list of int
+        Number of points to be used in each dimension
     """
-    def trim(data, n):
-        return data[...,:n]
+    datain = np.copy(data)
+
+    def trim(datain, n):
+        return datain[...,:n]
     
-    ndim = len(data.shape)
+    ndim = len(datain.shape)
     # if tdeff is a number, make it list
     if isinstance(tdeff, int):
         L = tdeff
         tdeff = []
         tdeff.append(L)
         del L
     
     tdeff = tdeff[::-1]     # to obtain correct final shape
     
     if len(tdeff) != ndim:       # Check
-        raise ValueError('Shape mismatch between data and tdeff')
+        raise ValueError('Shape mismatch between datain and tdeff')
     
     X = tuple(np.roll(np.arange(ndim),1)) # Roll the dimensions to the right
     
     for k in range(ndim):
         if tdeff[k]:
-            data = trim(data, tdeff[k])
-        data = np.transpose(data, X)
+            datain = trim(datain, tdeff[k])
+        datain = np.transpose(datain, X)
     
-    return data
+    return datain
     
     
     
 def fp(data, wf=None, zf=None, fcor=0.5, tdeff=0):
     """
-    Performs the full processing of a 1D NMR FID (data). Required parameters are:
-    - wf:   {'mode': function to be used, 
-                'parameters': different from each function}
-    - zf:   final size of spectrum
-    - fcor: weighting factor for the FID first point
-    - tdeff: number of points of the FID to be used for the processing.
+    Performs the full processing of a 1D NMR FID (data).
+    --------
+    Parameters:
+    - data: 1darray
+        Input data
+    - wf: dict
+        {'mode': function to be used, 'parameters': different from each function}
+    - zf: int
+        final size of spectrum
+    - fcor: float
+        weighting factor for the FID first point
+    - tdeff: int
+        number of points of the FID to be used for the processing.
+    ------
+    Returns:
+    - datap: 1darray
+        Processed data
     """
     # Window function
-    data = processing.td_eff(data, tdeff)
+    datap = processing.td_eff(data, tdeff)
     if wf is not None:
         if wf['mode'] == 'qsin':
-            data = processing.qsin(data, ssb=wf['ssb'])
+            datap = processing.qsin(datap, ssb=wf['ssb'])
         if wf['mode'] == 'sin':
-            data = processing.sin(data, ssb=wf['ssb'])
+            datap = processing.sin(datap, ssb=wf['ssb'])
         if wf['mode'] == 'em':
-            data = processing.em(data, lb=wf['lb'], sw=wf['sw'])
+            datap = processing.em(datap, lb=wf['lb'], sw=wf['sw'])
         if wf['mode'] == 'gm':
-            data = processing.gm(data, lb=wf['lb'], gb=wf['gb'], sw=wf['sw'], gc=wf['gc'])
+            datap = processing.gm(datap, lb=wf['lb'], gb=wf['gb'], sw=wf['sw'], gc=wf['gc'])
         if wf['mode'] == 'gmb':
-            data = processing.gmb(data, lb=wf['lb'], gb=wf['gb'], sw=wf['sw'])
+            datap = processing.gmb(datap, lb=wf['lb'], gb=wf['gb'], sw=wf['sw'])
     # Zero-filling
     if zf is not None:
-        data = processing.zf(data, zf)
+        datap = processing.zf(datap, zf)
     # FT
-    data = processing.ft(data, fcor=fcor)
-    return data
+    datap = processing.ft(datap, fcor=fcor)
+    return datap
     
     
 def interactive_fp(fid0, acqus, procs):
     """
     Perform the processing of a 1D NMR spectrum interactively. The GUI offers the opportunity to test different window functions, as well as different tdeff values and final sizes.
     The active parameters appear as blue text.
     -------
@@ -550,15 +763,15 @@
     - procs: dict
         Dictionary of processing parameters
     -------
     Returns:
     - pdata: 1darray
         Processed spectrum
     - procs: dict
-        Updated dictionary of processing parameters
+        Updated dictionary of processing parameters:
     """
     
     def get_apod(size, procs):
         """ Calculate the window function on the basis of 'procs' """
         Y = np.ones(size, dtype='complex64')    # array of ones
         # Process the array of ones and then revert FT to get everything but the processing
         apodf = processing.ift(processing.fp(Y, wf=procs['wf'], zf=procs['zf'], tdeff=procs['tdeff']))
@@ -585,15 +798,15 @@
     # Calculate the ppm scale
     fq_scale = processing.make_scale(data.shape[-1], acqus['dw'], rev=True)
     ppm_scale = misc.freq2ppm(fq_scale, acqus['SFO1'], acqus['o1p'])
     
     
     # Define useful things 
     modes = ['No', 'em', 'sin', 'qsin', 'gm', 'gmb']   # entries for the radiobuttons
-    act_keys = {    # Active parameters
+    act_keys = {    # Active Parameters:
             'No': [],
             'em': ['lb'],
             'sin': ['ssb'],
             'qsin': ['ssb'],
             'gm': ['lb', 'gb', 'gc'],
             'gmb': ['lb', 'gb'],
             }
@@ -773,55 +986,76 @@
     
     
     
     
     
 def inv_fp(data, wf=None, size=None, fcor=0.5):
     """
-    Performs the full inverse processing of a 1D NMR spectrum (data). Required parameters are:
+    Performs the full inverse processing of a 1D NMR spectrum (data).
+    -------
     Parameters:
+    - data: 1darray
+        Spectrum
     - wf: dict
         {'mode': function to be used, 'parameters': different from each function}
     - size: int
         initial size of the FID
     - fcor: float
         weighting factor for the FID first point
+    -------
+    Returns:
+    - pdata: 1darray
+        FID
     """
     # IFT
-    data = processing.ift(data, fcor=fcor)
+    data = processing.ift(pdata, fcor=fcor)
     # Reverse zero-filling
     if size is not None:
-        data = processing.td_eff(data, size)
+        pdata = processing.td_eff(pdata, size)
     # Reverse window function
     if wf is not None:
         if wf['mode'] == None:
-            apod = np.ones_like(data)
+            apod = np.ones_like(pdata)
         if wf['mode'] == 'qsin':
-            apod = processing.qsin(data, ssb=wf['ssb'])/data
+            apod = processing.qsin(pdata, ssb=wf['ssb'])/pdata
         if wf['mode'] == 'sin':
-            apod = processing.sin(data, ssb=wf['ssb'])/data
+            apod = processing.sin(pdata, ssb=wf['ssb'])/pdata
         if wf['mode'] == 'em':
-            apod = processing.em(data, lb=wf['lb'], sw=wf['sw'])/data
+            apod = processing.em(pdata, lb=wf['lb'], sw=wf['sw'])/pdata
         if wf['mode'] == 'gm':
-            apod = processing.gm(data, lb=wf['lb'], gb=wf['gb'], sw=wf['sw'])/data
-        data = data / apod
-    return data
+            apod = processing.gm(pdata, lb=wf['lb'], gb=wf['gb'], sw=wf['sw'])/pdata
+        pdata = pdata / apod
+    return pdata
     
     
     
 def xfb(data, wf=[None, None], zf=[None, None], fcor=[0.5,0.5], tdeff=[0,0], u=True, FnMODE='States-TPPI'):
     """
-    Performs the full processing of a 2D NMR FID (data). Required parameters are:
-    - wf:   list of two entries [F1, F2]. Each entry is a dictionary: 
-                {'mode': function to be used, 
-                'parameters': different from each function}
-    - zf:   list of two entries [zf F1, zf F2]
-    - fcor: first fid point weighting factor
-    - u :   if True, unpacks the hypercomplex spectrum and returns the 4 ser
-    - tdeff: number of points of the FID to be used for the processing.
+    Performs the full processing of a 2D NMR FID (data). 
+    The returned values depend on u: it is True, returns a sequence of 2darrays depending on FnMODE, otherwise just the complex/hypercomplex data after FT in both dimensions
+    --------
+    Parameters:
+    - data: 2darray
+        Input data
+    - wf: sequence of dict
+        (F1, F2); {'mode': function to be used, 'parameters': different from each function}
+    - zf: sequence of int
+        final size of spectrum, (F1, F2)
+    - fcor: sequence of float 
+        weighting factor for the FID first point, (F1, F2)
+    - tdeff: sequence of int
+        number of points of the FID to be used for the processing, (F1, F2)
+    - u: bool
+        choose if to unpack the hypercomplex spectrum into separate arrays or not
+    - FnMODE: str
+        Acquisition mode in F1
+    ------
+    Returns:
+    - datap: 2darray or tuple of 2darray
+        Processed data or tuple of 2darray
     """
     
     data = processing.td_eff(data, tdeff)
     
     # Processing the direct dimension
     # Window function
     if wf[1] is not None:
@@ -949,15 +1183,15 @@
     ppm_f1 = misc.freq2ppm(fq1_scale, acqu1s['SFO1'], acqu1s['o1p'])
     #   F2
     fq2_scale = processing.make_scale(data.shape[1], acqu2s['dw'], rev=True)
     ppm_f2 = misc.freq2ppm(fq2_scale, acqu2s['SFO1'], acqu2s['o1p'])
 
     # Define useful things 
     modes = ['No', 'em', 'sin', 'qsin', 'gm', 'gmb']   # entries for the radiobuttons
-    act_keys = {    # Active parameters
+    act_keys = {    # Active Parameters:
             'No': [],
             'em': ['lb'],
             'sin': ['ssb'],
             'qsin': ['ssb'],
             'gm': ['lb', 'gb', 'gc'],
             'gmb': ['lb', 'gb'],
             }
@@ -1352,31 +1586,29 @@
     # Calculate final spectrum. Do not unpack the hyperser
     datap = processing.xfb(fid, wf=procs['wf'], zf=procs['zf'], tdeff=procs['tdeff'], FnMODE=acqus['FnMODE'], u=False)
 
     # Return hyperser and updated procs dictionary
     return datap, procs
 
 
-def inv_xfb(data, wf=[None, None], size=[None, None], fcor=[0.5,0.5], FnMODE='States-TPPI'):
+def inv_xfb(data, wf=[None, None], size=(None, None), fcor=[0.5,0.5], FnMODE='States-TPPI'):
     """
-    Performs the full processing of a 2D NMR FID (data). Required parameters are:
+    Reverts the full processing of a 2D NMR FID (data).
     -------
     Parameters:
     - data: 2darray
-        Input data
+        Input data, hypercomplex
     - wf: list of dict
         list of two entries [F1, F2]. Each entry is a dictionary of window functions
-    - zf: list
-        list of two entries [zf F1, zf F2]
-    - fcor: list
+    - size: list of int
+        Initial size of FID
+    - fcor: list of float
         first fid point weighting factor [F1, F2]
-    - u : bool
-        If True, unpacks the hypercomplex spectrum and returns the 4 ser
-    - tdeff: list of int
-        number of points of the FID to be used for the processing, [F1, F2]
+    - FnMODE: str
+        Acquisition mode in F1
     --------
     Returns:
     - data: 2darray
         Processed data
     """
 
     # Processing the indirect dimension
@@ -1396,15 +1628,15 @@
     elif FnMODE == 'Echo-Antiecho' or FnMODE == 'QF':
         data = processing.ift(data, fcor=fcor[0])
     else:
         raise NotImplementedError('Unknown acquisition mode in F1. Aborting...')
 
     # Revert zero-filling
     if size[0] is not None:
-        data = processing.td_eff(data, size[0])
+        data = processing.td_eff(data, (0, size[0]))
 
     # Reverse window function
     if wf[0] is not None:
         if wf[0]['mode'] == None:
             apod = np.ones_like(data)
         if wf[0]['mode'] == 'qsin':
             apod = processing.qsin(data, ssb=wf[0]['ssb'])/data
@@ -1423,15 +1655,15 @@
         data = processing.tp_hyper(data)
 
     # IFT on F2
     data = processing.ift(data, fcor=fcor[1])
 
     # Revert zero-filling
     if size[1] is not None:
-        data = processing.td_eff(data, size[1])
+        data = processing.td_eff(data, (0, size[1]))
 
     # Reverse window function
     if wf[1] is not None:
         if wf[1]['mode'] == None:
             apod = np.ones_like(data)
         if wf[1]['mode'] == 'qsin':
             apod = processing.qsin(data, ssb=wf[1]['ssb'])/data
@@ -1444,18 +1676,28 @@
         data = data / apod
 
     return data
 
 
 def make_scale(size, dw, rev=True):
     """
-    Computes the frequency scale of the NMR spectrum, given 
-    the # of points and the employed dwell time (the REAL one, not
-    the TopSpin one!). "rev"=True is required for the correct frequency arrangement
-    in the NMR sense.
+    Computes the frequency scale of the NMR spectrum, given the # of points and the employed dwell time (the REAL one, not the TopSpin one!). 
+    "rev"=True is required for the correct frequency arrangement in the NMR sense.
+    --------
+    Parameters:
+    - size: int
+        Number of points of the frequency scale
+    - dw : float
+        Time spacing in the time dimension
+    - rev: bool
+        Reverses the scale
+    -------
+    Returns:
+    - fqscale: 1darray
+        The computed frequency scale.
     """
     fqscale = np.fft.fftshift(np.fft.fftfreq(size, d=dw))
     if rev:
         fqscale = fqscale[::-1]
     return fqscale
 
 # ------------------------------------------------------------------------------------
@@ -1575,23 +1817,24 @@
 
 
 
 # Phase correction
 def interactive_phase_1D(ppmscale, S):
     """
     This function allow to adjust the phase of 1D spectra interactively. Use the mouse scroll to regulate the values.
-    Parameters
-    -   ppmscale: 1darray
-            ppm scale of the spectrum. Used to regulate the pivot position
-    -   S:  1darray
-            Spectrum to be phased. Must be complex!
-
-    Returns
-    -   phased_data: 1darray
-            Phased spectrum
+    -------
+    Parameters:
+    - ppmscale: 1darray
+        ppm scale of the spectrum. Used to regulate the pivot position
+    - S:  1darray
+        Spectrum to be phased. Must be complex!
+    -------
+    Returns:
+    - phased_data: 1darray
+        Phased spectrum
     """
 
     def phase(data, p0=0, p1=0, pivot=None):
         """ This is the actual phase function """
         if data.dtype != 'complex64':
             data = data.astype('complex64')
         size = data.shape[-1]
@@ -1793,15 +2036,33 @@
     return phased_data, final_values
 
 
 
 def interactive_phase_2D(ppm_f1, ppm_f2, S, hyper=True):
     """
     Interactively adjust the phases of a 2D spectrum
-    S must be hypercomplex, so BEFORE TO UNPACK
+    S must be complex or hypercomplex, so BEFORE TO UNPACK
+    -------
+    Parameters:
+    - ppm_f1: 1darray
+        ppm scale of the indirect dimension
+    - ppm_f2: 1darray
+        ppm scale of the direct dimension
+    - S: 2darray
+        Data to be phase-adjusted
+    - hyper: bool
+        True if S is hypercomplex, False if S is just complex
+    -------
+    Returns:
+    - S: 2darray
+        Phased data
+    - final_values_f1: tuple
+        (p0_f1, p1_f1, pivot_f1)
+    - final_values_f2: tuple
+        (p0_f2, p1_f2, pivot_f2)
     """
 
     # Unpack the hyperser
     if hyper:
         S_rr, S_ri, S_ir, S_ii = processing.unpack_2D(S)
     else:
         S_rr, S_ii = S.real, S.imag
@@ -2134,15 +2395,15 @@
     seldim.on_clicked(change_dim)
     scroll = fig.canvas.mpl_connect('scroll_event', on_scroll)
     fig.canvas.mpl_connect('key_press_event', zoom_onoff)
 
 
     plt.show()
 
-    # Phase the spectrum with the final parameters
+    # Phase the spectrum with the final Parameters:
     S = phase(S, p0=p0_f2, p1=p1_f2, pivot=pivot_f2, dim='f2')
     if hyper:
         S = processing.tp_hyper(S)
     else:
         S = S.T
     S = phase(S, p0=p0_f1, p1=p1_f1, pivot=pivot_f1, dim='f1')
     if hyper:
@@ -2183,15 +2444,15 @@
     # Integration step
     dx = misc.calcres(x_in)
 
     if lims is None:    # whole range
         x_tr, fx_tr = np.copy(x_in), np.copy(fx_in)
     else:
         # Trim data according to lims
-        x_tr, fx_tr = misc.trim_data(x_in, fx_in, *lims)
+        x_tr, fx_tr = misc.trim_data(x_in, fx_in, lims)
     
     # Integrate
     Fx = np.cumsum(fx_tr, axis=-1) * dx
     return Fx
 
 def integral_2D(ppm_f1, t_f1, SFO1, ppm_f2, t_f2, SFO2, u_1=None, fwhm_1=200, utol_1=0.5, u_2=None, fwhm_2=200, utol_2=0.5, plot_result=False):
     """
@@ -2595,19 +2856,29 @@
     else:
         #data = np.concatenate([input_data[w] for w in range(nds)], axis=0).astype('complex128')
         data = np.concatenate(Q, axis=0).astype('complex128')
     return data
 
 
 def MCR_unpack(C, S, nds, H=True):
-    # Reverts matrix augmentation of stack_MCR.
-    # if H is True, converts C from dimensions (Y, n)    to (X, Y, n)
-    #                    and S from dimensions (n, X*Z)  to (X, n, Z)
-    # if H is False converts C from dimensions (Y, n)    to (X, Y, n)
-    #                    and S from dimensions (n, X*Z)  to (X, n, Z)
+    """
+    Reverts matrix augmentation of stack_MCR.
+    > if H is True: converts C from dimensions (Y, n) to (X, Y, n) and S from dimensions (n, X*Z)  to (X, n, Z)
+    > if H is False:  converts C from dimensions (Y, n) to (X, Y, n) and S from dimensions (n, X*Z)  to (X, n, Z)
+    --------
+    Parameters:
+    - C: 2darray
+        MCR C matrix
+    - S: 2darray
+        MCR S matrix
+    - nds: int
+        number of experiments
+    - H: bool
+        True for horizontal stacking, False for vertical
+    """
     if H:
         C_f = np.array([C for w in range(nds)])
         S_f = np.array(np.split(S, nds, axis=1))
     else:
         C_f = np.array(np.split(C, nds, axis=0))
         S_f = np.array([S for w in range(nds)])
     return C_f, S_f
@@ -2828,36 +3099,36 @@
 
 
 def MCR_ALS(D, C, S, itermax=10000, tol=1e-5):
     """
     Performs alternating least squares to get the final C and S matrices. Being the fundamental MCR equation:
         D = CS + E
     At the k-th step of the iterative cycle:
-        1. C(k) = DS+(k−1)
+        1. C(k) = DS+(k-1)
         2. S(k) = C+(k) D
-        3. E(k) = D − C(k) S(k)
+        3. E(k) = D - C(k) S(k)
     Defined rC and rS as the Frobenius norm of the difference of C and S matrices between two subsequent steps:
-        rC = || C(k) − C(k−1) ||
-        rS = || S(k) − S(k−1) ||
+        rC = || C(k) - C(k-1) ||
+        rS = || S(k) - S(k-1) ||
     The convergence is reached when:
         rC <= tol && rS <= tol
     -------
     Parameters:
     - D: 2darray
-        Input data, of dimensions m × n
+        Input data, of dimensions m x n
     - C: 2darray
         Estimation of the C matrix, of dimensions m x nc.
     - S: 2darray
         Estimation of the S matrix, of dimensions nc x n.
     - itermax: int
         Maximum number of iterations
     - tol: float
         Threshold for the arrest criterion.
     -------
-    Returns
+    Returns:
     - C: 2darray
         Optimized C matrix, of dimensions m x nc.
     - S: 2darray
         Optimized S matrix, of dimensions nc x n.
     """
 
     itermax = int(itermax)
@@ -2899,14 +3170,17 @@
         print ('\n\n\tMCR does not converge.')
     end_time = datetime.now()
     print( '\tTotal runtime: {}'.format(end_time - start_time))
 
     return C, S
     
 def new_MCR_ALS(D, C, S, itermax=10000, tol=1e-5, reg_f=None, reg_fargs=[]):
+    """
+    Modified function to do ALS
+    """
 
     itermax = int(itermax)
     E = D - C @ S
 
     start_time = datetime.now()
     print('\n-----------------------------------------------------\n')
     print('             MCR optimization running...             \n')
@@ -2955,97 +3229,27 @@
     if not convergence_flag:
         print ('\n\n\tMCR does not converge.')
     end_time = datetime.now()
     print( '\tTotal runtime: {}'.format(end_time - start_time))
 
     return C, S
 
-def MCR_WALS(D, C, S, errmat, itermax=10000, tol=1e-5):
-    itermax = int(itermax)
-    Vc = np.zeros((errmat.shape[0])).astype(D.dtype)
-    Vs = np.zeros((errmat.shape[1])).astype(D.dtype)
-    for i in range(D.shape[0]):
-        Vc[i] = np.std(errmat[i])**2
-    for j in range(D.shape[1]):
-        Vs[j] = np.std(errmat[:,j])**2
-    print(Vc.shape, Vs.shape)
-    plt.plot(Vc)
-    plt.show()
-    E = D - C @ S
-
-    start_time = datetime.now()
-    print('\n-----------------------------------------------------\n')
-    print('             MCR optimization running...             \n')
-
-    convergence_flag = 0
-    print( '#   \tC convergence\tS convergence')
-    X = np.zeros_like(D)
-    """
-    for i in range(D.shape[0]):
-        X[i,:] = D[i,:] * Vs
-    """
-    for j in range(D.shape[1]):
-        X[:,j] = D[:,j] * Vc
-    for kk in range(itermax):
-        # Copy from previous cycle
-        C0 = np.copy(C)
-        E0 = np.copy(E)
-        S0 = np.copy(S)
-
-        """
-        # Projection of D in S space
-        # Compute new C
-        Sp = np.array([S[w,:] * Vs for w in range(S.shape[0])])
-        C = X @ linalg.pinv(Sp)
-        # Compute new S
-        S = linalg.pinv(C) @ D
-        """
-        Cp = np.array([C[:,w] * Vc for w in range(C.shape[1])]).T
-        S = linalg.pinv(Cp) @ X
-        C = D @ linalg.pinv(S)
-
-        E = D - C @ S
-
-        # Compute the Frobenius norm of the difference matrices
-        # between two subsequent cycles
-        rC = linalg.norm(C - C0)
-        rS = linalg.norm(S - S0)
-
-        # Ongoing print of the residues
-        print(str(kk+1)+' \t{:.5e}'.format(rC)+ '\t'+'{:.5e}'.format(rS), end='\r')
-
-        # Arrest criterion
-        if (rC < tol) and (rS < tol):
-            end_time = datetime.now()
-            print( '\n\n\tMCR converges in '+str(kk+1)+' steps.')
-            convergence_flag = 1    # Set to 1 if the arrest criterion is reached
-            break
-
-    if not convergence_flag:
-        print ('\n\n\tMCR does not converge.')
-    end_time = datetime.now()
-    print( '\tTotal runtime: {}'.format(end_time - start_time))
-    
-
-    return C, S
-
-
 
 def MCR(input_data, nc, f=10, tol=1e-5, itermax=1e4, H=True, oncols=True):
     """
     This is an implementation of Multivariate Curve Resolution for the denoising of 2D NMR data.
     Let us consider a matrix D, of dimensions m x n, where the starting data are stored. The final purpose of MCR is to decompose the D matrix as follows:
         D = CS + E
     where C and S are matrices of dimension m x nc and nc x n, respectively, and E contains the part of the data that are not reproduced by the factorization.
     Being D the FID of a NMR spectrum, C will contain time evolutions of the indirect dimension, and S will contain transients in the direct dimension.
 
     The total MCR workflow can be separated in two parts: a first algorithm that produces an initial guess for the three matrices C, S and E (SIMPLISMA), and an optimization step that aims at the removal of the unwanted features of the data by iteratively filling the E matrix (MCR ALS).
     This function returns the denoised datasets, CS, and the single C and S matrices.
     -------
-    Parameters
+    Parameters:
     - input_data: 2darray or 3darray
         a 3D array containing the set of 2D NMR datasets to be coprocessed stacked along the first dimension. A single 2D array can be passed, if the denoising of a single dataset is desired.
     - nc: int
         number of purest components to be looked for;
     - f: float
         percentage of allowed noise;
     - tol: float
@@ -3053,15 +3257,15 @@
     - itermax: int
         maximum number of allowed iterations
     - H: bool
         True for horizontal stacking of data (default), False for vertical;
     - oncols: bool
         True to estimate S with processing.SIMPLISMA, False to estimate C.
     -------
-    Returns
+    Returns:
     - CS_f: 2darray or 3darray
         Final denoised data matrix
     - C_f: 2darray or 3darray
         Final C matrix
     - S_f: 2darray or 3darray
         Final S matrix
     """
@@ -3118,25 +3322,27 @@
     return CS_f, C_f, S_f
 
 # ---------------------------------------------------------------------------------------- #
 
 
 
 def new_MCR(input_data, nc, f=10, tol=1e-5, itermax=1e4, H=True, oncols=True, our_function=None, fargs=[], our_function2=None, f2args=[]):
+    """
     # This is an implementation of Multivariate Curve Resolution
     # for the denoising of 2D NMR data. It requires:
     # - input_data: a tensor containing the set of 2D NMR datasets to be coprocessed
     #   stacked along the first dimension;
     # - nc      : number of purest components;
     # - f       : percentage of allowed noise;
     # - tol     : tolerance for the arrest criterion;
     # - itermax : maximum number of allowed iterations, default 10000
     # - H       : True for horizontal stacking of data (default), False for vertical;
     # - oncols  : True to estimate S with purest components, False to estimate C
     # This function returns the denoised datasets, 'CS', and the 'C' and 'S' matrices.
+    """
 
     # Get number of datasets (nds) from the shape of the input tensor
     if isinstance(input_data, list):
         nds = len(input_data)
     else:
         if len(input_data.shape) == 3:
             nds = input_data.shape[0]
@@ -3275,18 +3481,34 @@
     4. Rebuild H' = U S' V
     5. Average the antidiagonals to rebuild the Hankel-type structure, then make 1D array
     6. Check arrest criterion: if it is not reached, go to 1, else exit.
 
     The arrest criterion is:
     | S(step k-1)[nc-1] / S(step k-1)[0] - S(step k)[nc-1] / S(step k)[0] | < f * S(step 0)[nc-1] / S(step 0)[0]
 
-    - itermax:      max number of iterations allowed
-    - f:            factor that appears in the arrest criterion
-    - print_time:   set it to True to show the time it took
-    - print_head:   set it to True to display the fancy heading.
+    --------
+    Parameters:
+    - data: 1darray
+        Data to be processed
+    - n: int
+        Number of columns of the Hankel matrix
+    - nc: int
+        Number of singular values to preserve
+    - itermax: int
+        max number of iterations allowed
+    - f: float
+        factor that appears in the arrest criterion
+    - print_time: bool
+        set it to True to show the time it took
+    - print_head: bool
+        set it to True to display the fancy heading.
+    --------
+    Returns:
+    - datap: 1darray
+        Denoised data
     """
 
     if print_head is True:
         print('\n*****************************************************')
         print('*                                                   *')
         print('*                   Cadzow denoising                *')
         print('*                                                   *')
@@ -3402,15 +3624,15 @@
     -------
     Parameters:
     - ppm: 1darray
         PPM scale of the spectrum
     - data: 1darray
         Spectrum to be partitioned
     -------
-    Returns
+    Returns:
     - coord: list
         List containing the coordinates of the windows, plus ppm[0] and ppm[-1]
     """
 
     # Make the figure
     fig = plt.figure()
     fig.set_size_inches(15,8)
```

### Comparing `klassez-0.1a1/klassez/sim.py` & `klassez-0.1a2/klassez/sim.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import seaborn as sns
 import nmrglue as ng
 import lmfit as l
 from datetime import datetime
 import warnings
 
 from . import fit, misc, sim, figures, processing
-from .config import CM
+from .config import CM, COLORS, cron
 #from .__init__ import CM
 
   
 gamma = {   # gyromagnetic ratio of all NMR active nuclei in MHz/T
 	'1H'	:	42.57748,
 	'2H'	:	6.53564,
 	'3H'	:	45.41461,
@@ -296,21 +296,21 @@
 
     return dic
 
 def sim_1D(File, pv=False):
     """
     Simulates a 1D NMR spectrum from the instructions written in File.
     -------
-    Parameters
+    Parameters:
     - File: str
         Path to the input file location
     - pv: bool
         True for pseudo-Voigt model, False for Voigt model.
     -------
-    Returns
+    Returns:
     - fid: 1darray
         FID of the simulated spectrum.
     """
     if isinstance(File, str):
         in_file = load_sim_1D(File)
     elif isinstance(File, dict):
         in_file = File
@@ -339,21 +339,21 @@
                 fid += sim.t_voigt(**sgn_par)
     return fid
 
 def load_sim_2D(File, states=True):
     """
     Creates a dictionary from the spectral parameters listed in the input file.
     -------
-    Parameters
+    Parameters:
     - File: str
         Path to the input file location
     - states: bool
         If FnMODE is States or States-TPPI, set it to True to get the correct timescale.
     -------
-    Returns
+    Returns:
     - dic: dict
         Dictionary of the parameters, ready to be read from the simulation functions.
     """
     inp = open(File, 'r').readlines()
     keys = []
     vals = []
     for i in range(len(inp)):
@@ -401,25 +401,25 @@
     return dic
 
 def sim_2D(File, states=True, alt=True, pv=False):
     """
     Simulates a 2D NMR spectrum from the instructions written in File.
     The indirect dimension is sampled with states-TPPI as default.
     --------
-    Parameters
+    Parameters:
     - File: str
         Path to the input file location
     - states: bool
         Set it to True to allow for correct spectral arrangement in the indirect dimension.
     - alt: bool
         Set it to True to allow for correct spectral arrangement in the indirect dimension.
     - pv: bool
         True for pseudo-Voigt model, False for Voigt model.
     --------
-    Returns
+    Returns:
     - fid: 2darray
         FID of the simulated spectrum.
     """
     
     # Generates a dictionary of parameters from an input file
     if isinstance(File, str):
         in_file = sim.load_sim_2D(File, states=states)
@@ -472,25 +472,25 @@
             fid += sim.t_2Dvoigt(t1, t2, freq1[p], freq2[p], fwhm1[p], fwhm2[p], A=amplitudes[p], x_g=x_g[p], states=states, alt=alt)
     return fid
 
 def noisegen(size, o2, t2, s_n=1):
     """
     Simulates additive noise in the time domain.
     --------
-    Parameters
+    Parameters:
     - size: int or tuple
         Dimension of the noise matrix
     - o2: float
         Carrier frequency, in Hz.
     - t2: 1darray
         Time scale of the last temporal dimension.
     - s_n: float
         Standard deviation of the noise.
     --------
-    Returns
+    Returns:
     - noise: 2darray
         Noise matrix, of dimensions size.
     """
 
     # correlated part of noise until ADC
     white_corr = np.random.normal(0, s_n, size)
     # white noise in FID has to be centered on the offset frequency
@@ -505,14 +505,15 @@
 
     # final noise is sum of the two parts
     noise = noise_corr + (noise_re + 1j*noise_im)
     return noise
 
 
 def mult_noise(data_size, mean, s_n):
+    """ Multiplicative noise model. """
     N = data_size[0]
 
     white = np.random.lognormal(mean, s_n, N)
     #white = np.random.normal(0, s_n, N)
 
     #noisemat = np.diag(1 - 0.25 * white)
     noisemat = np.diag(white)
@@ -520,29 +521,29 @@
 
 
 
 def water7(N, t2, vW, fwhm=300, A=1, spread=701.125):
     """
     Simulates a feature like the water ridge in HSQC spectra, in the time domain.
     --------
-    Parameters
+    Parameters:
     - N: int
         Number of transients
     - t2: 1darray
         Time scale of the last temporal dimension.
     - vW: float
         Nominal peak position, in Hz.
     - fwhm: float
-        Nominal full-width at half maximum of the peak.
+        Nominal full-width at half maximum of the peak, in rad/s.
     - A: float
         Signal intensity.
     - spread: float
         Standard deviation of the peak position distribution, in Hz.
     --------
-    Returns
+    Returns:
     - ridge: 2darray
         Matrix of the ridge.
     """
 
 
     uW = np.random.normal(vW, spread, N)
     s = fwhm / 2.355        # conversion from fwhm to sigma
@@ -554,49 +555,49 @@
     return ridge 
 
 
 def f_gaussian(x, u, s, A=1):
     """
     Gaussian function in the frequency domain:
     --------
-    Parameters
+    Parameters:
     - x: 1darray
         Independent variable
     - u: float
         Peak position
     - s: float
         Standard deviation
     - A: float
         Intensity
     --------
-    Returns
+    Returns:
     - f: 1darray
         Gaussian function.
     """
     if s > 0:
         f = A/(np.sqrt(2 * np.pi)*s) * np.exp(-1/2*((x-u)/s)**2)
     else:
         f = np.zeros_like(x)
     return f
 
 def f_lorentzian(x, u, fwhm, A=1):
     """
     Lorentzian function in the time domain:
     --------
-    Parameters
+    Parameters:
     - x: 1darray
         Independent variable
     - u: float
         Peak position
     - fwhm: float
-        Full-width at half-maximum, 2γ
+        Full-width at half-maximum
     - A: float
         Intensity
     --------
-    Returns
+    Returns:
     - f: 1darray
         Lorentzian function.
     """
 
     hwhm = fwhm/2   # half width at half maximum
     if hwhm > 0:
         f = A/(np.pi) * hwhm/((x-u)**2 + hwhm**2 )
@@ -604,163 +605,163 @@
         f = np.zeros_like(x)
     return f
 
 def f_pvoigt(x, u, fwhm, A=1, x_g=0):
     """
     Pseudo-Voigt function in the frequency domain:
     --------
-    Parameters
+    Parameters:
     - x: 1darray
         Independent variable
     - u: float
         Peak position
     - fwhm: float
         Full-width at half-maximum
     - A: float
         Intensity
     - x_g: float
         Fraction of gaussianity
     --------
-    Returns
+    Returns:
     - S: 1darray
         Pseudo-Voigt function.
     """
     s = fwhm / 2.355
     S = A* (sim.f_gaussian(x, u, s, A=x_g) + sim.f_lorentzian(x, u, fwhm, A=1-x_g))
     return S
 
 def t_gaussian(t, u, s, A=1, phi=0):
     """
     Gaussian function in the time domain.
     --------
-    Parameters
+    Parameters:
     - t: 1darray
         Independent variable
     - u: float
-        Peak position
+        Peak position, in Hz
     - s: float
-        Standard deviation
+        Standard deviation, in rad/s
     - A: float
         Intensity
     - phi: float
         Phase, in radians
     --------
-    Returns
+    Returns:
     - S: 1darray
         Gaussian function.
     """
     s = np.abs(s) # Avoid problems with s<0 
     if s >= 0:
         S = A * np.exp(1j*phi) * np.exp((1j*2*np.pi*u*t) - (t**2)*(s**2)/2)
     return S
 
 def t_lorentzian(t, u, fwhm, A=1, phi=0):
     """
     Lorentzian function in the time domain.
     --------
-    Parameters
+    Parameters:
     - t: 1darray
         Independent variable
     - u: float
-        Peak position
+        Peak position, in Hz
     - fwhm: float
-        Full-width at half-maximum, 2γ
+        Full-width at half-maximum, in rad/s
     - A: float
         Intensity
     - phi: float
         Phase, in radians
     --------
-    Returns
+    Returns:
     - S: 1darray
         Lorentzian function.
     """
     hwhm = np.abs(fwhm) / 2       
     S = A * np.exp(1j*phi) * np.exp((1j *2*np.pi *u * t)-(t*hwhm))
     return S
 
 def t_pvoigt(t, u, fwhm, A=1, x_g=0, phi=0):
     """
     Pseudo-Voigt function in the time domain:
     --------
-    Parameters
+    Parameters:
     - t: 1darray
         Independent variable
     - u: float
-        Peak position
+        Peak position, in Hz
     - fwhm: float
-        Full-width at half-maximum
+        Full-width at half-maximum, in rad/s
     - A: float
         Intensity
     - x_g: float
         Fraction of gaussianity
     - phi: float
         Phase, in radians
     --------
-    Returns
+    Returns:
     - S: 1darray
         Pseudo-Voigt function.
     """
 
     s = fwhm / 2.355
     S = A * (sim.t_gaussian(t, u, s, A=x_g, phi=phi) + sim.t_lorentzian(t, u, fwhm, A=1-x_g, phi=phi))
     return S
 
 def t_voigt(t, u, fwhm, A=1, x_g=0, phi=0):
     """
     Voigt function in the time domain. The parameter x_g affects the linewidth of the lorentzian and gaussian contributions.
     --------
-    Parameters
+    Parameters:
     - t: 1darray
         Independent variable
     - u: float
-        Peak position
+        Peak position, in Hz
     - fwhm: float
-        Full-width at half-maximum
+        Full-width at half-maximum, in rad/s
     - A: float
         Intensity
     - x_g: float
         Fraction of gaussianity
     - phi: float
         Phase, in radians
     --------
-    Returns
+    Returns:
     - S: 1darray
         Voigt function.
     """
 
     s = fwhm / 2.355
     S = A * np.exp(1j*phi) * sim.t_gaussian(t, u/2, s*x_g) * sim.t_lorentzian(t, u/2, fwhm*(1-x_g))
     return S
 
 
 def t_2Dgaussian(t1, t2, v1, v2, s1, s2, A=1, states=True, alt=True):
     """
     Bidimensional gaussian function.
     --------
-    Parameters
+    Parameters:
     - t1: 1darray
         Indirect evolution timescale
     - t2: 1darray
         Timescale of the direct dimension
     - v1: float
-        Peak position in the indirect dimension
+        Peak position in the indirect dimension, in Hz
     - v2: float
-        Peak position in the direct dimension
+        Peak position in the direct dimension, in Hz
     - s1: float
-        Standard deviation in the indirect dimension
+        Standard deviation in the indirect dimension, in rad/s
     - s2: float
-        Standard deviation in the direct dimension
+        Standard deviation in the direct dimension, in rad/s
     - A: float
         Intensity
     - states: bool
         Set to True for "FnMODE":"States-TPPI
     - alt: bool
         Set to True for "FnMODE":"States-TPPI
     --------
-    Returns
+    Returns:
     - S: 2darray
         Gaussian function.
     """
     if states:
         # States acquires twice the same point of the indirect dimension time domain
         t1[1::2] = t1[::2]
     if alt:
@@ -779,35 +780,35 @@
     S = A * F1.reshape(-1,1) @ F2.reshape(1,-1)
     return S
 
 def t_2Dlorentzian(t1, t2, v1, v2, fwhm1, fwhm2, A=1, states=True, alt=True):
     """
     Bidimensional lorentzian function.
     --------
-    Parameters
+    Parameters:
     - t1: 1darray
         Indirect evolution timescale
     - t2: 1darray
         Timescale of the direct dimension
     - v1: float
-        Peak position in the indirect dimension
+        Peak position in the indirect dimension, in Hz
     - v2: float
-        Peak position in the direct dimension45
+        Peak position in the direct dimension, in Hz
     - fwhm1: float
-        Full-width at half maximum in the indirect dimension
+        Full-width at half maximum in the indirect dimension, in rad/s
     - fwhm2: float
-        Full-width at half maximum in the direct dimension
+        Full-width at half maximum in the direct dimension, in rad/s
     - A: float
         Intensity
     - states: bool
         Set to True for "FnMODE":"States-TPPI
     - alt: bool
         Set to True for "FnMODE":"States-TPPI
     --------
-    Returns
+    Returns:
     - S: 2darray
         Lorentzian function.
     """
     hwhm1 = fwhm1 / 2
     hwhm2 = fwhm2 / 2
     if states:
         # States acquires twice the same point of the indirect dimension time domain
@@ -830,37 +831,37 @@
 
 def t_2Dpvoigt(t1, t2, v1, v2, fwhm1, fwhm2, A=1, x_g=0.5, states=True, alt=True):
     """
     Generates a 2D pseudo-voigt signal in the time domain.
     x_g states for the fraction of gaussianity, whereas A defines the overall amplitude of the total peak.
     Indexes ’1’ and ’2’ on the variables stand for ’F1’ and ’F2’, respectively.
     --------
-    Parameters
+    Parameters:
     - t1: 1darray
         Indirect evolution timescale
     - t2: 1darray
         Timescale of the direct dimension
     - v1: float
-        Peak position in the indirect dimension
+        Peak position in the indirect dimension, in Hz
     - v2: float
-        Peak position in the direct dimension
+        Peak position in the direct dimension, in Hz
     - fwhm1: float
-        Full-width at half maximum in the indirect dimension
+        Full-width at half maximum in the indirect dimension, in rad/s
     - fwhm2: float
-        Full-width at half maximum in the direct dimension
+        Full-width at half maximum in the direct dimension, in rad/s
     - A: float
         Intensity
     - x_g: float
         Fraction of gaussianity
     - states: bool
         Set to True for "FnMODE":"States-TPPI
     - alt: bool
         Set to True for "FnMODE":"States-TPPI46
     --------
-    Returns
+    Returns:
     - fid: 2darray
         Pseudo-Voigt function.
     """
 
     # stdev computed for the gaussian part.
     s1 = fwhm1 / 2.355
     s2 = fwhm2 / 2.355
@@ -872,37 +873,37 @@
 
 def t_2Dvoigt(t1, t2, v1, v2, fwhm1, fwhm2, A=1, x_g=0.5, states=True, alt=True):
     """
     Generates a 2D Voigt signal in the time domain.
     x_g states for the fraction of gaussianity, whereas A defines the overall amplitude of the total peak.
     Indexes ’1’ and ’2’ on the variables stand for ’F1’ and ’F2’, respectively.
     --------
-    Parameters
+    Parameters:
     - t1: 1darray
         Indirect evolution timescale
     - t2: 1darray
         Timescale of the direct dimension
     - v1: float
-        Peak position in the indirect dimension
+        Peak position in the indirect dimension, in Hz
     - v2: float
-        Peak position in the direct dimension
+        Peak position in the direct dimension, in Hz
     - fwhm1: float
-        Full-width at half maximum in the indirect dimension
+        Full-width at half maximum in the indirect dimension, in rad/s
     - fwhm2: float
-        Full-width at half maximum in the direct dimension
+        Full-width at half maximum in the direct dimension, in rad/s
     - A: float
         Intensity
     - x_g: float
         Fraction of gaussianity
     - states: bool
         Set to True for "FnMODE":"States-TPPI
     - alt: bool
         Set to True for "FnMODE":"States-TPPI
     --------
-    Returns
+    Returns:
     - S: 2darray
         Voigt function.
     """
     # stdev computed for the gaussian part.
     s1 = fwhm1 / 2.355
     s2 = fwhm2 / 2.355
     # hwhm computed for the lorentzian part.
```

### Comparing `klassez-0.1a1/klassez/test/acqus_2D` & `klassez-0.1a2/klassez/test/acqus_2D`

 * *Files identical despite different names*

### Comparing `klassez-0.1a1/klassez.egg-info/PKG-INFO` & `klassez-0.1a2/klassez.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: klassez
-Version: 0.1a1
+Version: 0.1a2
 Summary: A collection of functions for NMR data handling. Documentation: klassez.pdf in "docs" subfolder of your install dir.
-Home-page: https://test.pypi.org/legacy/klassez
+Home-page: https://github.com/MetallerTM/klassez
 Author: Francesco Bruno
 Author-email: bruno@cerm.unifi.it
 License: LICENSE.txt
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `klassez-0.1a1/setup.py` & `klassez-0.1a2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,19 +6,19 @@
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 except:
     long_description = 'LONG DESCRIPTION'
 
 setup(
         name='klassez',
-        version='0.1a.1',
+        version='0.1a.2',
         author='Francesco Bruno',
         author_email='bruno@cerm.unifi.it',
         description='A collection of functions for NMR data handling. Documentation: klassez.pdf in "docs" subfolder of your install dir.',
-        url='https://test.pypi.org/legacy/klassez',
+        url='https://github.com/MetallerTM/klassez',
         long_description=long_description,
         long_description_content_type = 'text/markdown',
         classifiers = [
             'Programming Language :: Python :: 3',
             'Operating System :: OS Independent',
             'License :: OSI Approved :: MIT License'
             ],
```


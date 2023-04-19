# Comparing `tmp/molecularprofiles-0.2.0.tar.gz` & `tmp/molecularprofiles-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecularprofiles-0.2.0.tar", last modified: Wed Mar 15 14:24:07 2023, max compression
+gzip compressed data, was "molecularprofiles-0.3.0.tar", last modified: Wed Apr 19 08:12:54 2023, max compression
```

## Comparing `molecularprofiles-0.2.0.tar` & `molecularprofiles-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-03-15 14:24:07.357323 molecularprofiles-0.2.0/
--rw-r--r--   0 mdalchen   (501) staff       (20)     1474 2022-11-22 15:24:35.000000 molecularprofiles-0.2.0/LICENSE
--rw-r--r--   0 mdalchen   (501) staff       (20)     2654 2023-03-15 14:24:07.356912 molecularprofiles-0.2.0/PKG-INFO
--rw-r--r--   0 mdalchen   (501) staff       (20)      450 2023-02-01 16:41:16.000000 molecularprofiles-0.2.0/README.md
--rw-r--r--   0 mdalchen   (501) staff       (20)     1657 2023-02-10 13:01:21.000000 molecularprofiles-0.2.0/pyproject.toml
--rw-r--r--   0 mdalchen   (501) staff       (20)       38 2023-03-15 14:24:07.357471 molecularprofiles-0.2.0/setup.cfg
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-03-15 14:24:07.350107 molecularprofiles-0.2.0/src/
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-03-15 14:24:07.351565 molecularprofiles-0.2.0/src/molecularprofiles/
--rwxr-xr-x   0 mdalchen   (501) staff       (20)      195 2023-03-14 16:06:53.000000 molecularprofiles-0.2.0/src/molecularprofiles/__init__.py
--rwxr-xr-x   0 mdalchen   (501) staff       (20)    20643 2023-03-15 14:16:23.000000 molecularprofiles-0.2.0/src/molecularprofiles/molecularprofiles.py
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-03-15 14:24:07.356382 molecularprofiles-0.2.0/src/molecularprofiles/utils/
--rw-r--r--   0 mdalchen   (501) staff       (20)       27 2023-02-03 15:27:32.000000 molecularprofiles-0.2.0/src/molecularprofiles/utils/__init__.py
--rwxr-xr-x   0 mdalchen   (501) staff       (20)     1048 2023-03-15 13:55:37.000000 molecularprofiles-0.2.0/src/molecularprofiles/utils/constants.py
--rw-r--r--   0 mdalchen   (501) staff       (20)     5600 2023-03-14 16:23:52.000000 molecularprofiles-0.2.0/src/molecularprofiles/utils/dataframe_ops.py
--rwxr-xr-x   0 mdalchen   (501) staff       (20)    16512 2023-03-14 17:16:31.000000 molecularprofiles-0.2.0/src/molecularprofiles/utils/grib_utils.py
--rwxr-xr-x   0 mdalchen   (501) staff       (20)     9537 2023-03-15 14:01:00.000000 molecularprofiles-0.2.0/src/molecularprofiles/utils/humidity.py
--rw-r--r--   0 mdalchen   (501) staff       (20)      327 2023-02-03 15:27:32.000000 molecularprofiles-0.2.0/src/molecularprofiles/utils/mdps_log.conf
--rwxr-xr-x   0 mdalchen   (501) staff       (20)    10000 2023-02-16 09:50:26.000000 molecularprofiles-0.2.0/src/molecularprofiles/utils/observatory.py
--rw-r--r--   0 mdalchen   (501) staff       (20)    12842 2023-03-15 14:06:30.000000 molecularprofiles-0.2.0/src/molecularprofiles/utils/rayleigh.py
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-03-15 14:24:07.353184 molecularprofiles-0.2.0/src/molecularprofiles.egg-info/
--rw-r--r--   0 mdalchen   (501) staff       (20)     2654 2023-03-15 14:24:07.000000 molecularprofiles-0.2.0/src/molecularprofiles.egg-info/PKG-INFO
--rw-r--r--   0 mdalchen   (501) staff       (20)      666 2023-03-15 14:24:07.000000 molecularprofiles-0.2.0/src/molecularprofiles.egg-info/SOURCES.txt
--rw-r--r--   0 mdalchen   (501) staff       (20)        1 2023-03-15 14:24:07.000000 molecularprofiles-0.2.0/src/molecularprofiles.egg-info/dependency_links.txt
--rw-r--r--   0 mdalchen   (501) staff       (20)      206 2023-03-15 14:24:07.000000 molecularprofiles-0.2.0/src/molecularprofiles.egg-info/requires.txt
--rw-r--r--   0 mdalchen   (501) staff       (20)       18 2023-03-15 14:24:07.000000 molecularprofiles-0.2.0/src/molecularprofiles.egg-info/top_level.txt
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-04-19 08:12:54.383834 molecularprofiles-0.3.0/
+-rw-r--r--   0 mdalchen   (501) staff       (20)     1474 2022-11-22 15:24:35.000000 molecularprofiles-0.3.0/LICENSE
+-rw-r--r--   0 mdalchen   (501) staff       (20)     2654 2023-04-19 08:12:54.383550 molecularprofiles-0.3.0/PKG-INFO
+-rw-r--r--   0 mdalchen   (501) staff       (20)      450 2023-02-01 16:41:16.000000 molecularprofiles-0.3.0/README.md
+-rw-r--r--   0 mdalchen   (501) staff       (20)     1656 2023-04-19 08:01:37.000000 molecularprofiles-0.3.0/pyproject.toml
+-rw-r--r--   0 mdalchen   (501) staff       (20)       38 2023-04-19 08:12:54.383919 molecularprofiles-0.3.0/setup.cfg
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-04-19 08:12:54.371595 molecularprofiles-0.3.0/src/
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-04-19 08:12:54.373057 molecularprofiles-0.3.0/src/molecularprofiles/
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)      195 2023-04-19 08:02:09.000000 molecularprofiles-0.3.0/src/molecularprofiles/__init__.py
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)    19996 2023-04-19 08:02:40.000000 molecularprofiles-0.3.0/src/molecularprofiles/molecularprofiles.py
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-04-19 08:12:54.382873 molecularprofiles-0.3.0/src/molecularprofiles/utils/
+-rw-r--r--   0 mdalchen   (501) staff       (20)       27 2023-02-03 15:27:32.000000 molecularprofiles-0.3.0/src/molecularprofiles/utils/__init__.py
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)     1257 2023-04-19 08:01:37.000000 molecularprofiles-0.3.0/src/molecularprofiles/utils/constants.py
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)    16618 2023-04-19 08:02:40.000000 molecularprofiles-0.3.0/src/molecularprofiles/utils/grib_utils.py
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)    10506 2023-04-19 08:01:37.000000 molecularprofiles-0.3.0/src/molecularprofiles/utils/humidity.py
+-rw-r--r--   0 mdalchen   (501) staff       (20)      327 2023-02-03 15:27:32.000000 molecularprofiles-0.3.0/src/molecularprofiles/utils/mdps_log.conf
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)    10235 2023-04-19 08:01:37.000000 molecularprofiles-0.3.0/src/molecularprofiles/utils/observatory.py
+-rw-r--r--   0 mdalchen   (501) staff       (20)    14698 2023-04-19 08:02:40.000000 molecularprofiles-0.3.0/src/molecularprofiles/utils/rayleigh.py
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-04-19 08:12:54.375210 molecularprofiles-0.3.0/src/molecularprofiles.egg-info/
+-rw-r--r--   0 mdalchen   (501) staff       (20)     2654 2023-04-19 08:12:54.000000 molecularprofiles-0.3.0/src/molecularprofiles.egg-info/PKG-INFO
+-rw-r--r--   0 mdalchen   (501) staff       (20)      621 2023-04-19 08:12:54.000000 molecularprofiles-0.3.0/src/molecularprofiles.egg-info/SOURCES.txt
+-rw-r--r--   0 mdalchen   (501) staff       (20)        1 2023-04-19 08:12:54.000000 molecularprofiles-0.3.0/src/molecularprofiles.egg-info/dependency_links.txt
+-rw-r--r--   0 mdalchen   (501) staff       (20)      205 2023-04-19 08:12:54.000000 molecularprofiles-0.3.0/src/molecularprofiles.egg-info/requires.txt
+-rw-r--r--   0 mdalchen   (501) staff       (20)       18 2023-04-19 08:12:54.000000 molecularprofiles-0.3.0/src/molecularprofiles.egg-info/top_level.txt
```

### Comparing `molecularprofiles-0.2.0/LICENSE` & `molecularprofiles-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molecularprofiles-0.2.0/PKG-INFO` & `molecularprofiles-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecularprofiles
-Version: 0.2.0
+Version: 0.3.0
 Summary: Meteorological data analysis suite
 Author-email: Pere Munar Adrover <pere.munar@uab.cat>, Markus Gaug <markus.gaug@uab.cat>, Scott Griffiths <sgriffiths@ifae.es>, Georgios Voutsinas <georgios.voutsinas@unige.ch>, Mykhailo Dalchenko <mykhailo.dalchenko@unige.ch>
 License: Copyright (c) 2020, Molecularprofiles Project
         
         Redistribution and use in source and binary forms, with or withoutmodification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
```

### Comparing `molecularprofiles-0.2.0/pyproject.toml` & `molecularprofiles-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 dynamic = ["version"]
 classifiers = [
     "License :: OSI Approved :: BSD License",
 ]
 requires-python = ">=3.8"
 
 dependencies = [
-    "pandas",
+    "numpy",
     "scipy",
     "astropy",
     "pygrib",
     "statsmodels"
 ]
 
 [project.urls]
```

### Comparing `molecularprofiles-0.2.0/src/molecularprofiles/molecularprofiles.py` & `molecularprofiles-0.3.0/src/molecularprofiles/molecularprofiles.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """
 This is a class that offers a set of functions to work with meteorological data
-in txt table format, separated with spaces.
-
-It makes use of the pandas dataframe objects in order to be more efficient
-
+in ecsv or grib(2) format.
 
 Created by Pere Munar-Adrover
 email: pere.munaradrover@gmail.com
-
+Further developed and mainted by
+Mykhailo Dalchenko (mykhailo.dalchenko@unige.ch) and
+Georgios Voutsinas (georgios.voutsinas@unige.ch)
 """
 
 import os
-import sys
 import logging
 
+import astropy.units as u
 from astropy.table import Table
 import numpy as np
 from scipy.interpolate import interp1d
 
 from molecularprofiles.utils.grib_utils import get_grib_file_data, extend_grib_data
-from molecularprofiles.utils.constants import DENSITY_SCALE_HEIGHT
-from molecularprofiles.utils.dataframe_ops import (
-    compute_averages_std,
-    avg_std_dataframe,
+from molecularprofiles.utils.constants import (
+    DENSITY_SCALE_HEIGHT,
+    N0_AIR,
+    STD_GRAVITATIONAL_ACCELERATION,
+    STD_AIR_DENSITY,
 )
+
 from molecularprofiles.utils.humidity import (
     compressibility,
     density_moist_air,
     molar_fraction_water_vapor,
     partial_pressure_water_vapor,
 )
 from molecularprofiles.utils.rayleigh import Rayleigh
@@ -46,16 +47,19 @@
     Methods within this class:
 
     get_data:                   it retrieves the data from the input file. If the input file
                                 is a grib file and there is no file in the working directory
                                 with the same name but with .txt extension the program extracts
                                 the data from the grib file through the grib_utils program. If
                                 there is such a txt file, it reads it directly
-    write_corsika:              pints the data into a txt file which format is compliant with the input card
+    write_corsika:              prints the data into a txt file which format is compliant with the input card
                                 for the CORSIKA air shower simulation software
+    create_mdp:                 creates an altitude profile of the molecular number density
+    rayleigh_extinction:        creates a file, in format to be directly fed to simtel simulation, with the
+                                extinction per altitude bin for wavelengths from 200 to 1000 nm
     """
 
     def __init__(self, data_file, data_server="server", observatory="north"):
         """
         Constructor
 
         :param data_file: txt file containing the data (string)
@@ -67,183 +71,128 @@
         self.data_file = data_file
         self.data_server = data_server
         self.observatory = observatory
 
     # =============================================================================================================
     # Private functions
     # =============================================================================================================
-    def _interpolate_simple(self, x_param, y_param, new_x_param):
+    def _interpolate_cubic(self, x_param, y_param, new_x_param):
         func = interp1d(x_param, y_param, kind="cubic", fill_value="extrapolate")
         return func(new_x_param)
 
     def _interpolate_param_to_h(self, param, height):
-        interpolated_param = []
-        group_mjd = self.dataframe.groupby("MJD")
-
-        logger.info("Computing the extrapolation of the values of density:")
-        logger.info("(This is to make it easier to compare ECMWF and GDAS, or any other")
-        logger.info("weather model)")
-
-        for mjd in self.dataframe.MJD.unique():
-            h_at_mjd = group_mjd.get_group(mjd)["h"].tolist()
-            param_at_mjd = group_mjd.get_group(mjd)[param].tolist()
-            func = interp1d(h_at_mjd, param_at_mjd, kind="cubic", fill_value="extrapolate")
-
-            if isinstance(height, int) or isinstance(height, float):
-                interpolated_param.append(np.float(func(height)))
-            else:
-                interpolated_param.append(func(height))
-        interpolated_param = np.array(interpolated_param)
-        if isinstance(height, float) or isinstance(height, int):
-            interpolated_param = np.array(interpolated_param)
-            return interpolated_param
+        logger.error("Not implemented")
+        raise NotImplementedError
+        # interpolated_param = []
+        # group_mjd = self.dataframe.groupby("MJD")
+
+        # logger.info("Computing the extrapolation of the values of density:")
+        # logger.info("(This is to make it easier to compare ECMWF and GDAS, or any other")
+        # logger.info("weather model)")
+
+        # for mjd in self.dataframe.MJD.unique():
+        #     h_at_mjd = group_mjd.get_group(mjd)["h"].tolist()
+        #     param_at_mjd = group_mjd.get_group(mjd)[param].tolist()
+        #     func = interp1d(h_at_mjd, param_at_mjd, kind="cubic", fill_value="extrapolate")
+
+        #     if isinstance(height, int) or isinstance(height, float):
+        #         interpolated_param.append(np.float(func(height)))
+        #     else:
+        #         interpolated_param.append(func(height))
+        # interpolated_param = np.array(interpolated_param)
+        # if isinstance(height, float) or isinstance(height, int):
+        #     interpolated_param = np.array(interpolated_param)
+        #     return interpolated_param
+        # else:
+        #     interpolated_param_avgs = compute_averages_std(interpolated_param)
+        #     return (
+        #         interpolated_param,
+        #         interpolated_param_avgs[0],
+        #         interpolated_param_avgs[1],
+        #         interpolated_param_avgs[2],
+        #         interpolated_param_avgs[3],
+        #     )
+
+    def _compute_mass_density(self, air="moist", co2_concentration=415):
+        """
+        Computes regular and exponential mass density of air.
+
+        Adds to data the following columns:
+        - 'Xw': molar fraction of water vapor (0 if air is dry)
+        - 'Compressibility'
+        - 'Mass Density'
+        - 'Exponential Mass Density'
+
+        Parameters
+        ----------
+        air : str
+            Type of air, can be 'moist' or 'dry'
+        co2_concentration : float
+            CO2 volume concentration in ppmv
+        """
+
+        if air == "moist":
+            self.data["Xw"] = molar_fraction_water_vapor(
+                self.data["Pressure"], self.data["Temperature"], self.data["Relative humidity"]
+            )
+        elif air == "dry":
+            self.data["Xw"] = 0.0
         else:
-            interpolated_param_avgs = compute_averages_std(interpolated_param)
-            return (
-                interpolated_param,
-                interpolated_param_avgs[0],
-                interpolated_param_avgs[1],
-                interpolated_param_avgs[2],
-                interpolated_param_avgs[3],
-            )
-
-    def _compute_mass_density(self, air="moist", co2_concentration=415, interpolate=False):
-        """
-        Uses the functions density_moist_air, molar_fraction_water_vapor and compressibility
-        from the LIDAR_analysis module humidity.py
-        input:
-            air: (str, optional) must be 'moist' or 'dry'
-
-        :return: density [kg/m^3], std_dev(density) [kg/m^3], peak2peak_minus, peak2peak_plus
-        """
-        # C :  CO2 average global concentration in ppm taken from Keeling curve
-        C = co2_concentration
-        rho_s = 1.225  # kg/m^3 standard air mass density (sea level, 15 degrees C)
-        rho = []
-
-        for i in np.arange(len(self.dataframe.P)):
-            if air == "moist":
-                Xw = molar_fraction_water_vapor(
-                    self.dataframe.P.iloc[i], self.dataframe.Temp.iloc[i], self.dataframe.RH.iloc[i]
-                )
-                Z = compressibility(self.dataframe.P.iloc[i], self.dataframe.Temp.iloc[i], Xw)
-                rho.append(
-                    density_moist_air(
-                        self.dataframe.P.iloc[i] * 100.0, self.dataframe.Temp.iloc[i], Z, Xw, C
-                    )
-                )
+            raise ValueError("Wrong air condition. It must be 'moist' or 'dry'.")
 
-            elif air == "dry":
-                Z = compressibility(self.dataframe.P.iloc[i], self.dataframe.Temp.iloc[i], 0.0)
-                rho.append(
-                    density_moist_air(
-                        self.dataframe.P.iloc[i] * 100.0, self.dataframe.Temp.iloc[i], Z, 0.0, C
-                    )
-                )
-            else:
-                logger.critical('Wrong air condition. It must be "moist" or "dry". Aborting!')
-                sys.exit()
-
-        self.dataframe["n_mass_" + air] = rho
-        self.dataframe["nexp_mass_" + air] = (
-            self.dataframe["n_mass_" + air]
-            / rho_s
-            * np.exp(self.dataframe.h / DENSITY_SCALE_HEIGHT)
+        self.data["Compressibility"] = compressibility(
+            self.data["Pressure"], self.data["Temperature"], self.data["Xw"]
         )
-
-    def _compare_models(self, model_1, model_2):
-        """
-        Compares two atmospheric models and returns statistical difference between them
-        """
-        pass
-        """
-        Reference content of removed similar function:
-        diff_with_magic = []
-        diff_with_prod3 = []
-
-        interpolated_density = self._interpolate_param_to_h("n_exp", self.x)[0]
-
-        self._get_prod3sim_data()
-        x = np.linspace(1000.0, 25000.0, num=15, endpoint=True)
-
-        logger.info("Computing the differences of the values of density:")
-        for i in np.arange(len(interpolated_density))):
-            diff_with_magic.append(
-                (interpolated_density[i] - self.func_magic(x)) / interpolated_density[i]
-            )
-            diff_with_prod3.append(
-                (interpolated_density[i] - self.func_prod3(x)) / interpolated_density[i]
-            )
-
-        self.diff_with_magic = np.asarray(diff_with_magic)
-        self.diff_with_prod3 = np.asarray(diff_with_prod3)
-        logger.info("DIFF PROD3", self.diff_with_prod3)
-        self.diff_MAGIC = compute_averages_std(self.diff_with_magic)
-        self.diff_PROD3 = compute_averages_std(self.diff_with_prod3)
-        """
+        self.data["Mass Density"] = density_moist_air(
+            self.data["Pressure"],
+            self.data["Temperature"],
+            self.data["Compressibility"],
+            self.data["Xw"],
+            co2_concentration,
+        )
+        self.data["Exponential Mass Density"] = (
+            self.data["Mass Density"] / STD_AIR_DENSITY
+        ).decompose() * np.exp((self.data["Altitude"] / DENSITY_SCALE_HEIGHT).decompose())
 
     # =============================================================================================================
     # Main get data function
     # =============================================================================================================
-    def get_data(
-        self,
-        select_good_weather=False,
-        RH_lim=100.0,
-        W_lim=10000.0,
-        filter_by_density=False,
-        n_exp_minvalue=0.0,
-        n_exp_maxvalue=1.0,
-    ):
-
-        """
-        Function that reads ECMWF or GDAS txt input files and returns quantities ready to plot.
-        If the input filename does not exist, the program searches for the same
-        input name with .grib extension and extracts the data from it
-
-               select_good_weather: (bool) if True it uses RH_lim and W_lim parameters to filter the
-                                    data by good weather conditions
-               RH_lim: (float) if select_good_weather is True, this is the RH upper limit value to use
-                       to filter the data
-               W_lim: (float) if select_good_weather is True, this is the Wind speed upper limit value
-                      to use to filter the data
-               filter_by_density: (bool) if set to True it filters the data by density values instead of
-                                  filtering by epoch
-
-        :return:
-            self.dataframe
-            self.h_avgs
-            self.n_avgs
-            self.Temp_avgs
-            self.wind_speed_avgs
-            self.wind_direction_avgs
-            self.RH_avgs
-            self.n_exp_avgs
+    def get_data(self):
+        """
+        Reads ECMWF or GDAS data in ecsv or grib(2) format
+        and computes statistical description of the data
         """
         file_ext = os.path.splitext(self.data_file)[1]
         if file_ext == ".grib" or file_ext == ".grib2":
-            data = get_grib_file_data(self.data_file)
-            data = extend_grib_data(data)
+            self.data = get_grib_file_data(self.data_file)
+            self.data = extend_grib_data(self.data)
         elif file_ext == ".ecsv":
-            data = Table.read(self.data_file, format="ascii.ecsv")
+            self.data = Table.read(self.data_file, format="ascii.ecsv")
         else:
             raise NotImplementedError(
                 f"Only grib (1,2) and ecsv formats are supported at the moment. Requested format: {file_ext}"
             )
-
-        self.dataframe = data.to_pandas()
-
-        # Various averaged values obtained after filtering (if no filter, averages are made over the whole dataframe)
-        self.group_by_p = self.dataframe.groupby("Pressure")
-        self.h_avgs = avg_std_dataframe(self.group_by_p, "Altitude")
-        self.n_avgs = avg_std_dataframe(self.group_by_p, "Density")
-        self.Temp_avgs = avg_std_dataframe(self.group_by_p, "Temperature")
-        self.wind_speed_avgs = avg_std_dataframe(self.group_by_p, "Wind Speed")
-        self.wind_direction_avgs = avg_std_dataframe(self.group_by_p, "Wind Direction")
-        self.RH_avgs = avg_std_dataframe(self.group_by_p, "Relative humidity")
-        self.n_exp_avgs = avg_std_dataframe(self.group_by_p, "Exponential Density")
+        self.stat_columns = [
+            "Pressure",
+            "Altitude",
+            "Density",
+            "Temperature",
+            "Wind Speed",
+            "Wind Direction",
+            "Relative humidity",
+            "Exponential Density",
+        ]
+        self.stat_data = self.data[self.stat_columns].group_by("Pressure")
+        self.stat_description = {
+            "avg": self.stat_data.groups.aggregate(np.mean),
+            "std": self.stat_data.groups.aggregate(np.std),
+            "mad": self.stat_data.groups.aggregate(lambda x: np.mean(np.absolute(x - np.mean(x)))),
+            "p2p_max": self.stat_data.groups.aggregate(lambda x: np.max(x) - np.mean(x)),
+            "p2p_min": self.stat_data.groups.aggregate(lambda x: np.mean(x) - np.min(x)),
+        }
 
     def _refractive_index(self, P, T, RH, wavelength, C):
         """Wrapper for Rayleigh.calculate_n()."""
         rayleigh = Rayleigh(wavelength, C, P, T, RH)
         return rayleigh.refractive_index
 
     # =======================================================================================================
@@ -252,143 +201,79 @@
 
     def write_corsika(self, outfile, co2_concentration):
         """
         Write an output file in the style of a CORSIKA atmospheric configuration file:
 
         alt (km)     rho (g/cm^3)   thick (g/cm^2)   (n-1)
         """
-        mbar2gcm2 = 1.019716213  # conversion from mbar (pressure in SI) to g/cm^2 (pressure in cgs)
-        # Loschmidt constant: number density of particles in an ideal gas at STP in m^-3
-        N0 = 2.079153e25  # Na divided by molar mass of air: 0.0289644
-        height = np.array(
-            [
-                1.0,
-                2.0,
-                3.0,
-                4.0,
-                5.0,
-                6.0,
-                7.0,
-                8.0,
-                9.0,
-                10.0,
-                11.0,
-                12.0,
-                13.0,
-                14.0,
-                15.0,
-                16.0,
-                17.0,
-                18.0,
-                19.0,
-                20.0,
-                21.0,
-                22.0,
-                23.0,
-                24.0,
-                25.0,
-                26.0,
-            ]
+        height = np.arange(0.0, 27000.0, 1000) * u.m
+        temperature = (
+            self._interpolate_cubic(
+                self.stat_description["avg"]["Altitude"],
+                self.stat_description["avg"]["Temperature"],
+                height,
+            )
+            * self.stat_description["avg"]["Temperature"].unit
+        )
+        relative_humidity = (
+            self._interpolate_cubic(
+                self.stat_description["avg"]["Altitude"],
+                self.stat_description["avg"]["Relative humidity"],
+                height,
+            )
+            * self.stat_description["avg"]["Relative humidity"].unit
+        )
+        pressure = (
+            self._interpolate_cubic(
+                self.stat_description["avg"]["Altitude"],
+                self.stat_description["avg"]["Pressure"],
+                height,
+            )
+            * self.stat_description["avg"]["Pressure"].unit
+        )
+        thickness = pressure / STD_GRAVITATIONAL_ACCELERATION
+        density = (
+            self._interpolate_cubic(
+                self.stat_description["avg"]["Altitude"],
+                self.stat_description["avg"]["Density"],
+                height,
+            )
+            * self.stat_description["avg"]["Density"].unit
+            / N0_AIR
+        )
+        rel_water_vapor_pressure = (
+            partial_pressure_water_vapor(temperature, relative_humidity) / pressure
+        ).decompose()
+        rel_refractive_index = (
+            self._refractive_index(
+                pressure, temperature, relative_humidity, 350.0 * u.nm, co2_concentration
+            )
+            - 1.0
         )
 
         with open(outfile, "w") as f:
 
             f.write("# Atmospheric Model ECMWF year/month/day   hour h\n")  # .format(**datedict))
             f.write(
                 "#Col. #1          #2           #3            #4        [ #5 ]        [ #6 ]       [ # 7 ]\n"
             )
             f.write(
                 "# Alt [km]    rho [g/cm^3] thick [g/cm^2]    n-1        T [k]       p [mbar]      pw / p\n"
             )
 
-            density = self.n_avgs[0].sort_index(ascending=False).values
-            density /= N0 * 1.0e-3
-            P = self.dataframe.Pressure.unique()[::-1]
-
-            # height = self.h_avgs[0].sort_index(ascending=False).values / 1.e3
-            # Temp = self.Temp_avgs[0].sort_index(ascending=False).values
-            # RH = self.RH_avgs[0].sort_index(ascending=False).values
-
-            T0 = float(
-                self._interpolate_simple(
-                    self.h_avgs[0].sort_index(ascending=False).values / 1e3,
-                    self.Temp_avgs[0].sort_index(ascending=False).values,
-                    0.0,
-                )
-            )
-            RH0 = float(
-                self._interpolate_simple(
-                    self.h_avgs[0].sort_index(ascending=False).values / 1e3,
-                    self.RH_avgs[0].sort_index(ascending=False).values,
-                    0.0,
-                )
-            )
-            P0 = float(
-                self._interpolate_simple(
-                    self.h_avgs[0].sort_index(ascending=False).values / 1e3, P, 0.0
-                )
-            )
-            density0 = float(
-                self._interpolate_simple(
-                    self.h_avgs[0].sort_index(ascending=False).values / 1e3, density, 0.0
-                )
-            )
-            thick0 = P0 * mbar2gcm2
-
-            pw0 = partial_pressure_water_vapor(T0, RH0) / P0
-
-            Temp = self._interpolate_simple(
-                self.h_avgs[0].sort_index(ascending=False).values / 1.0e3,
-                self.Temp_avgs[0].sort_index(ascending=False).values,
-                height,
-            )
-            RH = self._interpolate_simple(
-                self.h_avgs[0].sort_index(ascending=False).values / 1.0e3,
-                self.RH_avgs[0].sort_index(ascending=False).values,
-                height,
-            )
-            RH[RH < 0.0] = 1.0e-4
-            Pressure = self._interpolate_simple(
-                self.h_avgs[0].sort_index(ascending=False).values / 1.0e3, P, height
-            )
-            density = self._interpolate_simple(
-                self.h_avgs[0].sort_index(ascending=False).values / 1.0e3, density, height
-            )
-            thick = Pressure * mbar2gcm2
-            pwp = partial_pressure_water_vapor(Temp, RH) / Pressure
-
-            nm0 = self._refractive_index(P0, T0, RH0, 350.0, co2_concentration) - 1.0
-            outdict = {
-                "height": 0.000,
-                "rho": density0,
-                "thick": thick0,
-                "nm1": nm0,
-                "T": T0,
-                "p": P0,
-                "pw/p": pw0,
-            }
-            f.write(
-                "  {height:7.3f}     {rho:5.5E}  {thick:5.5E}  {nm1:5.5E}  {T:5.5E}  {p:5.5E}  {pw/p:5.5E}\n".format(
-                    **outdict
-                )
-            )
-
             for i in np.arange(len(height)):
-                nm1 = (
-                    self._refractive_index(Pressure[i], Temp[i], RH[i], 350, co2_concentration) - 1
-                )
 
                 outdict = {
-                    "height": height[i],
-                    "rho": density[i],
-                    "thick": thick[i],
-                    "nm1": nm1,
-                    "T": Temp[i],
-                    "p": Pressure[i],
-                    "pw/p": pwp[i],
+                    "height": height[i].to_value(u.km),
+                    "rho": density[i].to_value(u.g / u.cm**3),
+                    "thick": thickness[i].to_value(u.g / u.cm**2),
+                    "nm1": rel_refractive_index[i],
+                    "T": temperature[i].to_value(u.K),
+                    "p": pressure[i].to_value(u.mbar),
+                    "pw/p": rel_water_vapor_pressure[i],
                 }
                 f.write(
                     "  {height:7.3f}     {rho:5.5E}  {thick:5.5E}  {nm1:5.5E}  {T:5.5E}  {p:5.5E}  {pw/p:5.5E}\n".format(
                         **outdict
                     )
                 )
 
@@ -492,21 +377,120 @@
             )
 
     def create_mdp(self, mdp_file):
         """
         Write an output file with the molecular number density per height
         """
 
-        height = np.arange(
-            1.0, 27.0, 1
+        heights = (
+            np.arange(0.0, 27000.0, 1000) * u.m
         )  # FIXME: The hardcoded value 27 reflects the current ceiling of GDAS data (26km a.s.l.). Shouldn't be hardcoded and in general the binning and limits should be considered.
         with open(mdp_file, "w") as f:
 
-            number_density_exp = self._interpolate_simple(
-                self.h_avgs[0].sort_index(ascending=False).values / 1.0e3,
-                self.n_exp_avgs[0].sort_index(ascending=False).values,
-                height,
+            number_density = (
+                self._interpolate_cubic(
+                    self.stat_description["avg"]["Altitude"],
+                    self.stat_description["avg"]["Density"],
+                    heights,
+                )
+                * self.stat_description["avg"]["Density"].unit
             )
+            for i, height in enumerate(heights):
+                file_line = [str(height), "\t", str(number_density[i]), "\n"]
+                f.writelines(file_line)
 
-            for i in np.arange(len(height)):
-                file_line = [str(height[i]), "\t", str(number_density_exp[i]), "\n"]
+    def rayleigh_extinction(self, rayleigh_extinction_file, co2_concentration):
+        """
+        Calculates the integral optical depth due to Rayleigh scattering
+        per altitude bins as a function of wavelength.
+        The optical depth (AOD) for an altitude h over the observatory will be given by
+        the integral of the monochromatic volume coefficient beta, with integration limits
+        h_obs up to h.
+
+        returns:
+        --------
+            File with integral optical depth per height bin per wavelength bin. The format is the same with MODTRAN files.
+        """
+
+        # For now we work for La Palma site. We will most probably have to find an average
+        # altitude for each site. h_obs should become an attribute of observatory class.
+        height_obs = 2158
+        height = (
+            np.array(
+                [
+                    height_obs,
+                    2258,
+                    2358,
+                    2458,
+                    2658,
+                    2858,
+                    3158,
+                    3658,
+                    4158,
+                    4500,
+                    5000,
+                    5500,
+                    6000,
+                    7000,
+                    8000,
+                    9000,
+                    10000,
+                    11000,
+                    12000,
+                    13000,
+                    14000,
+                    15000,
+                    16000,
+                    18000,
+                    20000,
+                    22000,
+                    24000,
+                    26000,
+                ]
+            )
+            * u.m
+        )
+        # and here's the big question, still unanswered. What do we do with the altitudes that DAS values do not exist?
+        # , 28.000, 30.000, 32.500, 35.000, 37.500, 40.000, 45.000, 50.000, 60.000, 70.000, 80.000, 100.000 ]
+        bin_widths = np.diff(height)
+        bin_centers = (height[:-1] + height[1:]) / 2
+
+        temperature = (
+            self._interpolate_cubic(
+                self.stat_description["avg"]["Altitude"],
+                self.stat_description["avg"]["Temperature"],
+                bin_centers,
+            )
+            * self.stat_description["avg"]["Temperature"].unit
+        )
+        relative_humidity = (
+            self._interpolate_cubic(
+                self.stat_description["avg"]["Altitude"],
+                self.stat_description["avg"]["Relative humidity"],
+                bin_centers,
+            )
+            * self.stat_description["avg"]["Relative humidity"].unit
+        )
+        pressure = (
+            self._interpolate_cubic(
+                self.stat_description["avg"]["Altitude"],
+                self.stat_description["avg"]["Pressure"],
+                bin_centers,
+            )
+            * self.stat_description["avg"]["Pressure"].unit
+        )
+        wavelength_range = np.arange(200, 1001, 1) * u.nm
+
+        # Here is a schoolkid's, homemade numerical integration. Though it gives reasonable results.
+        with open(rayleigh_extinction_file, "w") as f:
+            for wavelength in wavelength_range:
+                aod = 0
+                file_line = [str(wavelength.to(u.nm)).split(" ")[0], "\t"]
+                for P, T, RH, dh in zip(pressure, temperature, relative_humidity, bin_widths):
+                    rayleigh = Rayleigh(wavelength, co2_concentration, P, T, RH)
+                    beta = rayleigh.beta
+                    aod += dh * beta
+                    file_line += [f"{aod:.6f}", "\t"]
+                file_line += ["\n"]
                 f.writelines(file_line)
+
+        return rayleigh_extinction_file
```

### Comparing `molecularprofiles-0.2.0/src/molecularprofiles/utils/constants.py` & `molecularprofiles-0.3.0/src/molecularprofiles/utils/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import astropy.units as u
+from astropy.constants import N_A
 
 # standard atmosphere thermodynamic values
 STD_NUMBER_DENSITY = (
     2.546899e19 / u.cm**3
 )  # [cm^-3] molecular number density for standard air conditions
 STD_AIR_PRESSURE = 1013.25 * u.hPa  # [hPa]   standard air pressure
 STD_AIR_TEMPERATURE = 288.15 * u.K  # [K]     standard air temperature
+STD_AIR_DENSITY = 1.225 * u.kg / u.m**3  # [kg/m^3] standard air density
 DENSITY_SCALE_HEIGHT = 9500.0 * u.km  # [km]    density scale hight for La Palma Winter
 STD_RELATIVE_HUMIDITY = 45.9 * u.percent  # [%]     standard air rel. humidity
 # atmospheric composition
 NITROGEN_RATIO = 0.78084 * u.dimensionless_unscaled
 OXYGEN_RATIO = 0.20946 * u.dimensionless_unscaled
 ARGON_RATIO = 0.00934 * u.dimensionless_unscaled
 GAS_CONSTANT = 8.31451 * u.J / (u.K * u.mol)  # gas constant [J/mol/K]
 MOLAR_MASS_WATER_VAPOR = 0.018015 * u.kg / u.mol  # molar mass of water vapor [kg/mol]
+MOLAR_MASS_AIR = 0.0289644 * u.kg / u.mol  # molar mass of air [kg/mol]
 # misc physics constants
 STD_GRAVITATIONAL_ACCELERATION = (
     9.80665 * u.m / u.s**2
 )  # standard acceleration of free fall [m/s^2]
 STD_EARTH_RADIUS = 6245 * u.km  # Earth radius for geopotential height conversion [km]
+N0_AIR = N_A / MOLAR_MASS_AIR
```

### Comparing `molecularprofiles-0.2.0/src/molecularprofiles/utils/grib_utils.py` & `molecularprofiles-0.3.0/src/molecularprofiles/utils/grib_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,27 +31,30 @@
     """
     Function to compute the real altitude from the geopotential value at
     a certain coordinate on Earth.
     Uses expression 20 from http://dx.doi.org/10.1029/2002JB002333
 
     Parameters
     ----------
-    geopotential : Quantity [u.m]
+    geopotential : astropy.units.Quantity [u.m]
         Geopotential height
-    latitude : Latitude
+    latitude : astropy.coordinates.Latitude
         Geographical latitude of interest.
 
     Returns
     -------
-    Quantity [u.m]
+    astropy.units.Quantity [u.m]
         Real altitude as fGeoidOffset.
     """
-    return (1.0 + 0.002644 * np.cos(2 * latitude)) * geopotential_height + (
-        1 + 0.0089 * np.cos(2 * latitude)
-    ) * geopotential_height**2 / STD_EARTH_RADIUS
+
+    lat = (np.asarray(latitude) * latitude.unit).to_value(u.rad)
+    return (
+        (1.0 + 0.002644 * np.cos(2 * lat)) * (geopotential_height)
+        + (1 + 0.0089 * np.cos(2 * lat)) * ((geopotential_height) ** 2 / STD_EARTH_RADIUS.to(u.m))
+    ).to(u.m)
 
 
 def get_gribfile_variables(filename):
     """
     Returns all the different variable names in a grib file.
 
     Parameters
@@ -168,15 +171,15 @@
     logger.debug("Getting all variable names...")
     variable_names, variable_short_names = get_gribfile_variables(filename)
     logger.info("Indexing the file %s (this might take a while...)", filename)
     grib_file = pg.index(filename, "shortName", "typeOfLevel")
     logger.debug(
         "Selecting the parameters information for %s (this might take a while...)", filename
     )
-    gpm = u.def_unit("gpm", u.m**2 / (STD_GRAVITATIONAL_ACCELERATION * u.s**2))
+    gpm = u.def_unit("gpm", u.m)
     u.add_enabled_units([gpm])
     data = Table()
     for short_name in variable_short_names:
         if short_name == "unknown":
             continue
         var = grib_file.select(shortName=short_name, typeOfLevel="isobaricInhPa")
         try:
@@ -213,15 +216,15 @@
     logger.debug("Compute altitude from geopotential")
     if "Geopotential Height" in data.keys():
         data["Altitude"] = get_altitude_from_geopotential_height(
             data["Geopotential Height"], data["Latitude"]
         )
     else:
         data["Altitude"] = get_altitude_from_geopotential_height(
-            data["Geopotential Height"] / STD_GRAVITATIONAL_ACCELERATION, data["Latitude"]
+            data["Geopotential"] / STD_GRAVITATIONAL_ACCELERATION, data["Latitude"]
         )
     logger.debug("Compute density")
     data["Density"] = (
         STD_NUMBER_DENSITY
         * data["Pressure"]
         / STD_AIR_PRESSURE
         * STD_AIR_TEMPERATURE
@@ -233,15 +236,17 @@
     )
     logger.debug("Compute wind speed")
     data["Wind Speed"] = np.sqrt(
         data["U component of wind"] ** 2 + data["V component of wind"] ** 2
     )
     logger.debug("Compute wind direction")
     data["Wind Direction"] = Angle(
-        np.array(np.arctan2(-data["V component of wind"].value, -data["U component of wind"].value)),
+        np.array(
+            np.arctan2(-data["V component of wind"].value, -data["U component of wind"].value)
+        ),
         unit=u.rad,
     ).wrap_at(360 * u.deg)
     return data
 
 
 def save_grib_table(data, filename, fmt="ecsv"):
     """
```

### Comparing `molecularprofiles-0.2.0/src/molecularprofiles/utils/observatory.py` & `molecularprofiles-0.3.0/src/molecularprofiles/utils/observatory.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 Module containing functionality allows to get observatory's coordinates
 and select meteorological data depending on the season for the South and North hemisphere
 
 """
 
 import math
 import logging
+from logging.config import fileConfig
 import os
 from datetime import date, timedelta
 from calendar import monthrange, month_abbr
 import numpy as np
 
 import astropy.units as u
 from astropy.coordinates import angular_separation, Longitude, Latitude
 
 
 ROOTDIR = os.path.dirname(os.path.abspath(__file__))
 log_config_file = f"{ROOTDIR}/mdps_log.conf"
-logging.config.fileConfig(fname=log_config_file, disable_existing_loggers=False)
+fileConfig(fname=log_config_file, disable_existing_loggers=False)
 logger = logging.getLogger(__name__)
 
 
 class Season:
     """
     Class, describing nature seasons.
     """
@@ -172,15 +173,15 @@
         Check if provided seasons provide no-gaps and no-overlaps full coverage of a year.
 
         Raises
         ------
         ValueError
             If the seasons overlap, if there's a gap between the seasons or they don't cover a year.
         """
-        dates = sorted([season.reference_dates for season in self.seasons], key=lambda x: x[0])
+        dates = sorted([season.reference_dates for season in self._seasons], key=lambda x: x[0])
         # check that there's one year between the first start and last end
         if dates[0][0] + timedelta(days=365) != dates[-1][1]:
             raise ValueError("The seasons don't cover a year")
         diffs = [j[0] - i[1] for i, j in zip(dates[:-1], dates[1:])]
         if not all(x == timedelta(days=1) for x in diffs):
             raise ValueError("The season coverage has gaps or overlaps!")
 
@@ -207,18 +208,18 @@
         return self._longitude, self._latitude
 
     @property
     def seasons(self):
         """
         Returns
         -------
-        list(str)
-            List of season names
+        dict
+            Dictionary of seasons in form {season name : season object}
         """
-        return [season.name for season in self._seasons]
+        return {season.name: season for season in self._seasons}
 
     def get_near_gridpoints(self, gridstep=1):
         """
         Get closest meteorological data point and a grid box, surrounding the observatory.
 
         The interpolation grids of the meteorological systems is assumed to start at (0,0) and be defined w.r.t. WGS84.
 
@@ -264,32 +265,37 @@
 
     def select_season_data(self, data, season_name):
         """
         Select data that belongs to a given season.
 
         Parameters
         ----------
-        data : pandas.DataFrame with atmospheric data. Must contain column
+        data : astropy.table.Table
+            Astropy table with meteorological data. Must contain 'Timestamp' column with astropy.time.Time
+        season_name : str
+            Season name
+
+        Returns
+        -------
+        astropy.table.Table
+            Selected data table according to provided season
         """
-        if season_name.upper() not in self.seasons:
+        if season_name.upper() not in self.seasons.keys():
             logger.error(
                 "Requested season (%s) is not defined for the observatory %s\n" "%s's seasons:\n%s",
                 season_name,
                 self.name,
                 self.name,
-                self.seasons,
+                self.seasons.keys(),
             )
             raise RuntimeError(f"{season_name} is not present in {self.name}'s seasons.")
-        return data.loc[
-            data.apply(
-                lambda x: date(year=int(x.year), month=int(x.month), day=int(x.day))
-                in self.seasons[season_name.upper()],
-                axis=1,
-            )
+        mask = [
+            ts.date() in self.seasons[season_name.upper()] for ts in data["Timestamp"].tt.datetime
         ]
+        return data[mask]
 
 
 # Define commonly used seasons and observatories
 
 cta_north_winter = Season(name="cta-north-winter", start_month=11, stop_month=4, start_day=16)
 cta_north_spring = Season(
     name="cta-north-spring", start_month=5, stop_month=6, start_day=1, stop_day=20
```

### Comparing `molecularprofiles-0.2.0/src/molecularprofiles/utils/rayleigh.py` & `molecularprofiles-0.3.0/src/molecularprofiles/utils/rayleigh.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import functools
-from math import pi, cos
+import numpy as np
+import astropy.units as u
 from molecularprofiles.utils import humidity
 from molecularprofiles.utils.constants import (
     STD_NUMBER_DENSITY,
     STD_AIR_PRESSURE,
     STD_AIR_TEMPERATURE,
     STD_RELATIVE_HUMIDITY,
     NITROGEN_RATIO,
@@ -45,225 +46,280 @@
     .. moduleauthor:: Scott Griffiths <sgriffiths@ifae.es>
     """
 
     def __init__(
         self,
         wavelength,
         co2_bkg,
-        pressure=STD_AIR_PRESSURE.to_value(),
-        temperature=STD_AIR_TEMPERATURE.to_value(),
-        relative_humidity=STD_RELATIVE_HUMIDITY.to_value(),
+        pressure=STD_AIR_PRESSURE,
+        temperature=STD_AIR_TEMPERATURE,
+        relative_humidity=STD_RELATIVE_HUMIDITY,
     ):
         """
         Constructor for Rayleigh-scattering class.
 
         Parameters
         ----------
-        wavelength : int
-            Wavelength of light [nm].
-        pressure : float
-            Pressure [hPa]
-        temperature : float
-            Temperature [K]
-        relative_humidity : float
-            Relative humidity [%]
+        wavelength : astropy.units.Quantity
+            Wavelength of light.
         co2_bkg : float
             CO2 concentration [ppmv]
+        pressure : astropy.units.Quantity
+            Atmospheric pressure
+        temperature : astropy.units.Quantity
+            Air temperature
+        relative_humidity : astropy.units.Quantity
+            Relative humidity [%]
         """
         # check inputs for bad values
-        if wavelength < 200 or wavelength > 4000:
+        if np.any(wavelength < 200 * u.nm) or np.any(wavelength > 4000 * u.nm):
             raise ValueError("Wavelength range only from 200 nm - 4 micrometer allowed.")
-        if pressure < 0 or pressure > 1400:
+        if np.any(pressure < 0 * u.hPa) or np.any(pressure > 1400 * u.hPa):
             raise ValueError("Pressure only in range 0 - 1400 hPa allowed.")
-        if temperature < 180 or temperature > 373.15:
-            raise ValueError("Temperatures only in range 200 - 373 K allowed.")
-        if relative_humidity < 0 or relative_humidity > 100:
-            raise ValueError("Relative humity must lie between 0 - 100.")
+        if np.any(temperature < 180 * u.K) or np.any(temperature > 373.15 * u.K):
+            raise ValueError("Temperatures only in range 180 - 373 K allowed.")
+        # if np.any(relative_humidity < 0) or np.any(relative_humidity > 100 * u.percent):
+        #    raise ValueError("Relative humity must lie between 0 - 100.")
+        # FIXME: Relative humidity can exceed 100%, in case of supersaturated air.
+        # The maximum limit should be thought better. However relative humidity cannot go negative.
+        # If we receive negative values it is most probably due to interpolation problems.
+        # Till we fix these issues it is better to comment out the minimum limit.
         if co2_bkg < 200 or co2_bkg > 1000:
             raise ValueError("CO2 concentrations only in range 200 - 1000 ppmv allowed.")
 
-        self.wavelength = wavelength  # [nm]    wavelenght of light
-        self.pressure = pressure  # [hPa]   air pressure
-        self.temperature = temperature  # [K]     air temperature
-        self.relative_humidity = relative_humidity  # [%]     relative humidity of air
+        self.wavelength = wavelength.to(u.nm)
+        self.pressure = pressure.to(u.hPa)
+        self.temperature = temperature.to(u.K, equivalencies=u.temperature())
+        self.relative_humidity = relative_humidity.to(u.percent)
         self.co2_bkg = co2_bkg  # [ppmv]  CO2 concentration of air
 
     @functools.cached_property
     def molecular_number_density(self):
         """
         Returns
         -------
-        float
-            Molecular number density [cm^-3] (Tomasi eq. 3)
+        astropy.units.Quantity
+            Molecular number density [cm^-3]
+
+        Notes
+        -----
+        See Eq. 3 in [1]_.
+
+        References
+        ----------
+        .. [1] C. Tomasi, V. Vitale, B. Petkov, A. Lupi, A. Cacciari
+           "Improved algorithm for calculations of Rayleigh-scattering optical depth
+           in standard atmospheres", Applied Optics 44 Nr. 16 (2005) 3320
         """
         return (
-            STD_NUMBER_DENSITY
-            * self.pressure
-            / STD_AIR_PRESSURE
-            * STD_AIR_TEMPERATURE
-            / self.temperature
+            (
+                STD_NUMBER_DENSITY
+                * self.pressure
+                / STD_AIR_PRESSURE
+                * STD_AIR_TEMPERATURE
+                / self.temperature
+            )
+            .decompose()
+            .to(1 / u.cm**3)
         )
 
     @functools.cached_property
     def scattering_cross_section(self):
         """
         Returns
         -------
-        float
-            Total Rayleigh scattering cross section per molecule [cm^-2].
+        astropy.units.Quantity
+            Total Rayleigh scattering cross section per molecule [cm^2].
+
+        Notes
+        -----
+        See Eq. 4 in [1]_.
+
+        References
+        ----------
+        .. [1] C. Tomasi, V. Vitale, B. Petkov, A. Lupi, A. Cacciari
+           "Improved algorithm for calculations of Rayleigh-scattering optical depth
+           in standard atmospheres", Applied Optics 44 Nr. 16 (2005) 3320
         """
         return (
-            24
-            * pow(pi, 3)
-            * (self.refractive_index**2 - 1) ** 2
-            / (
-                pow(self.wavelength * 1e-7, 4)
-                * self.molecular_number_density**2
-                * (self.refractive_index**2 + 2) ** 2
+            (
+                24
+                * np.pi**3
+                * (self.refractive_index**2 - 1) ** 2
+                / (
+                    self.wavelength**4
+                    * self.molecular_number_density**2
+                    * (self.refractive_index**2 + 2) ** 2
+                )
+                * self.king_factor
             )
-            * self.king_factor
+            .decompose()
+            .to(u.cm**2)
         )
 
     @functools.cached_property
     def beta(self):
         """
         Calculates the monochromatic volume coefficient for the total molecular
-        scattering in cloudless air, beta, in units of km^-1, following Tomasi, eq.2
+        scattering in cloudless air, beta.
 
         Returns
         -------
-        float
-            Monochromatic volume coefficient for the total molecular scattering in cloudless air [1/km]
+        astropy.units.Quantity
+            Monochromatic volume coefficient for the total molecular scattering
+            in cloudless air [1/km]
+
+        Notes
+        -----
+        See Eq. 2 in [1]_.
+
+        References
+        ----------
+        .. [1] C. Tomasi, V. Vitale, B. Petkov, A. Lupi, A. Cacciari
+           "Improved algorithm for calculations of Rayleigh-scattering optical depth
+           in standard atmospheres", Applied Optics 44 Nr. 16 (2005) 3320
         """
-        return 1e5 * self.molecular_number_density * self.scattering_cross_section
+        return (
+            (self.molecular_number_density * self.scattering_cross_section).decompose().to(1 / u.km)
+        )
 
     @functools.cached_property
     def refractive_index(self):
+
         """
         Ciddor formula for calculation of refractive index in moist air.
         The obtained refractive index is precise to 1e-7.
 
-        Cross-checked with:
-        http://emtoolbox.nist.gov/Wavelength/Documentation.asp#IndexofRefractionofAir
-
         Returns
         -------
         float
             Index of refraction of moist air
-        """
-        wavelength_mum = pow(self.wavelength / 1000, -2)  # convert wavelength to micrometers
 
-        # refractive index of standard dry air (e = 0) according to Ciddor, with 450 ppmv CO2
+        Notes
+        -----
+        Cross-checked with:
+        http://emtoolbox.nist.gov/Wavelength/Documentation.asp#IndexofRefractionofAir
+        """
         refractive_index_dry = (
-            1e-8 * (5792105 / (238.0185 - wavelength_mum) + 167917 / (57.362 - wavelength_mum)) + 1
+            1e-8
+            * (
+                5792105 / (238.0185 - 1 / self.wavelength.to_value(u.micron) ** 2)
+                + 167917 / (57.362 - 1 / self.wavelength.to_value(u.micron) ** 2)
+            )
+            + 1
         )  # Tomasi eq. 17
 
         # refractive index of dry air at standard p and T, for given C (e = 0)
         refractive_index_dry_std_air = (1 + 0.534e-6 * (self.co2_bkg - 450)) * (
             refractive_index_dry - 1
         ) + 1  # Tomasi eq. 18
 
         # refractive index of pure water vapor at standard T and e
         # (T* = 293.15 K = 20 C, and e* = 1333 Pa)
         refractive_index_water_vapour = (
             1.022e-8
             * (
                 295.235
-                + 2.6422 * wavelength_mum
-                - 0.032380 * wavelength_mum * wavelength_mum
-                + 0.004028 * wavelength_mum * wavelength_mum * wavelength_mum
+                + 2.6422 / self.wavelength.to_value(u.micron) ** 2
+                - 0.032380 / self.wavelength.to_value(u.micron) ** 4
+                + 0.004028 / self.wavelength.to_value(u.micron) ** 6
             )
             + 1
         )  # Tomasi eq. 19
 
         # calculate the respective densities (see Tomasi et al., pp. 3325 ff)
-        molar_mass_dry_air = 1e-3 * (
-            28.9635 + 12.011e-6 * (self.co2_bkg - 400)
-        )  # molar mass of dry air [kg/mol]
-        molar_mass_water_vapour = 0.018015  # molar mass of water vapor [kg/mol]
+        molar_mass_dry_air = (
+            1e-3 * (28.9635 + 12.011e-6 * (self.co2_bkg - 400)) * u.kg / u.mol
+        )  # Tomasi eq. 13
+        molar_mass_water_vapour = 0.018015 * u.kg / u.mol
         molar_fraction_water_vapour = humidity.molar_fraction_water_vapor(
             self.pressure, self.temperature, self.relative_humidity
         )  # molar fraction of water vapor in moist air
         compressibility_dry_air = humidity.compressibility(
-            STD_AIR_PRESSURE.to_value(), STD_AIR_TEMPERATURE.to_value(), 0
+            STD_AIR_PRESSURE, STD_AIR_TEMPERATURE, 0
         )  # compressibility of dry air
         compressibility_water_vapour = humidity.compressibility(
-            13.33, 293.15, 1
+            1333 * u.Pa, 293.15 * u.K, 1
         )  # compressibility of pure water vapor
         compressibility_moist_air = humidity.compressibility(
             self.pressure, self.temperature, molar_fraction_water_vapour
         )  # compressibility of moist air
 
         # density of dry air at standard p and T
         dry_air_density_stdpt = humidity.density_moist_air(
-            STD_AIR_PRESSURE.to_value(), STD_AIR_TEMPERATURE.to_value(), compressibility_dry_air, 0, self.co2_bkg
+            STD_AIR_PRESSURE, STD_AIR_TEMPERATURE, compressibility_dry_air, 0, self.co2_bkg
         )
 
         # density of pure water vapor at at standard T and e (T* = 293.15 K = 20 C, and e* = 1333 Pa)
         water_vapour_density_stdpt = humidity.density_moist_air(
-            13.33, 293.15, compressibility_water_vapour, 1, self.co2_bkg
+            1333 * u.Pa, 293.15 * u.K, compressibility_water_vapour, 1, self.co2_bkg
         )
 
         # density of the dry component of moist air
         density_dry_comp_moist_air = (
-            (100 * self.pressure)
+            self.pressure
             * molar_mass_dry_air
             * (1 - molar_fraction_water_vapour)
-            / (compressibility_moist_air * GAS_CONSTANT.to_value() * self.temperature)
-        )
+            / (compressibility_moist_air * GAS_CONSTANT * self.temperature)
+        ).decompose()
 
         # density of the water vapor component of moist air
         density_water_vapour_moist_air = (
-            (100 * self.pressure)
+            self.pressure
             * molar_mass_water_vapour
             * molar_fraction_water_vapour
-            / (compressibility_moist_air * GAS_CONSTANT.to_value() * self.temperature)
-        )
+            / (compressibility_moist_air * GAS_CONSTANT * self.temperature)
+        ).decompose()
 
         return (
             1
             + (density_dry_comp_moist_air / dry_air_density_stdpt)
             * (refractive_index_dry_std_air - 1)
             + (density_water_vapour_moist_air / water_vapour_density_stdpt)
             * (refractive_index_water_vapour - 1)
         )  # Ciddor eq. 5, Tomasi eq. 11
 
     @functools.cached_property
     def king_factor(self):
         """
         Calculates the current best estimate of the King factor of moist air.
 
+        Returns
+        -------
+        float
+            King factor [dimensionless]
+
+        Notes
+        -----
         The King factor is used to take into account effects due to the anisotropic
         properties of air molecules since anisotropic molecules scatter more radiation
         at 90 degrees scattering angles than isotropic molecules with the same index
         of refraction.
 
         Precision not stated in Tomasi et al., but probably better than 1e-4.
         Effects of relative_humidity are of the order of several times 1e-4.
-
-        Returns
-        -------
-        float
-            King factor [dimensionless]
         """
-        wavelength_mum = pow(self.wavelength / 1000, -2)  # convert to micrometers
-        water_vapour_partial_press = humidity.partial_pressure_water_vapor(
+        water_vapour_partial_pressure = humidity.partial_pressure_water_vapor(
             self.temperature, self.relative_humidity
         )  # water vapor partial pressure [hPa]
 
-        king_factor_n2 = 1.034 + 3.17e-4 * wavelength_mum  # partial King factor for N2 molecules
+        king_factor_n2 = (
+            1.034 + 3.17e-4 / self.wavelength.to_value(u.micron) ** 2
+        )  # partial King factor for N2 molecules
         king_factor_o2 = (
-            1.096 + 1.385e-3 * wavelength_mum + 1.448e-4 * wavelength_mum * wavelength_mum
+            1.096
+            + 1.385e-3 / self.wavelength.to_value(u.micron) ** 2
+            + 1.448e-4 / self.wavelength.to_value(u.micron) ** 4
         )  # partial King factor for O2 molecules
         king_factor_ar = 1.00  # partial King factor for Ar molecules
         king_factor_co2 = 1.15  # partial King factor for CO2 molecules
         king_factor_wv = 1.001  # partial King factor for water vapor
 
         co2_ratio = 1e-6 * self.co2_bkg  # CO2
-        water_vapour_ratio = water_vapour_partial_press / self.pressure  # water vapor mixing ratio
+        water_vapour_ratio = (water_vapour_partial_pressure / self.pressure).decompose().to_value()
 
         return (
             NITROGEN_RATIO * king_factor_n2
             + OXYGEN_RATIO * king_factor_o2
             + ARGON_RATIO * king_factor_ar
             + co2_ratio * king_factor_co2
             + water_vapour_ratio * king_factor_wv
@@ -286,54 +342,58 @@
         """
         return (
             6 * (self.king_factor - 1) / (3 + 7 * self.king_factor)
         )  # Tomasi eq. 5, solved for rho
 
     def phase_function(self, angle):
         """
-        Calculates the Chandrasekhar phase function.
+        Calculates the Chandrasekhar phase function according to Eq. 255 of [1]_.
 
         Parameters
         ----------
-        angle : float
-            Scattering angle in radians.
+        angle : astropy.units.Quantity
+            Scattering angle.
 
         Returns
         -------
             Chandrasekhar phase function for scattering of natural light.
+
+        References
+        ----------
+        .. [1] S. Chandrasekhar, Radiative Transfer, Dover Publications, 1960.
         """
         rho = self.depolarization
 
         # need to solve Chandrasekhar eq. 254 for gamma as a function of rho
         f_1 = (2 + 2 * rho) / (2 + rho)
         f_2 = (1 - rho) / (1 + rho)
-        return 0.75 * f_1 * (1 + f_2 * pow(cos(angle), 2))  # Chandrasekhar eq. 255
+        return 0.75 * f_1 * (1 + f_2 * np.cos(angle) ** 2)  # Chandrasekhar eq. 255
 
     # TODO: where does this come from? Needs unit test
     def back_scattering_coefficient(self, angle):
         """
         Back-scattering coefficient for a given scattering angle.
 
         Parameters
         ----------
-        angle : float
-            Scattering angle in radians
+        angle : astropy.units.Quantity
+            Scattering angle.
 
         Returns
         -------
-        float
+        astropy.units.Quantity
             Back-scattering coefficient [1/km]
         """
-        return self.phase_function(angle) * self.beta / (4 * pi)
+        return self.phase_function(angle) * self.beta / (4 * np.pi)
 
     def print_params(self):
         """Prints Rayleigh scattering parameters."""
-        print(f"Wavelength:              {self.wavelength} nm")
-        print(f"Air Pressure:            {self.pressure} hPa")
-        print(f"Air Temperature:         {self.temperature} K")
-        print(f"Rel. Humidity:           {self.relative_humidity} %")
+        print(f"Wavelength:              {self.wavelength}")
+        print(f"Air Pressure:            {self.pressure}")
+        print(f"Air Temperature:         {self.temperature}")
+        print(f"Rel. Humidity:           {self.relative_humidity}")
         print(f"CO2 concentration:       {self.co2_bkg} ppmv")
         print(f"Refractive Index:        {self.refractive_index}")
         print(f"King Factor:             {self.king_factor}")
         print(f"Depolarization:          {self.depolarization}")
-        print(f"Mol. cross section:      {self.scattering_cross_section} cm^-2")
-        print(f"Volume scattering coeff: {self.beta} km^-1")
+        print(f"Mol. cross section:      {self.scattering_cross_section}")
+        print(f"Volume scattering coeff: {self.beta}")
```

### Comparing `molecularprofiles-0.2.0/src/molecularprofiles.egg-info/PKG-INFO` & `molecularprofiles-0.3.0/src/molecularprofiles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecularprofiles
-Version: 0.2.0
+Version: 0.3.0
 Summary: Meteorological data analysis suite
 Author-email: Pere Munar Adrover <pere.munar@uab.cat>, Markus Gaug <markus.gaug@uab.cat>, Scott Griffiths <sgriffiths@ifae.es>, Georgios Voutsinas <georgios.voutsinas@unige.ch>, Mykhailo Dalchenko <mykhailo.dalchenko@unige.ch>
 License: Copyright (c) 2020, Molecularprofiles Project
         
         Redistribution and use in source and binary forms, with or withoutmodification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
```

### Comparing `molecularprofiles-0.2.0/src/molecularprofiles.egg-info/SOURCES.txt` & `molecularprofiles-0.3.0/src/molecularprofiles.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,13 +6,12 @@
 src/molecularprofiles.egg-info/PKG-INFO
 src/molecularprofiles.egg-info/SOURCES.txt
 src/molecularprofiles.egg-info/dependency_links.txt
 src/molecularprofiles.egg-info/requires.txt
 src/molecularprofiles.egg-info/top_level.txt
 src/molecularprofiles/utils/__init__.py
 src/molecularprofiles/utils/constants.py
-src/molecularprofiles/utils/dataframe_ops.py
 src/molecularprofiles/utils/grib_utils.py
 src/molecularprofiles/utils/humidity.py
 src/molecularprofiles/utils/mdps_log.conf
 src/molecularprofiles/utils/observatory.py
 src/molecularprofiles/utils/rayleigh.py
```


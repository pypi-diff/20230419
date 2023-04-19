# Comparing `tmp/ztfimg-0.7.0.tar.gz` & `tmp/ztfimg-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ztfimg-0.7.0.tar", last modified: Thu Mar 18 19:33:29 2021, max compression
+gzip compressed data, was "dist/ztfimg-0.8.0.tar", last modified: Fri Mar 19 09:43:32 2021, max compression
```

## Comparing `ztfimg-0.7.0.tar` & `ztfimg-0.8.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2021-03-18 19:33:29.720101 ztfimg-0.7.0/
--rw-r--r--   0 mrigault   (501) staff       (20)      692 2021-03-18 19:33:29.719726 ztfimg-0.7.0/PKG-INFO
--rw-r--r--   0 mrigault   (501) staff       (20)     5061 2021-03-18 13:39:00.000000 ztfimg-0.7.0/README.md
--rw-r--r--   0 mrigault   (501) staff       (20)       38 2021-03-18 19:33:29.720287 ztfimg-0.7.0/setup.cfg
--rw-r--r--   0 mrigault   (501) staff       (20)     1859 2021-03-18 19:33:08.000000 ztfimg-0.7.0/setup.py
-drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2021-03-18 19:33:29.717650 ztfimg-0.7.0/ztfimg/
--rw-r--r--   0 mrigault   (501) staff       (20)       21 2021-03-18 19:33:03.000000 ztfimg-0.7.0/ztfimg/__init__.py
--rw-r--r--   0 mrigault   (501) staff       (20)    10920 2021-03-18 19:24:28.000000 ztfimg-0.7.0/ztfimg/catalog.py
--rw-r--r--   0 mrigault   (501) staff       (20)     7791 2020-05-05 11:57:50.000000 ztfimg-0.7.0/ztfimg/dao.py
--rw-r--r--   0 mrigault   (501) staff       (20)    31619 2021-03-18 19:21:07.000000 ztfimg-0.7.0/ztfimg/image.py
--rw-r--r--   0 mrigault   (501) staff       (20)     6971 2021-03-18 14:49:17.000000 ztfimg-0.7.0/ztfimg/io.py
--rw-r--r--   0 mrigault   (501) staff       (20)    13283 2020-12-31 09:26:52.000000 ztfimg-0.7.0/ztfimg/stamps.py
--rw-r--r--   0 mrigault   (501) staff       (20)    11729 2021-03-18 13:12:10.000000 ztfimg-0.7.0/ztfimg/tools.py
-drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2021-03-18 19:33:29.719247 ztfimg-0.7.0/ztfimg.egg-info/
--rw-r--r--   0 mrigault   (501) staff       (20)      692 2021-03-18 19:33:29.000000 ztfimg-0.7.0/ztfimg.egg-info/PKG-INFO
--rw-r--r--   0 mrigault   (501) staff       (20)      251 2021-03-18 19:33:29.000000 ztfimg-0.7.0/ztfimg.egg-info/SOURCES.txt
--rw-r--r--   0 mrigault   (501) staff       (20)        1 2021-03-18 19:33:29.000000 ztfimg-0.7.0/ztfimg.egg-info/dependency_links.txt
--rw-r--r--   0 mrigault   (501) staff       (20)        7 2021-03-18 19:33:29.000000 ztfimg-0.7.0/ztfimg.egg-info/top_level.txt
+drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2021-03-19 09:43:32.350239 ztfimg-0.8.0/
+-rw-r--r--   0 mrigault   (501) staff       (20)      692 2021-03-19 09:43:32.349862 ztfimg-0.8.0/PKG-INFO
+-rw-r--r--   0 mrigault   (501) staff       (20)     4489 2021-03-19 09:42:46.000000 ztfimg-0.8.0/README.md
+-rw-r--r--   0 mrigault   (501) staff       (20)       38 2021-03-19 09:43:32.350358 ztfimg-0.8.0/setup.cfg
+-rw-r--r--   0 mrigault   (501) staff       (20)     1961 2021-03-19 09:43:06.000000 ztfimg-0.8.0/setup.py
+drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2021-03-19 09:43:32.347032 ztfimg-0.8.0/ztfimg/
+-rw-r--r--   0 mrigault   (501) staff       (20)       21 2021-03-19 09:42:59.000000 ztfimg-0.8.0/ztfimg/__init__.py
+-rw-r--r--   0 mrigault   (501) staff       (20)     3067 2021-03-19 08:59:24.000000 ztfimg-0.8.0/ztfimg/astrometry.py
+-rw-r--r--   0 mrigault   (501) staff       (20)    10920 2021-03-18 19:24:28.000000 ztfimg-0.8.0/ztfimg/catalog.py
+-rw-r--r--   0 mrigault   (501) staff       (20)     7791 2020-05-05 11:57:50.000000 ztfimg-0.8.0/ztfimg/dao.py
+-rw-r--r--   0 mrigault   (501) staff       (20)    30287 2021-03-19 09:11:26.000000 ztfimg-0.8.0/ztfimg/image.py
+-rw-r--r--   0 mrigault   (501) staff       (20)     6971 2021-03-18 14:49:17.000000 ztfimg-0.8.0/ztfimg/io.py
+-rw-r--r--   0 mrigault   (501) staff       (20)    13283 2020-12-31 09:26:52.000000 ztfimg-0.8.0/ztfimg/stamps.py
+-rw-r--r--   0 mrigault   (501) staff       (20)    11729 2021-03-18 13:12:10.000000 ztfimg-0.8.0/ztfimg/tools.py
+drwxr-xr-x   0 mrigault   (501) staff       (20)        0 2021-03-19 09:43:32.349399 ztfimg-0.8.0/ztfimg.egg-info/
+-rw-r--r--   0 mrigault   (501) staff       (20)      692 2021-03-19 09:43:32.000000 ztfimg-0.8.0/ztfimg.egg-info/PKG-INFO
+-rw-r--r--   0 mrigault   (501) staff       (20)      272 2021-03-19 09:43:32.000000 ztfimg-0.8.0/ztfimg.egg-info/SOURCES.txt
+-rw-r--r--   0 mrigault   (501) staff       (20)        1 2021-03-19 09:43:32.000000 ztfimg-0.8.0/ztfimg.egg-info/dependency_links.txt
+-rw-r--r--   0 mrigault   (501) staff       (20)        7 2021-03-19 09:43:32.000000 ztfimg-0.8.0/ztfimg.egg-info/top_level.txt
```

### Comparing `ztfimg-0.7.0/PKG-INFO` & `ztfimg-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ztfimg
-Version: 0.7.0
+Version: 0.8.0
 Summary:  ZTFimg 
 Home-page: https://github.com/MickaelRigault/ztfimg
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 Maintainer: Mickael Rigault
 Maintainer-email: m.rigault@ipnl.in2p3.fr
 License: BSD (3-clause)
```

### Comparing `ztfimg-0.7.0/README.md` & `ztfimg-0.8.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,133 +1,139 @@
 # ztfimg
 ZTF Images tools 
 
 # Installation
 
-This package uses `sep` for source extraction, background estimation and aperture photometry. [sep](https://sep.readthedocs.io/en/v1.0.x/api/sep.extract.html) is a python version of sextractor.  
+[![PyPI](https://img.shields.io/pypi/v/ztfimg.svg?style=flat-square)](https://pypi.python.org/pypi/ztfimg)
 
-## Getting the PS1Calibrator files
-
-Ask Mickael
+or git:
+```
+git clone https://github.com/MickaelRigault/ztfimg.git
+cd ztfim
+pyton setup.py install
+```
 
-# ztfimg
+#### Dependencies
 
-## Main Objects:
-- `ScienceImage`: to load ZTF's `sciimg.fits` together with it's `mskimg.fits`)
-- `ReferenceImage`: to load ZTF's `refimg.fits`
-`ScienceImage` and `ReferenceImage` have the same methods and almost the same attributes. 
+- This package uses `sep` for source extraction, background estimation and aperture photometry. [sep](https://sep.readthedocs.io/en/v1.0.x/api/sep.extract.html) is a python version of sextractor.  
+- This packages uses ztfquery for accessing ztf image product. [ztfquery](https://github.com/MickaelRigault/ztfquery)
 
-- `DAOPhotReader`: Simple Class to read the .psf doaphot outputs.
 
-## usage
+***
+# quick start
 
 Say you have a sciimg and its associated mask:
 ```python
 sciimg = "ztf_20200204197199_000812_zr_c04_o_q3_sciimg.fits"
 mask = "ztf_20200204197199_000812_zr_c04_o_q3_mskimg.fits"
 ```
 then:
 ```python
 from ztfimg import image
 z = image.ScienceImage(sciimg, mask)
-z.load_source_background()
-z.show()
+z.show('dataclean')
+```
+
+<p align="left">
+  <img src="examples/sciimg_masked_bkgdsub.png" width="500" title="hover text">
+</p>
+
+
+**Alternative loading**: If you don't know the exact path of the ztf file (or if you never downloaded it), use the `from_filenam()` class method to instanciate the image. It will look for the file and download it if necessary. See `ztfquery` for details on how this works. The sciimg only is necessary, it will look itself for the corresponding mskimg. However, you can still force the use of another mskimg (though you should not).
+
+```python
+from ztfimg import image
+z = image.ScienceImage.from_filename(sciimg)
+z.show('dataclean')
+```
+
+## Data
+ZTFImages hold three data attributes:
+- `self.data`: the image data as loaded
+- `self.datamasked`: the image data as loaded by masked for bad pixel values (see `self.get_mask()`)
+- `self.dataclean`: masked images background subtracted (see `self.get_background()`)
+
+In addition you have:
+- `self.mask`: the bitmask data as loaded
+- `self.background`: the default background image constructed (see `self.set_background()` and `self.load_source_background()`
+
+**Note**: the ztf mask has by default the following arguments
+```python
+z.get_mask( tracks=True, ghosts=True, spillage=True, spikes=True,
+            dead=True, nan=True, saturated=True, brightstarhalo=True,
+            lowresponsivity=True, highresponsivity=True, noisy=True,
+            sexsources=False, psfsources=False)
 ```
-![](examples/sciimg_masked_bkgdsub.png)
 
 
-This image is masked for bad pixels values (see bitmasking below) and background subtracted. The background is the sep.Background estimated on the bad-pixels and sources-masked out data.
+## Astrometry
+`ztfimg` uses `astropy.wcs` for loading the WCS solution given the image's header. We use the following definitions:
+- `xy`: image pixel coordinates
+- `radec`: world system RA, Dec coordinates (in degree)
+- `uv`: tangent plane coordinates (in arcsec)
+
+(`uv` needs `pointing` correcly set. Change the header pointing key if neccesary `self.load_wcs(header, pointingkey=["RA","DEC")` )
+
+Object holder wcs solutions have the system conversion methods, e.g. `xy_to_radec`, `uv_to_radec`, `xy_to_uv`
+
+
+## Flux / Counts / Mags
 
-## Conversions
+- `counts`: values from the images
+- `flux`: flux (erg/s/cm2/A) using the `magzp` from the header and assuming the effective filter wavelength (see `self.filter_lbda`)
+- `mag`: magnitude (ab) using the `magzp` from the header  and assuming the effective filter wavelength (see `self.filter_lbda`)
 
-- *counts, flux, mags*: You have all the `count_to_flux` or `mag_to_counts` ets combinations as methods.
-- *(RA,Dec) vs. (x,y)*: use `z.coords_to_pixels(ra, dec)` or `z.pixels_to_coords(x,y)`
+Images have the convertion methods, e.g. `counts_to_mag`, `flux_to_counts` or `mag_to_flux`.
 
 
-## Source Extraction 
+***
+# Source Extraction 
 
 You can run `sep.extract` to extract ellipses à la sextractor. Run:
 ```python
 z.extract_sources(data="dataclean", setmag=True)
 ```
 
 Access the results as:
 ```python
 z.sources
 ```
 
-## Masking
+***
+# Aperture Photometry
 
-### source-masking
-
-### ScienceImage: Bitmasking access
-```python
-# Here is the default masking, True, means datamasked=nan for these cases
-z.get_mask( tracks=True, ghosts=True, spillage=True, spikes=True,
-            dead=True, nan=True, saturated=True, brightstarhalo=True,
-            lowresponsivity=True, highresponsivity=True, noisy=True,
-            sexsources=False, psfsources=False)
-```
-
-## Aperture Photometry
-
-you have the `get_aperture()` method that measure the exact aperture photometry given a (list of) position(s) and radius. You can also provide the annulus size if you want the aperture to be corrected for this as background.
+The `get_aperture()` method measures the exact aperture photometry given a (list of) position(s) and radius (in pixels). 
+You can also provide the annulus size if you want the aperture to be corrected for this as background.
+The returned values (value, errors) could be in any `counts`, `flux` or `mag`.
 
 For intance, you want the aperture photometry, in mag, on RA, Dec coordinates with 5 pixels radius:
 ```python
-x,y = z.coords_to_pixels(RA, Dec)
+x,y = z.radec_to_xy(RA, Dec)
 mag, magerr = z.get_aperture(x,y, 5, unit="mag")
 ```
 
-## Catalogs & Catalog Matching
-Remark that both `sources`, `ps1cat` and any other catalog you set using the `set_catalog()` method are stored inside a `ztfimg.CatalogCollection` instance `z.catalogs`. This instance has all the matching functionalities between two catalogs you stored. 
+***
+# Catalogs
+
+to be done.
 
-For instance, you can also directly get matched values such as (x,y) ccd positions, (ra,dec) or mag beetwen `sources` and `ps1cat` by doing
-```python
-z.catalogs.get_matched_entries(["ra","dec","x","y","mag"], 'sources', 'ps1cat')
-```
-```
-ps1cat_index	sources_index	angsep_arcsec	ps1cat_ra	sources_ra	ps1cat_dec	sources_dec	ps1cat_x	sources_x	ps1cat_y	sources_y	ps1cat_mag	sources_mag
-0	0	200	0.177830	80.458424	80.458457	59.081236	59.081190	1524.971933	1524.929682	109.828648	109.999139	14.300	14.298286
-1	1	439	0.091733	80.580818	80.580863	59.042257	59.042246	1315.658142	1315.579032	269.438577	269.482766	14.407	14.391963
-2	2	2692	0.134097	80.643587	80.643647	58.627628	58.627608	1341.017199	1340.913537	1748.049916	1748.132412	14.422	14.414028
-3	3	203	0.212481	80.378699	80.378784	59.076712	59.076673	1671.527068	1671.384957	111.507782	111.662257	14.432	14.426520
-4	4	1222	0.195256	80.465035	80.465061	58.895667	58.895614	1577.243713	1577.213421	767.680720	767.871187	14.340	14.335927
-5	5	2185	0.161587	79.866613	79.866664	58.679673	58.679636	2752.683959	2752.603432	1419.232736	1419.370579	14.317	14.305793
-6	6	1496	0.072166	81.037901	81.037929	58.867203	58.867217	538.472196	538.415826	966.704057	966.660447	14.529	14.509354
-```
 
-## Get a Stamp
+***
+# Stamp
 
-You can get a stamp of anywhere in the image, for instance center on a star matched both by `sources` and `ps1cat` as returned by `z.catalogs.get_matched_entries(["x","y"], 'sources', 'ps1cat')`. Once you have the `(x,y)` coordinates, do:
 ```python 
 stamp = z.get_stamp(x,y, dx=23, dy=23)
 stamp.show()
 ```
 The stamp is centered on the pixel containing the given coordinates. The actual requested `(x,y)` is shown with the white cross.
 
-![image](examples/StarStamp.png)
+
+<p align="left">
+  <img src="examples/StarStamp.png" width="200" title="hover text">
+</p>
 
 You can also simply do:
 ```python
 stampdata =  z.get_stamp(x,y, dx=23, dy=23, asarray=True)
 ```
 to get the 2D numpy array rather than a `ztfimg.Stamp` object.
 
-
-# DAOPhotReader
-
-There is a simply class object that allows you to open the DAOPhot output data.
-Given a  `sciimgdao.psf` file (aka. psffile) you have:
-```python
-from ztfimg import dao
-d = dao.DAOPhotReader(psffile)
-d.show()
-```
-![image](examples/daophot_composition.png)
-
-The actual PSF is a combination of the base-profile (here "gaussian") and the structures. 
-So to get the PSF made of 1 base-profile and 0.1 of each stamp:
-```python
-psf = d.get_psf(1, [0.1,0.1,0.1])
-```
-
```

### Comparing `ztfimg-0.7.0/setup.py` & `ztfimg-0.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 DISTNAME = 'ztfimg'
 AUTHOR = 'Mickael Rigault'
 MAINTAINER = 'Mickael Rigault' 
 MAINTAINER_EMAIL = 'm.rigault@ipnl.in2p3.fr'
 URL = 'https://github.com/MickaelRigault/ztfimg'
 LICENSE = 'BSD (3-clause)'
 DOWNLOAD_URL = 'https://github.com/MickaelRigault/ztfimg'
-VERSION = '0.7.0'
+VERSION = '0.8.0'
 
 try:
     from setuptools import setup, find_packages
     _has_setuptools = True
 except ImportError:
     from distutils.core import setup
     _has_setuptools = False
@@ -23,14 +23,19 @@
 def check_dependencies():
     install_requires = []
     try:
         import sep
     except ImportError:
         install_requires.append('sep')
 
+    try:
+        import ztfquery
+    except ImportError:
+        install_requires.append('ztfquery')
+
     return install_requires
 
 if __name__ == "__main__":
 
     install_requires = check_dependencies()
 
     if _has_setuptools:
```

### Comparing `ztfimg-0.7.0/ztfimg/catalog.py` & `ztfimg-0.8.0/ztfimg/catalog.py`

 * *Files identical despite different names*

### Comparing `ztfimg-0.7.0/ztfimg/dao.py` & `ztfimg-0.8.0/ztfimg/dao.py`

 * *Files identical despite different names*

### Comparing `ztfimg-0.7.0/ztfimg/image.py` & `ztfimg-0.8.0/ztfimg/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """ """
 import pandas
 import numpy as np
 
 from astropy.io import fits
-from astropy.wcs import WCS
 from astropy.nddata import bitmask
 from .io import PS1Calibrators, GaiaCalibrators
 from . import tools
 ZTF_FILTERS = {"ztfg":{"wave_eff":4813.97, "fid":1},
                "ztfr":{"wave_eff":6421.81, "fid":2},
                "ztfi":{"wave_eff":7883.06, "fid":3}
                 }
 
 
-class ZTFImage( object ):
+from .astrometry import WCSHolder
+    
+class ZTFImage( WCSHolder ):
     """ """
     BITMASK_KEY = [ "tracks","sexsources","lowresponsivity","highresponsivity",
                     "noisy","ghosts","spillage","spikes","saturated",
                     "dead","nan","psfsources","brightstarhalo"]
 
     def __init__(self, imagefile=None, maskfile=None):
         """ """
@@ -55,15 +56,16 @@
         self._mask = fits.getdata(maskfile,**kwargs)
         self._maskheader = fits.getheader(maskfile,**kwargs)
 
     def load_wcs(self, header=None):
         """ """
         if header is None:
             header = self.header
-        self._wcs = WCS(header)
+            
+        super().load_wcs(header)
 
     def load_source_background(self, r=5, setit=True, datamasked=None, **kwargs):
         """
         kwargs goes to """
         from sep import Background
         if datamasked is None:
             if self.sources is None:
@@ -74,15 +76,14 @@
             datamasked = self.get_data(applymask=True, from_sources=from_sources,
                                         r=r, rmbkgd=False)
 
         self._sourcebackground = Background(datamasked.byteswap().newbyteorder())
         if setit:
             self.set_background(self._sourcebackground.back())
 
-
     def load_ps1_calibrators(self, setxy=True):
         """ """
         self.set_catalog( self.get_ps1_calibrators(setxy=setxy), "ps1cat")
 
     def load_gaia_calibrators(self, setxy=True):
         """ """
         self.set_catalog( self.get_gaia_calibrators(setxy=setxy), "gaia")
@@ -111,64 +112,64 @@
 
     def set_catalog(self, dataframe, label):
         """ """
         if "ra" not in dataframe.columns and "x" not in dataframe.columns:
             raise ValueError("The dataframe must contains either (x,y) coords or (ra,dec) coords")
 
         if "ra" in dataframe.columns and "x" not in dataframe.columns:
-            x,y = self.coords_to_pixels(dataframe["ra"], dataframe["dec"])
+            x,y = self.radec_to_xy(dataframe["ra"], dataframe["dec"])
             dataframe["x"] = x
             dataframe["y"] = y
 
         if "x" in dataframe.columns and "ra" not in dataframe.columns:
-            ra,dec = self.pixels_to_coords(dataframe["x"], dataframe["y"])
+            ra,dec = self.xy_to_radec(dataframe["x"], dataframe["y"])
             dataframe["ra"] = ra
             dataframe["dec"] = dec
 
         if "u" not in dataframe.columns:
-            u, v = self.coords_to_uv(dataframe["ra"], dataframe["dec"])
+            u, v = self.radec_to_uv(dataframe["ra"], dataframe["dec"])
             dataframe["u"] = u
             dataframe["v"] = v
             
         self.catalogs.set_catalog(dataframe, label)
 
     # -------- #
     # GETTER   #
     # -------- #
     def _setxy_to_cat_(self, cat, drop_outside=True, pixelbuffer=10):
         """ """
-        x,y = self.coords_to_pixels(cat["ra"], cat["dec"])
-        u,v = self.coords_to_uv(cat["ra"], cat["dec"])
+        x,y = self.radec_to_xy(cat["ra"], cat["dec"])
+        u,v = self.radec_to_uv(cat["ra"], cat["dec"])
         cat["x"] = x
         cat["y"] = y
         cat["u"] = u
         cat["v"] = v
 
         if drop_outside:
             ymax, xmax = self.shape
             cat = cat[cat["x"].between(-pixelbuffer, xmax+pixelbuffer) & \
                       cat["y"].between(-pixelbuffer, ymax+pixelbuffer)]
         return cat
     
     def get_ps1_calibrators(self, setxy=True, drop_outside=True, pixelbuffer=10):
         """ """
         # remark: radec is going to be used only the fieldid is not already downloaded.
-        ps1cat = PS1Calibrators(self.rcid, self.fieldid, radec=self.get_center(inpixel=False)).data
+        ps1cat = PS1Calibrators(self.rcid, self.fieldid, radec=self.get_center(system="radec")).data
         
         # Set mag as the current band magnitude
         ps1cat['mag'] = ps1cat["%smag"%self.filtername.split("_")[-1]]
         ps1cat['e_mag'] = ps1cat["e_%smag"%self.filtername.split("_")[-1]]
         if setxy and ("ra" in ps1cat.columns and "x" not in ps1cat.columns):
             ps1cat = self._setxy_to_cat_(ps1cat, drop_outside=drop_outside, pixelbuffer=pixelbuffer)
 
         return ps1cat
 
     def get_gaia_calibrators(self, setxy=True, drop_namag=True, drop_outside=True, pixelbuffer=10):
         """ """
-        cat = GaiaCalibrators(self.rcid, self.fieldid, radec=self.get_center(inpixel=False)).data
+        cat = GaiaCalibrators(self.rcid, self.fieldid, radec=self.get_center(system="radec")).data
         
         if drop_namag:
             cat = cat[~pandas.isna(cat[["gmag","rpmag","bpmag"]]).any(axis=1)]
         cat[["ps1_id","sdssdr13_id"]] = cat[["ps1_id","sdssdr13_id"]].fillna("None")
         
         # Set mag as the current band magnitude
         cat['mag'] = cat["gmag"]
@@ -381,20 +382,26 @@
         if unit in ["count","counts"]:
             return counts, counterr
         if unit in ["flux"]:
             return self.counts_to_flux(counts, counterr)
         if unit in ["mag"]:
             return self.counts_to_mag(counts, counterr)
 
-    def get_center(self, inpixel=True):
+    def get_center(self, system="xy"):
         """ x and y or RA, Dec coordinates of the centroid. (shape[::-1]) """
-        if inpixel:
+        if system in ["xy","pixel","pixels","pxl"]:
             return (np.asarray(self.shape[::-1])+1)/2
+
+        if system in ["uv","tangent"]:
+            return np.squeeze(self.xy_to_uv(*self.get_center(system="xy")) )
         
-        return np.squeeze(self.pixels_to_coords(*self.get_center(inpixel=True)) )
+        if system in ["radec","coords","worlds"]:
+            return np.squeeze(self.xy_to_radec(*self.get_center(system="xy")) )
+
+        raise ValueError(f"cannot parse the given system {system}, use xy, radec or uv")
 
     def get_diagonal(self, inpixel=True):
         """ Get the size of the diagonal [[0,0]->[-1,-1]].
         If inpixel is False, it is given in degrees. """
         from astropy import units
         height, width = self.shape
         diagonal_pixels = np.sqrt(width**2+height**2)
@@ -407,45 +414,23 @@
     # CONVERT  #
     # -------- #
     #    
     # WCS
     # pixel->
     def pixels_to_coords(self, x, y):
         """ get sky ra, dec [in deg] coordinates given the (x,y) ccd positions  """
-        return self.wcs.all_pix2world(np.asarray([np.atleast_1d(x),
-                                                  np.atleast_1d(y)]).T,
-                                      0).T
-    
-    def pixels_to_uv(self, x, y):
-        """ w,y to u, v tangent plane projection (in arcsec from pointing center). 
-        This uses pixels_to_coords->coords_to_uv
-        """
-        ra, dec = self.pixels_to_coords( x, y)
-        return self.coords_to_uv(ra, dec)
+        print("pixels_to_coords is DEPRECATED, use xy_to_radec")
+        return self.xy_to_radec(x, y)
 
     # coords -> 
     def coords_to_pixels(self, ra, dec):
         """ get the (x,y) ccd positions given the sky ra, dec [in deg] corrdinates """
-        return self.wcs.all_world2pix(np.asarray([np.atleast_1d(ra),
-                                                  np.atleast_1d(dec)]).T,
-                                      0).T
-    
-    def coords_to_uv(self, ra, dec):
-        """ radec to u, v tangent plane projection (in arcsec from pointing center) """
-        return np.asarray(tools.project([ra, dec], self.pointing))*180/np.pi * 3600
-    
-    # uv -> 
-    def uv_to_pixels(self, u, v):
-        """ get the x, y ccd position given the tangent plane coordinates u, v """
-        ra, dec = self.uv_to_coords(u, v)
-        return self.coords_to_pixels(ra, dec)
+        print("coords_to_pixels is DEPRECATED, use radec_to_xy")
+        return self.radec_to_xy(ra,dec)
     
-    def uv_to_coords(self, u, v):
-        """ get the ra, dec coordinates given the tangent plane coordinates u, v """
-        return np.asarray(tools.deproject([u, v], self.pointing))*180/np.pi
     #
     # Flux - Counts - Mags
     def counts_to_mag(self, counts, dcounts=None):
         """ converts counts into flux [erg/s/cm2/A] """
         return tools.counts_to_mag(counts,dcounts, self.magzp, self.filter_lbda)
 
     def counts_to_flux(self, counts, dcounts=None):
@@ -721,27 +706,14 @@
         return self.header.get("FIELDID", self.header.get("DBFIELD", None))
 
     @property
     def filterid(self):
         """ """
         return self.header.get("FILTERID", self.header.get("DBFID", None)) #science vs. ref
 
-    @property
-    def pointing(self):
-        """ requested telescope pointing [in degree] """
-        if not hasattr(self, "_pointing") or self._pointing is None:
-            pra, pdec = self.header.get("RA", None), self.header.get("DEC", None)
-            if pra is None or pdec is None:
-                return None
-            
-            from astropy import coordinates, units
-            sc = coordinates.SkyCoord(pra, pdec, unit=(units.hourangle, units.deg))
-            self._pointing = sc.ra.value, sc.dec.value
-            
-        return self._pointing
     
     
 class ScienceImage( ZTFImage ):
 
     def __init__(self, imagefile=None, maskfile=None):
         """ """
         if imagefile is not None:
```

### Comparing `ztfimg-0.7.0/ztfimg/io.py` & `ztfimg-0.8.0/ztfimg/io.py`

 * *Files identical despite different names*

### Comparing `ztfimg-0.7.0/ztfimg/stamps.py` & `ztfimg-0.8.0/ztfimg/stamps.py`

 * *Files identical despite different names*

### Comparing `ztfimg-0.7.0/ztfimg/tools.py` & `ztfimg-0.8.0/ztfimg/tools.py`

 * *Files identical despite different names*

### Comparing `ztfimg-0.7.0/ztfimg.egg-info/PKG-INFO` & `ztfimg-0.8.0/ztfimg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ztfimg
-Version: 0.7.0
+Version: 0.8.0
 Summary:  ZTFimg 
 Home-page: https://github.com/MickaelRigault/ztfimg
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 Maintainer: Mickael Rigault
 Maintainer-email: m.rigault@ipnl.in2p3.fr
 License: BSD (3-clause)
```


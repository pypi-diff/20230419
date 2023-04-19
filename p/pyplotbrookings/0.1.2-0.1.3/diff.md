# Comparing `tmp/pyplotbrookings-0.1.2.tar.gz` & `tmp/pyplotbrookings-0.1.3.tar.gz`

## Comparing `pyplotbrookings-0.1.2.tar` & `pyplotbrookings-0.1.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/examples/.DS_Store
--rw-r--r--   0        0        0   544308 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/examples/Examples.ipynb
--rw-r--r--   0        0        0   556797 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/examples/.ipynb_checkpoints/Examples-checkpoint.ipynb
--rw-r--r--   0        0        0    50649 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/figures/Figure1A.png
--rw-r--r--   0        0        0   110676 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/figures/Figure2.png
--rw-r--r--   0        0        0    41346 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/figures/Figure3.png
--rw-r--r--   0        0        0    30774 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/figures/logo.png
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/.DS_Store
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/__init__.py
--rw-r--r--   0        0        0    18369 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/pyplotbrookings.py
--rw-r--r--   0        0        0   931903 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/.ipynb_checkpoints/Examples-checkpoint.ipynb
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/LICENSE.txt
--rw-r--r--   0        0        0   168060 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-Black.ttf
--rw-r--r--   0        0        0   174108 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-BlackItalic.ttf
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-Italic.ttf
--rw-r--r--   0        0        0   167000 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-Light.ttf
--rw-r--r--   0        0        0   173172 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-LightItalic.ttf
--rw-r--r--   0        0        0   168644 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-Medium.ttf
--rw-r--r--   0        0        0   173416 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-MediumItalic.ttf
--rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-Regular.ttf
--rw-r--r--   0        0        0   168488 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-Thin.ttf
--rw-r--r--   0        0        0   172860 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-ThinItalic.ttf
--rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/b_logo.png
--rw-r--r--   0        0        0    21136 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/bc.png
--rw-r--r--   0        0        0    12097 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/bi.png
--rw-r--r--   0        0        0    17913 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/brookings.png
--rw-r--r--   0        0        0    18458 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/cc.png
--rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/ccf.png
--rw-r--r--   0        0        0   101943 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/ceaps.png
--rw-r--r--   0        0        0    26494 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/cepm.png
--rw-r--r--   0        0        0    56387 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/chp.png
--rw-r--r--   0        0        0   107876 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/cmep.png
--rw-r--r--   0        0        0   107158 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/crm.png
--rw-r--r--   0        0        0    22586 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/csd.png
--rw-r--r--   0        0        0    93053 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/cti.png
--rw-r--r--   0        0        0    20197 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/cue.png
--rw-r--r--   0        0        0    96557 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/cuse.png
--rw-r--r--   0        0        0    14692 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/es.png
--rw-r--r--   0        0        0    13597 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/fp.png
--rw-r--r--   0        0        0    21605 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/global.png
--rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/gs.png
--rw-r--r--   0        0        0    47345 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/hc.png
--rw-r--r--   0        0        0    20101 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/metro.png
--rw-r--r--   0        0        0     8222 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/src/pyplotbrookings/logos/thp.png
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/LICENSE
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/README.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/examples/.DS_Store
+-rw-r--r--   0        0        0   544308 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/examples/Examples.ipynb
+-rw-r--r--   0        0        0   556797 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/examples/.ipynb_checkpoints/Examples-checkpoint.ipynb
+-rw-r--r--   0        0        0    50649 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/figures/Figure1A.png
+-rw-r--r--   0        0        0   110676 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/figures/Figure2.png
+-rw-r--r--   0        0        0    41346 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/figures/Figure3.png
+-rw-r--r--   0        0        0    30774 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/figures/logo.png
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/.DS_Store
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/__init__.py
+-rw-r--r--   0        0        0    18385 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/pyplotbrookings.py
+-rw-r--r--   0        0        0   931903 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/.ipynb_checkpoints/Examples-checkpoint.ipynb
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/LICENSE.txt
+-rw-r--r--   0        0        0   168060 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-Black.ttf
+-rw-r--r--   0        0        0   174108 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-BlackItalic.ttf
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   167000 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-Light.ttf
+-rw-r--r--   0        0        0   173172 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-LightItalic.ttf
+-rw-r--r--   0        0        0   168644 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-Medium.ttf
+-rw-r--r--   0        0        0   173416 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-MediumItalic.ttf
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-Regular.ttf
+-rw-r--r--   0        0        0   168488 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-Thin.ttf
+-rw-r--r--   0        0        0   172860 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-ThinItalic.ttf
+-rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/b_logo.png
+-rw-r--r--   0        0        0    21136 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/bc.png
+-rw-r--r--   0        0        0    12097 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/bi.png
+-rw-r--r--   0        0        0    17913 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/brookings.png
+-rw-r--r--   0        0        0    18458 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/cc.png
+-rw-r--r--   0        0        0    20676 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/ccf.png
+-rw-r--r--   0        0        0   101943 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/ceaps.png
+-rw-r--r--   0        0        0    26494 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/cepm.png
+-rw-r--r--   0        0        0    56387 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/chp.png
+-rw-r--r--   0        0        0   107876 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/cmep.png
+-rw-r--r--   0        0        0   107158 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/crm.png
+-rw-r--r--   0        0        0    22586 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/csd.png
+-rw-r--r--   0        0        0    93053 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/cti.png
+-rw-r--r--   0        0        0    20197 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/cue.png
+-rw-r--r--   0        0        0    96557 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/cuse.png
+-rw-r--r--   0        0        0    14692 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/es.png
+-rw-r--r--   0        0        0    13597 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/fp.png
+-rw-r--r--   0        0        0    21605 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/global.png
+-rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/gs.png
+-rw-r--r--   0        0        0    47345 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/hc.png
+-rw-r--r--   0        0        0    20101 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/metro.png
+-rw-r--r--   0        0        0     8222 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/src/pyplotbrookings/logos/thp.png
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/README.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6802 2020-02-02 00:00:00.000000 pyplotbrookings-0.1.3/PKG-INFO
```

### Comparing `pyplotbrookings-0.1.2/.DS_Store` & `pyplotbrookings-0.1.3/.DS_Store`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 040a 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0006  ................
-00000050: 0000 0001 0000 1000 0070 006c 0065 0073  .........p.l.e.s
-00000060: 6473 636c 0000 0000 0000 0000 0000 0000  dscl............
+00000040: 0000 0000 0000 0002 0000 0000 0000 0007  ................
+00000050: 0000 0001 0000 1000 6473 636c 626f 6f6c  ........dsclbool
+00000060: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -58,49 +58,49 @@
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000400: 0000 0000 0000 0000 0000 0006 0000 0008  ................
-00000410: 0065 0078 0061 006d 0070 006c 0065 0073  .e.x.a.m.p.l.e.s
-00000420: 6473 636c 626f 6f6c 0100 0000 0700 6600  dsclbool......f.
-00000430: 6900 6700 7500 7200 6500 7362 7773 7062  i.g.u.r.e.sbwspb
-00000440: 6c6f 6200 0000 b862 706c 6973 7430 30d6  lob....bplist00.
-00000450: 0102 0304 0506 0708 0708 0b08 5d53 686f  ............]Sho
-00000460: 7753 7461 7475 7342 6172 5b53 686f 7754  wStatusBar[ShowT
-00000470: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
-00000480: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
-00000490: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
-000004a0: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
-000004b0: 6172 0809 0809 5f10 187b 7b31 3238 2c20  ar...._..{{128, 
-000004c0: 3334 387d 2c20 7b39 3230 2c20 3433 367d  348}, {920, 436}
-000004d0: 7d09 0815 232f 3b52 5f6b 6c6d 6e6f 8a00  }...#/;R_klmno..
-000004e0: 0000 0000 0001 0100 0000 0000 0000 0d00  ................
-000004f0: 0000 0000 0000 0000 0000 0000 0000 8b00  ................
-00000500: 0000 0700 6600 6900 6700 7500 7200 6500  ....f.i.g.u.r.e.
-00000510: 7376 5372 6e6c 6f6e 6700 0000 0100 0000  svSrnlong.......
-00000520: 0300 7300 7200 6362 7773 7062 6c6f 6200  ..s.r.cbwspblob.
-00000530: 0000 b862 706c 6973 7430 30d6 0102 0304  ...bplist00.....
-00000540: 0506 0708 0708 0b08 5d53 686f 7753 7461  ........]ShowSta
-00000550: 7475 7342 6172 5b53 686f 7754 6f6f 6c62  tusBar[ShowToolb
-00000560: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
-00000570: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
-00000580: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
-00000590: 6473 5b53 686f 7753 6964 6562 6172 0809  ds[ShowSidebar..
-000005a0: 0809 5f10 187b 7b31 3238 2c20 3334 387d  .._..{{128, 348}
-000005b0: 2c20 7b39 3230 2c20 3433 367d 7d09 0815  , {920, 436}}...
-000005c0: 232f 3b52 5f6b 6c6d 6e6f 8a00 0000 0000  #/;R_klmno......
-000005d0: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
-000005e0: 0000 0000 0000 0000 0000 8b00 0000 0300  ................
-000005f0: 7300 7200 6364 7363 6c62 6f6f 6c00 0000  s.r.cdsclbool...
-00000600: 0003 0073 0072 0063 7653 726e 6c6f 6e67  ...s.r.cvSrnlong
-00000610: 0000 0001 0000 0000 0000 0000 0000 0000  ................
-00000620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000400: 0000 0000 0000 0000 0000 0007 0000 0004  ................
+00000410: 0064 0069 0073 0074 6473 636c 626f 6f6c  .d.i.s.tdsclbool
+00000420: 0100 0000 0800 6500 7800 6100 6d00 7000  ......e.x.a.m.p.
+00000430: 6c00 6500 7364 7363 6c62 6f6f 6c01 0000  l.e.sdsclbool...
+00000440: 0007 0066 0069 0067 0075 0072 0065 0073  ...f.i.g.u.r.e.s
+00000450: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
+00000460: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
+00000470: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00000480: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00000490: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+000004a0: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+000004b0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+000004c0: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
+000004d0: 3132 382c 2033 3438 7d2c 207b 3932 302c  128, 348}, {920,
+000004e0: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
+000004f0: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
+00000500: 0000 000d 0000 0000 0000 0000 0000 0000  ................
+00000510: 0000 008b 0000 0007 0066 0069 0067 0075  .........f.i.g.u
+00000520: 0072 0065 0073 7653 726e 6c6f 6e67 0000  .r.e.svSrnlong..
+00000530: 0001 0000 0003 0073 0072 0063 6277 7370  .......s.r.cbwsp
+00000540: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
+00000550: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
+00000560: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00000570: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00000580: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00000590: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+000005a0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+000005b0: 6261 7208 0908 095f 1018 7b7b 3132 382c  bar...._..{{128,
+000005c0: 2033 3438 7d2c 207b 3932 302c 2034 3336   348}, {920, 436
+000005d0: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
+000005e0: 0000 0000 0000 0101 0000 0000 0000 000d  ................
+000005f0: 0000 0000 0000 0000 0000 0000 0000 008b  ................
+00000600: 0000 0003 0073 0072 0063 6473 636c 626f  .....s.r.cdsclbo
+00000610: 6f6c 0000 0000 0300 7300 7200 6376 5372  ol......s.r.cvSr
+00000620: 6e6c 6f6e 6700 0000 0100 0000 0000 0000  nlong...........
 00000630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `pyplotbrookings-0.1.2/examples/.DS_Store` & `pyplotbrookings-0.1.3/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/examples/Examples.ipynb` & `pyplotbrookings-0.1.3/examples/Examples.ipynb`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/examples/.ipynb_checkpoints/Examples-checkpoint.ipynb` & `pyplotbrookings-0.1.3/examples/.ipynb_checkpoints/Examples-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/figures/Figure1A.png` & `pyplotbrookings-0.1.3/figures/Figure1A.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/figures/Figure2.png` & `pyplotbrookings-0.1.3/figures/Figure2.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/figures/Figure3.png` & `pyplotbrookings-0.1.3/figures/Figure3.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/figures/logo.png` & `pyplotbrookings-0.1.3/figures/logo.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/.DS_Store` & `pyplotbrookings-0.1.3/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/.DS_Store` & `pyplotbrookings-0.1.3/src/pyplotbrookings/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/pyplotbrookings.py` & `pyplotbrookings-0.1.3/src/pyplotbrookings/pyplotbrookings.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,15 +325,15 @@
 
     # Get current figure
     fig = plt.gcf()
     # Add an axis for the logo plot
     ax = fig.add_axes(logo_loc, zorder=1)
 
     # Add logo to new axis and turn off axis labeling
-    ax.imshow(logo)
+    ax.imshow(logo, cmap='viridis')
     ax.axis('off')
 
 
 def get_cmap(name, reverse=False):
     '''
     Given a palette name returns a Brookings theme colormap. 
     Note not all palettes (e.g., brand 1) should be used as colormaps.
```

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/.ipynb_checkpoints/Examples-checkpoint.ipynb` & `pyplotbrookings-0.1.3/src/pyplotbrookings/.ipynb_checkpoints/Examples-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/LICENSE.txt` & `pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-Black.ttf` & `pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-BlackItalic.ttf` & `pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-Bold.ttf` & `pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-BoldItalic.ttf` & `pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-Italic.ttf` & `pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-Light.ttf` & `pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-LightItalic.ttf` & `pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-Medium.ttf` & `pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-MediumItalic.ttf` & `pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-Regular.ttf` & `pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-Thin.ttf` & `pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/fonts/Roboto-ThinItalic.ttf` & `pyplotbrookings-0.1.3/src/pyplotbrookings/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/b_logo.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/b_logo.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/bc.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/bc.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/bi.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/bi.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/brookings.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/brookings.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/cc.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/cc.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/ccf.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/ccf.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/ceaps.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/ceaps.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/cepm.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/cepm.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/chp.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/chp.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/cmep.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/cmep.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/crm.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/crm.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/csd.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/csd.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/cti.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/cti.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/cue.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/cue.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/cuse.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/cuse.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/es.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/es.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/fp.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/fp.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/global.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/global.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/gs.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/gs.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/hc.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/hc.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/metro.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/metro.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/src/pyplotbrookings/logos/thp.png` & `pyplotbrookings-0.1.3/src/pyplotbrookings/logos/thp.png`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/LICENSE` & `pyplotbrookings-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/README.md` & `pyplotbrookings-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyplotbrookings-0.1.2/pyproject.toml` & `pyplotbrookings-0.1.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyplotbrookings"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Adam Sedlak", email="asedlak@brookings.edu" },
 ]
 description = "A plotting package for the Brookings Institution"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyplotbrookings-0.1.2/PKG-INFO` & `pyplotbrookings-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplotbrookings
-Version: 0.1.2
+Version: 0.1.3
 Summary: A plotting package for the Brookings Institution
 Project-URL: Homepage, https://github.com/Adam-Sedlak-Brookings/pyplotbrookings
 Author-email: Adam Sedlak <asedlak@brookings.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


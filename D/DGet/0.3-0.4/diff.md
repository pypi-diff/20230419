# Comparing `tmp/DGet-0.3.tar.gz` & `tmp/DGet-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DGet-0.3.tar", last modified: Tue Mar 28 03:54:36 2023, max compression
+gzip compressed data, was "DGet-0.4.tar", last modified: Wed Apr 19 05:39:46 2023, max compression
```

## Comparing `DGet-0.3.tar` & `DGet-0.4.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 03:54:36.063148 DGet-0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 03:54:36.063148 DGet-0.3/DGet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-28 03:54:36.000000 DGet-0.3/DGet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-28 03:54:36.000000 DGet-0.3/DGet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 03:54:36.000000 DGet-0.3/DGet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-28 03:54:36.000000 DGet-0.3/DGet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-28 03:54:36.000000 DGet-0.3/DGet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-28 03:54:36.000000 DGet-0.3/DGet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-28 03:54:24.000000 DGet-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-28 03:54:36.063148 DGet-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-28 03:54:24.000000 DGet-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 03:54:36.063148 DGet-0.3/dget/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-28 03:54:24.000000 DGet-0.3/dget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-03-28 03:54:24.000000 DGet-0.3/dget/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-03-28 03:54:24.000000 DGet-0.3/dget/convolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-03-28 03:54:24.000000 DGet-0.3/dget/dget.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 03:54:36.063148 DGet-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-28 03:54:24.000000 DGet-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:39:46.995087 DGet-0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:39:46.995087 DGet-0.4/DGet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-19 05:39:46.000000 DGet-0.4/DGet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-19 05:39:46.000000 DGet-0.4/DGet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 05:39:46.000000 DGet-0.4/DGet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 05:39:46.000000 DGet-0.4/DGet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-19 05:39:46.000000 DGet-0.4/DGet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 05:39:46.000000 DGet-0.4/DGet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-19 05:39:35.000000 DGet-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-19 05:39:46.995087 DGet-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-19 05:39:35.000000 DGet-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:39:46.995087 DGet-0.4/dget/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 05:39:35.000000 DGet-0.4/dget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-19 05:39:35.000000 DGet-0.4/dget/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-19 05:39:35.000000 DGet-0.4/dget/adduct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-19 05:39:35.000000 DGet-0.4/dget/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-04-19 05:39:35.000000 DGet-0.4/dget/dget.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 05:39:46.995087 DGet-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-19 05:39:35.000000 DGet-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 05:39:46.995087 DGet-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-19 05:39:35.000000 DGet-0.4/tests/test_adducts.py
```

### Comparing `DGet-0.3/LICENSE` & `DGet-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `DGet-0.3/dget/__main__.py` & `DGet-0.4/dget/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,16 +5,25 @@
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser("dget")
     parser.add_argument(
         "formula", help="Molecular formula of the compound, see molmass."
     )
-    parser.add_argument("--adduct", help="Formula of adduct.")
-    parser.add_argument("--loss", help="Formula of loss.")
+    parser.add_argument(
+        "--adduct",
+        default="[M]+",
+        help="Type of adduct in form [xM<+-><adduct>]x<+->. Valid examples are [M]-, "
+        "[M+H]+, [2M+Na2]2+, [M-H2]2-. Defaults to [M]+.",
+    )
+    parser.add_argument(
+        "--autoadduct",
+        action="store_true",
+        help="Guess the adduct from the mass spectra base peak. Overrides --adduct.",
+    )
     parser.add_argument("tofdata", type=Path, help="Path to mass spec data file.")
     parser.add_argument("--delimiter", default="\t", help="MS data file delimiter.")
     parser.add_argument(
         "--columns",
         metavar=("MASS", "SIGNAL"),
         type=int,
         default=(0, 1),
@@ -43,14 +52,17 @@
         action="store_true",
         help="Force alignment of MS data with predicted spectra, "
         "please just calibrate your MS.",
     )
 
     args = parser.parse_args()
 
+    if args.autoadduct:
+        args.adduct = "[M]+"
+
     if "D" not in args.formula:
         parser.error("--formula, must contain at least one D atom.")
 
     return args
 
 
 def main():
@@ -60,22 +72,28 @@
         "skiprows": args.skiprows,
         "usecols": args.columns,
     }
     dget = DGet(
         args.formula,
         args.tofdata,
         adduct=args.adduct,
-        loss=args.loss,
         loadtxt_kws=loadtxt_kws,
     )
+    if args.autoadduct:
+        adduct, diff = dget.guess_adduct_from_base_peak()
+        dget.formula = adduct
+        print(f"Adduct difference from base peak m/z: {diff:.4f}")
+        print()
+
     dget.mass_width = args.masswidth
     if args.realign:
         dget.align_tof_with_spectra()
 
-    print(f"Formula          : {dget.formula}")
+    print(f"Formula          : {dget.base.empirical}")
+    print(f"Adduct           : {dget.adduct}")
     print(f"M/Z              : {dget.formula.mz}")
     print(f"Monoisotopic M/Z : {dget.formula.isotope.mz}")
     print(f"%D               : {dget.deuteration * 100.0:.2f}")
     print()
     print("Deuteration Ratio Spectra")
     for i, p in enumerate(dget.deuteration_probabilites):
         print(f"D{i:<2}              : {p:.4f}")
```


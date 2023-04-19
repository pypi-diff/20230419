# Comparing `tmp/pysces-1.0.3.tar.gz` & `tmp/pysces-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysces-1.0.3.tar", last modified: Sun Sep 18 19:38:16 2022, max compression
+gzip compressed data, was "pysces-1.1.0.tar", last modified: Wed Apr 19 11:19:30 2023, max compression
```

## Comparing `pysces-1.0.3.tar` & `pysces-1.1.0.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.399903 pysces-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-09-18 19:38:13.000000 pysces-1.0.3/ADDITIONAL_LICENCES.md
--rw-r--r--   0 runner    (1001) docker     (121)     3612 2022-09-18 19:38:13.000000 pysces-1.0.3/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-09-18 19:38:13.000000 pysces-1.0.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-09-18 19:38:13.000000 pysces-1.0.3/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (121)     3204 2022-09-18 19:38:13.000000 pysces-1.0.3/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-09-18 19:38:13.000000 pysces-1.0.3/LATEST.md
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-09-18 19:38:13.000000 pysces-1.0.3/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2022-09-18 19:38:13.000000 pysces-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-09-18 19:38:13.000000 pysces-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-09-18 19:38:16.399903 pysces-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5394 2022-09-18 19:38:13.000000 pysces-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-09-18 19:38:13.000000 pysces-1.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.391903 pysces-1.0.3/pysces/
--rw-r--r--   0 runner    (1001) docker     (121)     3916 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesConfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     6369 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesContrib.py
--rw-r--r--   0 runner    (1001) docker     (121)     1096 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesContribUser.py
--rw-r--r--   0 runner    (1001) docker     (121)     9360 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesInterfaces.py
--rw-r--r--   0 runner    (1001) docker     (121)    32049 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesJWSParse.py
--rw-r--r--   0 runner    (1001) docker     (121)    53189 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesLink.py
--rw-r--r--   0 runner    (1001) docker     (121)    19989 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesMiniModel.py
--rw-r--r--   0 runner    (1001) docker     (121)   348341 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesModel.py
--rw-r--r--   0 runner    (1001) docker     (121)    12084 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesModelMap.py
--rw-r--r--   0 runner    (1001) docker     (121)    13017 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesParScan.py
--rw-r--r--   0 runner    (1001) docker     (121)    55941 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesParse.py
--rw-r--r--   0 runner    (1001) docker     (121)    31204 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesPlot.py
--rw-r--r--   0 runner    (1001) docker     (121)    53012 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesPlot2.py
--rw-r--r--   0 runner    (1001) docker     (121)    32648 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesRandom.py
--rw-r--r--   0 runner    (1001) docker     (121)    30871 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesSBML.py
--rw-r--r--   0 runner    (1001) docker     (121)    18256 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesSED.py
--rw-r--r--   0 runner    (1001) docker     (121)    20294 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesScan.py
--rw-r--r--   0 runner    (1001) docker     (121)    56644 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesStoich.py
--rw-r--r--   0 runner    (1001) docker     (121)    34243 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesTest.py
--rw-r--r--   0 runner    (1001) docker     (121)    12587 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesUtils.py
--rw-r--r--   0 runner    (1001) docker     (121)    14492 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/PyscesWeb.py
--rw-r--r--   0 runner    (1001) docker     (121)     2204 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)    57145 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/RateChar.py
--rw-r--r--   0 runner    (1001) docker     (121)    18277 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2250 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/_multicorescan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.391903 pysces-1.0.3/pysces/contrib/
--rw-r--r--   0 runner    (1001) docker     (121)     2593 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.391903 pysces-1.0.3/pysces/contrib/demo/
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/contrib/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/contrib/demo/demotest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.391903 pysces-1.0.3/pysces/core2/
--rw-r--r--   0 runner    (1001) docker     (121)    18572 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/core2/InfixParser.py
--rw-r--r--   0 runner    (1001) docker     (121)    54863 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/core2/PyscesCore2.py
--rw-r--r--   0 runner    (1001) docker     (121)    80362 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/core2/PyscesCore2Interfaces.py
--rw-r--r--   0 runner    (1001) docker     (121)    24562 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/core2/PyscesCore2Modules.py
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/core2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    42905 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/core2/lex.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/core2/version.py
--rw-r--r--   0 runner    (1001) docker     (121)   137736 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/core2/yacc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.391903 pysces-1.0.3/pysces/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/docs/DOCS.txt
--rw-r--r--   0 runner    (1001) docker     (121)    26145 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/docs/HISTORY.txt
--rw-r--r--   0 runner    (1001) docker     (121)   468326 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/docs/userguide.pdf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.395903 pysces-1.0.3/pysces/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     4105 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/examples/benchmark.ipy
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/examples/parallelscan.ipy
--rw-r--r--   0 runner    (1001) docker     (121)     4553 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/examples/pysces_stochpy.py
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/examples/testRunScatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2949 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/examples/testinvalidstate.py
--rw-r--r--   0 runner    (1001) docker     (121)     2944 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/examples/testparscanner.py
--rw-r--r--   0 runner    (1001) docker     (121)     3277 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/examples/testratechar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.395903 pysces-1.0.3/pysces/kraken/
--rw-r--r--   0 runner    (1001) docker     (121)    15458 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/kraken/Kraken.py
--rw-r--r--   0 runner    (1001) docker     (121)     6758 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/kraken/KrakenDataTools.py
--rw-r--r--   0 runner    (1001) docker     (121)    14998 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/kraken/KrakenNET.py
--rw-r--r--   0 runner    (1001) docker     (121)    11029 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/kraken/KrakenServer.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/kraken/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.395903 pysces-1.0.3/pysces/kraken/controllers/
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/kraken/controllers/kill_tentacles.py
--rw-r--r--   0 runner    (1001) docker     (121)     5975 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/kraken/controllers/kraken_continuation.py
--rw-r--r--   0 runner    (1001) docker     (121)    11564 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/kraken/controllers/kraken_continuation_eigen.py
--rw-r--r--   0 runner    (1001) docker     (121)     5040 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/kraken/controllers/kraken_continuation_eigen2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3304 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/kraken/controllers/kraken_intersect.py
--rw-r--r--   0 runner    (1001) docker     (121)    13710 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/kraken/controllers/kraken_scanner2.py
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/kraken/server_list
--rw-r--r--   0 runner    (1001) docker     (121)     3491 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/kraken/startup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.395903 pysces-1.0.3/pysces/lib/
--rw-r--r--   0 runner    (1001) docker     (121)     9861 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/lib/FirstDerivatives.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    42905 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/lib/lex.py
--rw-r--r--   0 runner    (1001) docker     (121)   124351 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/lib/miriamids.py
--rw-r--r--   0 runner    (1001) docker     (121)   151642 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/lib/pyparsing.py
--rw-r--r--   0 runner    (1001) docker     (121)   137736 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/lib/yacc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.395903 pysces-1.0.3/pysces/metatool/
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/metatool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.399903 pysces-1.0.3/pysces/nleq2/
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/nleq2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/nleq2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18561 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/nleq2/linalg_nleq2.f
--rw-r--r--   0 runner    (1001) docker     (121)    55672 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/nleq2/nleq2-4.3.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)   127885 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/nleq2/nleq2.f
--rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/nleq2/nleq2.pyf
--rw-r--r--   0 runner    (1001) docker     (121)     5594 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/nleq2/nleq2_readme.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5594 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/nleq2/readme
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/nleq2/readme.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/nleq2/wnorm.f
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/nleq2/zibconst.f
--rw-r--r--   0 runner    (1001) docker     (121)    10975 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/nleq2/zibmon.f
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/nleq2/zibsec.f
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.399903 pysces-1.0.3/pysces/pitcon/
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/pitcon/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/pitcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   132416 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/pitcon/dpcon61.f
--rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/pitcon/dpcon61w.f
--rw-r--r--   0 runner    (1001) docker     (121)    30665 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/pitcon/pcon61subd.f
--rw-r--r--   0 runner    (1001) docker     (121)     2898 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/pitcon/pitcon.pyf
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/pitcon/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.399903 pysces-1.0.3/pysces/pscmodels/
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/pscmodels/Burstmodel.psc
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/pscmodels/isola2a.psc
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/pscmodels/lin5_hill.psc
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/pscmodels/noisy_lin4.psc.txt
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/pscmodels/pysces_test_branch1.psc
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/pscmodels/pysces_test_linear1.psc
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/pscmodels/pysces_test_moiety1.psc
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/pscmodels/pysces_test_pitcon.psc
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-09-18 19:38:16.000000 pysces-1.0.3/pysces/pyscfg.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.399903 pysces-1.0.3/pysces/sandbox/
--rw-r--r--   0 runner    (1001) docker     (121)    12084 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/sandbox/Intersect.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/sandbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.399903 pysces-1.0.3/pysces/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/version.py
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-18 19:38:13.000000 pysces-1.0.3/pysces/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-18 19:38:16.391903 pysces-1.0.3/pysces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-09-18 19:38:16.000000 pysces-1.0.3/pysces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3100 2022-09-18 19:38:16.000000 pysces-1.0.3/pysces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-18 19:38:16.000000 pysces-1.0.3/pysces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-18 19:38:16.000000 pysces-1.0.3/pysces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-09-18 19:38:16.000000 pysces-1.0.3/pysces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-18 19:38:16.000000 pysces-1.0.3/pysces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-18 19:38:13.000000 pysces-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-18 19:38:16.399903 pysces-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     8182 2022-09-18 19:38:13.000000 pysces-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.458885 pysces-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-19 11:19:27.000000 pysces-1.1.0/ADDITIONAL_LICENCES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-04-19 11:19:27.000000 pysces-1.1.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-19 11:19:27.000000 pysces-1.1.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-19 11:19:27.000000 pysces-1.1.0/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-19 11:19:27.000000 pysces-1.1.0/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-19 11:19:27.000000 pysces-1.1.0/LATEST.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-19 11:19:27.000000 pysces-1.1.0/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-19 11:19:27.000000 pysces-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-19 11:19:27.000000 pysces-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-19 11:19:30.458885 pysces-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-04-19 11:19:27.000000 pysces-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-19 11:19:27.000000 pysces-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.450885 pysces-1.1.0/pysces/
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesContrib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesContribUser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesInterfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32019 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesJWSParse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53189 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesLink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19980 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesMiniModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)   349989 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesModelMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesParScan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57192 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesParse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31204 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53012 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesPlot2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32648 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesRandom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30871 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesSBML.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesSED.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20294 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesScan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56341 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesStoich.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34243 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/PyscesWeb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    57145 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/RateChar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18277 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/_multicorescan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.450885 pysces-1.1.0/pysces/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.450885 pysces-1.1.0/pysces/contrib/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/contrib/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/contrib/demo/demotest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.450885 pysces-1.1.0/pysces/core2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18572 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/core2/InfixParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55235 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/core2/PyscesCore2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81721 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/core2/PyscesCore2Interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24562 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/core2/PyscesCore2Modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/core2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42905 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/core2/lex.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/core2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137736 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/core2/yacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.450885 pysces-1.1.0/pysces/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/docs/DOCS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26145 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/docs/HISTORY.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   488229 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/docs/userguide.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.454885 pysces-1.1.0/pysces/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/examples/benchmark.ipy
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/examples/parallelscan.ipy
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/examples/pysces_stochpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/examples/testRunScatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/examples/testinvalidstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/examples/testparscanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/examples/testratechar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.454885 pysces-1.1.0/pysces/kraken/
+-rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/Kraken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/KrakenDataTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14998 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/KrakenNET.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/KrakenServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.454885 pysces-1.1.0/pysces/kraken/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/controllers/kill_tentacles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/controllers/kraken_continuation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/controllers/kraken_continuation_eigen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/controllers/kraken_continuation_eigen2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/controllers/kraken_intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/controllers/kraken_scanner2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/server_list
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/kraken/startup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.454885 pysces-1.1.0/pysces/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/lib/FirstDerivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42905 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/lib/lex.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124351 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/lib/miriamids.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151642 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/lib/pyparsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137736 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/lib/yacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.454885 pysces-1.1.0/pysces/metatool/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/metatool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.458885 pysces-1.1.0/pysces/nleq2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18561 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/linalg_nleq2.f
+-rw-r--r--   0 runner    (1001) docker     (123)    55672 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/nleq2-4.3.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   127885 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/nleq2.f
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/nleq2.pyf
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/nleq2_readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/readme
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/wnorm.f
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/zibconst.f
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/zibmon.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/nleq2/zibsec.f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.458885 pysces-1.1.0/pysces/pitcon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pitcon/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pitcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132416 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pitcon/dpcon61.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pitcon/dpcon61w.f
+-rw-r--r--   0 runner    (1001) docker     (123)    30665 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pitcon/pcon61subd.f
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pitcon/pitcon.pyf
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pitcon/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.458885 pysces-1.1.0/pysces/pscmodels/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pscmodels/Burstmodel.psc
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pscmodels/isola2a.psc
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pscmodels/lin5_hill.psc
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pscmodels/noisy_lin4.psc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pscmodels/pysces_test_branch1.psc
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pscmodels/pysces_test_linear1.psc
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pscmodels/pysces_test_moiety1.psc
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/pscmodels/pysces_test_pitcon.psc
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-19 11:19:30.000000 pysces-1.1.0/pysces/pyscfg.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.458885 pysces-1.1.0/pysces/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/sandbox/Intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/sandbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.458885 pysces-1.1.0/pysces/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 11:19:27.000000 pysces-1.1.0/pysces/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:19:30.450885 pysces-1.1.0/pysces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-19 11:19:30.000000 pysces-1.1.0/pysces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-19 11:19:30.000000 pysces-1.1.0/pysces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:19:30.000000 pysces-1.1.0/pysces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:19:30.000000 pysces-1.1.0/pysces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-19 11:19:30.000000 pysces-1.1.0/pysces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 11:19:30.000000 pysces-1.1.0/pysces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 11:19:27.000000 pysces-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 11:19:30.458885 pysces-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-04-19 11:19:27.000000 pysces-1.1.0/setup.py
```

### Comparing `pysces-1.0.3/ADDITIONAL_LICENCES.md` & `pysces-1.1.0/ADDITIONAL_LICENCES.md`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/CONTRIBUTORS.md` & `pysces-1.1.0/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/INSTALL.md` & `pysces-1.1.0/INSTALL.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 * Download and install 
   [Anaconda for Python 3](https://www.anaconda.com/products/individual#Downloads)
 * Obtain [Git for Windows](https://git-scm.com/download/win)
 * Create a PySCeS environment using conda and activate it:
 
 ```bash
 $ conda create -n pyscesdev -c conda-forge python=3.8 numpy scipy \ 
-  matplotlib sympy packaging pip wheel nose ipython python-libsbml \
+  matplotlib sympy packaging pip wheel ipython python-libsbml \
   fortran-compiler assimulo scikit-build
 $ conda activate pyscesdev
 ```
 
 * Clone and enter the PySCeS code repository using git
 
 ```bash
```

### Comparing `pysces-1.0.3/LATEST.md` & `pysces-1.1.0/LATEST.md`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/LICENCE.txt` & `pysces-1.1.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/LICENSE` & `pysces-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/MANIFEST.in` & `pysces-1.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/PKG-INFO` & `pysces-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysces
-Version: 1.0.3
+Version: 1.1.0
 Summary: The Python Simulator for Cellular Systems - simulation and analysis tools for modelling biological systems
 Home-page: http://pysces.sourceforge.net
 Download-URL: https://pypi.org/project/pysces/#files
 Author: Brett G. Olivier and Johann M. Rohwer
 Author-email: pysces@googlegroups.com
 Maintainer: Brett G. Olivier and Johann M. Rohwer
 Maintainer-email: pysces@googlegroups.com
```

### Comparing `pysces-1.0.3/README.md` & `pysces-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -131,8 +131,8 @@
 This information can also be found in [CONTRIBUTORS.md](./CONTRIBUTORS.md)
 In addition we would like to acknowledge financial support from the following funding
 organisations:
 
 * The South African National Bioinformatics Network (2003-2008)
 * The South African National Research Foundation (2000-2004)
 
-© Brett G. Olivier & Johann M. Rohwer, August 2021
+© Brett G. Olivier & Johann M. Rohwer, April 2023
```

### Comparing `pysces-1.0.3/pysces/PyscesConfig.py` & `pysces-1.1.0/pysces/PyscesConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/PyscesContrib.py` & `pysces-1.1.0/pysces/PyscesContrib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/PyscesContribUser.py` & `pysces-1.1.0/pysces/PyscesContribUser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/PyscesInterfaces.py` & `pysces-1.1.0/pysces/PyscesInterfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
@@ -44,16 +44,16 @@
     """
 
     core = None
     sbml = None
     core2sbml = None
     core2psc = None
     sbml2core = None
-    sbml_level = 2
-    sbml_version = 1
+    sbml_level = 3
+    sbml_version = 2
 
     def __buildPscComponents__(self):
         """
         Builds the PSC file
         """
         self.core2psc.setHeader()
         self.core2psc.setFixed()
```

### Comparing `pysces-1.0.3/pysces/PyscesJWSParse.py` & `pysces-1.1.0/pysces/PyscesJWSParse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
@@ -28,17 +28,17 @@
     pass
 
 import os, copy
 from .lib import lex
 from .lib import yacc
 from getpass import getuser
 from time import sleep, strftime
-from numpy import MachAr
+from numpy import finfo
 
-MyMachArr = MachAr()
+mach_eps = finfo(float).eps
 
 
 class JWSParser:
     """JWSParser written by Johann, based on Jannie's lexparse and integrated into PySCeS by brett  -- converts PySCeS (.psc) files to JWS Online (jws) files"""
 
     ReactionIDs = []  # List of reaction names
     Names = []  # List of all reagent, parameter and function names
@@ -52,15 +52,14 @@
     Reagents = []  # All reagents found during parsing of reactions
     VarReagents = []  # Variable reagents that occur in reactions
     FixedReagents = []  # Fixed reagents
     ReacParams = []  # Temporary list of reaction parameters
     InitParams = []  # Initialised parameters
     ParseErrors = []
 
-    mach_spec = MyMachArr
     AllRateEqsGiven = 1  # Flag to check that all rate equations have been given
     Debug = 0
 
     ##############
     # Build the lexer
     ##############
 
@@ -287,15 +286,15 @@
                 ]  # Key for reagent with stoichcoef value
         killList = []
         # brett: however for the case of X + Y > Y + Z where the sum of the coefficients
         # is zero we can delete the key (Y) out of the reaction list altgether (hopefully!)
         for i in self.NetworkDict[ReacID]['Reagents']:
             if (
                 abs(self.NetworkDict[ReacID]['Reagents'][i])
-                < self.mach_spec.eps * 100.0
+                < mach_eps * 100.0
             ):
                 killList.append(i)
                 # print self.mach_spec.eps*100.0, self.NetworkDict[ReacID]['Reagents']
         # print killList, self.NetworkDict[ReacID]['Reagents']
         # brett: and the easiest way of doing this is putting the zero keys in a list
         # and deleting them out of the dictionary
         if len(killList) != 0:
```

### Comparing `pysces-1.0.3/pysces/PyscesLink.py` & `pysces-1.1.0/pysces/PyscesLink.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/PyscesMiniModel.py` & `pysces-1.1.0/pysces/PyscesMiniModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
@@ -29,18 +29,17 @@
 except NameError:
     pass
 import os, copy, time
 import numpy
 from pysces import PyscesStoich
 from pysces import PyscesParse
 
-mach_spec = numpy.MachAr()
+mach_eps = numpy.finfo(float).eps
 pscParser = PyscesParse.PySCeSParser(debug=0)
 
-
 class PyscesInputFileParser(object):
     """
     This class contains the PySCeS model loading and Stoichiometric Analysis methods
     """
 
     ModelDir = None
     ModelFile = None
@@ -53,15 +52,15 @@
         self.ModelFile = model_file
         if output_dir == None:
             self.ModelOutput = os.getcwd()
         else:
             assert os.path.exists(output_dir), "\n%s is not a valid path" % output_dir
         self.__settings__ = {}
         # Initialize stoichiometric precision
-        self.__settings__['stoichiometric_analysis_fp_zero'] = mach_spec.eps * 2.0e4
+        self.__settings__['stoichiometric_analysis_fp_zero'] = mach_eps * 2.0e4
         self.__settings__['stoichiometric_analysis_lu_precision'] = self.__settings__[
             'stoichiometric_analysis_fp_zero'
         ]
         self.__settings__['stoichiometric_analysis_gj_precision'] = (
             self.__settings__['stoichiometric_analysis_lu_precision'] * 10.0
         )
         self.__settings__['enable_deprecated_attr'] = False
@@ -338,29 +337,29 @@
                 '\nWARNING: values in L0matrix are close to stoichiometric precision!'
             )
             print(
                 'Stoichiometric LU precision:',
                 self.__structural__.stoichiometric_analysis_lu_precision,
             )
             print('L0 smallest abs(value)', abs(lsmall))
-            print('Machine precision:', mach_spec.eps)
+            print('Machine precision:', mach_eps)
             SmallValueError = 1
         if (
             abs(ksmall)
             < self.__structural__.stoichiometric_analysis_lu_precision * 10.0
         ):
             print(
                 '\nWARNING: values in K0matrix are close to stoichiometric precision!'
             )
             print(
                 'Stoichiometric precision:',
                 self.__structural__.stoichiometric_analysis_lu_precision,
             )
             print('K0 smallest abs(value)', abs(ksmall))
-            print('Machine precision:', mach_spec.eps)
+            print('Machine precision:', mach_eps)
             SmallValueError = 1
         if SmallValueError:
             input(
                 '\nStructural Analysis results may not be reliable!!!.\n\nTry change <mod>.__settings__["stoichiometric_analysis_lu_precision"] (see reference manual for details)\n\n\t press any key to continue: '
             )
 
         # cross check that rank is consistant between K0 and L0
```

### Comparing `pysces-1.0.3/pysces/PyscesModel.py` & `pysces-1.1.0/pysces/PyscesModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
@@ -32,24 +32,22 @@
             create the model and associated data objects
 
             '''
 import os, copy, gc, time
 import math, operator, re
 import pprint, pickle, io
 import warnings
-
 try:
     input = raw_input  # Py2 compatibility
 except NameError:
     pass
 import numpy
 import scipy
 import scipy.linalg
 import scipy.integrate
-
 ScipyDerivative = None
 HAVE_SCIPY_DERIV = False
 try:
     ScipyDerivative = scipy.derivative
     HAVE_SCIPY_DERIV = True
 except AttributeError:
     try:
@@ -66,14 +64,15 @@
 
 from . import model_dir as MODEL_DIR
 from . import output_dir as OUTPUT_DIR
 from . import install_dir as INSTALL_DIR
 from . import PyscesRandom as random
 from .PyscesScan import Scanner
 from .core2.InfixParser import MyInfixParser
+from .core2.PyscesCore2 import NewCoreBase, NumberBase
 
 from . import (
     nleq2,
     nleq2_switch,
     pitcon,
     plt,
     gplt,
@@ -93,15 +92,15 @@
 
 # this is incredibly crude but effectively masks off unsupported random functions
 del (
     random.setstate,
     random.getstate,
 )  # random.division,
 del random.randrange, random.Random, random.choice
-del random.sample, random.shuffle, random.jumpahead
+del random.shuffle, random.jumpahead   # random.sample
 del random.SystemRandom, random.WichmannHill, random.triangular
 # used by functions random.NV_MAGICCONST, random.SG_MAGICCONST, random.BPF, random.RECIP_BPF
 
 
 # Scipy version check
 if (
     int(scipy.__version__.split('.')[0]) < 1
@@ -159,50 +158,77 @@
             if self.mod.__HAS_RATE_RULES__:
                 self.mod.ExecRateRules()
             return eout
 
         def handle_event(self, solver, event_info):
             self.event_times.append(solver.t)
             state_info = event_info[0]
-            idx = state_info.index(-1)
-            ev = self.events[idx]
-            if ev._assign_now:
-                for ass in ev.assignments:
-                    if ass.variable in self.mod.L0matrix.getLabels()[1] or (
-                        self.mod.mode_integrate_all_odes
-                        and ass.variable in self.mod.__species__
-                    ):
-                        assVal = ass.getValue()
-                        assIdx = self.mod.__species__.index(ass.variable)
-                        if self.mod.__KeyWords__["Species_In_Conc"]:
-                            solver.y[assIdx] = assVal * getattr(
-                                self.mod, self.mod.__CsizeAllIdx__[assIdx]
+            state_info = numpy.array(state_info)
+            idx = numpy.where(state_info == -1)
+            event_list = [self.events[j] for j in idx[0]]
+            sequence = self.setSequence(event_list)
+            for ev in sequence:
+                if ev._assign_now:
+                    print('executing', ev.name)
+                    for ass in ev.assignments:
+                        ass.evaluateAssignment()
+                        if ass.variable in self.mod.L0matrix.getLabels()[1] or (
+                            self.mod.mode_integrate_all_odes
+                            and ass.variable in self.mod.__species__
+                        ):
+                            assVal = ass.getValue()
+                            assIdx = self.mod.__species__.index(ass.variable)
+                            if self.mod.__KeyWords__["Species_In_Conc"]:
+                                solver.y[assIdx] = assVal * getattr(
+                                    self.mod, self.mod.__CsizeAllIdx__[assIdx]
+                                )
+                                setattr(self.mod, ass.variable, assVal * getattr(
+                                    self.mod, self.mod.__CsizeAllIdx__[assIdx]))
+                            else:
+                                solver.y[assIdx] = assVal
+                                setattr(self.mod, ass.variable, assVal)
+                        elif (
+                            not self.mod.mode_integrate_all_odes
+                            and ass.variable in self.mod.L0matrix.getLabels()[0]
+                        ):
+                            print(
+                                'Event assignment to dependent species consider setting "mod.mode_integrate_all_odes = True"'
                             )
+                            setattr(self.mod, ass.variable, ass.value)
+                        elif (
+                            self.mod.__HAS_RATE_RULES__ and ass.variable in self.mod.__rate_rules__
+                        ):
+                            assVal = ass.getValue()
+                            rrIdx = self.mod.__rate_rules__.index(ass.variable)
+                            self.mod.__rrule__[rrIdx] = assVal
+                            solver.y[self.mod.L0matrix.shape[1] + rrIdx] = assVal
+                            setattr(self.mod, ass.variable, assVal)
                         else:
-                            solver.y[assIdx] = assVal
-                    elif (
-                        not self.mod.mode_integrate_all_odes
-                        and ass.variable in self.mod.L0matrix.getLabels()[0]
-                    ):
-                        print(
-                            'Event assignment to dependent species consider setting "mod.mode_integrate_all_odes = True"'
-                        )
-                    elif (
-                        self.mod.__HAS_RATE_RULES__ and ass.variable in self.mod.__rate_rules__
-                    ):
-                        assVal = ass.getValue()
-                        rrIdx = self.mod.__rate_rules__.index(ass.variable)
-                        self.mod.__rrule__[rrIdx] = assVal
-                        solver.y[self.mod.L0matrix.shape[1] + rrIdx] = assVal
-                        setattr(self.mod, ass.variable, assVal)
-                    else:
-                        ass()
-            # track any parameter changes
-            self.parvals.append([getattr(self.mod, p) for p in self.mod.parameters])
+                            ass()
+                            setattr(self.mod, ass.variable, ass.value)
+                # track any parameter changes
+                self.parvals.append([getattr(self.mod, p) for p in self.mod.parameters])
+
+        def setSequence(self, event_list):
+            no_prio = [ev for ev in event_list if ev.priority is None]
+            prio = [ev for ev in event_list if ev.priority is not None]
+
+            random_prio_sample = random.sample(prio, len(prio))
+            prio_sorted = sorted(random_prio_sample, reverse=True, key=lambda x: x.priority)
+
+            if not no_prio:
+                sequence = prio_sorted
+            elif not prio_sorted:
+                sequence = random.sample(no_prio, len(no_prio))
+            else:
+                sequence = prio_sorted
+                for i in no_prio:
+                    sequence.insert(random.randint(0, len(prio_sorted)), i)
 
+            return sequence
 
 # for future fun
 _HAVE_VPYTHON = False
 _VPYTHON_LOAD_ERROR = ''
 __psyco_active__ = 0
 '''
 try:
@@ -222,15 +248,15 @@
     psyco.profile()
     __psyco_active__ = 1
     print('PySCeS Model module is now PsycoActive!')
 except:
     __psyco_active__ = 0
 '''
 # machine specs
-mach_spec = numpy.MachAr()
+mach_eps = numpy.finfo(float).eps
 # grab a parser
 pscParser = PyscesParse.PySCeSParser(debug=0)
 
 
 def chkpsc(File):
     """
     chkpsc(File)
@@ -1064,58 +1090,18 @@
                 )
         if not lbls:
             return output
         else:
             return output, lout
 
 
-# this must stay in sync with core2
-class NewCoreBase(object):
-    """
-    Core2 base class, needed here as we use Core2 derived classes
-    in PySCes
-    """
-
-    name = None
-    __DEBUG__ = False
-
-    def getName(self):
-        return self.name
-
-    def setName(self, name):
-        self.name = name
-
-    def get(self, attr):
-        """Return an attribute whose name is str(attr)"""
-        return self.__getattribute__(attr)
-
-
-# this must stay in sync with core2
-class NumberBase(NewCoreBase):
-    """
-    Derived Core2 number class.
-    """
-
-    value = None
-    value_initial = None
-
-    def __call__(self):
-        return self.value
-
-    def getValue(self):
-        return self.value
-
-    def setValue(self, v):
-        self.value = v
-
-
 # Finally killed my lambda functions - brett07
 class ReactionObj(NewCoreBase):
     """
-    Defines a reaction with a KineticLaw *kl8, *formula* and *name* bound
+    Defines a reaction with a KineticLaw *kl*, *formula* and *name* bound
     to a model instance, *mod*.
     """
 
     formula = None
     mod = None
     rate = None
     xcode = None
@@ -1276,44 +1262,52 @@
     _ASS_TIME_ = 0.0
     _need_action = False
     _assign_now = False
     symbols = None
     _time_symbol = None
     piecewises = None
     mod = None
+    priority = None
+    persistent = True
     __DEBUG__ = True
 
     def __init__(self, name, mod):
         self.setName(name)
         self.assignments = []
         self.mod = mod
 
     def __call__(self, time):
         self._TIME_ = time
         exec(self.xcode)
         ret = False
         if self.state0 and not self.state:
             self.state0 = self.state
         if not self.state0 and self.state:
-            for ass in self.assignments:
-                ass.evaluateAssignment()
             self.state0 = self.state
             self._need_action = True
             self._ASS_TIME_ = time + self.delay
             if self.__DEBUG__:
                 print('\nevent {} is evaluating at {}'.format(self.name, time))
             ret = True
         if self._need_action and self._TIME_ >= self._ASS_TIME_:
-            self._assign_now = True
-            if self.__DEBUG__:
-                print(
-                    'event {} is assigning at {} (delay={})'.format(
-                        self.name, time, self.delay
+            if not self.persistent and not self.state:
+                self._assign_now = False
+                if self.__DEBUG__:
+                    print('event {} NOT assigning after delay...'.format(self.name))
+                    print(
+                        '    ...non-persistent event, trigger ({}) no longer valid'.format(self.formula)
+                    )
+            else:
+                self._assign_now = True
+                if self.__DEBUG__:
+                    print(
+                        'event {} is assigning at {} (delay={})'.format(
+                            self.name, time, self.delay
+                        )
                     )
-                )
             self._need_action = False
             ret = True
         return ret
 
     def setTrigger(self, formula, delay=0.0):
         self.formula = formula
         self.delay = delay
@@ -1331,14 +1325,20 @@
     def setAssignment(self, var, formula):
         ass = EventAssignment(var, mod=self.mod)
         ass.setVariable(var)
         ass.setFormula(formula)
         self.assignments.append(ass)
         self.__setattr__('_' + var, ass)
 
+    def setPriority(self, priority):
+        self.priority = priority
+
+    def setPersistent(self, persistent):
+        self.persistent = persistent
+
     def reset(self):
         self.state0 = False
         self.state = False
         self._TIME_ = 0.0
         self._ASS_TIME_ = 0.0
 
 
@@ -1567,15 +1567,15 @@
             )
         self.__settings__['display_debug'] = 0
         self.ModelOutput = OUTPUT_DIR
 
         # Initialize serial directory
         self.__settings__['serial_dir'] = os.path.join(self.ModelOutput, 'pscdat')
         # Initialize stoichiometric precision
-        self.__settings__['stoichiometric_analysis_fp_zero'] = mach_spec.eps * 2.0e4
+        self.__settings__['stoichiometric_analysis_fp_zero'] = mach_eps * 2.0e4
         self.__settings__['stoichiometric_analysis_lu_precision'] = self.__settings__[
             'stoichiometric_analysis_fp_zero'
         ]
         self.__settings__['stoichiometric_analysis_gj_precision'] = (
             self.__settings__['stoichiometric_analysis_lu_precision'] * 10.0
         )
 
@@ -1691,15 +1691,15 @@
         ##  self.eModeExe_int = os.path.join(self.__metatool,'meta43_int')
         ##  self.eModeExe_dbl = os.path.join(self.__metatool,'meta43_double')
         ##  print 'Done.'
 
         # Initialize serial directory
         self.__settings__['serial_dir'] = os.path.join(self.ModelOutput, 'pscdat')
         # Initialize stoichiometric precision
-        self.__settings__['stoichiometric_analysis_fp_zero'] = mach_spec.eps * 2.0e4
+        self.__settings__['stoichiometric_analysis_fp_zero'] = mach_eps * 2.0e4
         self.__settings__['stoichiometric_analysis_lu_precision'] = self.__settings__[
             'stoichiometric_analysis_fp_zero'
         ]
         self.__settings__['stoichiometric_analysis_gj_precision'] = (
             self.__settings__['stoichiometric_analysis_lu_precision'] * 10.0
         )
 
@@ -2251,29 +2251,29 @@
                 '\nWARNING: values in L0matrix are close to stoichiometric precision!'
             )
             print(
                 'Stoichiometric LU precision:',
                 self.__structural__.stoichiometric_analysis_lu_precision,
             )
             print('L0 smallest abs(value)', abs(lsmall))
-            print('Machine precision:', mach_spec.eps)
+            print('Machine precision:', mach_eps)
             SmallValueError = 1
         if (
             abs(ksmall)
             < self.__structural__.stoichiometric_analysis_lu_precision * 10.0
         ):
             print(
                 '\nWARNING: values in K0matrix are close to stoichiometric precision!'
             )
             print(
                 'Stoichiometric precision:',
                 self.__structural__.stoichiometric_analysis_lu_precision,
             )
             print('K0 smallest abs(value)', abs(ksmall))
-            print('Machine precision:', mach_spec.eps)
+            print('Machine precision:', mach_eps)
             SmallValueError = 1
         if SmallValueError:
             input(
                 '\nStructural Analysis results may not be reliable!!!.\n\nTry change <mod>.__settings__["stoichiometric_analysis_lu_precision"] (see reference manual for details)\n\n\t press any key to continue: '
             )
 
         # cross check that rank is consistant between K0 and L0
@@ -2732,14 +2732,16 @@
         self.__settings__['cvode_return_event_timepoints'] = True
         self.__events__ = []
         # for each event
         for e in self.__eDict__:
             ev = Event(e, self)
             ev._time_symbol = self.__eDict__[e]['tsymb']
             ev.setTrigger(self.__eDict__[e]['trigger'], self.__eDict__[e]['delay'])
+            ev.setPriority(self.__eDict__[e]['priority'])
+            ev.setPersistent(self.__eDict__[e]['persistent'])
             # for each assignment
             for ass in self.__eDict__[e]['assignments']:
                 ev.setAssignment(ass, self.__eDict__[e]['assignments'][ass])
             self.__events__.append(ev)
             setattr(self, ev.name, ev)
         if len(self.__events__) > 0:
             self.__HAS_EVENTS__ = True
@@ -2795,15 +2797,15 @@
         self.__mapFunc__ = compile(mapString, 'mapString', 'exec')
         self.__mapFunc_R__ = compile(mapString_R, 'mapString_R', 'exec')
         self.__vFunc__ = compile(vString, 'vString', 'exec')
         ##  exec(lambdaFuncsC)
 
         # Machine specific values (for IEEE compliant FP machines this is around 2.e-16)
         # FutureNote: investigate arbitrary precision FP in Python, probably GNU-GMP based - brett 20040326
-        self.__settings__['mach_floateps'] = mach_spec.eps
+        self.__settings__['mach_floateps'] = mach_eps
 
         # PySCeS mode switches
         # this affects number output formatting in PySCeS)
         self.__settings__['mode_number_format'] = '%2.4e'
         # 0:initval, 1:zeroval, 2:lastss 3:sim_res[-1]
         self.__settings__['mode_sim_init'] = 0
         # maximum number of auto-stepsize adjustments
@@ -3021,14 +3023,16 @@
         self.__settings__["cvode_stats"] = False
         # the step size to be attempted on the first step.
         self.__settings__["cvode_h0"] = 0.0
         self.__settings__["cvode_hmax"] = 0.0  # the maximum absolute step size allowed.
         self.__settings__["cvode_hmin"] = 0.0  # the minimum absolute step size allowed.
         # maximum order to be used by the solver
         self.__settings__["cvode_mxord"] = 5
+        # Option not to add cvode solver class to model after simulation as cython objects prevent serialization
+        self.__settings__["cvode_access_solver"] = True
 
         if self.__HAS_PIECEWISE__ and self.__settings__["cvode_reltol"] <= 1.0e-9:
             self.__settings__["cvode_reltol"] = 1.0e-6
             print(
                 'INFO: Piecewise functions detected increasing CVODE tolerance slightly\n\
 (mod.__settings__[\"cvode_reltol\"] = 1.0e-6 ).'
             )
@@ -3860,15 +3864,16 @@
             del out
 
         problem = EventsProblem(self, rhs=rhs, y0=initial)
         # for direct access to the problem class
         self._problem = problem
         sim = CVode(problem)
         # for direct access to the solver class
-        self._solver = sim
+        if self.__settings__["cvode_access_solver"]:
+            self._solver = sim
 
         # initialise CVODE settings
         if self.__settings__["cvode_stats"]:
             sim.verbosity = 10
         else:
             sim.verbosity = 40
         sim.atol = self.__settings__["cvode_abstol"]
@@ -4195,15 +4200,15 @@
 
         if self.__settings__['nleq2_jacgen'] == 1:
             print(
                 '(nleq2)User supplied Jacobian not supported yet ... setting __settings__[\'nleq2_jacgen\'] = 0'
             )
             self.__settings__['nleq2_jacgen'] = 0
 
-        rtol = mach_spec.eps * 10.0 * N
+        rtol = mach_eps * 10.0 * N
         iopt[2] = self.__settings__['nleq2_jacgen']  # 2
         iopt[8] = self.__settings__['nleq2_iscaln']  # 0
         iopt[10] = 0
         iopt[11] = 6
         iopt[12] = 0
         iopt[13] = 6
         iopt[14] = 0
@@ -8697,15 +8702,15 @@
                 + ') '
                 + time.strftime("%a, %d %b %Y %H:%M:%S")
             )
         else:
             plt.setGraphTitle(title)
         plt.replot()
         if filename != None:
-            plt.export(filename, directory=self.ModelOutput, type='png')
+            plt.export(filename, directory=self.ModelOutput, outtype='png')
 
     def Scan1(self, range1=[], runUF=0):
         """
         Scan1(range1=[],runUF=0)
 
         Perform a single dimension parameter scan using the steady-state solvers. The parameter to be scanned is defined (as a model attribute "P") in mod.scan_in while the required output is entered into the list mod.scan_out.
         Results of a parameter scan can be easilly viewed with Scan1Plot().
@@ -8989,15 +8994,15 @@
                 + ') '
                 + time.strftime("%a, %d %b %Y %H:%M:%S")
             )
         else:
             plt.setGraphTitle(title)
         plt.replot()
         if filename != None:
-            plt.export(filename, directory=self.ModelOutput, type='png')
+            plt.export(filename, directory=self.ModelOutput, outtype='png')
 
     def Scan2D(self, p1, p2, output, log=False):
         """
         Generate a 2 dimensional parameter scan using the steady-state solvers.
 
         - *p1* is a list of [parameter1, start, end, points]
         - *p2* is a list of [parameter2, start, end, points]
@@ -9049,15 +9054,15 @@
                 + ') '
                 + time.strftime("4a, %d %b %Y %H:%M:%S")
             )
         else:
             plt.setGraphTitle(title)
         plt.replot()
         if filename != None:
-            plt.export(filename, directory=self.ModelOutput, type='png')
+            plt.export(filename, directory=self.ModelOutput, outtype='png')
 
     def SetQuiet(self):
         """
         SetQuiet()
 
         Turn off as much solver reporting noise as possible:
         mod.__settings__['hybrd_mesg'] = 0
```

### Comparing `pysces-1.0.3/pysces/PyscesModelMap.py` & `pysces-1.1.0/pysces/PyscesModelMap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/PyscesParScan.py` & `pysces-1.1.0/pysces/PyscesParScan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Johann Rohwer (jrohwer@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/PyscesParse.py` & `pysces-1.1.0/pysces/PyscesParse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
@@ -416,15 +416,15 @@
         self.cbm_ObjectiveFunctions = {}  # objective functions for a CB model
         self.cbm_UserFluxConstraints = {}  # objective functions for a CB model
 
         self.mach_spec_eps2k = 2.2204460492503131e-14
         self.AllRateEqsGiven = (
             1  # Flag to check that all rate equations have been given
         )
-        self.Debug = 0
+        self.Debug = False
 
         # elementary regular expressions used as building blocks
         self.Int = r'\d+'  # Integer
         self.Dec = self.Int + '\.' + self.Int  # Decimal
         self.Exp = r'([E|e][\+|\-]?)' + self.Int  # Exponent
         self.Real = (
             self.Dec + '(' + self.Exp + ')?' + '|' + self.Int + self.Exp
@@ -786,38 +786,73 @@
         )
         self.Show('RateRuleDec:', t[0])
 
     def p_eventdec(self, t):
         '''EventDec : EVENTDEC'''
         rawf = t[1].replace('Event:', '').lstrip()
         args = rawf[: rawf.find('{')].strip().split(',')
-        name = args.pop(0)
-        delay = float(args.pop(-1))
-        trigger = ''
-        for a in args:
-            trigger = trigger + a + ','
-        trigger = trigger[:-1]
+        posargs = args[:2] + [i for i in args[2:] if '=' not in i]
+        kwargs = [i.strip() for i in args[2:] if '=' in i]
 
-        rawF = rawf[rawf.find('{') + 1 : rawf.find('}')].split('\n')
-        assignments = {}
-        for ass in rawF:
-            if len(ass.strip()) > 0:
-                ass = ass.split('=')
-                assignments.update({ass[0].strip(): ass[1].strip()})
+        if len(posargs) > 3:
+            raise ValueError('invalid event syntax, see https://pyscesdocs.readthedocs.io/en/latest/inputfile_doc.html#events')
+        elif len(posargs) == 3:  # handle legacy delay
+            print(
+                '''deprecation warning: event delay should be specified with keyword,
+        see https://pyscesdocs.readthedocs.io/en/latest/inputfile_doc.html#events'''
+            )
+            delay = float(posargs[2])
+        else:
+            delay = 0.0
+
+        name = posargs[0].strip()
+        trigger = posargs[1].strip()
+
+        # default kwargs
         self.Events.update(
             {
                 name: {
-                    'delay': delay,
                     'name': name,
                     'trigger': trigger,
-                    'assignments': assignments,
+                    'delay': delay,
+                    'persistent': True,
+                    'priority': None,
                     'tsymb': None,
                 }
             }
         )
+
+        for arg in kwargs:
+            key, val = arg.split('=')
+            key = key.strip()
+            val = val.strip()
+            assert key in [
+                'delay',
+                'priority',
+                'persistent',
+            ], f'"{key}" is an invalid event attribute'
+            if key == 'delay':
+                val = float(val)
+            if key == 'priority':
+                if val == 'None':
+                    val = None
+                else:
+                    val = int(val)
+            if key == 'persistent':
+                val = eval(val)
+            self.Events[name][key] = val
+
+        rawF = rawf[rawf.find('{') + 1 : rawf.find('}')].split('\n')
+        assignments = {}
+        for ass in rawF:
+            if len(ass.strip()) > 0:
+                ass = ass.split('=')
+                assignments.update({ass[0].strip(): ass[1].strip()})
+        self.Events[name]['assignments'] = assignments
+
         self.Show('EventDec:', t[0])
 
     def p_objfuncdec(self, t):
         '''ObjFuncDec : OBJFUNCDEC'''
         rawf = t[1].replace('ObjectiveFunctions:', '').lstrip()
         args = rawf[: rawf.find('{')].strip().split(',')
         rawf = [
```

### Comparing `pysces-1.0.3/pysces/PyscesPlot.py` & `pysces-1.1.0/pysces/PyscesPlot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/PyscesPlot2.py` & `pysces-1.1.0/pysces/PyscesPlot2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/PyscesRandom.py` & `pysces-1.1.0/pysces/PyscesRandom.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/PyscesSBML.py` & `pysces-1.1.0/pysces/PyscesSBML.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/PyscesSED.py` & `pysces-1.1.0/pysces/PyscesSED.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/PyscesScan.py` & `pysces-1.1.0/pysces/PyscesScan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/PyscesStoich.py` & `pysces-1.1.0/pysces/PyscesStoich.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
@@ -43,19 +43,14 @@
           ------------
           PySCeS stoichiometric analysis classes.
 
           """
 
 ##  print 'Stoichiometry ver ' + __version__ + ' runtime: '+ time.strftime("%H:%M:%S")
 
-##stoich_zero_valM = scipy.machar.MachAr().eps*2.0e4 # safer --> about 4e-11 (unofficially - a minpivot size)
-##stoich_zero_valM = scipy.machar.MachAr().eps*2.0e4 # safe --> about 4e-12 (unofficially - a minpivot size)
-##print '\tStoichiometric precision = ', stoich_zero_valM
-
-
 class StructMatrix:
     """
     This class is specifically designed to store structural matrix information
     give it an array and row/col index permutations it can generate its own
     row/col labels given the label src.
     """
 
@@ -422,28 +417,27 @@
 
     __stoichdiagmode__ = 0
     __version__ = __version__
     __TimeFormat = "%H:%M:%S"
     USE_QR = False
     info_moiety_conserve = False
 
+    # Create a machine specific instance
+    from numpy import finfo
+    mach_eps = finfo(float).eps
+
     def __init__(self, input):
         """Initialize class variables"""
 
         self.nmatrix = input
         row, col = self.nmatrix.shape
         self.nmatrix_col = tuple(numpy.array(list(range(col))))
         self.nmatrix_row = tuple(numpy.array(list(range(row))))
 
-        # Create a machine specific instance
-        from numpy import MachAr
-
-        mach_spec = MachAr()
-
-        self.stoichiometric_analysis_fp_zero = mach_spec.eps * 2.0e4
+        self.stoichiometric_analysis_fp_zero = self.mach_eps * 2.0e4
         self.stoichiometric_analysis_lu_precision = self.stoichiometric_analysis_fp_zero
         self.stoichiometric_analysis_gj_precision = (
             self.stoichiometric_analysis_lu_precision * 10.0
         )
 
         self.species = None
         self.reactions = None
@@ -1426,15 +1420,15 @@
         TrMat = 0
         if ncol > nrow:
             # 'INFO: SVD is more accurate for tall matrices using (N)T\n'
             matrix = numpy.transpose(matrix)
             TrMat = 1
 
         u, s, vh = scipy.linalg.svd(matrix)
-        maskF = scipy.machar.machar_double.eps * factor
+        maskF = self.mach_eps * factor
 
         if TrMat == 0:
             print('SVD zero mask:', maskF)
             print(
                 'LU factorization effective zero:',
                 self.stoichiometric_analysis_lu_precision,
             )
```

### Comparing `pysces-1.0.3/pysces/PyscesTest.py` & `pysces-1.1.0/pysces/PyscesTest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/PyscesUtils.py` & `pysces-1.1.0/pysces/PyscesUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/PyscesWeb.py` & `pysces-1.1.0/pysces/PyscesWeb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/README.txt` & `pysces-1.1.0/pysces/README.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/RateChar.py` & `pysces-1.1.0/pysces/RateChar.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/__init__.py` & `pysces-1.1.0/pysces/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
 this distribution for specifics.
 
 NO WARRANTY IS EXPRESSED OR IMPLIED.  USE AT YOUR OWN RISK.
 
@@ -36,15 +36,15 @@
             Authors: Brett G. Olivier and Johann M. Rohwer (see CONTRIBUTORS.md for details)
 
             Permission to use, modify, and distribute this software is given under the
             terms of the PySceS (BSD style) license. See LICENSE.txt that came with
             this distribution for specifics.
 
             NO WARRANTY IS EXPRESSED OR IMPLIED.  USE AT YOUR OWN RISK.
-            Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+            Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
             """
 
 import os, time
 from pkg_resources import get_build_platform
 from . import PyscesConfig
 from . import PyscesParse
 from . import PyscesLink as link
@@ -512,15 +512,15 @@
     print(
         '* Welcome to PySCeS ('
         + __version__
         + ') - Python Simulator for Cellular Systems   *'
     )
     print('*                http://pysces.sourceforge.net                        *')
     ##  print '*                       Somewhere In Time                             *'
-    print('* Copyright(C) B.G. Olivier, J.M. Rohwer, J.-H.S. Hofmeyr, 2004-2022  *')
+    print('* Copyright(C) B.G. Olivier, J.M. Rohwer, J.-H.S. Hofmeyr, 2004-2023  *')
     print('* Triple-J Group for Molecular Cell Physiology                        *')
     print('* Stellenbosch University, ZA and VU University Amsterdam, NL         *')
     print('* PySCeS is distributed under the PySCeS (BSD style) licence, see     *')
     print('* LICENCE.txt (supplied with this release) for details                *')
     ##  print '*                 ** Read about PySCeS **                             *'
     print('* Please cite PySCeS with: doi:10.1093/bioinformatics/bti046          *')
     print('***********************************************************************')
```

### Comparing `pysces-1.0.3/pysces/_multicorescan.py` & `pysces-1.1.0/pysces/_multicorescan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Johann Rohwer (jrohwer@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/contrib/__init__.py` & `pysces-1.1.0/pysces/contrib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/contrib/demo/demotest.py` & `pysces-1.1.0/pysces/contrib/demo/demotest.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/core2/InfixParser.py` & `pysces-1.1.0/pysces/core2/InfixParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/core2/PyscesCore2.py` & `pysces-1.1.0/pysces/core2/PyscesCore2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
@@ -50,14 +50,18 @@
         list.__init__(self, *args)
 
     def asSet(self):
         return set(self.__getslice__(0, self.__len__()))
 
 
 class NewCoreBase(object):
+    """
+    Core2 base class
+    """
+
     __DEBUG__ = False
     name = None
     annotations = None
 
     def getName(self):
         return self.name
 
@@ -78,14 +82,18 @@
         """Set an annotation as a key:value pair"""
         if self.annotations == None:
             self.annotations = {}
         self.annotations.update({key: value})
 
 
 class NumberBase(NewCoreBase):
+    """
+    Derived Core2 number class.
+    """
+
     value = None
     value_initial = None
 
     def __call__(self):
         return self.value
 
     def getValue(self):
@@ -767,15 +775,15 @@
         InfixParser.setNameStr('self.', '()')
         ##  InfixParser.SymbolReplacements = {'_TIME_':'_TIME_()'}
         InfixParser.parse(formula)
         self._names = InfixParser.names
         self.code_string = 'self.value=%s' % InfixParser.output
         self.xcode = compile(self.code_string, '<string>', 'exec')
         if self.__DEBUG__:
-            '\t', self.name, self.code_string
+            print('\t', self.name, self.code_string)
 
     def evaluateAssignment(self):
         exec(self.xcode)
 
 
 class Event(NewCoreBase):
     trigger = None
@@ -790,14 +798,16 @@
 
     assignments = None
     _TIME_ = None
     _ASS_TIME_ = 0.0
     _need_action = False
     _names = None
     _time_symbol = None
+    priority = None
+    persistent = True
 
     def __init__(self, name):
         self.setName(name)
         self.assignments = []
 
     def __call__(self, time):
         self._TIME_.set(time)
@@ -836,28 +846,33 @@
         if self._time_symbol != None:
             InfixParser.setNameStr('', '')
             InfixParser.SymbolReplacements = {self._time_symbol: '_TIME_'}
             InfixParser.parse(formula)
             self.formula = InfixParser.output
         self.xcode = compile(self.code_string, '<string>', 'exec')
         if self.__DEBUG__:
-            self.name, self.code_string
+            print(self.name, self.code_string)
 
     def setTriggerAttributes(self, core):
         # TODO: experimental
         for n in self._names:
             self.__setattr__(n, core.__getattribute__(n))
 
     def setAssignment(self, var, formula):
         ass = EventAssignment(var.name)
         ass.setVariable(var)
         ass.setFormula(formula)
         self.assignments.append(ass)
         self.__setattr__('_' + var.name, ass)
 
+    def setPriority(self, priority):
+        self.priority = priority
+
+    def setPersistent(self, persistent):
+        self.persistent = persistent
 
 class PieceWise(NewCoreBase):
     """
     Generic piecewise class written by me!
 
     - *args* a dictionary of piecewise information generated by the InfixParser
     """
@@ -1433,14 +1448,16 @@
 
         ev = Event(e['name'])
         ev._time_symbol = e['tsymb']
         ev.setTrigger(e['trigger'], e['delay'])
         # associate model attributes with event
         # TODO: check that this still works
         ev.setTriggerAttributes(self)
+        ev.setPriority(e['priority'])
+        ev.setPersistent(e['persistent'])
         ##  for n in ev._names:
         ##  setattr(ev, n, self.__getattribute__(n))
         # for each assignment
         for ass in e['assignments']:
             ev.setAssignment(self.__getattribute__(ass), e['assignments'][ass])
             assref = getattr(ev, '_' + ass)  # don\t like this at all :-(
             # associate model attributes with assignment
```

### Comparing `pysces-1.0.3/pysces/core2/PyscesCore2Interfaces.py` & `pysces-1.1.0/pysces/core2/PyscesCore2Interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
@@ -427,20 +427,19 @@
     def setEvents(self):
         out = ''
         start = True
         for ev in self.core.events:
             if start:
                 out = '# Event definitions\n'
                 start = False
-            ##  formula = ev.code_string.split('=',1)
-            formula = ev.formula
-            out += 'Event: %s, %s, %s \n{\n' % (ev.name, formula, ev.delay)
+            out += f'Event: {ev.name}, {ev.formula}, delay={ev.delay}, priority={ev.priority}, persistent={ev.persistent}'
+            out += ' {\n'
             for ass in ev.assignments:
-                out += '%s = %s\n' % (ass.variable.name, ass.formula)
-            out += '}\n'
+                out += '    {} = {}\n'.format(ass.variable.name, ass.formula)
+            out += '    }\n\n'
         if out != '':
             out += ' \n'
         self.event_block = out
 
     def setNotes(self, s=''):
         if len(s) > 1:
             out = '# Notes\n# '
@@ -597,16 +596,16 @@
 # TODO: PIECEWISE WRITING
 
 
 class CoreToSBML(object):
     core = None
     name = None
     SBML = None
-    level = 2
-    version = 1
+    level = 3
+    version = 2
     model = None
     document = None
     time = None
     __events__ = None
     __DEBUG__ = False
     UNINIT_DEFAULT = 1e-3
 
@@ -705,20 +704,20 @@
             print('Posix sbml load error')
             self.SBML = None
 
     def createModel(self):
         """
         Create an SBML model and document uses the class attributes:
 
-         - *self.level* [default=2] SBML level
-         - *self.version* [default=4] SBML version
+         - *self.level* [default=3] SBML level
+         - *self.version* [default=2] SBML version
 
         and creates:
 
-         - self.model and SBML model
+         - self.model an SBML model
          - self.document an SBML document
 
         """
         if self.SBML.getLibSBMLVersion() < 40000:
             self.model = self.SBML.Model()
             self.model.setName(self.name)
             self.document = self.SBML.SBMLDocument()
@@ -930,36 +929,29 @@
 
     def astSetCSymbolTime(self, ast):
         """set ASTNode type <cn> _TIME_ </cn> to <csymbol> time </csymbol>"""
         strBuf = io.StringIO()
         mathMLin = self.SBML.writeMathMLToString(ast)
         strBuf.write(mathMLin)
         strBuf.seek(0)
+        ElementTree.register_namespace('', "http://www.w3.org/1998/Math/MathML")
         etree = ElementTree.parse(strBuf)
         root = etree.getroot()
-        counter = itertools.count(1)
-
-        def idxNode(node, idx=0):
+        for node in root.findall('.//{http://www.w3.org/1998/Math/MathML}ci'):
             if node.text != None and node.text.strip() == '_TIME_':
                 # <csymbol encoding="text" definitionURL="http://www.sbml.org/sbml/symbols/time"> t </csymbol>
                 node.text = node.text.replace('_TIME_', 'time')
                 node.tag = "{http://www.sbml.org/sbml/symbols/time}csymbol"
                 node.attrib.update({'encoding': 'text'})
                 node.attrib.update(
                     {'definitionURL': 'http://www.sbml.org/sbml/symbols/time'}
                 )
 
-            children = node.getchildren()
-            for child in range(len(children)):
-                idxNode(children[child], next(counter))
-
-        idxNode(root, idx=0)
-
         strBuf = io.StringIO()
-        etree.write(strBuf)
+        etree.write(strBuf, xml_declaration=True, encoding='unicode', method='xml')
         strBuf.seek(0)
         mathMLout = strBuf.read()
         return self.SBML.readMathMLFromString(mathMLout)
 
     def setRules(self):
         """Set rate rules"""
         for rule in self.core.rate_rules:
@@ -1024,35 +1016,45 @@
         """Set events"""
         for ev in self.core.events:
             if self.__DEBUG__:
                 print('Adding event: %s' % ev.getName())
             EV = self.model.createEvent()
             EV.setName(ev.getName())
             EV.setId(ev.getName())
+            EV.setUseValuesFromTriggerTime(True)  # default, PySCeS does not handle False
 
             #print(ev.getName())
             #print(ev.formula)
             #print(ev.code_string)
             # replace PySCeS infix with libSBML infix
             #print('LOOKATME PARSE EVENT line 979')
             form = ev.code_string.replace('self.state=', '').replace('self.', '').replace('()', '')
             #print(form)
             form = self.infixPSC2SBML(form)
             #print(form)
             if self.__DEBUG__:
                 print('\tTrigger: %s' % form)
             ASTnode = self.SBML.parseL3Formula(form)
             assert ASTnode != None, "ERROR: unable to parse formula (%s) to AST" % form
-            #print(self.SBML.formulaToL3String(ASTnode))
             ## set _TIME_ ASTnode tag to <csymbol> time
-            #ASTnode = self.astSetCSymbolTime(ASTnode)
+            ASTnode = self.astSetCSymbolTime(ASTnode)
 
             tr = self.SBML.Trigger(self.level, self.version)
+            tr.setInitialValue(True)  # default, PySCeS does not handle False
+            tr.setPersistent(ev.persistent)
             tr.setMath(ASTnode)
             EV.setTrigger(tr)
+
+            # priority
+            if ev.priority is not None:
+                prio = self.SBML.Priority(self.level, self.version)
+                ASTnode = self.SBML.parseL3Formula(str(ev.priority))
+                prio.setMath(ASTnode)
+                EV.setPriority(prio)
+
             ea_cntr = 0
             for ass in ev.assignments:
                 #print('LOOKATME PARSE EVENTASSIGNMENT line 1003')
                 if self.__DEBUG__:
                     print('\tAssignment: %s = %s' % (ass.getName(), ass.formula))
                 #print(ass.getName())
                 #print(ass.formula)
@@ -1070,15 +1072,16 @@
                 eass.setVariable(ass.variable.getName())
                 assert eass.setMath(ASTnode) == 0, 'ERROR: EventAssignment math set error.'
                 EV.addEventAssignment(eass)
             if ev.delay != 0:
                 dform = self.infixPSC2SBML(ev.delay)
                 ASTnodeD = self.SBML.parseFormula(dform)
                 ASTnodeD = self.astSetCSymbolTime(ASTnodeD)
-                D = self.SBML.Delay(ASTnodeD)
+                D = self.SBML.Delay(self.level, self.version)
+                D.setMath(ASTnodeD)
                 EV.setDelay(D)
 
     def setReactions(self):
         for rxn in self.core.reactions:
             # print 'Adding reaction:', rxn.name
             SBML_R = self.model.createReaction()
             SBML_R.setId(rxn.name)
@@ -1206,16 +1209,16 @@
         F.flush()
         F.close()
         print('Model %s exported as: %s' % (self.name, filename))
 
 
 class SbmlToCore(object):
     SBML = None
-    level = 2
-    version = 5
+    level = 3
+    version = 2
     sbml_string = None
     sbml_file = None
     model = None
     document = None
     core = None
     # old
     ModelFile = None
@@ -1348,22 +1351,22 @@
         """
         print('Check SBML support is at action level {}'.format(2))
         print('SBML file is L{}V{}'.format(self.__model_in_level__, self.__model_in_version__))
         logfile = '{}-sbml_conversion_errors.txt'.format(os.path.split(self.sbml_file)[-1])
         warn = []
         fatal = []
 
-        if self.model.getLevel() >  2:
-            warn.append('Model is encoded as SBML Level 3, PySCeS only officially supports L2V5.')
+        # if self.model.getLevel() >  2:
+        #     warn.append('Model is encoded as SBML Level 3, PySCeS only officially supports L2V5.')
         if self.model.getNumConstraints() > 0:
             fatal.append('PySCeS does not support Constraints.')
         if self.model.getNumInitialAssignments() > 0:
             fatal.append('PySCeS does not support InitialAssignments.')
-        if self.model.getNumEvents() > 0 and self.model.getLevel() >  2:
-            fatal.append('PySCeS does not support L3 events.')
+        # if self.model.getNumEvents() > 0 and self.model.getLevel() >  2:
+        #     fatal.append('PySCeS does not support L3 events.')
         if len([r.getType() for r in  self.model.getListOfRules() if r.getType() > 1]) > 0:
             fatal.append('PySCeS only supports rate and assignment rules.')
 
 
         if len(warn) == 0 and len(fatal) == 0:
             return
         else:
@@ -1376,15 +1379,15 @@
                     print('FATAL: {}'.format(err))
                     F.write('FATAL: {}\n'.format(err))
             print('\n*********ERRORS***********\n')
             print('\nPossible errors detected in SBML conversion, Model may be incomplete. Please check the error log file \"{}\" for details.\n'.format(logfile))
             if action == 1:
                 raise RuntimeError
             elif action == 2:
-                time.sleep(5)
+                time.sleep(1)
             else:
                 time.sleep(0.1)
 
 
     def getUnits(self):
         self.__uDict__ = {
             'substance': {'exponent': 1, 'multiplier': 1.0, 'scale': 0, 'kind': 'mole'},
@@ -1420,14 +1423,35 @@
 
     def getEvents(self):
         self.__eDict__ = {}
         for ev in self.model.getListOfEvents():
             name = self.getId(ev)
             trigger = ev.getTrigger()
             triggerf = self.sbmlFormulaToInfix(trigger.getMath())
+            persistent = trigger.getPersistent()
+            if trigger.initial_value == False:
+                raise NotImplementedError(
+                    '''
+    "trigger.initial_value = False" not implemented.
+        Change to True to run the model with PySCeS.
+                    '''
+                )
+            if ev.use_values_from_trigger_time == False:
+                raise NotImplementedError(
+                    '''
+    "event.use_values_from_trigger_time = False" not implemented.
+        PySCeS evaluates event assignments at trigger time.
+                    '''
+                )
+
+            priority = ev.getPriority()
+            if priority is not None:
+                priorityf = self.sbmlFormulaToInfix(priority.getMath())
+            else:
+                priorityf = None
 
             # check for csymbol time
             hasTimeS = self.searchForCsymbolTime(trigger.getMath())
             tSymb = None
             if hasTimeS != None:
                 tSymb = hasTimeS.group()[hasTimeS.group().find('>') :]
                 tSymb = tSymb.replace('>', '').replace('<', '').strip()
@@ -1443,15 +1467,17 @@
                 delay = 0.0
 
             self.__eDict__.update(
                 {
                     name: {
                         'name': name,
                         'trigger': triggerf,
+                        'persistent': persistent,
                         'delay': delay,
+                        'priority': priorityf,
                         'assignments': {},
                         'tsymb': tSymb,
                     }
                 }
             )
             for a in ev.getListOfEventAssignments():
                 self.__eDict__[name]['assignments'].update(
```

### Comparing `pysces-1.0.3/pysces/core2/PyscesCore2Modules.py` & `pysces-1.1.0/pysces/core2/PyscesCore2Modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/core2/__init__.py` & `pysces-1.1.0/pysces/core2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/core2/lex.py` & `pysces-1.1.0/pysces/core2/lex.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/core2/yacc.py` & `pysces-1.1.0/pysces/core2/yacc.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/docs/HISTORY.txt` & `pysces-1.1.0/pysces/docs/HISTORY.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/docs/userguide.pdf` & `pysces-1.1.0/pysces/docs/userguide.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 17% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 PySCeS User Guide
-Release 1.0.0
+Release 1.1.0
 
 Brett Olivier, Johann Rohwer, Jannie Hofmeyr
 
-Sep 19, 2021
+Apr 18, 2023
 
 CONTENTS
 
 1
 
 Introduction
 
@@ -84,43 +84,43 @@
 9
 
 Input file guide
 35
 9.1 The PySCeS Model Description Language . . . . . . . . . . . . . . . . . . . . . . . . 35
 
 10 Module documentation
-47
-10.1 PySCeS Module documentation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 47
+49
+10.1 PySCeS Module documentation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 49
 11 Indices and tables
 
-93
+101
 
 i
 
 Python Module Index
 
-95
+103
 
 Index
 
-97
+105
 
 ii
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 PySCeS: the Python Simulator for Cellular Systems is an extendable toolkit for the analysis
 and investigation of cellular systems. PySCeS is available for download at http://pysces.
 github.io and on GitHub where the source code is maintained: https://github.com/PySCeS/
 pysces
 
 CONTENTS
 
 1
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 2
 
 CONTENTS
 
 CHAPTER
 
@@ -141,15 +141,15 @@
 We hope that you will enjoy using our software. If, however, you find any unexpected features (i.e. bugs)
 or have any suggestions on how we can improve PySCeS please let us know by opening an issue on
 Github.
 The PySCeS development team.
 
 3
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 4
 
 Chapter 1. Introduction
 
 CHAPTER
 
@@ -179,33 +179,33 @@
 Parallel scanner is available
 PySCeS environment
 ******************
 pysces.model_dir = /home/jr/Pysces/psc
 pysces.output_dir = /home/jr/Pysces
 
 ***********************************************************************
-* Welcome to PySCeS (1.0.0) - Python Simulator for Cellular Systems
+* Welcome to PySCeS (1.1.0) - Python Simulator for Cellular Systems
 *
 *
 http://pysces.sourceforge.net
 *
-* Copyright(C) B.G. Olivier, J.M. Rohwer, J.-H.S. Hofmeyr, 2004-2021 *
+* Copyright(C) B.G. Olivier, J.M. Rohwer, J.-H.S. Hofmeyr, 2004-2023 *
 * Triple-J Group for Molecular Cell Physiology
 *
 * Stellenbosch University, ZA and VU University Amsterdam, NL
 *
 * PySCeS is distributed under the PySCeS (BSD style) licence, see
 *
 * LICENCE.txt (supplied with this release) for details
 *
 (continues on next page)
 
 5
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 (continued from previous page)
 
 * Please cite PySCeS with: doi:10.1093/bioinformatics/bti046
 *
 ***********************************************************************
 PySCeS is now ready to use. If you would like to test your installation try running the test suite:
@@ -248,15 +248,15 @@
 Parsing file: /home/jr/Pysces/psc/orca/test_lin1s.psc
 (continues on next page)
 
 6
 
 Chapter 2. Getting started
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 (continued from previous page)
 
 Calculating L matrix . . . . . . .
 Calculating K matrix . . . . . . .
 
 done.
@@ -287,22 +287,23 @@
 2.3 Basic model attributes
 Some basic model properties are accessible once the model is loaded:
 • mod.ModelFile, the name of the model file that was used.
 • mod.ModelDir, the input file directory.
 • mod.ModelOutput, the PySCeS work/output directory.
 • Parameters are available as attributes directly as specified in the input file, e.g. k1 is mod.k1.
 • External (fixed) species are made available in the same way.
-• Internal (variable) species are treated in a similar way except that an additional attribute (parameter)
-is created to hold the species’ initial value (as specified in the input file), e.g., from s1, mod.s1
-and mod.s1_init are instantiated as model object attributes.
+
 2.3. Basic model attributes
 
 7
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
+• Internal (variable) species are treated in a similar way except that an additional attribute (parameter)
+is created to hold the species’ initial value (as specified in the input file), e.g., from s1, mod.s1
+and mod.s1_init are instantiated as model object attributes.
 • Compartments are also are assigned an initial value.
 • Rate equations are translated into objects that return their current value when called, e.g. mod.
 R1().
 All basic model attributes that are described here can be changed interactively. However, if the model
 rate equations need to be changed, this should be done in the input file after which the model should be
 re-instantiated and reloaded.
 
@@ -361,15 +362,15 @@
 1
 
 Hofmeyr, J.-H.S. (2001) Metabolic control analysis in a nutshell, in T.-M. Yi, M. Hucka, M. Morohashi, and H. Kitano,
 eds, Proceedings of the 2nd International Conference on Systems Biology, pp. 291-300.
 
 9
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 • .getIndexes() return the matrix indices (relative to the Stoichiometric matrix) as tuple((rows),
 (columns))
 • .getColsByIdx() extract column(s) referenced by index
 • .getRowsByIdx() extract row(s) referenced by index
 
 3.1.2 Structural Analysis - legacy
 • mod.nmatrix, N: displayed with mod.showN()
@@ -405,15 +406,15 @@
 >>> mod.sim_end = 20
 (continues on next page)
 
 10
 
 Chapter 3. Modelling
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 (continued from previous page)
 
 >>> mod.sim_points = 50
 >>> mod.Simulate()
 2. Using the mod.doSim() method where only the end time and points need to be specified. For
 example, running a 20-point simulation from time 0 to 10:
@@ -443,20 +444,19 @@
 Starting with PySCeS versions 0.7.x the simulation results have been consolidated into a new mod.
 data_sim object. By default species concentrations/amounts, reaction rates and rate rules are automatically added to the data_sim object. If extra information (parameters, compartments, assignment rules) is
 required this can easily be added using mod.CVODE_extra_output, a list containing any model attribute
 which is not added by default.
 The mod.data_sim object has many methods for extracting simulation data including:
 • data_sim.getTime() returns a vector of time points
 • data_sim.getSpecies() returns array([[time], [species]])
-
 3.2. Time simulation
 
 11
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 • data_sim.getRates() returns array([[time], [rates]])
 • data_sim.getRules() returns array([[time], [rate rules]])
 • data_sim.getXData returns array([[time], [CVODE_extra_output]])
 • data_sim.getSimData(*args) return an array consisting of time plus any available data series:
 >>> mod.data_sim.getSimdata('s1', 'R1', 'Rule1', 'xData2')
 • data_sim.getAllSimData() return an array of all simulation data
 • data_sim.getDataAtTime(time) return the results of the simulation at time.
@@ -480,27 +480,28 @@
 'lsoda_rtol': 1.0e-7
 'lsoda_mxordn': 12
 'lsoda_mxords': 5
 'lsoda_mxstep': 0
 where atol and rtol are the absolute and relative tolerances, while mxstep=0 means that LSODA chooses
 the number of steps (up to 500). If this is still not enough, PySCeS automatically increases the number
 of steps necessary to find a solution.
-The following options can be set for CVODE, with their defaults indicated:
-'cvode_abstol': 1.0e-15
-'cvode_mxstep': 1000
+The following are the most common options that can be set for CVODE, with their defaults indicated:
+'cvode_abstol': 1.0e-9
+'cvode_mxstep': 5000
 'cvode_reltol': 1.0e-9
 'cvode_stats': False
 'cvode_return_event_timepoints': True
-where atol, rtol and mxstep are as above. If CVODE cannot find a solution in the given number of steps it
-automatically increases cvode_mxstep and tries again, however, it also keeps track of the number of times
+
 12
 
 Chapter 3. Modelling
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
+where atol, rtol and mxstep are as above. If CVODE cannot find a solution in the given number of steps it
+automatically increases cvode_mxstep and tries again, however, it also keeps track of the number of times
 that this adjustment is required and if a specific threshold is passed it will begin to increase cvode_reltol
 by 1.0e3 (to a maximal value of 1.0e-3). If cvode_stats is enabled CVODE will display a report of its
 internal parameters after the simulation is complete. Finally, CVODE will by default also output the time
 points when events are triggered, even if these were not originally specified in mod.sim_time. To disable
 this behaviour and strictly report only the times in mod.sim_time, set cvode_return_event_timepoints
 to False.
 
@@ -531,15 +532,15 @@
 • mod.mode_state_init initialises the solver using either the initial values specified in the input
 file (0), or a value close to zero (1). The default behaviour is to use the initial values.
 
 3.3. Steady-state analysis
 
 13
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 3.3.1 The steady-state data object
 Since PySCeS version 0.7 the mod.data_sstate object by default stores steady-state data (species,
 fluxes, rate rules) in a manner similar to mod.data_sim. One notable exception is that the current
 steady-state values are also made available as attributes to this object (e.g. species S1’s steady-state
 value is stored as mod.data_sstate.S1). Using the mod.STATE_extra_output list it is possible to
 store user-defined data in the data_sstate object. Steady-state data can be easily retrieved using the by
@@ -575,15 +576,15 @@
 effector strength, Eur. J. Biochem. 42, 89-95.
 3
 
 14
 
 Chapter 3. Modelling
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 3.4.1 Elasticities
 The elasticities towards both the variable species and parameters can be calculated using mod.doElas()
 which generates as output:
 • Scaled elasticities referenced as mod.ecRate_Species, e.g. mod.ecR4_s2.
 • mod.showEvar() displays the non-zero elasticities calculated with respect to the variable species.
 • mod.showEpar() displays the non-zero parameter elasticities.
@@ -617,15 +618,15 @@
 • rc.row: row labels
 • rc.col: column labels
 
 3.4. Metabolic Control Analysis
 
 15
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 3.4.4 Response coefficients with respect to moiety-conserved sums
 The mod.doMcaRC() method only calculates response coefficients with respect to explicit model parameters. However, in models with moiety-conservation the total concentration of all the species that form
 part of a particular moiety-conserved cycle is also a parameter of the model. PySCeS infers such moietyconserved sums from the initial species concentrations specified by the user. In some cases it might be
 interesting to consider the effects that a change in the total concentration of a moiety will have on the
 steady-state. This analysis may be done with the method mod.doMcaRCT().
 Since moiety-conserved sums are not explicitly named in PySCeS model files, 'T_' is prepended to all
@@ -670,15 +671,15 @@
 Scanning ...
 11 (hybrd) The solution converged.
 (hybrd) The solution converged ...
 done.
 
 17
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 When the scan has been successfully completed, the results are stored in the array (mod.scan_res)
 that has mod.scan_in as its first column followed by columns that represent the data defined in mod.
 scan_out (if invalid steady states are generated during the scan they are replaced by NaN). Scan1 also
 reports the scan parameter values which generated the invalid states. If one or more of the specified input
 or output parameters are not valid model attributes, they will be ignored. Once the parameter scan data
 has been generated, the next step is to visualise it using the mod.Scan1Plot() method:
 >>> mod.Scan1Plot(plot=[], title=None, log=None, format='lines',␣
@@ -710,15 +711,15 @@
 • format the backend dependent line format (default= 'lines') or the CommonStyle 'lines' or
 'points'.
 
 18
 
 Chapter 4. Parameter scanning
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 4.3 Multi-dimensional parameter scans
 This PySCeS feature allows multi-dimensional parameter scanning. Any combination of parameters
 is possible and can be added as leader parameters that change independently or follower parameters
 whose change is coordinated with the previously defined parameter. Unlike mod.Scan1() this function
 is accessed via the pysces.Scanner class that is separately instantiated with a loaded PySCeS model
 object:
@@ -756,15 +757,15 @@
 • sc1.UserOutputResults an array containing only the output
 • sc1.ScanSpace the generated list of input parameters.
 
 4.3. Multi-dimensional parameter scans
 
 19
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 4.4 Parallel parameter scans
 When performing large multi-dimensional parameter scans, PySCeS has the option to perform the computation in parallel, either on a single machine with a multi-core CPU, or on a multi-node cluster. This
 requires a working ipyparallel installation (see also Installation). The functionality is accessed via the
 pysces.ParScanner class, which has the same methods as the pysces.Scanner class (see above) with
 a few multiprocessing-specific additions.
 The parallel scanner class is instantiated with a loaded PySCeS model object:
@@ -820,15 +821,15 @@
 • formats a list (per line) of format strings, if formats only contains a single item, this format is used
 for all lines.
 splot(data, x, y, z, title='', format='') plot a surface, i.e. data[z] vs data[y] vs data[x]
 • data the data array
 
 21
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 • x x column index
 • y y column index
 • z z column index
 • title the surface key (legend text)
 • format a format string (default=”)
 splotSurfaces(data, x, y, z=[], titles=[], formats=['']) plot multiple surfaces, i.e.
 data[z1, z2, ] vs data[y] vs data[x]
@@ -861,27 +862,27 @@
 • axis is one of x, y, z, xy, xz, yz, zyx
 setNoLogScale(axis) set axis to a linear scale
 
 22
 
 Chapter 5. Plotting
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 • axis is one of x, y, z, xy, xz, yz, zyx
 setRange(axis, min=None, max=None) set one or more axis ranges
 • axis is one of x, y, z, xy, xz, yz, zyx
 • min is the range(s) lower bound (default=None, back-end auto-scales)
 • max is the range(s) upper bound (default=None, back-end auto-scales)
 setGrid(value) enable or disable the graph grid
 • value (boolean) True (on) or False (off)
 plt.closeAll() Close all active Matplolib figures.
 
 23
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 24
 
 Chapter 5. Plotting
 
 CHAPTER
 
@@ -915,15 +916,15 @@
 • getstrbuf : if True a StringIO buffer is returned instead of writing to disk
 For example, assuming you have loaded a model and run mod.doState() the following code opens
 a Python file object (rFile), writes the steady-state results to the file associated with the file object
 (results.txt) and then closes it again:
 
 25
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 >>> rFile = open('results.txt','w')
 >>> mod.showState()
 # print the results to screen
 >>> mod.showState(rFile) # write the results to the file results.txt
 >>> rFile.close()
 
@@ -965,15 +966,15 @@
 By default, each time an array is written, PySCeS includes an array header consisting of the
 model name and the time the array was written. This behaviour can be disabled by setting: mod.
 write_array_header = 0
 26
 
 Chapter 6. Displaying data
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 6.2.2 Write_array_latex()
 The Write_array_latex() method functions similarly to the generic Write_array() method except
 that it generates a formatted array that can be included directly in a LaTeX document. Additionally, there
 is no separator argument, column headings are not truncated and row labels appear to the left of the
 matrix.
 >>> mod.Write_array_latex(input, File=None, Row=None, Col=None)
@@ -1013,15 +1014,15 @@
 0.0000
 0.0000
 -0.5065
 1.0130
 
 27
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 28
 
 Chapter 6. Displaying data
 
 CHAPTER
 
@@ -1030,16 +1031,16 @@
 INSTALLING AND CONFIGURING
 
 PySCeS is developed primarily in Python and has been designed to operate on multiple operating systems,
 i.e. Linux, Microsoft Windows and macOS. PySCeS makes use of NumPy and SciPy for a number of
 functions and needs a working SciPy stack (https://www.scipy.org) to install and run.
 
 7.1 General requirements
-• Python 3.6+
-• Numpy 1.14+
+• Python 3.7+
+• Numpy 1.17+
 • SciPy 1.0+
 • Matplotlib (with TkAgg backend)
 • GnuPlot (optional, alternative plotting back-end)
 • IPython or the Jupyter notebook (optional, highly recommended for interactive modelling sessions)
 • libSBML (optional). Python bindings for SBML support can be installed via
 $ pip install python-libsbml
 This software stack provides a powerful scientific programming platform which is used by PySCeS to
@@ -1052,53 +1053,53 @@
 • pysces_metatool (available via https://github.com/PySCeS/pysces-metatool) to add elementary
 mode analysis support to PySCeS.
 By default PySCeS installs with a version of ZIB’s NLEQ2 non-linear solver. This software is distributed
 under its own non-commercial licence. Please see https://github.com/PySCeS/pysces for details.
 
 29
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 7.2 Installation
-Binary install packages for all three OSs and Python versions 3.6-3.9 are provided. Anaconda users can
+Binary install packages for all three OSs and Python versions 3.7-3.10 are provided. Anaconda users can
 conveniently install PySCeS with:
 $ conda install -c conda-forge -c pysces pysces
 Any dependencies will be installed automatically, including the optional dependencies Assimulo, ipyparallel and libSBML.
 Alternatively, you can use pip to install PySCeS from PyPI. Core dependencies will be installed automatically.
 $ pip install pysces
 To install the optional dependences:
 • pip install "pysces[parscan]" - for ipyparallel
 • pip install "pysces[sbml]" - for libSBML
 • pip install "pysces[cvode]" - for Assimulo
 • pip install "pysces[all]" - for all of the above
 Note: Installation of Assimulo via pip may well require C and Fortran compilers to be properly set up
 on your system, as binary packages are only provided for a very limited number of Python versions and
-operating systems on PyPI. This is not guaranteed to work! If you require Assimulo, the conda install
-is by far the easier option as up-to-date binaries are supplied for all OS and recent Python versions.
+operating systems on PyPI. This is not guaranteed to work! In addition, the Assimulo version on PyPI
+is severely outdated. If you require Assimulo, the conda install is by far the easier option as up-to-date
+binaries are supplied for all OS and recent Python versions.
 
 7.3 Compilation from source
 As an alternative to a binary installation, you can also build your own PySCeS installation from source.
 This requires Fortran and C compilers.
 
 7.3.1 Windows build
 The fastest way to build your own copy of PySCeS is to use Anaconda Python.
 • Download and install Anaconda for Python 3
 • Obtain Git for Windows
 • Create a PySCeS environment using conda and activate it:
-> conda create -n pyscesdev -c conda-forge python=3.8 numpy scipy \
+> conda create -n pyscesdev -c conda-forge python=3.10 numpy scipy \
 matplotlib sympy packaging pip wheel nose ipython \
 python-libsbml fortran-compiler assimulo
 > conda activate pyscesdev
 • Clone and enter the PySCeS code repository using git
-
 30
 
 Chapter 7. Installing and configuring
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 (pyscesdev)> git clone https://github.com/PySCeS/pysces.git pysces˓→src
 (pyscesdev)> cd pysces-src
 • Now you can build and install PySCeS into the pyscesdev environment
 (pyscesdev)> python setup.py build
 (pyscesdev)> python setup.py install
 
@@ -1112,34 +1113,34 @@
 The Anaconda build method, described above for Windows, should also work on macOS.
 Alternatively, Python 3 may be obtained via Homebrew and the compilers may be installed via Xcode.
 Clone the source from Github as described above, change into the source directory and run:
 $ python setup.py install
 
 7.4 Configuration
 PySCeS has two configuration (*.ini) files that allow one to specify global (per installation) and local (per
-user) options. Currently the multiuser options are only fully realised on Linux based systems. Global
-options are stored in the pyscfg.ini file which is created in your PySCeS installation directory upon install. The example below is a Windows version; the exact values of install_dir and gnuplot_dir (if
-available) will depend on your individual OS and Python setup and are determined on install.
+user) options. Global options are stored in the pyscfg.ini file which is created in your PySCeS installation
+directory upon install. The example below is a Windows version; the exact values of install_dir and
+gnuplot_dir (if available) will depend on your individual OS and Python setup and are determined on
+install.
 [Pysces]
 install_dir = c:\Python38\Lib\site-packages\pysces
 gnuplot_dir = c:\model\gnuplot\binaries
 model_dir = os.path.join(os.path.expanduser('~'),'Pysces','psc')
 output_dir = os.path.join(os.path.expanduser('~'),'Pysces')
 silentstart = False
 change_dir_on_start = False
 The [Pysces] section contains information on the installation directory, the directory where the GnuPlot
 executable(s) can be found and the default model file and output directories.
 This section also contains two further key-value pairs. If silentstart (default False) is set to True,
 informational messages about the PySCeS installation are not printed to the console on startup. The key
-
 7.4. Configuration
 
 31
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 change_dir_on_start specifies if the working directory should be changed to the PySCeS output directory
 (typically $HOME/Pysces or %USERPROFILE%\Pysces) on startup. When set to False (the default), the
 working directory is not changed.
 As we shall see some of these defaults can be overridden by the local configuration options.
 [ExternalModules]
 nleq2 = True
 [PyscesModules]
@@ -1171,15 +1172,15 @@
 
 EIGHT
 
 REFERENCES
 
 33
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 34
 
 Chapter 8. References
 
 CHAPTER
 
@@ -1211,19 +1212,19 @@
 practical purposes PySCeS requires a minimum of a single reaction. Once this information is obtained it
 can be organised and written as a PySCeS input file. While this list is the minimum information required
 for a PySCeS input file, the MDL allows the definition of advanced models that contain compartments,
 global units, functions, rate and assignment rules.
 
 35
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 Model keywords
-Since PySCeS 0.7 it is now possible to define keywords that specify model information. Keywords have
-the general form
+Since PySCeS 0.7 it is possible to define keywords that specify model information. Keywords have the
+general form
 <keyword>:
 
 <value>
 
 The Modelname (optional) keyword, containing only alphanumeric characters (or _), describes the model
 filename (typically used when the model is exported via the PySCeS interface module) while the Description keyword is a (short) single line model description.
 Modelname: rohwer_sucrose1
@@ -1249,15 +1250,15 @@
 UnitArea: metre, 1, 0, 2
 Please note that defining these values does not affect the numerical analysis of the model in any way.
 
 36
 
 Chapter 9. Input file guide
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 Symbol names and comments
 Symbol names (i.e. reaction, species, compartment, function, rule and parameter names etc.) must start
 with either an underscore or letter and be followed by any combination of alpha-numeric characters or
 an underscore. Like all other elements of the input file names are case sensitive:
 R1
 _subA
@@ -1272,38 +1273,38 @@
 """
 This is a comment
 spread over a
 few lines.
 """
 
 Compartment definition
-By default (as is the case in all PySCeS versions < 0.7) PySCeS assumes that the model exists in a
-single unit volume compartment. In this case it is not necessary to define a compartment and the ODEs
-therefore describe changes in concentration per time. However, if a compartment is defined, PySCeS
-assumes that the ODEs describe changes in substance amount per time. Doing this affects how the
-model is defined in the input file (especially with respect to the definitions of rate equations and species)
-and the user is strongly advised to read the Users Guide before building models in this way. The general
-compartment definition is Compartment: <name>, <size>, <dimensions>, where <name> is the
-unique compartment id, <size> is the size of the compartment (i.e. length, volume or area) defined by
-the number of <dimensions> (e.g. 1,2,3):
+By default (as is the case in all PySCeS versions < 0.7) PySCeS assumes that the model exists in a single
+unit volume compartment. In this case it is not necessary to define a compartment and the ODEs therefore
+describe changes in concentration per time. However, if a compartment is defined, PySCeS assumes that
+the ODEs describe changes in substance amount per time in keeping with the SBML standard. Doing
+this affects how the model is defined in the input file (especially with respect to the definitions of rate
+equations and species) and the user is strongly advised to read the User Guide before building models in
+this way. The general compartment definition is Compartment: <name>, <size>, <dimensions>,
+where <name> is the unique compartment id, <size> is the size of the compartment (i.e. length, volume
+or area) defined by the number of <dimensions> (e.g. 1,2,3):
 Compartment: Cell, 2.0, 3
 Compartment: Memb, 1.0, 2
 
+9.1. The PySCeS Model Description Language
+
+37
+
+PySCeS User Guide, Release 1.1.0
+
 Function definitions
 A relatively recent addition to the PySCeS MDL is the ability to define SBML-styled functions. Simply put these are code substitutions that can be used in rate equation definitions to, for example, simplify
 the kinetic law. The general syntax for a function is Function: <name>, <arglist> {<formula>}
 where <name> is the unique function id, <arglist> is one or more comma separated function arguments.
 The <formula> field, enclosed in curly braces, may only make use of arguments listed in the <arglist>
 and therefore cannot reference model attributes directly. If this functionality is required a forcing function/assignment rule (see Assignment rules) may be what you are looking for.
-9.1. The PySCeS Model Description Language
-
-37
-
-PySCeS User Guide, Release 1.0.0
-
 Function: rmm_num, Vf, s, p, Keq {
 Vf*(s - p/Keq)
 }
 Function: rmm_den, s, p, Ks, Kp {
 s + Ks*(1.0 + p/Kp)
 }
 The syntax for function definitions has been adapted from Antimony.
@@ -1325,43 +1326,42 @@
 <rate equation>
 The <name> argument follows the syntax as discussed in Symbol names and comments above; however,
 when more than one compartment has been defined it is important to locate the reaction in its specific
 compartment. This is done using the @ operator:
 <name>@<compartment>:
 <stoichiometry>
 <rate equation>
+
+38
+
+Chapter 9. Input file guide
+
+PySCeS User Guide, Release 1.1.0
 where <compartment> is a valid compartment name. In either case this then followed (either directly or
 on the next line) by the reaction stoichiometry.
 Each <stoichiometry> argument is defined in terms of reaction substrates, appearing on the left hand
 side, and products on the right hand side of an identifier which labels the reaction as either reversible (=)
 or irreversible (>). If required each reagent’s stoichiometric coefficient (PySCeS accepts both integer and
 floating point) should be included in curly braces {} immediately preceding the reagent name. If these
 are omitted a coefficient of one is assumed.
-
-38
-
-Chapter 9. Input file guide
-
-PySCeS User Guide, Release 1.0.0
-
 {2.0}Hex_P = Suc6P + UDP
 Fru_ex > Fru
 species_5 > $pool
 
 # reversible reaction
 # irreversible reaction
 # a reaction to a sink
 
 The PySCeS MDL also allows the use of the $pool token that represents a placeholder reagent for
 reactions that have no net substrate or product. The reversibility of a reaction is only used when exporting
 the model to other formats (such as SBML) and in the calculation of elementary modes. It does not affect
 the numerical evaluation of the rate equations in any way.
-Central to any reaction definition is the <rate equation> (SBML kinetic law). This should be written as
-valid Python expression and may fall across more than one line. Standard Python operators + - * / **
-are supported (note the Python power e.g. 2^4 is written as 2**4). There is no shorthand for multiplication with a bracket so -2(a+b)^h would be written as -2*(a+b)**h} and normal operator precedence
+Central to any reaction definition is the <rate equation> (SBML kinetic law). This should be written
+as valid Python expression and may fall across more than one line. Standard Python operators + - * /
+** are supported (note the Python power e.g. 2^4 is written as 2**4). There is no shorthand for multiplication with a bracket so -2(a+b)^h would be written as -2*(a+b)**h and normal operator precedence
 applies:
 +, *, /
 +x,-x
 **
 
 addition, subtraction
 multiplication, division
@@ -1380,25 +1380,24 @@
 • notanumber, pi, infinity, exponentiale
 Logical operators are supported in rules, events, etc., but not in rate equation definitions. The PySCeS
 parser understands Python infix as well as libSBML and NumPy prefix notation.
 • and or xor not
 • > gt(x,y) greater(x,y)
 • < lt(x,y) less(x,y)
 • >= ge(x,y) geq(x,y) greater_equal(x,y)
+9.1. The PySCeS Model Description Language
+
+39
+
+PySCeS User Guide, Release 1.1.0
 • <= le(x,y) leq(x,y) less_equal(x,y)
 • == eq(x,y) equal(x,y)
 • != neq(x,y) not_equal(x,y)
 Note that currently the MathML delay and factorial functions are not supported. Delay is handled by
 simply removing it from any expression, e.g. delay(f(x), delay) would be parsed as f(x). Support for
-
-9.1. The PySCeS Model Description Language
-
-39
-
-PySCeS User Guide, Release 1.0.0
 piecewise has been recently added to PySCeS and will be discussed in the advanced features section (see
 Piecewise).
 A reaction definition when no compartments are defined:
 R5: Fru + ATP = Hex_P + ADP
 Vmax5/(1 + Fru/Ki5_Fru)*(Fru/Km5_Fru)*(ATP/Km5_ATP) /
 (1 + Fru/Km5_Fru + ATP/Km5_ATP + Fru*ATP/(Km5_Fru*Km5_ATP) + ADP/Ki5_ADP)
 and using the previously defined functions:
@@ -1422,28 +1421,28 @@
 in a way that is interoperable with other software.
 Species and parameter initialisation
 The general form of any species (fixed, free) and parameter is simply:
 property = value
 Initialisations can be written in any order anywhere in the input file but for enhanced human readability
 these are usually placed after the reaction that uses them or grouped at the end of the input file. Both
 decimal and scientific notation are allowed with the following provisions that neither floating point (1.)
-nor scientific shorthand (1.e-3) syntax should be used, instead use the full form (1.0e-3, 0.001 or
-1.0).
-Variable or free species are initialised differently depending on whether compartments are present in the
-model. Although the variable species concentrations are determined by the parameters of the system,
-their initial values are used in various places, calculating total moiety concentrations (if present), time
-simulation initial values (e.g. time=zero) and as initial guesses for the steady-state algorithms. If an
 
 40
 
 Chapter 9. Input file guide
 
-PySCeS User Guide, Release 1.0.0
-empty initial species pool is required it is not recommended to initialise these values to zero (in order to
-prevent potential divide-by-zero errors) but rather to a small value (e.g. 1.0e-8).
+PySCeS User Guide, Release 1.1.0
+nor scientific shorthand (1.e-3) syntax should be used, instead use the full form (1.0e-3, 0.001 or
+1.0).
+Variable or free species are initialised differently depending on whether compartments are present in
+the model or not. Although the variable species concentrations are determined by the parameters of the
+system, their initial values are used in various places, calculating total moiety concentrations (if present),
+time simulation initial values (e.g. time=zero) and as initial guesses for the steady-state algorithms. If
+an empty initial species pool is required it is not recommended to initialise these values to zero (in order
+to prevent potential divide-by-zero errors) but rather to a small value (e.g. 1.0e-8).
 For a model with no compartments these initial values are assumed to be concentrations:
 NADH = 0.001
 ATP = 2.3e-3
 sucrose = 1
 In a model with compartments it is expected that the species are located in a compartment (even if
 Species_In_Conc: False); this is done using the @ symbol:
 s1@Memb = 0.01
@@ -1451,16 +1450,16 @@
 A word of warning, the user is responsible for making sure that the units of the initialised species match
 those of the model. Please keep in mind that all species (and anything that depends on them) are defined
 in terms of the Species_In_Conc keyword. For example, if the preceding initialisations were for R1 (see
 Reaction section) then they would be concentrations (as Species_In_Conc: True). However, in the next
 example, we are initialising species for R4 and they are therefore in amounts (Species_In_Conc: False).
 s3@Memb = 1.0
 s4@Cell = 2.0
-Fixed species are defined in a similar way and although they technically parameters, they should be given
-a location in compartmental models:
+Fixed species are defined in a similar way and although they are technically parameters, they should be
+given a location in compartmental models:
 # InitExt
 X0 = 10.0
 X4@Cell = 1.0
 However, fixed species are true parameters in the sense that their associated compartment size does
 not affect their value when it changes size. If compartment size-dependent behaviour is required, an
 assignment or rate rule should be considered.
 Finally, the parameters should be initialised. PySCeS checks if a parameter is defined that is not present
@@ -1471,15 +1470,15 @@
 Vf2 = 10.0
 Ks4 = 1.0
 
 9.1. The PySCeS Model Description Language
 
 41
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 9.1.2 Advanced model construction
 Assignment rules
 Assignment rules or forcing functions are used to set the value of a model attribute before the ODEs are
 evaluated. This model attribute can either be a parameter used in the rate equations (this is traditionally
 used to describe an equilibrium block), a compartment, or an arbitrary parameter (commonly used to
 define some sort of tracking function). Assignment rules can access other model attributes directly and
@@ -1497,52 +1496,95 @@
 by the <formula>. It may also be defined anywhere in the input file:
 RateRule: Mem_Area {
 (sigma_P)*(Mem_Area*k4*(P)) + (sigma_L)*(Mem_Area*k5*(L))
 }
 RateRule: Vcyt {(1.0/Co)*(R1()+(1-m1)*R2()+(1-m2)*R3()-R4()-R5())}
 Remember to initialise any new parameters defined in the rate rules.
 Events
-Time-dependant events may be defined whose definition follows the event framework described in the
-SBML L2V1 specification. The general form of an event is Event: <name>, <trigger>, <delay>
-{ <assignments> }. As can be seen, an event consists of essentially three parts, a conditional <trigger>, a set of one or more <assignments> and a <delay> between when the trigger is fired (and the
-assignments are evaluated) and the eventual assignment to the model. Assignments have the general
-form <par> = <formula>. Events have access to the “current” simulation time using the _TIME_ symbol:
-Event: event1, _TIME_ > 10 and A > 150.0, 0 {
+Time-dependent events may be defined. Since PySCeS 1.1.0 their definition follows the event framework
+described in the SBML L3V2 specification. The general form of an event is:
+Event:
+
+<name>, <trigger>, <optional_kwargs> { <assignments> }
+
+As can be seen, an event consists of essentially two parts, a conditional <trigger>, and a set of one or
+more <assignments>. Assignments have the general form <par> = <formula>. Events have access to
+the “current” simulation time using the _TIME_ symbol:
+Event: event1, _TIME_ > 10 and A > 150.0 {
 V1 = V1*vfact
 V2 = V2*vfact
 }
-The following event illustrates the use of a delay of ten time units as well as the prefix notation (used by
-libSBML) for the trigger (PySCeS understands both notations):
+
 42
 
 Chapter 9. Input file guide
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
-Event: event2, geq(_TIME_, 15.0), 10 {
+Note: In order for PySCeS to handle events it is necessary to have Assimulo installed (refer to General
+requirements).
+In line with the SBML L3V2 specification, three optional keyword arguments can be defined as a
+comma-separated list following the trigger definition. The general syntax is <attribute>=<value>.
+The keywords are:
+• delay (float): specifies a delay between when the trigger is fired (and the assignments are evaluated)
+and the eventual assignment to the model. If this keyword is not specified, a value of 0.0 is
+assumed.
+• priority (integer or None): specifies a priority for events that trigger at the same simulation time.
+Events with a higher priority are executed before those with a lower priority, while events without
+a priority (None) are executed in random positions in the sequence. If this keyword is not specified,
+a value of None is assumed.
+• persistent (boolean): is only relevant to events with a delay, where the situation may occur that the
+trigger condition no longer holds by the time the delay in the simulation has passed. The persistent
+attribute specifies how to deal with this situation: if True, the event executes nevertheless; if
+False, the event does not execute if the trigger condition is no longer valid. If the keyword is not
+specified, a default of True is assumed.
+The reader is referred to the SBML Specification for further details.
+The following event illustrates the use of a delay of ten time units with a non-persistent trigger and a
+priority of 3. In addition, the prefix notation (used by libSBML) for the trigger is illustrated (PySCeS
+understands both notations):
+Event: event2, geq(_TIME_, 15.0), delay=10.0, persistent=False, priority=3 {
 V3 = V3*vfact2
 }
 
-Note: In order for PySCeS to handle events it is necessary to have Assimulo installed (refer to General
-requirements).
+Note:
+1. The legacy event specification (PySCeS versions <1.1), which did not include keywords for priority and persistent, and in which the delay was specified as a third positional argument (without
+keyword), is still supported but deprecated:
+Event:
+
+<name>, <trigger>, <delay> { <assignments> }
+
+2. The following SBML event attributes are not implemented:
+• event.use_values_from_trigger_time=False For an event with a delay, PySCeS always uses the assignment values from the time when the event is triggered. When loading an
+SBML model (see SBML import and export) that uses the assignment values from the time
+of event firing and thus has this event attribute set, a NotImplementedError is raised.
+• trigger.initial_value=False PySCeS always assumes that the initial value of a trigger
+is True, i.e. the event cannot fire at time zero, but that the simulation has to run for at least
+one iteration before the trigger can be fired. When loading and SBML model that has the
+initial value set to False, a NotImplementedError is raised.
+
+9.1. The PySCeS Model Description Language
+
+43
+
+PySCeS User Guide, Release 1.1.0
 
 Piecewise
 Although technically an operator, piecewise functions are sufficiently complicated to warrant their own
 section. A piecewise operator is essentially an if, elif, . . . , else logical operator that can be used to conditionally “set” the value of some model attribute. Currently piecewise is supported in rule constructs and
 has not been tested directly in rate equation definitions. The piecewise function’s most basic incarnation
 is piecewise(<val1>, <cond>, <val2>), which is evaluated as:
 if <cond>:
 return <val1>
 else:
 return <val2>
 Alternatively, piecewise(<val1>, <cond1>, <val2>, <cond2>, <val3>, <cond3>)
 if <cond1>:
 return <val1>
 elif <cond2>:
-return <val1>
+return <val2>
 elif <cond3>:
 return <val3>
 Or piecewise(<val1>, <cond1>, <val2>, <cond2>, <val3>, <cond3>, <val4>)
 if <cond1>:
 return <val1>
 elif <cond2>:
 return <val2>
@@ -1550,33 +1592,60 @@
 return <val3>
 else:
 return <val4>
 can also be used. A “real-life” example of an assignment rule with a piecewise function:
 !F Ca2plus=piecewise(0.1, lt(_TIME_,60), 0.1, gt(_TIME_,66.0115), 1)
 In principle there is no limit on the number of conditional statements present in a piecewise function; the
 condition can be a compound statement (a or b and c) and may include the _TIME_ symbol.
-
-9.1. The PySCeS Model Description Language
-
-43
-
-PySCeS User Guide, Release 1.0.0
-
 Reagent placeholder
 Some models contain reactions that are defined as only having substrates or products, with the fixed
 (external) species not specified:
 R1: A + B >
 R2: > C + D
 The implication is that the relevant reagents appear from or disappear into a constant pool. Unfortunately
 the PySCeS parser does not accept such an unbalanced reaction definition and requires these pools to be
 represented with a $pool token:
+44
+
+Chapter 9. Input file guide
+
+PySCeS User Guide, Release 1.1.0
+
 R1: A + B > $pool
 R2: $pool > C + D
 $pool is neither counted as a reagent nor does it ever appear in the stoichiometry (think of it as dev/null)
 and no other $<str> tokens are allowed.
+SBML import and export
+SBML models can be imported into PySCeS by first converting them to the input file (*.psc) format and
+then loading the input file into PySCeS as usual. The conversion is done with the pysces.interface.
+convertSBML2PSC() method:
+>>> pysces.interface.convertSBML2PSC(sbmlfile, sbmldir=None, pscfile=None,␣
+˓→pscdir=None)
+where:
+• sbmlfile: the SBML filename
+• sbmldir: the directory of SBML files (if None, the current working directory is assumed)
+• pscfile: the output PSC file name (if None, <sbmlfile>.psc is used)
+• pscdir: the PSC output directory (if None, the pysces.model_dir is used)
+An instantiated PySCeS model can be exported to SBML using the pysces.interface.
+writeMod2SBML() method:
+>>> pysces.interface.writeMod2SBML(mod, filename=None, directory=None,␣
+˓→iValues=True, getdocument=False, getstrbuf=False)
+where:
+• mod: is the PySCeS model object
+• filename: writes <filename>.xml or <model_name>.xml if None
+• directory: (optional) an output directory
+• iValues: if True, the model initial values are used (or the current values if False)
+• getdocument: if True an SBML document object is returned instead of writing to disk
+• getstrbuf : if True a StringIO buffer is returned instead of writing to disk
+
+9.1. The PySCeS Model Description Language
+
+45
+
+PySCeS User Guide, Release 1.1.0
 
 9.1.3 Example PySCeS input files
 Basic model definition
 PySCeS test model: pysces_test_linear1.psc - this file is distributed with PySCeS and copied to your
 model directory (typically $HOME/Pysces/psc) after installation, when running pysces.test() for the
 first time.
 FIX: x0 x3
@@ -1592,24 +1661,14 @@
 x0 = 10.0
 x3 = 1.0
 # InitPar
 k1 = 10.0
 k2 = 1.0
 k3 = 5.0
 k4 = 1.0
-(continues on next page)
-
-44
-
-Chapter 9. Input file guide
-
-PySCeS User Guide, Release 1.0.0
-
-(continued from previous page)
-
 k5 = 3.0
 k6 = 1.0
 k7 = 2.0
 k8 = 1.0
 # InitVar
 s0 = 1.0
 s1 = 1.0
@@ -1618,14 +1677,24 @@
 Advanced example
 This model includes the use of Compartments, KeyWords, Units and Rules:
 Modelname: MWC_wholecell2c
 Description: Surovtsev whole cell model using J-HS Hofmeyr's framework
 Species_In_Conc: True
 Output_In_Conc: True
 # Global unit definition
+(continues on next page)
+
+46
+
+Chapter 9. Input file guide
+
+PySCeS User Guide, Release 1.1.0
+
+(continued from previous page)
+
 UnitVolume: litre, 1.0, -3, 1
 UnitSubstance: mole, 1.0, -6, 1
 UnitTime: second, 60, 0, 1
 # Compartment definition
 Compartment: Vcyt, 1.0, 3
 Compartment: Vout, 1.0, 3
 Compartment: Mem_Area, 5.15898, 2
@@ -1638,24 +1707,14 @@
 Vcyt*k3*(M)*(P)**2
 R4@Mem_Area: P = Pmem
 Mem_Area*k4*(P)
 R5@Mem_Area: L = Lmem
 Mem_Area*k5*(L)
 # Rate rule definition
 RateRule: Vcyt {(1.0/Co)*(R1()+(1-m1)*R2()+(1-m2)*R3()-R4()-R5())}
-(continues on next page)
-
-9.1. The PySCeS Model Description Language
-
-45
-
-PySCeS User Guide, Release 1.0.0
-
-(continued from previous page)
-
 RateRule: Mem_Area {(sigma_P)*R4() + (sigma_L)*R5()}
 # Rate rule initialisation
 Co = 3.07e5 # uM p_env/(R*T)
 m1 = 244
 m2 = 42
 sigma_P = 0.00069714285714285711
 sigma_L = 0.00012
@@ -1666,14 +1725,24 @@
 !F Pconc = (P)/P_init
 # Assignment rule initialisations
 M_init = 199693.0
 L_init = 102004
 P_init = 5303
 Mconc = 1.0
 Lconc = 1.0
+(continues on next page)
+
+9.1. The PySCeS Model Description Language
+
+47
+
+PySCeS User Guide, Release 1.1.0
+
+(continued from previous page)
+
 Pconc = 1.0
 # Species initialisations
 N@Vout = 3.07e5
 Pmem@Mem_Area = 37.38415
 Lmem@Mem_Area = 8291.2350678770199
 M@Vcyt = 199693.0
 L@Vcyt = 102004
@@ -1687,15 +1756,15 @@
 """
 Simulate this model to 200 for maximum happiness and
 watch the surface to volume ratio and scaled concentrations.
 """
 This example illustrates almost all of the features included in the PySCeS MDL. Although it may be
 slightly more complicated than the basic model described above it is still, by our definition, human readable.
 
-46
+48
 
 Chapter 9. Input file guide
 
 CHAPTER
 
 TEN
 
@@ -1723,20 +1792,21 @@
 Reset the number of steps of timer <name> in the TimerBox to zero
 • name the step timer whose steps should be reset
 step_timer(name, maxsteps)
 Creates a step timer method with <name> in the TimerBox instance. Step timers print the
 elapsed time as well as the next step out of maxsteps when called.
 • name the timer name
 • maxsteps the maximum number of steps associated with this timer
-stop(name)
-Delete the timer <name> from the TimerBox instance
 
-47
+49
+
+PySCeS User Guide, Release 1.1.0
 
-PySCeS User Guide, Release 1.0.0
+stop(name)
+Delete the timer <name> from the TimerBox instance
 • name the timer name to delete
 pysces.PyscesUtils.VersionCheck(ver='0.1.5')
 class pysces.PyscesUtils.WriteOutput
 This code is adapted from:
 CBMPy: CBTools module
 Constraint Based Modelling in Python (http://cbmpy.sourceforge.net) Copyright (C) 2009-2017
 Brett G. Olivier, VU University Amsterdam, Amsterdam, The Netherlands
@@ -1763,23 +1833,23 @@
 • names the list of row names
 • fname the output filename
 exportLabelledArray2TXT(arr, names, fname)
 Export an array with row names to fname.txt
 • arr the an array like object
 • names the list of row names
 • fname the output filename
-exportLabelledArrayWithHeader(arr, names, header, fname, sep=',', format='%f')
-Export an array with row names and header
-• arr the an array like object
 
-48
+50
 
 Chapter 10. Module documentation
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
+exportLabelledArrayWithHeader(arr, names, header, fname, sep=',', format='%f')
+Export an array with row names and header
+• arr the an array like object
 • names the list of row names
 • header the list of column names
 • fname the output filename
 • sep [default=’,’] the column separator
 • format [default=’%s’] the output number format
 • appendlist [default=False] if True append the array to fname otherwise create a new file
 exportLabelledArrayWithHeader2CSV(arr, names, header, fname)
@@ -1805,17 +1875,17 @@
 • appendlist [default=False] if True append the array to fname otherwise create a new file
 pysces.PyscesUtils.str2bool(s)
 Tries to convert a string to a Python boolean
 • s True if ‘True’, ‘true’ or’1’ else False
 
 10.1. PySCeS Module documentation
 
-49
+51
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 10.1.2 PyscesPlot2
 PyscesPlot2 is a new graphics susbsystem for PySCeS which will include a Unified Plotting Interface
 which can take advantage of different plotting backends via a common user interface.
 class pysces.PyscesPlot2.FIFOBuffer(size)
 Simple fixed size FIFO buffer.
 add(x)
@@ -1858,22 +1928,23 @@
 Write a GnuPlot format 3D dataset. The yaxis argument specifies the column that should be
 used to split the dataset into GnuPlot slices.
 • arr the array (r>1, c>2)
 • fmt default ‘%.8e’
 • yaxis default 1
 g_pause()
 A small pause defined by self.PAUSE_TIME (multiplied by 2 when in multiplot).
-g_write(cmd)
-Write a command to the GnuPlot interpreter
 
-50
+52
 
 Chapter 10. Module documentation
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
+
+g_write(cmd)
+Write a command to the GnuPlot interpreter
 • cmd the GnuPlot command
 plot(data, x, y, title='', format='w l')
 Plot a single line data[y] vs data[x] where:
 • data the data array
 • x x column index
 • y y column index
 • title is the line key
@@ -1901,22 +1972,23 @@
 set(key, value='')
 Send set <key> or optionally set <key> <value> to GnuPlot.
 setAxisLabel(axis, label='')
 Set the axis label:
 • axis = x, y, z, xy, xz, yz, zyx
 • label = string (default=”)
 Called with only the axis argument clears the axis label.
-setDataFileNumberFormat(format='%.8e')
-Sets the format string for data written to file
-• format format string (default=’%.8e’)
 10.1. PySCeS Module documentation
 
-51
+53
+
+PySCeS User Guide, Release 1.1.0
 
-PySCeS User Guide, Release 1.0.0
+setDataFileNumberFormat(format='%.8e')
+Sets the format string for data written to file
+• format format string (default=’%.8e’)
 setGraphTitle(title='PySCeS Plot')
 Set the graph title, unset if title argument is None
 • title (string, default=’PySCeS Plot’) the graph title
 setGrid(value)
 Display or remove graph grid.
 • value (boolean) True (on) or False (off)
 setKey(value=False)
@@ -1943,25 +2015,25 @@
 If only the axis argument is provided, GnuPlot will autoscale the ranges to the data.
 setSize(width=1.0, height=1.0)
 Set the size of the next plot relative to the GnuPlot canvas (e.g. screen) size which is defined
 to be 1. For example if width = height = 0.5 the plot is 1/4 the size of the viewable
 canvas. If no arguments are supplied reset size to 1,1.
 • width of next plot (default = 1.0)
 • height of next plot (default = 1.0)
+
+54
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
 setSizeAndOrigin(width=1, height=1, xpos=0, ypos=0)
 Set the size and origin of the next plot. If no arguments are supplied, reset the size to 1,1 and
 origin to 0.0
 • width of next plot (default = 1.0)
 • height of next plot (default = 1.0)
-
-52
-
-Chapter 10. Module documentation
-
-PySCeS User Guide, Release 1.0.0
 • xpos of next plot (default = 0)
 • ypos of next plot (default = 0)
 setTerminal(name, options='')
 Sets the terminal, gnuplot: set terminal name options
 splot(data, x, y, z, titles='', format='w l')
 Plot a surface data[z] vs data[y] vs data[x] where:
 • data the data array
@@ -1988,28 +2060,28 @@
 class pysces.PyscesPlot2.MatplotlibUPI(work_dir=None, backend=None)
 Refactored Matplotlib backend to the Unified Plotting Interface
 • work_dir (optional) working directory
 CommonStyleDefs = {'lines':
 
 '-', 'points':
 
+10.1. PySCeS Module documentation
+
 'o'}
 
+55
+
+PySCeS User Guide, Release 1.1.0
+
 MAX_OPEN_WINDOWS = 10
 closeAll()
 Close all open matplotlib figures.
 export(name, directory=None, outtype='png')
 Export the current plot as a <format> file.
 • filename the filename
-
-10.1. PySCeS Module documentation
-
-53
-
-PySCeS User Guide, Release 1.0.0
 • directory optional (default = current working directory)
 • outtype the file format (default=’png’).
 Currently only PNG is guaranteed to be available in all interfaces.
 hold(hold=False)
 Enable plot holding where each new graph is plotted on top of the previous one.
 • hold boolean (default = False)
 isnotebook()
@@ -2031,27 +2103,28 @@
 If formats only contains a single item, this format is used for all lines and can also be the
 CommonStyle ‘lines’ or ‘points’.
 pyplot = None
 save(name, directory=None, dfmt='%.8e')
 Save the plot data to
 • filename the filename
 • directory optional (default = current working directory)
+
+56
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
 • dfmt the data format string (default=’%.8e’)
 setAxisLabel(axis, label='')
 Set the axis label:
 • axis = x, y, z, xy, xz, yz, zyx
 • label = string (default=”)
 Called with only the axis argument clears the axis label.
 setGraphTitle(title='PySCeS Plot')
 Set the graph title, unset if title=None
-54
-
-Chapter 10. Module documentation
-
-PySCeS User Guide, Release 1.0.0
 • title (string, default=’PySCeS Plot’) the graph title
 setGrid(value)
 Display or remove graph grid.
 • value (boolean) True (on) or False (off)
 setKey(value=False)
 Enable or disable the current plot key, no arguments removes key.
 • value boolean (default = False)
@@ -2079,29 +2152,29 @@
 
 ''}
 
 axisInputStringToList(input)
 Extracts axis information from a string input, returns a boolean triple representing
 (x=True/False, y=True/False, z=True/False).
 • input the input string
+
+10.1. PySCeS Module documentation
+
+57
+
+PySCeS User Guide, Release 1.1.0
 export(name, directory=None, outtype='png')
 Export the current plot as a <format> file.
 • filename the filename
 • directory optional (default = current working directory)
 • outtype the file format (default=’png’).
 Currently only PNG is guaranteed to be available in all interfaces.
 plot(data, x, y, title='', format='')
 Plot a single line data[y] vs data[x] where:
 • data the data array
-
-10.1. PySCeS Module documentation
-
-55
-
-PySCeS User Guide, Release 1.0.0
 • x x column index
 • y y column index
 • title is the line key
 • format is the XXX format string (default=”)
 Format can also be the CommonStyle ‘lines’ or ‘points’
 plotLines(data, x, y=[], titles=[], formats=[''])
 Plot a multiple lines data[y1, y2, ] vs data[x] where:
@@ -2121,30 +2194,30 @@
 Set the axis label:
 • axis = x, y, z, xy, xz, yz, zyx
 • label = string (default=”)
 Called with only the axis argument clears the axis label.
 setGraphTitle(title='PySCeS Plot')
 Set the graph title, unset if title=None
 • title (string, default=’PySCeS Plot’) the graph title
+
+58
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
+
 setGrid(value)
 Display or remove graph grid.
 • value (boolean) True (on) or False (off)
 setKey(value=False)
 Enable or disable the current plot key, no arguments removes key.
 • value boolean (default = False)
 setLogScale(axis)
 Set axis to logscale where:
 • axis = x, y, z, xy, xz, yz, zyx
-
-56
-
-Chapter 10. Module documentation
-
-PySCeS User Guide, Release 1.0.0
-
 setNoLogScale(axis)
 Set axis to a linear scale where:
 • axis = x, y, z, xy, xz, yz, zyx
 setRange(axis, min=None, max=None)
 Set axis range where
 • axis = x, y, z, xy, xz, yz, zyx
 • min = range(s) lower bound (default=None) autoscale
@@ -2164,32 +2237,32 @@
 • x x column index
 • y y column index
 • z list of z column indexes, if empty all of z not including x, y are plotted
 • titles is a list of surface keys, if empty Surf1, Surf2, Surf3 is used
 • formats is a list (per line) of XXX format strings (default=”).
 If formats only contains a single item, this format is used for all surfaces and can also be the
 CommonStyle ‘lines’ or ‘points’.
+
+10.1. PySCeS Module documentation
+
+59
+
+PySCeS User Guide, Release 1.1.0
+
 wait(seconds=3)
 Wait seconds (default = 3) or until enter is pressed (seconds = -1)
 class pysces.PyscesPlot2.PyscesUPI
 This is the frontend to the PySCeS Unified Plotting Interface (pysces.plt.*) that allows one to
 specify which backend should be used to plot when a UPI method is called. More than one interface
 can be active at the same time and so far the Matplotlib and GnuPlot backends are available for
 use.
 This is an experiment which must be refactored into a more general way of doing things. Basically,
 I want an instance of the abstract plotting class which will plot to one, any or all currently available
 backends. If anybody has an idea how I can generate this class automatically please let me know
 ;-)
-
-10.1. PySCeS Module documentation
-
-57
-
-PySCeS User Guide, Release 1.0.0
-
 closeAll()
 Close all active Matplolib figures
 export(name, directory=None, outtype='png')
 Export the current plot as a <format> file.
 • filename the filename
 • directory optional (default = current working directory)
 • outtype the file format (default=’png’).
@@ -2209,31 +2282,30 @@
 • name the interface name currently one of [‘matplotlib’,’gnuplot’]
 • instance an instance of a PlotBase derived (UPI) interface
 plot(data, x, y, title='', format='')
 Plot a single line data[y] vs data[x] where:
 • data the data array
 • x x column index
 • y y column index
+
+60
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
 • title is the line key
 • format is the backend format string (default=”)
 plotLines(data, x, y=[], titles=[], formats=[''])
 Plot a multiple lines data[y1, y2, ] vs data[x] where:
 • data the data array
 • x x column index
 • y is a list of line indexes, if empty all of y not including x is plotted
 • titles is a list of line keys, if empty Line1,Line2,Line3 is used
 • formats is a list (per line) of XXX format strings.
 If formats only contains a single item, this format is used for all lines.
-
-58
-
-Chapter 10. Module documentation
-
-PySCeS User Guide, Release 1.0.0
-
 replot()
 Replot the current figure for all active interfaces
 save(name, directory=None, dfmt='%.8e')
 Save the plot data and (optionally) XXX format file
 • filename the filename
 • directory optional (default = current working directory)
 • dfmt the data format string (default=’%.8e’)
@@ -2250,33 +2322,35 @@
 • value (boolean) True (on) or False (off)
 setKey(value=False)
 Enable or disable the current plot key, no arguments removes key.
 • value boolean (default = False)
 setLogScale(axis)
 Set axis to logscale where:
 • axis = x, y, z, xy, xz, yz, zyx
+
+10.1. PySCeS Module documentation
+
+61
+
+PySCeS User Guide, Release 1.1.0
+
 setNoLogScale(axis)
 Set axis to a linear scale where:
 • axis = x, y, z, xy, xz, yz, zyx
 setRange(axis, min=None, max=None)
 Set axis range where
 • axis = x, y, z, xy, xz, yz, zyx
 • min = range(s) lower bound (default=None) autoscale
 • max = range(s) upper bound (default=None) autoscale
 splot(data, x, y, z, titles='', format='')
 Plot a surface data[z] vs data[y] vs data[x] where:
 • data the data array
 • x x column index
 • y y column index
 • z z column index
-10.1. PySCeS Module documentation
-
-59
-
-PySCeS User Guide, Release 1.0.0
 • titles is a list of surface keys whose len matches data columns
 • format is the XXX format string (default=”)
 splotSurfaces(data, x, y, z=[], titles=[], formats=[''])
 Plot data[z1, z2, ] vs data[y] vs data[x] where:
 • data the data array
 • x x column index
 • y y column index
@@ -2289,14 +2363,21 @@
 This module contains the core PySCeS classes which create the model and associated data objects
 class pysces.PyscesModel.BagOfStuff(matrix, row, col)
 A collection of attributes defined by row and column lists used by Response coefficients etc matrix
 is an array of values while row/col are lists of row colummn name strings
 col = None
 get(attr1, attr2)
 Returns a single attribute “attr1_attr2” or None
+
+62
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
+
 list()
 Return all attributes as a attr:val dictionary
 listAllOrdered(order='descending', absolute=True)
 Return an ordered list of (attr, value) tuples
 • order [default=’descending’] the order to return as: ‘descending’ or ‘ascending’
 • absolute [default=True] use the absolute value
 load()
@@ -2307,30 +2388,35 @@
 an index for both left and right attr then: search=’a’ : both left and right attributes (default)
 search=’l’ : left attributes only search=’r’ : right attributes
 class pysces.PyscesModel.Event(name, mod)
 Events have triggers and fire EventAssignments when required. Ported from Core2.
 assignments = None
 code_string = None
 delay = 0.0
-60
-
-Chapter 10. Module documentation
-
-PySCeS User Guide, Release 1.0.0
-
 formula = None
 mod = None
+persistent = True
 piecewises = None
+priority = None
 reset()
 setAssignment(var, formula)
+setPersistent(persistent)
+setPriority(priority)
 setTrigger(formula, delay=0.0)
 state = False
 state0 = False
 symbols = None
 trigger = None
+
+10.1. PySCeS Module documentation
+
+63
+
+PySCeS User Guide, Release 1.1.0
+
 xcode = None
 class pysces.PyscesModel.EventAssignment(name, mod)
 Event assignments are actions that are triggered by an event. Ported from Core2 to build an event
 handling framework fro PySCeS
 code_string = None
 evaluateAssignment()
 formula = None
@@ -2345,31 +2431,31 @@
 handle_event(solver, event_info)
 Defines how to handle a discontinuity. This functions gets called when a discontinuity has
 been found in the supplied event functions. The solver is the solver attribute while the
 event_info is a list of length 2 where the first element is a list containing information about
 state events and the second element is a Boolean for indicating if there has been a time event.
 If there has not been a state event the first element is an empty list. The state event list contains
 a set of integers of values (-1,0,1), the values indicates which state event has triggered (determined from state_event(. . . ) ) and the value indicates to where the state event is ‘headed’.
+setSequence(event_list)
 state_events(t, y, sw)
 class pysces.PyscesModel.Function(name, mod)
 Function class ported from Core2 to enable the use of functions in PySCeS.
 addFormula(formula)
-
-10.1. PySCeS Module documentation
-
-61
-
-PySCeS User Guide, Release 1.0.0
-
 argsl = None
 code_string = None
 formula = None
 functions = None
 mod = None
 piecewises = None
+
+64
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
 setArg(var, value=None)
 symbols = None
 value = None
 xcode = None
 class pysces.PyscesModel.IntegrationDataObj
 This class is specifically designed to store the results of a time simulation It has methods for setting
 the Time, Labels, Species and Rate data and getting Time, Species and Rate (including time) arrays.
@@ -2394,22 +2480,22 @@
 getDataInTimeInterval(time, bounds=None)
 getDataInTimeInterval(time, bounds=None) returns an array of all data points where: timebounds <= time <= time+bounds where bound defaults to stepsize
 getOutput(*args, **kwargs)
 Old alias for getSimData() getOutput(*args) feed this method species/rate labels and it will
 return an array of [time, sp1, r1, . . . .]
 getRates(lbls=False)
 return time+rate array
-62
+getRules(lbls=False)
+Return time+rule array
 
-Chapter 10. Module documentation
+10.1. PySCeS Module documentation
 
-PySCeS User Guide, Release 1.0.0
+65
 
-getRules(lbls=False)
-Return time+rule array
+PySCeS User Guide, Release 1.1.0
 getSimData(*args, **kwargs)
 getSimData(*args) feed this method species/rate labels and it will return an array of [time,
 sp1, r1, . . . .]
 getSpecies(lbls=False)
 return time+species array
 getTime(lbls=False)
 return the time vector
@@ -2433,39 +2519,25 @@
 Sets extra simulation data
 species = None
 species_labels = None
 time = None
 time_label = 'Time'
 xdata = None
 xdata_labels = None
-class pysces.PyscesModel.NewCoreBase
-Core2 base class, needed here as we use Core2 derived classes in PySCes
-get(attr)
-Return an attribute whose name is str(attr)
-getName()
-name = None
-
-10.1. PySCeS Module documentation
-
-63
-
-PySCeS User Guide, Release 1.0.0
-
-setName(name)
-class pysces.PyscesModel.NumberBase
-Derived Core2 number class.
-getValue()
-setValue(v)
-value = None
-value_initial = None
 class pysces.PyscesModel.PieceWise(pwd, mod)
 Generic piecewise class adapted from Core2 that generates a compiled Python code block that
 allows evaluation of arbitrary length piecewise functions. Piecewise statements should be defined
 in assignment rules as piecewise(<Piece>, <Conditional>, <OtherValue>) where there can be an
 arbitrary number of <Piece>, <Conditional> pairs.
+
+66
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
 • args a dictionary of piecewise information generated by the InfixParser as InfixParser.piecewises
 code_string = None
 formula = None
 name = None
 value = None
 xcode = None
 class pysces.PyscesModel.PysMod(File=None, dir=None, loader='file', fString=None,
@@ -2485,26 +2557,28 @@
 Arguments:
 initial: vector containing initial species concentrations
 CVODE_VPYTHON(s)
 Future VPython hook for CVODE
 CVODE_continue(tvec)
 Experimental: continues a simulation over a new time vector, the CVODE memobj is reused
 and not reinitialised and model parameters can be changed between calls to this method. The
-64
-
-Chapter 10. Module documentation
-
-PySCeS User Guide, Release 1.0.0
 mod.data_sim objects from the initial simulation and all calls to this method are stored in the
 list mod.CVODE_continuous_result.
 • tvec a numpy array of time points
 CVODE_continuous_result = None
 CleanNaNsFromArray(arr, replace_val=0.0)
 Scan a matrix for NaN’s and replace with zeros:
 • arr the array to be cleaned
+
+10.1. PySCeS Module documentation
+
+67
+
+PySCeS User Guide, Release 1.1.0
+
 EvalCC()
 Calculate the MCA control coefficients using the current steady-state solution.
 mod.__settings__[“mca_ccj_upsymb”] = 1 attach the flux control coefficients to the model
 instance mod.__settings__[“mca_ccs_upsymb”] = 1 attach the concentration control coefficients to the model instance
 Arguments: None
 EvalEigen()
 Calculate the eigenvalues or vectors of the unscaled Jacobian matrix and thereby analyse the
@@ -2529,36 +2603,38 @@
 Both inputs (input1=species,input2=rates) should be valid (steady state for MCA) solutions
 and given in the correct order for them to be used. If either or both are missing the last state
 values are used automatically. Elasticities are scaled using input 1 and 2.
 Arguments:
 - input [default=None]: species concentration vector
 - input2 [default=None]: reaction rate vector
 Settings, set in mod.__settings__:
-10.1. PySCeS Module documentation
-
-65
-
-PySCeS User Guide, Release 1.0.0
-
 - elas_evar_upsymb
 [default = 1] attach individual elasticity␣
 ˓→symbols to model instance
 - elas_zero_conc_fix [default=False] if zero concentrations are␣
 ˓→detected in a steady-state solution make it a very small number
 - elas_zero_flux_fix [default=False] if zero fluxes are detected in␣
 ˓→a steady-state solution make it a very small number
 - elas_scaling_div0_fix [default=False] if INf's are detected after␣
 ˓→scaling set to zero
+
+68
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
+
 EvalRC()
 Calculate the MCA response coefficients using the current steady-state solution.
 Arguments: None
 EvalRCT()
 Calculate the MCA response coefficients using the current steady-state solution.
 Responses to changes in the sums of moiety conserved cycles are also calculated.
 Arguments: None
+ExecRateRules()
 FINTSLV(initial)
 Forward integration steady-state solver. Finds a steady state when the maximum change in
 species concentration falls within a specified tolerance. Returns the steady-state solution and
 a error flag. Algorithm controls are available as mod.fintslv_<control>
 Arguments:
 initial: vector of initial concentrations
 Fix_S_fullinput(s_vec)
@@ -2574,27 +2650,27 @@
 Deprecated
 FluxGenSim(s)
 Deprecated
 Forcing_Function()
 User defined forcing function either defined in the PSC input file as !F or by overwriting this
 method. This method is evaluated prior to every rate equation evaluation.
 Arguments: None
-
-66
-
-Chapter 10. Module documentation
-
-PySCeS User Guide, Release 1.0.0
-
 HYBRD(initial)
 PySCeS interface to the HYBRD solver. Returns a steady-state solution and error flag. Good
 general purpose solver. Algorithm controls are available as mod.hybrd_<control>
 Arguments:
 initial: vector of initial species concentrations
 InitialiseCompartments()
+
+10.1. PySCeS Module documentation
+
+69
+
+PySCeS User Guide, Release 1.1.0
+
 InitialiseConservationArrays()
 Initialise conservation related vectors/array was in InitialiseModel but has been moved out
 so is can be called by when the stoichiometry is reanalysed
 InitialiseEvents()
 InitialiseFunctions()
 InitialiseInputFile()
 Parse the input file associated with the PySCeS model instance and assign the basic model
@@ -2621,25 +2697,24 @@
 filename is not supplied the pysces.model_dir directory contents is displayed and the model
 name can be entered at the promp (<ctrl>+C exits the loading process).
 Arguments:
 File [default=None]: the name of the PySCeS input file dir [default=pysces.model_dir]: the
 optional directory where the PSC file can be found
 LoadFromString(File=None, fString=None)
 Docstring required
-
-10.1. PySCeS Module documentation
-
-67
-
-PySCeS User Guide, Release 1.0.0
-
 ModelLoad(stoich_load=0)
 Load and instantiate a PySCeS model so that it can be used for further analyses. This function
 replaces the pre-0.7.1 doLoad() method.
 • stoich_load try to load a structural analysis saved with Stoichiometry_Save_Serial() (default=0)
+70
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
+
 NLEQ2(initial)
 PySCeS interface to the (optional) NLEQ2 algorithm. This is a powerful steady-state solver
 that can usually find a solution for when HYBRD() fails. Algorithm controls are available
 as: mod.nleq2_<control> Returns as steady-state solution and error flag.
 Arguments:
 initial: vector of initial species concentrations
 PITCON(scanpar, scanpar3d=None)
@@ -2667,23 +2742,23 @@
 Scale the K and L matrices with current steady state (if either input1 or 2 == None) or user
 input.
 Arguments:
 input: vector of species concentrations input2: vector of reaction rates
 Scan1(range1=[], runUF=0)
 Perform a single dimension parameter scan using the steady-state solvers. The parameter to
 be scanned is defined (as a model attribute “P”) in mod.scan_in while the required output is
-68
-
-Chapter 10. Module documentation
-
-PySCeS User Guide, Release 1.0.0
 entered into the list mod.scan_out. Results of a parameter scan can be easilly viewed with
 Scan1Plot().
 mod.scan_in - a model attribute written as in the input file (eg. P, Vmax1 etc) mod.scan_out
 - a list of required output [‘A’,’T2’, ‘ecR1_s1’, ‘ccJR1_R1’, ‘rcJR1_s1’, . . . ] mod.scan_res
+10.1. PySCeS Module documentation
+
+71
+
+PySCeS User Guide, Release 1.1.0
 - the results of a parameter scan mod.scan - numpy record array with the scan results (scan_in and scan_out), call as mod.scan.Vmax, mod.scan.A_ss, mod.scan.J_R1, etc.
 mod.__settings__[“scan1_mca_mode”] - force the scan algorithm to evaluate the elasticities
 (1) and control coefficients (2) (this should also be auto-detected by the Scan1 method).
 Arguments:
 range1 [default=[]]: a predefined range over which to scan. runUF [default=0]: run (1) the
 user defined function mod.User_Function (!U) before evaluating the steady state.
 Scan1Plot(plot=[], title=None, log=None, format='lines', filename=None)
@@ -2710,22 +2785,23 @@
 SerialDecode(filename)
 Decode and return a serialised object saved with SerialEncode.
 Arguments:
 filename: the filename (.pscdat is assumed)
 SerialEncode(data, filename)
 Serialise and save a Python object using a binary pickle to file. The serialised object is saved
 as <filename>.pscdat in the directory defined by mod.model_serial.
+Arguments:
+data: pickleable Python object filename: the ouput filename
 
-10.1. PySCeS Module documentation
+72
 
-69
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
 
-PySCeS User Guide, Release 1.0.0
-Arguments:
-data: pickleable Python object filename: the ouput filename
 SetLoud()
 Turn on as much solver reporting noise as possible: mod.__settings__[‘hybrd_mesg’]
 = 1 mod.__settings__[‘nleq2_mesg’] = 1 mod.__settings__[“lsoda_mesg”] = 1
 mod.__settings__[‘mode_state_mesg’] = 1 mod.__settings__[‘scan1_mesg’] = 1
 mod.__settings__[‘solver_switch_warning’] = True
 Arguments: None
 SetQuiet()
@@ -2754,26 +2830,27 @@
 PySCeS integration driver routine that evolves the system over the time. Resulting array of
 species concentrations is stored in the mod.data_sim object Initial concentrations can be
 selected using mod.__settings__[‘mode_sim_init’] (default=0):
 • 0 initialise with intial concentrations
 • 1 initialise with a very small (close to zero) value
 • 2 initialise with results of previously calculated steady state
 • 3 initialise with final point of previous simulation
+userinit values can be (default=0):
 
-70
+10.1. PySCeS Module documentation
 
-Chapter 10. Module documentation
+73
 
-PySCeS User Guide, Release 1.0.0
-userinit values can be (default=0):
-• 0: initial species concentrations intitialised from (mod.S_init), time array calculated from sim_start/sim_end/sim_points
+PySCeS User Guide, Release 1.1.0
+• 0: initial species concentrations intitialised from (mod.S_init),
+time array calculated from sim_start/sim_end/sim_points
 • 1: intial species concentrations intitialised from (mod.S_init) existing
 “mod.sim_time” used directly
-• 2: initial species concentrations read from “mod.__inspec__”, “mod.sim_time”
-used directly
+• 2: initial species concentrations read from “mod.__inspec__”,
+“mod.sim_time” used directly
 State()
 PySCeS non-linear solver driver routine.
 Solve for a steady state using HYBRD/NLEQ2/FINTSLV algorithms.
 Results are stored in mod.state_species and
 mod.state_flux. The results of a steady-state analysis can be viewed with the mod.showState()
 method.
 The solver can be initialised in 3 ways using the mode_state_init switch. mod.mode_state_init
@@ -2796,23 +2873,21 @@
 Arguments:
 override [default=0]: override stoichiometric analysis intialisation from parsed data load [default=0]: load a presaved stoichiometry
 Stoichiometry_Init(nmatrix, load=0)
 Initialize the model stoichiometry. Given a stoichiometric matrix N, this method will return an instantiated PyscesStoich instance and status flag. Alternatively, if load is enabled,
 PySCeS will attempt to load a previously saved stoichiometric analysis (saved with Stoichiometry_Save_Serial) and test it’s correctness. The status flag indicates 0 = reanalyse stoichiometry or 1 = complete structural analysis preloaded.
 Arguments:
 nmatrix: The input stoichiometric matrix, N load [default=0]: try to load a saved stoichiometry (1)
-
-10.1. PySCeS Module documentation
-
-71
-
-PySCeS User Guide, Release 1.0.0
-
 Stoichiometry_Load_Serial()
 Load a saved stoichiometry saved with mod.Stoichiometry_Save_Serial() and return a stoichiometry instance.
+74
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
 Arguments: None
 Stoichiometry_ReAnalyse()
 Reanalyse the stoichiometry using the current N matrix ie override=1 (for use with
 mod.Stoich_matrix_SetValue)
 Arguments: None
 Stoichiometry_Save_Serial()
 Serialize and save a Stoichiometric instance to binary pickle Stoichiometry_Save_Serial()
@@ -2844,19 +2919,19 @@
 input: the array to be written File [default=None]: an open, writable Python file object Row
 [default=None]: a list of row labels Col [default=None]: a list of column labels name [default=None]: an HTML table description line close_file [default=0]: close the file after write
 (1) or leave open (0)
 Write_array_latex(input, File=None, Row=None, Col=None, close_file=0)
 Write an array to an open file as a ‘LaTeX’ {array}
 Arguments:
 
-72
+10.1. PySCeS Module documentation
 
-Chapter 10. Module documentation
+75
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 input: the array to be written File [default=None]: an open, writable Python file object Row
 [default=None]: a list of row labels Col [default=None]: a list of column labels close_file
 [default=0]: close the file after write (1) or leave open (0)
 clone()
 Returns a deep copy of this model object (experimental!)
 doEigen()
 Calculate the eigenvalues, automatically performs a steady state and elasticity analysis.
@@ -2887,20 +2962,19 @@
 Arguments: None
 doMcaRC()
 doMca()
 Perform a complete Metabolic Control Analysis on the model, automatically calculates a
 steady state.
 Calls: State() EvalEvar() EvalEpar() EvalCC() EvalRC()
 Arguments: None
+76
 
-10.1. PySCeS Module documentation
-
-73
+Chapter 10. Module documentation
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 doMcaRCT()
 Perform a complete Metabolic Control Analysis on the model, automatically calculates a
 steady state.
 In additional, response coefficients to the sums of moiety-conserved cycles are calculated.
 Calls: State() EvalEvar() EvalEpar() EvalCC() EvalRC() EvalRCT()
 Arguments: None
@@ -2929,32 +3003,32 @@
 Calls: State()
 Arguments: None
 doStateShow()
 Calculate the steady-state solution of a system and show the results.
 Calls: State() showState()
 Arguments: None
 
-74
+10.1. PySCeS Module documentation
 
-Chapter 10. Module documentation
+77
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 exportSimAsSedML(output='files', return_sed=False, vc_given='PySCeS',
 vc_family='Software', vc_email='', vc_org='pysces.sourceforge.net')
 Exports the current simulation as SED-ML in various ways it creates and stores the SED-ML
 files in a folder generated from the model name.
 • output [default=’files’] the SED-ML export type can be one or more comma separated
 e.g. ‘files,combine’
 • files export the plain SBML and SEDML XML files
 • archive export as a SED-ML archive <file>.sedx containing the SBML and SEDML xml
 files
 • combine export as a COMBINE archive <file>.omex containing the SBML, SEDML,
 manifest (XML) and metadata (RDF) - vc_given [default=’PySCeS’] - vc_family [default=’Software’] - vc_email [default=’bgoli@users.sourceforge.net’] - vc_org [default=’<pysces.sourceforge.net>’]
 random = <module 'pysces.PyscesRandom' from
-'/home/jr/src/git/pysces/pysces/PyscesRandom.py'>
+'/home/jr/src/git/pysces/docs/source/../../pysces/PyscesRandom.py'>
 reLoad(stoich_load=0)
 Re-load and instantiate a PySCeS model so that it can be used for further analyses. This is
 just a convenience call to the ModelLoad() method.
 • stoich_load try to load a structural analysis saved with Stoichiometry_Save_Serial() (default=0)
 property scan
 showCC(File=None)
 Print all control coefficients as ‘LaTex’ formatted strings to the screen or file.
@@ -2970,20 +3044,19 @@
 Arguments:
 File [default=None]: an open, writable Python file object
 showElas(File=None)
 Print all elasticities to screen or file as ‘LaTeX’ compatible strings. Calls showEvar() and
 showEpar()
 Arguments:
 File [default=None]: an open writable Python file object
+78
 
-10.1. PySCeS Module documentation
-
-75
+Chapter 10. Module documentation
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 showEpar(File=None)
 Write out all nonzero parameter elasticities as ‘LaTeX’ formatted strings, alternatively write
 to file.
 Arguments:
 File [default=None]: an open writable Python file object
 showEvar(File=None)
@@ -3013,20 +3086,19 @@
 showModifiers(File=None)
 Prints the current value of the model’s modifiers per reaction to screen or file.
 Arguments:
 File [default=None]: an open, writable Python file object
 showN(File=None, fmt='%2.3f')
 Print the stoichiometric matrix (N), including row and column labels to screen or File.
 Arguments:
+10.1. PySCeS Module documentation
 
-76
-
-Chapter 10. Module documentation
+79
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 File [default=None]: an open, writable Python file object fmt [default=’%2.3f’]: output number format
 showNr(File=None, fmt='%2.3f')
 Print the reduced stoichiometric matrix (Nr), including row and column labels to screen or
 File.
 Arguments:
 File [default=None]: an open, writable Python file object fmt [default=’%2.3f’]: output number format
 showODE(File=None, fmt='%2.3f')
@@ -3054,32 +3126,32 @@
 Arguments:
 File [default=None]: an open, writable Python file object
 showSpeciesFixed(File=None)
 Prints the current value of the model’s fixed species values (mod.X) to screen or file.
 Arguments:
 File [default=None]: an open, writable Python file object
 
-10.1. PySCeS Module documentation
+80
 
-77
+Chapter 10. Module documentation
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 showSpeciesI(File=None)
 Prints the current value of the model’s variable species initial values (mod.X_init) to screen
 or file.
 Arguments:
 File [default=None]: an open, writable Python file object
 showState(File=None)
 Prints the result of the last steady-state analyses. Both steady-state flux’s and species concentrations are shown.
 Arguments:
 File [default=None]: an open, writable Python file object
 property sim
 class pysces.PyscesModel.ReactionObj(mod, name, kl, klrepl='self.')
-Defines a reaction with a KineticLaw kl8, *formula and name bound to a model instance, mod.
+Defines a reaction with a KineticLaw kl, formula and name bound to a model instance, mod.
 code_string = None
 compartment = None
 formula = None
 mod = None
 piecewises = None
 rate = None
 setKineticLaw(kl, klrepl='self.')
@@ -3092,24 +3164,24 @@
 HAS_MOD_DATA = False
 HAS_RULES = False
 HAS_SET_LABELS = False
 HAS_SPECIES = False
 HAS_XDATA = False
 OPEN = True
 addModData(mod, *args)
+
+10.1. PySCeS Module documentation
+
+81
+
+PySCeS User Guide, Release 1.1.0
 addPoint(ipar, ssdata)
 takes a list/array of input parameter values and the associated ssdata object
 closeScan()
 flux_labels = None
-78
-
-Chapter 10. Module documentation
-
-PySCeS User Guide, Release 1.0.0
-
 fluxes = None
 getAllScanData(lbls=False)
 getFluxes(lbls=False)
 getModData(lbls=False)
 getRules(lbls=False)
 getScanData(*args, **kwargs)
 getScanData(*args) feed this method species/flux/rule/mod labels and it will return an array
@@ -3129,30 +3201,30 @@
 xdata = None
 xdata_labels = None
 class pysces.PyscesModel.StateDataObj
 New class used to store steady-state data.
 HAS_FLUXES = False
 HAS_RULES = False
 HAS_SPECIES = False
+
+82
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
+
 HAS_XDATA = False
 IS_VALID = True
 flux_labels = None
 fluxes = None
 getAllStateData(lbls=False)
 Return all available data as species+fluxes+rules if lbls=True returns (array,labels) else just
 array
 getFluxes(lbls=False)
 return flux array
-
-10.1. PySCeS Module documentation
-
-79
-
-PySCeS User Guide, Release 1.0.0
-
 getRules(lbls=False)
 Return rule array
 getSpecies(lbls=False)
 return species array
 getStateData(*args, **kwargs)
 getSimData(*args) feed this method species/rate labels and it will return an array of [time,
 sp1, r1, . . . .]
@@ -3172,25 +3244,26 @@
 species_labels = None
 xdata = None
 xdata_labels = None
 class pysces.PyscesModel.WasteManagement
 pysces.PyscesModel.chkmdir()
 Import and grab pysces.model_dir
 Arguments: None
+
+10.1. PySCeS Module documentation
+
+83
+
+PySCeS User Guide, Release 1.1.0
+
 pysces.PyscesModel.chkpsc(File)
 Chekc whether the filename “File” has a ‘.psc’ extension and adds one if not.
 Arguments:
 File: filename string
 
-80
-
-Chapter 10. Module documentation
-
-PySCeS User Guide, Release 1.0.0
-
 10.1.4 PyscesScan
 PySCeS classes for continuations and multi-dimensional parameter scans
 class pysces.PyscesScan.PITCONScanUtils(model)
 Static Bifurcation Scanning utilities using PITCON, call with loaded model object. Hopefully
 nobody else was trying to use the older class as it was horrible. This new one is is leaner, meaner
 and pretty cool ;-)
 analyseData(analysis='elas')
@@ -3212,28 +3285,29 @@
 pitcon_range_low = None
 pitcon_res = None
 pitcon_scan_density = None
 pitcon_scan_parameter = None
 pitcon_scan_parameter_3d = None
 res_eigen = None
 res_flux = None
+
+84
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
+
 res_idx = None
 res_metab = None
 res_user = None
 runContinuation(parameter, low, high, density, par3d=None, logrange=True,
 runQuiet=True)
 Run the continuation using the following parameters:
 Args:
 • parameter = str(the parameter to be scanned)
-
-10.1. PySCeS Module documentation
-
-81
-
-PySCeS User Guide, Release 1.0.0
 • low = float(lower bound)
 • high = float(upper bound)
 • density = int(the number of initial points)
 • par3d = float(extra 3d parameter to insert into the output array) this parameter is not set
 ONLY used in output
 • logrange = boolean [default = True], if True generate the result using
 logspace(log10(low), log10(high), density) otherwise use a linear range
@@ -3254,31 +3328,32 @@
 output can be found in self.UserOutputResults - brett 2007.
 Analyze()
 The analysis method, the mode is automatically set by the self.addUserOutput() method but
 can be reset by the user.
 HAS_STATE_OUTPUT = True
 HAS_USER_OUTPUT = False
 MSG_PRINT_INTERVAL = 500
+
+10.1. PySCeS Module documentation
+
+85
+
+PySCeS User Guide, Release 1.1.0
+
 Run(ReRun=False)
 Run the parameter scan
 RunAgain()
 While it is impossible to change the generator/range structure of a scanner (just build another
 one) you can ‘in principle’ change the User Output and run it again.
 StoreData()
 Internal function which concatenates and stores the data generated by Analyze.
 addScanParameter(name, start, end, points, log=False, follower=False)
 Add a parameter to scan (an axis if you like) input is:
 • str(name) = model parameter name
 • float(start) = lower bound of scan
-
-82
-
-Chapter 10. Module documentation
-
-PySCeS User Guide, Release 1.0.0
 • float(end) = upper bound of scan
 • int(points) = number of points in scan range
 • bool(log) = Use a logarithmic (base10) range
 • bool(follower) = Scan parameters can be leaders i.e. an independent axis or a “follower”
 which moves synchronously with the previously defined parameter range.
 The first ScanParameter cannot be a follower.
 addUserOutput(*kw)
@@ -3298,31 +3373,30 @@
 otherwise [scan_parameters]+[Useroutput].
 invalid_state_list = None
 invalid_state_list_idx = None
 makeRange(start, end, points, log)
 Should be pretty self evident it defines a range:
 • float(start)
 • float(end)
+86
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
 • int(points)
 • bool(log)
 nan_on_bad_state = True
 quietRun = False
 rangeGen(name, start, end, points, log)
 This is where things get more interesting. This function creates a cycling generator which
 loops over a parameter range.
 • parameter name
 • start value
 • end value
 • points
-
-10.1. PySCeS Module documentation
-
-83
-
-PySCeS User Guide, Release 1.0.0
 • log scale
 resetInputParameters()
 Just remembered what this does, I think it resets the input model parameters after a scan run.
 setModValue(name, value)
 An easy one, assign value to name of the instantiated PySCeS model attribute
 stepGen(offset)
 Another looping generator function. The idea here is to create a set of generators for the
@@ -3339,14 +3413,21 @@
 Arbitrary dimension generic distributed scanner. Subclassed from pysces.PyscesScan.Scanner.
 This class is initiated with a loaded PySCeS model and then allows the user to define scan parameters, see self.addScanParameter() and user output, see self.addUserOutput(). Steadystate results are always stored in self.SteadyStateResults while user output can be found
 in self.UserOutputResults. Distributed (parallel) execution is achieved with the clustering
 capability of IPython. See ipcluster –help.
 The optional ‘engine’ argument specifies the parallel engine to use.
 • ‘multiproc’ – multiprocessing (default)
 • ‘ipcluster’ – IPython cluster
+
+10.1. PySCeS Module documentation
+
+87
+
+PySCeS User Guide, Release 1.1.0
+
 GatherScanResult()
 Concatenates and combines output result fragments from the parallel scan.
 HAS_USER_OUTPUT = False
 MSG_PRINT_INTERVAL = 500
 Prepare(ReRun=False)
 Internal method to prepare the parameters and generate ScanSpace.
 Run(ReRun=False)
@@ -3354,20 +3435,14 @@
 RunScatter(ReRun=False)
 Run the parameter scan by using scatter and gather for the ScanSpace. Not load balanced,
 equal number of scan runs per node.
 StoreData(result)
 Internal function which concatenates and stores single result generated by Analyze.
 • result IPython client result object
 genOn = True
-84
-
-Chapter 10. Module documentation
-
-PySCeS User Guide, Release 1.0.0
-
 genScanSpace()
 Generates the parameter scan space, partitioned according to self.scans_per_run
 invalid_state_list = None
 invalid_state_list_idx = None
 nan_on_bad_state = True
 scans_per_run = 100
 pysces.PyscesParScan.flush()
@@ -3380,35 +3455,36 @@
 class pysces.PyscesInterfaces.Core2interfaces
 Defines interfaces for translating PySCeS model objects into and from other formats.
 convertSBML2PSC(sbmlfile, sbmldir=None, pscfile=None, pscdir=None)
 Convert an SBML file to a PySCeS MDL input file.
 • sbmlfile: the SBML file name
 • sbmldir: the directory of SBML files (if None current working directory is assumed)
 • pscfile: the output PSC file name (if None sbmlfile.psc is used)
+
+88
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
 • pscdir: the PSC output directory (if None the pysces.model_dir is used)
 core = None
 core2psc = None
 core2sbml = None
 readMod2Core(mod, iValues=True)
 Convert a PySCeS model object to core2
 • iValues: if True then the models initial values are used (or the current values if False).
 readSBMLToCore(filename, directory=None)
 Reads the SBML file specified with filename and converts it into a core2 object
 pysces.interface.core
 • filename: the SBML file
 • directory: (optional) the SBML file directory None means try the current working directory
 sbml = None
 sbml2core = None
-sbml_level = 2
-sbml_version = 1
-10.1. PySCeS Module documentation
-
-85
-
-PySCeS User Guide, Release 1.0.0
+sbml_level = 3
+sbml_version = 2
 writeCore2PSC(filename=None, directory=None, getstrbuf=False)
 Writes a Core2 object to a PSC file.
 • filename: writes <filename>.xml or <model_name>.xml if None
 • directory: (optional) an output directory
 • getstrbuf : if True a StringIO buffer is returned instead of writing to disk
 writeCore2SBML(filename=None, directory=None, getdocument=False)
 Writes Core2 object to an SBML file.
@@ -3418,14 +3494,20 @@
 or
 writeMod2PSC(mod, filename=None, directory=None, iValues=True, getstrbuf=False)
 Writes a PySCeS model object to a PSC file.
 • filename: writes <filename>.psc or <model_name>.psc if None
 • directory: (optional) an output directory
 • iValues: if True then the models initial values are used (or the current values if False).
 • getstrbuf : if True a StringIO buffer is returned instead of writing to disk
+
+10.1. PySCeS Module documentation
+
+89
+
+PySCeS User Guide, Release 1.1.0
 writeMod2SBML(mod, filename=None, directory=None, iValues=True, getdocument=False,
 getstrbuf=False)
 Writes a PySCeS model object to an SBML file.
 • filename: writes <filename>.xml or <model_name>.xml if None
 • directory: (optional) an output directory
 • iValues: if True then the models initial values are used (or the current values if False).
 • getdocument: if True an SBML document object is returned instead of writing to disk
@@ -3438,35 +3520,34 @@
 PySCeS array functions - used by Stoich
 LinAlgError = 'LinearAlgebraError'
 MatrixFloatFix(mat, val=1.e-15)
 Clean an array removing any floating point artifacts defined as being smaller than a specified
 value. Processes an array inplace
 Arguments:
 mat: the input 2D array val [default=1.e-15]: the threshold value (effective zero)
-
-86
-
-Chapter 10. Module documentation
-
-PySCeS User Guide, Release 1.0.0
-
 MatrixValueCompare(matrix)
 Finds the largest/smallest abs(value) > 0.0 in a matrix. Returns a tuple containing (smallest,largest) values
 Arguments:
 matrix: the input 2D array
 SwapCol(res_a, r1, r2)
 Swap two columns using BLAS swap, arrays can be (or are upcast to) type double (d) or
 double complex (D). Returns the colswapped array
 Arguments:
 res_a: the input array r1: the first column to be swapped r2: the second column to be swapped
 SwapCold(res_a, c1, c2)
 Swaps two double (d) columns in an array using BLAS DSWAP. Returns the colswapped
 array.
 Arguments:
 res_a: input array c1: column index 1 c2: column index 2
+
+90
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
 SwapColz(res_a, c1, c2)
 Swaps two double complex (D) columns in an array using BLAS ZSWAP. Returns the colswapped array.
 Arguments:
 res_a: input array c1: column index 1 c2: column index 2
 SwapElem(res_a, r1, r2)
 Swaps two elements in a 1D vector
 Arguments:
@@ -3482,20 +3563,14 @@
 Arguments:
 res_a: input array c1: row index 1 c2: row index 2
 SwapRowz(res_a, c1, c2)
 Swaps two double complex (D) rows in an array using BLAS ZSWAP. Returns the
 rowswapped array.
 Arguments:
 res_a: input array c1: row index 1 c2: row index 2
-
-10.1. PySCeS Module documentation
-
-87
-
-PySCeS User Guide, Release 1.0.0
 array_kind = {'D': 1, 'F': 1, 'd':
 
 0, 'f':
 
 array_precision = {'D': 1, 'F': 0, 'd':
 
 0, 'i':
@@ -3517,14 +3592,21 @@
 Check that we are using a 2D array
 Arguments:
 *arrays: input array(s)
 castCopyAndTranspose(type, \*arrays)
 Cast numeric arrays to required type and transpose
 Arguments:
 type: the required type to cast to *arrays: the arrays to be processed
+
+10.1. PySCeS Module documentation
+
+91
+
+PySCeS User Guide, Release 1.1.0
+
 commonType(\*arrays)
 Numeric detect and set array precision (will be replaced with new scipy.core compatible code
 when ready)
 Arguments:
 *arrays: input arrays
 class pysces.PyscesStoich.Stoich(input)
 PySCeS stoichiometric analysis class: initialized with a stoichiometric matrix N (input)
@@ -3547,28 +3629,29 @@
 column tracking vector
 GetUpperMatrix(a)
 Core analysis algorithm; an input is preconditioned using PivotSort_initial and then cycles of
 PLUfactorize and PivotSort are run until the factorization is completed. During this process
 the matrix is reordered by column swaps which emulates a full pivoting LU factorization.
 Returns the pivot matrix P, upper factorization U as well as the row/col tracking vectors.
 Arguments:
-88
-
-Chapter 10. Module documentation
-
-PySCeS User Guide, Release 1.0.0
 a: a stoichiometric matrix
 GetUpperMatrixUsingQR(a)
 GetUpperMatrix(a)
 Core analysis algorithm; an input is preconditioned using PivotSort_initial and then cycles of
 PLUfactorize and PivotSort are run until the factorization is completed. During this process
 the matrix is reordered by column swaps which emulates a full pivoting LU factorization.
 Returns the pivot matrix P, upper factorization U as well as the row/col tracking vectors.
 Arguments:
 a: a stoichiometric matrix
+
+92
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
 K_split_R(R_a, row_vector, column_vector)
 Using the R factorized form of the stoichiometric matrix we now form the K and Ko matrices.
 Returns the r_ipart,Komatrix,Krow,Kcolumn,Kmatrix,Korow,info
 Arguments:
 R_a: the Gauss-Jordan reduced stoichiometric matrix row_vector: row tracking vector column_vector: column tracking vector
 L_split_R(Nfull, R_a, row_vector, column_vector)
 Takes the Gauss-Jordan factorized N^T and extract the L, Lo, conservation (I -Lo) and reduced stoichiometric matrices. Returns: lmatrix_col_vector, lomatrix, lomatrix_row, lomatrix_co, nrmatrix, Nred_vector_row, Nred_vector_col, info
@@ -3590,37 +3673,164 @@
 PivotSort_initial(a, row_vector, column_vector)
 This is a sorting routine that accepts a matrix and row/colum vectors and then sorts them so
 that: the abs(largest) pivots are moved onto the diagonal to maintain numerical stability i.e.
 the matrix diagonal is in descending max(abs(value)). Row and column swaps are recorded
 in the tracking vectors.
 Arguments:
 a: the input array row_vector: row tracking vector column_vector: column tracking vector
-10.1. PySCeS Module documentation
-
-89
-
-PySCeS User Guide, Release 1.0.0
 SVD_Rank_Check(matrix=None, factor=1.0e4, resultback=0)
 Calculates the dimensions of L/L0/K/K) by way of SVD and compares them to the GuassJordan results. Please note that for LARGE ill conditioned matrices the SVD can become
 numerically unstable when used for nullspace determinations
 Arguments:
 matrix [default=None]: the stoichiometric matrix default is self.Nmatrix factor [default=1.0e4]: factor used to calculate the ‘zero pivot’ mask = mach_eps*factor resultback
 [default=0]: return the SVD results, U, S, vh
+
+10.1. PySCeS Module documentation
+
+93
+
+PySCeS User Guide, Release 1.1.0
+
 ScalePivots(a_one)
 Given an upper triangular matrix U, this method scales the diagonal (pivot values) to one.
 Arguments:
 a_one: an upper triangular matrix U
 SplitLU(plu, row, col, t)
 PLU takes the combined LU factorization computed by PLUfactorize and extracts the upper
 matrix. Returns U.
 Arguments:
 plu: LU factorization row: row tracking vector col: column tracking vector t [default=None)]:
 typecode argument (currently not used)
 USE_QR = False
+class finfo(dtype)
+Machine limits for floating point types.
+
+10.1.8 Attributes
+bits
+[int] The number of bits occupied by the type.
+dtype
+[dtype] Returns the dtype for which finfo returns information. For complex input, the
+returned dtype is the associated float* dtype for its real and complex components.
+eps
+[float] The difference between 1.0 and the next smallest representable float larger than
+1.0. For example, for 64-bit binary floats in the IEEE-754 standard, eps = 2**-52,
+approximately 2.22e-16.
+epsneg
+[float] The difference between 1.0 and the next smallest representable float less than
+1.0. For example, for 64-bit binary floats in the IEEE-754 standard, epsneg = 2**-53,
+approximately 1.11e-16.
+iexp
+[int] The number of bits in the exponent portion of the floating point representation.
+machar
+[MachAr] The object which calculated these parameters and holds more detailed information.
+Deprecated since version 1.22.
+machep
+[int] The exponent that yields eps.
+max
+[floating point number of the appropriate type] The largest representable number.
+maxexp
+[int] The smallest positive power of the base (2) that causes overflow.
+
+94
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
+
+min
+[floating point number of the appropriate type] The smallest representable number, typically -max.
+minexp
+[int] The most negative power of the base (2) consistent with there being no leading 0’s
+in the mantissa.
+negep
+[int] The exponent that yields epsneg.
+nexp
+[int] The number of bits in the exponent including its sign and bias.
+nmant
+[int] The number of bits in the mantissa.
+precision
+[int] The approximate number of decimal digits to which this kind of float is precise.
+resolution
+[floating point number of the appropriate type] The approximate decimal resolution of
+this type, i.e., 10**-precision.
+tiny
+[float] An alias for smallest_normal, kept for backwards compatibility.
+smallest_normal
+[float] The smallest positive floating point number with 1 as leading bit in the mantissa
+following IEEE-754 (see Notes).
+smallest_subnormal
+[float] The smallest positive floating point number with 0 as leading bit in the mantissa
+following IEEE-754.
+
+10.1.9 Parameters
+dtype
+[float, dtype, or instance] Kind of floating point or complex floating point data-type about
+which to get information.
+
+10.1.10 See Also
+MachAr : The implementation of the tests that produce this information. iinfo : The equivalent for integer data types. spacing : The distance between a value and the nearest adjacent
+number nextafter : The next floating point value after x1 towards x2
+
+10.1. PySCeS Module documentation
+
+95
+
+PySCeS User Guide, Release 1.1.0
+
+10.1.11 Notes
+For developers of NumPy: do not instantiate this at the module level. The initial calculation
+of these parameters is expensive and negatively impacts import times. These objects are
+cached, so calling finfo() repeatedly inside your functions is not a problem.
+Note that smallest_normal is not actually the smallest positive representable value in a
+NumPy floating point type. As in the IEEE-754 standard1 , NumPy floating point types make
+use of subnormal numbers to fill the gap between 0 and smallest_normal. However, subnormal numbers may have significantly reduced precision2 .
+This function can also be used for complex data types as well. If used, the output will be the
+same as the corresponding real float type (e.g. numpy.finfo(numpy.csingle) is the same as
+numpy.finfo(numpy.single)). However, the output is true for the real and imaginary components.
+
+10.1.12 References
+10.1.13 Examples
+>>> np.finfo(np.float64).dtype
+dtype('float64')
+>>> np.finfo(np.complex64).dtype
+dtype('float32')
+property machar
+The object which calculated these parameters and holds more detailed information.
+Deprecated since version 1.22.
+property smallest_normal
+Return the value for the smallest normal.
+Returns
+smallest_normal
+[float] Value for the smallest normal.
+Warns
+UserWarning
+If the calculated value for the smallest normal is requested for double-double.
+property tiny
+Return the value for tiny, alias of smallest_normal.
+1
+
+IEEE Standard for Floating-Point Arithmetic, IEEE Std 754-2008, pp.1-70, 2008, http://www.doi.org/10.1109/IEEESTD.
+2008.4610935
+2
+Wikipedia, “Denormal Numbers”, https://en.wikipedia.org/wiki/Denormal_number
+
+96
+
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
+
+Returns
+tiny
+[float] Value for the smallest normal, alias of smallest_normal.
+Warns
+UserWarning
+If the calculated value for the smallest normal is requested for double-double.
 info_moiety_conserve = False
+mach_eps = 2.220446049250313e-16
 class pysces.PyscesStoich.StructMatrix(array, ridx, cidx, row=None, col=None)
 This class is specifically designed to store structural matrix information give it an array and row/col
 index permutations it can generate its own row/col labels given the label src.
 array = None
 cidx = None
 col = None
 getByIdx(row, col)
@@ -3633,35 +3843,35 @@
 Return the matrix indexes ([rows],[cols]) where axis=’row’/’col’/’all’
 getLabels(axis='all')
 Return the matrix labels ([rows],[cols]) where axis=’row’/’col’/’all’
 getRowsByIdx(*args)
 Return the rows referenced by index (1,3,5)
 getRowsByName(*args)
 Return the rows referenced by label (‘s’,’x’,’d’)
-
-90
-
-Chapter 10. Module documentation
-
-PySCeS User Guide, Release 1.0.0
-
 ridx = None
 row = None
 setByIdx(row, col, val)
 setByName(row, col, val)
+
+10.1. PySCeS Module documentation
+
+97
+
+PySCeS User Guide, Release 1.1.0
+
 setCol(src)
 Assuming that the col index array is a permutation (full/subset) of a source label array by
 supplying that src to setCol maps the row labels to cidx and creates self.col (col label list)
 setRow(src)
 Assuming that the row index array is a permutation (full/subset) of a source label array by
 supplying that source to setRow it maps the row labels to ridx and creates self.row (row label
 list)
 shape = None
 
-10.1.8 PyscesLink
+10.1.14 PyscesLink
 Interfaces to external software and API’s, has replaced the PySCeS contrib classes.
 class pysces.PyscesLink.METATOOLlink(mod, __metatool_path__=None)
 New interface to METATOOL binaries
 doEModes()
 Calculate the elementary modes by way of an interface to MetaTool.
 METATOOL is a C program developed from 1998 to 2000 by Thomas Pfeiffer (Berlin) in
 cooperation with Stefan Schuster and Ferdinand Moldenhauer (Berlin) and Juan Carlos Nuno
@@ -3679,21 +3889,22 @@
 DEBUGMODE = False
 DRAWNETWORKLOADED = False
 LAYOUTMODULELOADED = False
 drawNetworkGetSBMLwithLayout()
 drawNetworkLoadSBML()
 getSBML()
 getSBMLlayout()
-10.1. PySCeS Module documentation
+getSVG()
 
-91
+98
 
-PySCeS User Guide, Release 1.0.0
+Chapter 10. Module documentation
+
+PySCeS User Guide, Release 1.1.0
 
-getSVG()
 getVersion()
 layoutModuleGetSVG()
 layoutModuleLoadSBML()
 loadSBMLFileFromDisk(File, Dir=None)
 loadSBMLFromString(str)
 sbml = None
 sbmllayout = None
@@ -3713,1378 +3924,1389 @@
 SBW_loadModule(module_name)
 moduleDict = None
 modules = None
 psbw = None
 sbw = None
 sbwModuleProxy = None
 
-92
+10.1. PySCeS Module documentation
+
+99
+
+PySCeS User Guide, Release 1.1.0
+
+100
 
 Chapter 10. Module documentation
 
 CHAPTER
 
 ELEVEN
 
 INDICES AND TABLES
 
 • genindex
 • modindex
 • search
 
-93
+101
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
-94
+102
 
 Chapter 11. Indices and tables
 
 PYTHON MODULE INDEX
 
 p
-pysces.PyscesInterfaces, 85
-pysces.PyscesLink, 91
-pysces.PyscesModel, 60
-pysces.PyscesParScan, 84
-pysces.PyscesPlot2, 49
-pysces.PyscesScan, 80
-pysces.PyscesStoich, 86
-pysces.PyscesUtils, 47
+pysces.PyscesInterfaces, 88
+pysces.PyscesLink, 98
+pysces.PyscesModel, 62
+pysces.PyscesParScan, 87
+pysces.PyscesPlot2, 51
+pysces.PyscesScan, 84
+pysces.PyscesStoich, 90
+pysces.PyscesUtils, 49
 
-95
+103
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
-96
+104
 
 Python Module Index
 
 INDEX
 
 A
 
-55
+57
 
 add() (pysces.PyscesPlot2.FIFOBuffer method),
 B
-50
+52
 addFormula()
 (pysces.PyscesModel.Function BackSubstitution()
 (pysces.PyscesStoich.Stoich
 method),
-method), 61
-88
+method), 64
+92
 addModData() (pysces.PyscesModel.ScanDataObj
-BagOfStuff (class in pysces.PyscesModel), 60
-method), 78
+BagOfStuff (class in pysces.PyscesModel), 62
+method), 81
 addPoint() (pysces.PyscesModel.ScanDataObj
 C
-method), 78
+method), 81
 castCopyAndTranspose()
 addScanParameter()
 (pysces.PyscesStoich.MathArrayFunc
-(pysces.PyscesScan.Scanner method), 82
-method), 88
+(pysces.PyscesScan.Scanner method), 86
+method), 91
 addUserOutput() (pysces.PyscesScan.Scanner
 chkmdir()
-(in module pysces.PyscesModel), 80
-method), 83
-ALL_VALID (pysces.PyscesModel.ScanDataObj chkpsc() (in module pysces.PyscesModel), 80
+(in module pysces.PyscesModel), 83
+method), 86
+ALL_VALID (pysces.PyscesModel.ScanDataObj chkpsc() (in module pysces.PyscesModel), 83
 cidx (pysces.PyscesStoich.StructMatrix attribute),
-attribute), 78
-90
+attribute), 81
+97
 analyseData() (pysces.PyscesScan.PITCONScanUtils
 CleanNaNsFromArray()
-method), 81
+method), 84
 (pysces.PyscesModel.PysMod method),
 AnalyseK() (pysces.PyscesStoich.Stoich method),
-65
-88
+67
+92
 clone()
 (pysces.PyscesModel.PysMod method),
 AnalyseL() (pysces.PyscesStoich.Stoich method),
-73
-88
+76
+92
 closeAll()
 (pysces.PyscesPlot2.MatplotlibUPI
-Analyze() (in module pysces.PyscesParScan), 84
+Analyze() (in module pysces.PyscesParScan), 87
 method),
-53
+56
 Analyze() (pysces.PyscesScan.Scanner method),
 closeAll()
 (pysces.PyscesPlot2.PyscesUPI
-82
+85
 method),
-57
+60
 argsl (pysces.PyscesModel.Function attribute),
 closeScan() (pysces.PyscesModel.ScanDataObj
-61
-method), 78
+64
+method), 82
 array (pysces.PyscesStoich.StructMatrix atcode_string
-(pysces.PyscesModel.Event attribute), 90
-tribute), 60
+(pysces.PyscesModel.Event attribute), 97
+tribute), 63
 array_kind (pysces.PyscesStoich.MathArrayFunc
 code_string
 (pysces.PyscesModel.EventAssignment
-attribute), 87
+attribute), 91
 attribute),
-61
+64
 array_precision
 code_string (pysces.PyscesModel.Function at(pysces.PyscesStoich.MathArrayFunc
-tribute), 62
-attribute), 88
-array_type (pysces.PyscesStoich.MathArrayFunc code_string (pysces.PyscesModel.PieceWise attribute), 64
-attribute), 88
+tribute), 64
+attribute), 91
+array_type (pysces.PyscesStoich.MathArrayFunc code_string (pysces.PyscesModel.PieceWise attribute), 67
+attribute), 91
 code_string
 (pysces.PyscesModel.ReactionObj
 assertRank2() (pysces.PyscesStoich.MathArrayFunc
-attribute), 78
-method), 88
+attribute), 81
+method), 91
 col
 (pysces.PyscesModel.BagOfStuff
-attribute), 60
+attribute), 62
 assignments (pysces.PyscesModel.Event atcol (pysces.PyscesStoich.StructMatrix attribute),
-tribute), 60
-90
+tribute), 63
+97
 axisInputStringToList()
 CommonStyleDefs
 (pysces.PyscesPlot2.PlotBase method),
-97
+105
 
-PySCeS User Guide, Release 1.0.0
-method), 73
+PySCeS User Guide, Release 1.1.0
+method), 76
 (pysces.PyscesPlot2.GnuPlotUPI
 atdoEigenShow() (pysces.PyscesModel.PysMod
-tribute), 50
-method), 73
+tribute), 52
+method), 76
 CommonStyleDefs
 doElas() (pysces.PyscesModel.PysMod method),
 (pysces.PyscesPlot2.MatplotlibUPI
-73
-attribute), 53
-CommonStyleDefs (pysces.PyscesPlot2.PlotBase doEModes() (pysces.PyscesLink.METATOOLlink
-method), 91
+76
 attribute), 55
+CommonStyleDefs (pysces.PyscesPlot2.PlotBase doEModes() (pysces.PyscesLink.METATOOLlink
+method), 98
+attribute), 57
 commonType() (pysces.PyscesStoich.MathArrayFuncdoLoad() (pysces.PyscesModel.PysMod method),
-73
-method), 88
+76
+method), 91
 compartment (pysces.PyscesModel.ReactionObj doMca() (pysces.PyscesModel.PysMod method),
-73
-attribute), 78
+76
+attribute), 81
 (pysces.PyscesModel.PysMod
 ConvertFileD2U()
 (in
 module doMcaRC()
-method), 73
-pysces.PyscesUtils), 47
+method), 76
+pysces.PyscesUtils), 49
 (pysces.PyscesModel.PysMod
 ConvertFileU2D()
 (in
 module doMcaRCT()
-method), 73
-pysces.PyscesUtils), 47
+method), 77
+pysces.PyscesUtils), 49
 doSim() (pysces.PyscesModel.PysMod method),
 convertSBML2PSC()
-74
+77
 (pysces.PyscesInterfaces.Core2interfaces
 doSimPerturb() (pysces.PyscesModel.PysMod
-method), 85
-method), 74
-CopyModels() (in module pysces.PyscesUtils), 47
+method), 88
+method), 77
+CopyModels() (in module pysces.PyscesUtils), 49
 (pysces.PyscesModel.PysMod
 CopyTestModels()
 (in
 module doSimPlot()
-method), 74
-pysces.PyscesUtils), 47
+method), 77
+pysces.PyscesUtils), 49
 (pysces.PyscesModel.PysMod
 core (pysces.PyscesInterfaces.Core2interfaces at- doState()
-method), 74
-tribute), 85
+method), 77
+tribute), 89
 Core2interfaces
 (class
 in doStateShow() (pysces.PyscesModel.PysMod
-method), 74
-pysces.PyscesInterfaces), 85
+method), 77
+pysces.PyscesInterfaces), 88
 core2psc (pysces.PyscesInterfaces.Core2interfaces drawNetworkGetSBMLwithLayout()
 (pysces.PyscesLink.SBWLayoutWebLink
-attribute), 85
-method), 91
+attribute), 89
+method), 98
 core2sbml (pysces.PyscesInterfaces.Core2interfaces
 DRAWNETWORKLOADED
-attribute), 85
+attribute), 89
 (pysces.PyscesLink.SBWLayoutWebLink
 CVODE() (pysces.PyscesModel.PysMod method),
-attribute), 91
-64
+attribute), 98
+67
 drawNetworkLoadSBML()
 CVODE_continue()
 (pysces.PyscesLink.SBWLayoutWebLink
 (pysces.PyscesModel.PysMod method),
-method), 91
-64
+method), 98
+67
 CVODE_continuous_result
 (pysces.PyscesModel.PysMod attribute), E
 EvalCC() (pysces.PyscesModel.PysMod method),
-65
-65
+67
+67
 CVODE_VPYTHON() (pysces.PyscesModel.PysMod
 EvalEigen()
 (pysces.PyscesModel.PysMod
-method), 64
-method), 65
+method), 67
+method), 68
 D
 EvalEpar()
 (pysces.PyscesModel.PysMod
-method), 65
+method), 68
 DATF_FORMAT (pysces.PyscesPlot2.GnuPlotUPI
 EvalEvar()
 (pysces.PyscesModel.PysMod
-attribute), 50
-method), 65
+attribute), 52
+method), 68
 DEBUGLEVEL (pysces.PyscesLink.SBWLayoutWebLink
 EvalRC() (pysces.PyscesModel.PysMod method),
-attribute), 91
-66
+attribute), 98
+68
 DEBUGMODE (pysces.PyscesLink.SBWLayoutWebLink
 EvalRCT()
 (pysces.PyscesModel.PysMod
-attribute), 91
-method), 66
-delay (pysces.PyscesModel.Event attribute), 60
+attribute), 98
+method), 69
+delay (pysces.PyscesModel.Event attribute), 63
 doEigen()
 (pysces.PyscesModel.PysMod evaluateAssignment()
 (pysces.PyscesModel.EventAssignment
-method), 73
-method), 61
+method), 76
+method), 64
 doEigenMca()
 (pysces.PyscesModel.PysMod
 
-98
+106
 
 Index
 
-PySCeS User Guide, Release 1.0.0
-Event (class in pysces.PyscesModel), 60
+PySCeS User Guide, Release 1.1.0
+Event (class in pysces.PyscesModel), 63
 EventAssignment (class in pysces.PyscesModel),
-61
+64
 EventsProblem (class in pysces.PyscesModel),
-61
+64
+ExecRateRules() (pysces.PyscesModel.PysMod
+method), 69
 export()
 (pysces.PyscesPlot2.GnuPlotUPI
-method), 50
+method), 52
 export()
 (pysces.PyscesPlot2.MatplotlibUPI
-method), 53
+method), 56
 export() (pysces.PyscesPlot2.PlotBase method),
-55
+57
 export()
 (pysces.PyscesPlot2.PyscesUPI
-method), 58
+method), 60
 exportArray2CSV()
 (pysces.PyscesUtils.WriteOutput
-method), 48
+method), 50
 exportArray2TXT()
 (pysces.PyscesUtils.WriteOutput
-method), 48
+method), 50
 exportLabelledArray()
 (pysces.PyscesUtils.WriteOutput
-method), 48
+method), 50
 exportLabelledArray2CSV()
 (pysces.PyscesUtils.WriteOutput
-method), 48
+method), 50
 exportLabelledArray2TXT()
 (pysces.PyscesUtils.WriteOutput
-method), 48
+method), 50
 exportLabelledArrayWithHeader()
 (pysces.PyscesUtils.WriteOutput
-method), 48
+method), 50
 exportLabelledArrayWithHeader2CSV()
 (pysces.PyscesUtils.WriteOutput
-method), 49
+method), 51
 exportLabelledArrayWithHeader2TXT()
 (pysces.PyscesUtils.WriteOutput
-method), 49
+method), 51
 exportLabelledLinkedList()
 (pysces.PyscesUtils.WriteOutput
-method), 49
+method), 51
 exportSimAsSedML()
 (pysces.PyscesModel.PysMod method),
-74
+77
 
+(pysces.PyscesModel.PysMod method),
+69
 Fix_S_indinput()
 (pysces.PyscesModel.PysMod method),
-66
+69
 Fix_Sim()
 (pysces.PyscesModel.PysMod
-method), 66
-flush() (in module pysces.PyscesParScan), 85
+method), 69
+flush() (in module pysces.PyscesParScan), 88
 flux_labels (pysces.PyscesModel.ScanDataObj
-attribute), 78
+attribute), 82
 flux_labels (pysces.PyscesModel.StateDataObj
-attribute), 79
+attribute), 83
 fluxes
 (pysces.PyscesModel.ScanDataObj
-attribute), 79
+attribute), 82
 fluxes
 (pysces.PyscesModel.StateDataObj
-attribute), 79
+attribute), 83
 FluxGenSim()
 (pysces.PyscesModel.PysMod
-method), 66
+method), 69
 Forcing_Function()
 (pysces.PyscesModel.PysMod method),
-66
-formula (pysces.PyscesModel.Event attribute), 61
+69
+formula (pysces.PyscesModel.Event attribute), 63
 formula (pysces.PyscesModel.EventAssignment
-attribute), 61
+attribute), 64
 formula
 (pysces.PyscesModel.Function
-attribute), 62
-formula (pysces.PyscesModel.PieceWise attribute), 64
+attribute), 64
+formula (pysces.PyscesModel.PieceWise attribute), 67
 formula
 (pysces.PyscesModel.ReactionObj
-attribute), 78
-Function (class in pysces.PyscesModel), 61
-functions (pysces.PyscesModel.Function attribute), 62
+attribute), 81
+Function (class in pysces.PyscesModel), 64
+functions (pysces.PyscesModel.Function attribute), 64
 
 G
 
-g (pysces.PyscesPlot2.PyscesUPI attribute), 58
+g (pysces.PyscesPlot2.PyscesUPI attribute), 60
 g_file_write_array()
 (pysces.PyscesPlot2.GnuPlotUPI
-method), 50
+method), 52
 g_file_write_array3D()
 (pysces.PyscesPlot2.GnuPlotUPI
-method), 50
+method), 52
 g_pause()
 (pysces.PyscesPlot2.GnuPlotUPI
-method), 50
+method), 52
 g_write()
 (pysces.PyscesPlot2.GnuPlotUPI
-method), 50
+method), 52
 F
 GatherScanResult()
 (pysces.PyscesParScan.ParScanner
-FIFOBuffer (class in pysces.PyscesPlot2), 50
-method), 84
+FIFOBuffer (class in pysces.PyscesPlot2), 52
+method), 87
 FINTSLV()
 (pysces.PyscesModel.PysMod
-genOn (pysces.PyscesParScan.ParScanner atmethod), 66
-tribute), 84
+genOn (pysces.PyscesParScan.ParScanner atmethod), 69
+tribute), 88
 Fix_S_fullinput()
-(pysces.PyscesModel.PysMod method), genOn (pysces.PyscesScan.Scanner attribute), 83
-genScanSpace()
-66
 
 Index
 
-99
+107
 
-PySCeS User Guide, Release 1.0.0
-method), 62
-(pysces.PyscesParScan.ParScanner
-getOutput()
-(pysces.PyscesScan.Scanner
-method), 85
-method), 83
-get() (pysces.PyscesModel.BagOfStuff method),
+PySCeS User Guide, Release 1.1.0
+method), 86
+genOn (pysces.PyscesScan.Scanner attribute), 86
 getRates() (pysces.PyscesModel.IntegrationDataObj
-60
-method), 62
-get()
-(pysces.PyscesModel.NewCoreBase
+genScanSpace()
+method), 65
+(pysces.PyscesParScan.ParScanner
 getResultMatrix()
-method), 63
-(pysces.PyscesScan.Scanner method), 83
-get() (pysces.PyscesPlot2.FIFOBuffer method),
+method), 88
+(pysces.PyscesScan.Scanner method), 86
+get() (pysces.PyscesModel.BagOfStuff method),
 getRowsByIdx()
-50
+62
 (pysces.PyscesStoich.StructMatrix
-getAllScanData()
-method), 90
-(pysces.PyscesModel.ScanDataObj
+get() (pysces.PyscesPlot2.FIFOBuffer method),
+method), 97
+52
 getRowsByName()
-method), 79
+getAllScanData()
 (pysces.PyscesStoich.StructMatrix
+(pysces.PyscesModel.ScanDataObj
+method), 97
+method), 82
+getRules() (pysces.PyscesModel.IntegrationDataObj
 getAllSimData()
-method), 90
+method), 65
 (pysces.PyscesModel.IntegrationDataObj
-getRules() (pysces.PyscesModel.IntegrationDataObj
-method), 62
-method), 62
-getAllStateData()
 getRules() (pysces.PyscesModel.ScanDataObj
-(pysces.PyscesModel.StateDataObj
-method), 79
-method), 79
+method), 65
+method), 82
+getAllStateData()
 getRules() (pysces.PyscesModel.StateDataObj
+(pysces.PyscesModel.StateDataObj
+method), 83
+method), 83
+getSBML() (pysces.PyscesLink.SBWLayoutWebLink
 getArrayListAsArray()
-method), 79
+method), 98
 (pysces.PyscesScan.PITCONScanUtils
-getSBML() (pysces.PyscesLink.SBWLayoutWebLink
-method), 81
-method), 91
-getByIdx() (pysces.PyscesStoich.StructMatrix
 getSBMLlayout()
-method), 90
+method), 84
 (pysces.PyscesLink.SBWLayoutWebLink
-getByName() (pysces.PyscesStoich.StructMatrix
-method), 91
-method), 90
-getScanData() (pysces.PyscesModel.ScanDataObj
+getByIdx() (pysces.PyscesStoich.StructMatrix
+method), 98
+method), 97
+getByName() (pysces.PyscesStoich.StructMatrix getScanData() (pysces.PyscesModel.ScanDataObj
+method), 82
+method), 97
+getSimData() (pysces.PyscesModel.IntegrationDataObj
 getColsByIdx()
-method), 79
+method), 65
 (pysces.PyscesStoich.StructMatrix
-getSimData() (pysces.PyscesModel.IntegrationDataObj
-method), 90
-method), 63
-getColsByName()
 getSpecies() (pysces.PyscesModel.IntegrationDataObj
-(pysces.PyscesStoich.StructMatrix
-method), 63
-method), 90
+method), 97
+method), 66
+getColsByName()
 getSpecies() (pysces.PyscesModel.ScanDataObj
+(pysces.PyscesStoich.StructMatrix
+method), 82
+method), 97
+getSpecies() (pysces.PyscesModel.StateDataObj
 getDataAtTime()
-method), 79
+method), 83
 (pysces.PyscesModel.IntegrationDataObj
-getSpecies() (pysces.PyscesModel.StateDataObj
-method), 62
-method), 80
-getDataInTimeInterval()
-(pysces.PyscesModel.IntegrationDataObj getStateData()
+getStateData()
+method), 65
 (pysces.PyscesModel.StateDataObj
-method), 62
-method), 80
-getEModes() (pysces.PyscesLink.METATOOLlink
+getDataInTimeInterval()
+method), 83
+(pysces.PyscesModel.IntegrationDataObj
 getSVG() (pysces.PyscesLink.SBWLayoutWebLink
-method), 91
-method), 92
-getFluxes() (pysces.PyscesModel.ScanDataObj
+method), 65
+method), 98
+getEModes() (pysces.PyscesLink.METATOOLlink
 getTime() (pysces.PyscesModel.IntegrationDataObj
-method), 79
-method), 63
-getFluxes() (pysces.PyscesModel.StateDataObj
+method), 98
+method), 66
+getFluxes() (pysces.PyscesModel.ScanDataObj
 GetUpperMatrix() (pysces.PyscesStoich.Stoich
-method), 79
-method), 88
-getIndexes() (pysces.PyscesStoich.StructMatrix
+method), 82
+method), 92
+getFluxes() (pysces.PyscesModel.StateDataObj
 GetUpperMatrixUsingQR()
-method), 90
+method), 83
 (pysces.PyscesStoich.Stoich
 method),
-getLabels() (pysces.PyscesStoich.StructMatrix
-89
-method), 90
-getModData() (pysces.PyscesModel.ScanDataObj getValue() (pysces.PyscesModel.NumberBase
-method), 64
-method), 79
-getName() (pysces.PyscesModel.NewCoreBase getVersion() (pysces.PyscesLink.SBWLayoutWebLink
-method), 92
-method), 63
-getXData() (pysces.PyscesModel.IntegrationDataObj
+getIndexes() (pysces.PyscesStoich.StructMatrix
+92
+method), 97
+getLabels() (pysces.PyscesStoich.StructMatrix getVersion() (pysces.PyscesLink.SBWLayoutWebLink
+method), 98
+method), 97
+getModData() (pysces.PyscesModel.ScanDataObj getXData() (pysces.PyscesModel.IntegrationDataObj
+method), 66
+method), 82
+getXData() (pysces.PyscesModel.ScanDataObj
 getOutput() (pysces.PyscesModel.IntegrationDataObj
+method), 82
+method), 65
+getOutput()
+(pysces.PyscesScan.Scanner getXData() (pysces.PyscesModel.StateDataObj
 
-100
+108
 
 Index
 
-PySCeS User Guide, Release 1.0.0
-HYBRD() (pysces.PyscesModel.PysMod method),
-method), 63
-66
-getXData() (pysces.PyscesModel.ScanDataObj
-method), 79
-getXData() (pysces.PyscesModel.StateDataObj I
-info_moiety_conserve
-method), 80
-(pysces.PyscesStoich.Stoich attribute), 90
-GnuPlotUPI (class in pysces.PyscesPlot2), 50
+PySCeS User Guide, Release 1.1.0
+(pysces.PyscesStoich.Stoich attribute), 97
 InitialiseCompartments()
-H
 (pysces.PyscesModel.PysMod method),
-67
+H
+69
 handle_event()
 InitialiseConservationArrays()
 (pysces.PyscesModel.EventsProblem
 (pysces.PyscesModel.PysMod method),
-method), 61
-67
-HAS_FLUXES (pysces.PyscesModel.ScanDataObj
-InitialiseEvents()
-attribute), 78
+method), 64
+69
+HAS_FLUXES (pysces.PyscesModel.ScanDataObj InitialiseEvents()
+attribute), 81
 (pysces.PyscesModel.PysMod method),
 HAS_FLUXES (pysces.PyscesModel.StateDataObj
-67
-attribute), 79
-HAS_MOD_DATA (pysces.PyscesModel.ScanDataObj InitialiseFunctions()
+70
+attribute), 82
+InitialiseFunctions()
+HAS_MOD_DATA (pysces.PyscesModel.ScanDataObj
 (pysces.PyscesModel.PysMod method),
-attribute), 78
-67
-HAS_RATES (pysces.PyscesModel.IntegrationDataObj
-InitialiseInputFile()
-attribute), 62
+attribute), 81
+70
+HAS_RATES (pysces.PyscesModel.IntegrationDataObjInitialiseInputFile()
+attribute), 65
 (pysces.PyscesModel.PysMod method),
 HAS_RULES (pysces.PyscesModel.IntegrationDataObj
-67
-attribute), 62
-HAS_RULES (pysces.PyscesModel.ScanDataObj InitialiseModel()
+70
+attribute), 65
+InitialiseModel()
+HAS_RULES (pysces.PyscesModel.ScanDataObj
 (pysces.PyscesModel.PysMod method),
-attribute), 78
-67
-HAS_RULES (pysces.PyscesModel.StateDataObj
-InitialiseOldFunctions()
-attribute), 79
+attribute), 81
+70
+HAS_RULES (pysces.PyscesModel.StateDataObj InitialiseOldFunctions()
+attribute), 82
 (pysces.PyscesModel.PysMod method),
 HAS_SET_LABELS
-67
+70
 (pysces.PyscesModel.ScanDataObj
 InitialiseRuleChecks()
-attribute), 78
+attribute), 81
 (pysces.PyscesModel.PysMod method),
 HAS_SPECIES (pysces.PyscesModel.IntegrationDataObj
-67
-attribute), 62
-HAS_SPECIES (pysces.PyscesModel.ScanDataObj InitialiseRules()
+70
+attribute), 65
+InitialiseRules()
+HAS_SPECIES (pysces.PyscesModel.ScanDataObj
 (pysces.PyscesModel.PysMod method),
-attribute), 78
-67
-HAS_SPECIES (pysces.PyscesModel.StateDataObj
-IntegrationDataObj
+attribute), 81
+70
+HAS_SPECIES (pysces.PyscesModel.StateDataObj IntegrationDataObj
 (class
 in
-attribute), 79
-pysces.PyscesModel), 62
-HAS_STATE_OUTPUT (pysces.PyscesScan.Scanner
-invalid_state_list
 attribute), 82
+pysces.PyscesModel), 65
+HAS_STATE_OUTPUT (pysces.PyscesScan.Scanner invalid_state_list
+attribute), 85
 (pysces.PyscesParScan.ParScanner
 HAS_TIME (pysces.PyscesModel.IntegrationDataObj
-attribute), 85
-attribute), 62
+attribute), 88
+attribute), 65
 invalid_state_list
 HAS_USER_OUTPUT
 (pysces.PyscesScan.Scanner attribute),
 (pysces.PyscesParScan.ParScanner
-83
-attribute), 84
-HAS_USER_OUTPUT (pysces.PyscesScan.Scanner invalid_state_list_idx
+86
+attribute), 88
+invalid_state_list_idx
+HAS_USER_OUTPUT (pysces.PyscesScan.Scanner
 (pysces.PyscesParScan.ParScanner
-attribute), 82
 attribute), 85
-HAS_XDATA (pysces.PyscesModel.IntegrationDataObj
-invalid_state_list_idx
-attribute), 62
+attribute), 88
+HAS_XDATA (pysces.PyscesModel.IntegrationDataObjinvalid_state_list_idx
+attribute), 65
 (pysces.PyscesScan.Scanner attribute),
 HAS_XDATA (pysces.PyscesModel.ScanDataObj
-83
-attribute), 78
-HAS_XDATA (pysces.PyscesModel.StateDataObj invalid_states
+86
+attribute), 81
+invalid_states
+HAS_XDATA (pysces.PyscesModel.StateDataObj
 (pysces.PyscesModel.ScanDataObj
-attribute), 79
-attribute), 79
+attribute), 82
+attribute), 82
 hold()
-(pysces.PyscesPlot2.MatplotlibUPI
-IS_VALID (pysces.PyscesModel.IntegrationDataObj
-method), 54
+(pysces.PyscesPlot2.MatplotlibUPI IS_VALID (pysces.PyscesModel.IntegrationDataObj
+method), 56
+attribute), 65
+HYBRD() (pysces.PyscesModel.PysMod method), IS_VALID (pysces.PyscesModel.StateDataObj at69
+tribute), 83
+isnotebook() (pysces.PyscesPlot2.MatplotlibUPI
+I
+method), 56
+info_moiety_conserve
+method), 83
+GnuPlotUPI (class in pysces.PyscesPlot2), 52
 
 Index
 
-101
+109
+
+PySCeS User Guide, Release 1.1.0
 
-PySCeS User Guide, Release 1.0.0
-matrix (pysces.PyscesModel.BagOfStuff atattribute), 62
-tribute), 60
-IS_VALID (pysces.PyscesModel.StateDataObj atMatrixFloatFix()
-tribute), 79
-(pysces.PyscesStoich.MathArrayFunc
-isnotebook() (pysces.PyscesPlot2.MatplotlibUPI
-method), 86
-method), 54
-MatrixValueCompare()
 K
+
+MatrixFloatFix()
 (pysces.PyscesStoich.MathArrayFunc
 K_split_R()
 (pysces.PyscesStoich.Stoich
-method), 86
-method), 89
-MAX_OPEN_WINDOWS
-(pysces.PyscesPlot2.MatplotlibUPI
+method), 90
+method), 92
+MatrixValueCompare()
 L
-attribute), 53
+(pysces.PyscesStoich.MathArrayFunc
+method), 90
 L_split_R()
-(pysces.PyscesStoich.Stoich METATOOLlink (class in pysces.PyscesLink), 91
-method), 89
-mod (pysces.PyscesModel.Event attribute), 61
+(pysces.PyscesStoich.Stoich
+MAX_OPEN_WINDOWS
+method), 93
+(pysces.PyscesPlot2.MatplotlibUPI
 layoutModuleGetSVG()
-mod
-(pysces.PyscesModel.EventAssignment
+attribute), 55
 (pysces.PyscesLink.SBWLayoutWebLink
-attribute), 61
-method), 92
-mod (pysces.PyscesModel.Function attribute), 62
+METATOOLlink (class in pysces.PyscesLink), 98
+method), 99
+mod (pysces.PyscesModel.Event attribute), 63
 LAYOUTMODULELOADED
-mod (pysces.PyscesModel.ReactionObj attribute),
-(pysces.PyscesLink.SBWLayoutWebLink
-78
-attribute), 91
-mod_data (pysces.PyscesModel.ScanDataObj atlayoutModuleLoadSBML()
-tribute), 79
-(pysces.PyscesLink.SBWLayoutWebLink mod_data_labels
-method), 92
+(pysces.PyscesModel.EventAssignment
+(pysces.PyscesLink.SBWLayoutWebLink mod
+attribute), 64
+attribute), 98
+mod
+(pysces.PyscesModel.Function
+attribute), 64
+layoutModuleLoadSBML()
+(pysces.PyscesLink.SBWLayoutWebLink mod (pysces.PyscesModel.ReactionObj attribute),
+81
+method), 99
+mod_data
+(pysces.PyscesModel.ScanDataObj atLinAlgError (pysces.PyscesStoich.MathArrayFunc
+tribute), 82
+attribute), 90
+mod_data_labels
+list() (pysces.PyscesModel.BagOfStuff method),
 (pysces.PyscesModel.ScanDataObj
-LinAlgError (pysces.PyscesStoich.MathArrayFunc
-attribute), 79
-attribute), 86
-model (pysces.PyscesScan.PITCONScanUtils atlist() (pysces.PyscesModel.BagOfStuff method),
-tribute), 81
-60
+62
+attribute), 82
+listAllOrdered()
+model
+(pysces.PyscesScan.PITCONScanUtils
+at(pysces.PyscesModel.BagOfStuff
+tribute), 84
+method), 63
 ModelLoad()
 (pysces.PyscesModel.PysMod
-listAllOrdered()
-method), 67
-(pysces.PyscesModel.BagOfStuff
-module
-method), 60
-pysces.PyscesInterfaces, 85
 load() (pysces.PyscesModel.BagOfStuff method),
-pysces.PyscesLink, 91
-60
-pysces.PyscesModel, 60
-LoadFromFile() (pysces.PyscesModel.PysMod
-pysces.PyscesParScan, 84
-method), 67
-pysces.PyscesPlot2, 49
+method), 70
+63
+LoadFromFile() (pysces.PyscesModel.PysMod module
+pysces.PyscesInterfaces, 88
+method), 70
+pysces.PyscesLink, 98
 LoadFromString()
-pysces.PyscesScan, 80
+pysces.PyscesModel, 62
 (pysces.PyscesModel.PysMod method),
-pysces.PyscesStoich, 86
-67
-pysces.PyscesUtils, 47
+pysces.PyscesParScan, 87
+70
+pysces.PyscesPlot2, 51
 loadSBMLFileFromDisk()
-moduleDict (pysces.PyscesLink.SBWlink at(pysces.PyscesLink.SBWLayoutWebLink
-tribute), 92
-method), 92
-modules (pysces.PyscesLink.SBWlink attribute),
+pysces.PyscesScan, 84
+(pysces.PyscesLink.SBWLayoutWebLink
+pysces.PyscesStoich, 90
+method), 99
+pysces.PyscesUtils, 49
 loadSBMLFromString()
-92
-(pysces.PyscesLink.SBWLayoutWebLink MSG_PRINT_INTERVAL
-method), 92
-(pysces.PyscesParScan.ParScanner
+moduleDict
+(pysces.PyscesLink.SBWlink at(pysces.PyscesLink.SBWLayoutWebLink
+tribute), 99
+method), 99
+modules
+(pysces.PyscesLink.SBWlink attribute),
 LSODA() (pysces.PyscesModel.PysMod method),
-attribute), 84
-67
+99
+70
 MSG_PRINT_INTERVAL
-(pysces.PyscesScan.Scanner attribute),
 M
-82
-m (pysces.PyscesPlot2.PyscesUPI attribute), 58
+(pysces.PyscesParScan.ParScanner
+attribute), 88
+m (pysces.PyscesPlot2.PyscesUPI attribute), 60
+mach_eps (pysces.PyscesStoich.Stoich attribute), MSG_PRINT_INTERVAL
+(pysces.PyscesScan.Scanner attribute),
+97
+85
+machar (pysces.PyscesStoich.Stoich.finfo property), 96
 makeRange()
 (pysces.PyscesScan.Scanner N
-method), 83
-name (pysces.PyscesModel.NewCoreBase atMathArrayFunc (class in pysces.PyscesStoich), 86
+name (pysces.PyscesModel.PieceWise attribute),
+method), 86
+67
+MathArrayFunc (class in pysces.PyscesStoich), 90
+MatplotlibUPI (class in pysces.PyscesPlot2), 55 nan_on_bad_state
+(pysces.PyscesParScan.ParScanner
+matrix (pysces.PyscesModel.BagOfStuff atattribute), 88
 tribute), 63
-MatplotlibUPI (class in pysces.PyscesPlot2), 53 name (pysces.PyscesModel.PieceWise attribute),
-
-102
+110
 
 Index
 
-PySCeS User Guide, Release 1.0.0
-64
-nan_on_bad_state
-(pysces.PyscesParScan.ParScanner
-attribute), 85
-nan_on_bad_state (pysces.PyscesScan.Scanner
-attribute), 83
-NewCoreBase (class in pysces.PyscesModel), 63
-NLEQ2() (pysces.PyscesModel.PysMod method),
-68
-normal_timer() (pysces.PyscesUtils.TimerBox
-method), 47
-NumberBase (class in pysces.PyscesModel), 64
-
-pitcon_range_low
+PySCeS User Guide, Release 1.1.0
+nan_on_bad_state (pysces.PyscesScan.Scanner pitcon_scan_density
 (pysces.PyscesScan.PITCONScanUtils
-attribute), 81
-pitcon_res (pysces.PyscesScan.PITCONScanUtils
-attribute), 81
-pitcon_scan_density
-(pysces.PyscesScan.PITCONScanUtils
-attribute), 81
+attribute), 87
+attribute), 84
+NLEQ2() (pysces.PyscesModel.PysMod method),
 pitcon_scan_parameter
+70
 (pysces.PyscesScan.PITCONScanUtils
-attribute), 81
+normal_timer() (pysces.PyscesUtils.TimerBox
+attribute), 84
+method), 49
 pitcon_scan_parameter_3d
-(pysces.PyscesScan.PITCONScanUtils
 O
-attribute), 81
-OPEN (pysces.PyscesModel.ScanDataObj at- PITCONScanUtils (class in pysces.PyscesScan),
-tribute), 78
-81
+(pysces.PyscesScan.PITCONScanUtils
+OPEN (pysces.PyscesModel.ScanDataObj atattribute), 84
+tribute), 81
+PITCONScanUtils (class in pysces.PyscesScan),
+84
+P
 PivotSort()
 (pysces.PyscesStoich.Stoich
-P
-method), 89
 p_activateInterface()
-PivotSort_initial()
-(pysces.PyscesPlot2.PyscesUPI method),
+method), 93
+(pysces.PyscesPlot2.PyscesUPI method), PivotSort_initial()
+60
 (pysces.PyscesStoich.Stoich
 method),
-58
-89
 p_deactivateInterface()
-plot()
+93
+(pysces.PyscesPlot2.PyscesUPI method), plot()
 (pysces.PyscesPlot2.GnuPlotUPI
-(pysces.PyscesPlot2.PyscesUPI method),
-method), 51
-58
+60
+method), 53
+p_setInterface()
 plot()
 (pysces.PyscesPlot2.MatplotlibUPI
-p_setInterface()
-method), 54
-(pysces.PyscesPlot2.PyscesUPI method), plot() (pysces.PyscesPlot2.PlotBase method), 55
-58
-plot() (pysces.PyscesPlot2.PyscesUPI method),
+(pysces.PyscesPlot2.PyscesUPI method),
+method), 56
+60
+plot() (pysces.PyscesPlot2.PlotBase method), 58
 parameter_labels
-58
+plot() (pysces.PyscesPlot2.PyscesUPI method),
 (pysces.PyscesModel.ScanDataObj
-PlotBase (class in pysces.PyscesPlot2), 55
-attribute), 79
-plotLines() (pysces.PyscesPlot2.GnuPlotUPI
-parameters (pysces.PyscesModel.ScanDataObj
-method), 51
-attribute), 79
-plotLines() (pysces.PyscesPlot2.MatplotlibUPI
+60
+attribute), 82
+PlotBase (class in pysces.PyscesPlot2), 57
+parameters (pysces.PyscesModel.ScanDataObj plotLines() (pysces.PyscesPlot2.GnuPlotUPI
+attribute), 82
+method), 53
 ParGenSim()
-(pysces.PyscesModel.PysMod
-method), 54
-method), 68
-plotLines()
-(pysces.PyscesPlot2.PlotBase
-ParScanner (class in pysces.PyscesParScan), 84
+(pysces.PyscesModel.PysMod plotLines() (pysces.PyscesPlot2.MatplotlibUPI
+method), 71
 method), 56
-PAUSE_TIME (pysces.PyscesPlot2.GnuPlotUPI at- plotLines()
+ParScanner (class in pysces.PyscesParScan), 87 plotLines()
+(pysces.PyscesPlot2.PlotBase
+PAUSE_TIME (pysces.PyscesPlot2.GnuPlotUPI atmethod), 58
+tribute), 52
+plotLines()
 (pysces.PyscesPlot2.PyscesUPI
-tribute), 50
-method), 58
-PieceWise (class in pysces.PyscesModel), 64
+persistent (pysces.PyscesModel.Event atmethod), 61
+tribute), 63
 PLUfactorize()
 (pysces.PyscesStoich.Stoich
-piecewises (pysces.PyscesModel.Event atmethod), 89
-tribute), 61
-Prepare() (pysces.PyscesParScan.ParScanner
-piecewises (pysces.PyscesModel.EventAssignment
-method), 84
-attribute), 61
-psbw (pysces.PyscesLink.SBWlink attribute), 92
+PieceWise (class in pysces.PyscesModel), 66
+method), 93
+piecewises (pysces.PyscesModel.Event at- Prepare() (pysces.PyscesParScan.ParScanner
+tribute), 63
+method), 88
+piecewises (pysces.PyscesModel.EventAssignment priority (pysces.PyscesModel.Event attribute),
+attribute), 64
+63
 piecewises
-(pysces.PyscesModel.Function pyplot
+(pysces.PyscesModel.Function psbw (pysces.PyscesLink.SBWlink attribute), 99
+attribute), 64
+pyplot
 (pysces.PyscesPlot2.MatplotlibUPI
-attribute), 62
-attribute), 54
-piecewises (pysces.PyscesModel.ReactionObj pysces.PyscesInterfaces
-attribute), 78
-module, 85
-PITCON() (pysces.PyscesModel.PysMod method), pysces.PyscesLink
-68
-module, 91
+piecewises (pysces.PyscesModel.ReactionObj
+attribute), 56
+attribute), 81
+pysces.PyscesInterfaces
+PITCON() (pysces.PyscesModel.PysMod method),
+module, 88
+71
+pysces.PyscesLink
 pitcon_range_high
-pysces.PyscesModel
+module, 98
 (pysces.PyscesScan.PITCONScanUtils
-module, 60
-attribute), 81
+pysces.PyscesModel
+attribute), 84
+module, 62
+pitcon_range_low
 pysces.PyscesParScan
-
+(pysces.PyscesScan.PITCONScanUtils
+module, 87
+attribute), 84
+pysces.PyscesPlot2
+pitcon_res (pysces.PyscesScan.PITCONScanUtils
+module, 51
+attribute), 84
 Index
 
-103
+111
 
-PySCeS User Guide, Release 1.0.0
-res_flux (pysces.PyscesScan.PITCONScanUtils
-attribute), 81
-res_idx (pysces.PyscesScan.PITCONScanUtils
-attribute), 81
+PySCeS User Guide, Release 1.1.0
 res_metab (pysces.PyscesScan.PITCONScanUtils
-attribute), 81
+attribute), 85
 res_user (pysces.PyscesScan.PITCONScanUtils
-attribute), 81
-reset() (pysces.PyscesModel.Event method), 61
+attribute), 85
+reset() (pysces.PyscesModel.Event method), 63
 reset_step()
 (pysces.PyscesUtils.TimerBox
-method), 47
+method), 49
 resetInputParameters()
+(pysces.PyscesScan.Scanner method), 87
 Q
-(pysces.PyscesScan.Scanner method), 84
-quietRun (pysces.PyscesScan.Scanner attribute), ResetNumberFormat()
-83
+ResetNumberFormat()
+quietRun (pysces.PyscesScan.Scanner attribute),
 (pysces.PyscesModel.PysMod method),
-68
-R
+87
+71
 ridx (pysces.PyscesStoich.StructMatrix attribute),
-random (pysces.PyscesModel.PysMod attribute),
-90
-75
-row (pysces.PyscesModel.BagOfStuff attribute), 60
-rangeGen()
-(pysces.PyscesScan.Scanner row (pysces.PyscesStoich.StructMatrix attribute),
-method), 83
-91
-rate (pysces.PyscesModel.ReactionObj attribute), rules (pysces.PyscesModel.IntegrationDataObj
+R
+97
+random (pysces.PyscesModel.PysMod attribute), row (pysces.PyscesModel.BagOfStuff attribute), 63
 78
-attribute), 63
-rate_labels (pysces.PyscesModel.IntegrationDataObj
-rules (pysces.PyscesModel.ScanDataObj atattribute), 63
-tribute), 79
-rates (pysces.PyscesModel.IntegrationDataObj rules (pysces.PyscesModel.StateDataObj atattribute), 63
-tribute), 80
-ReactionObj (class in pysces.PyscesModel), 78
+row (pysces.PyscesStoich.StructMatrix attribute),
+rangeGen()
+(pysces.PyscesScan.Scanner
+97
+method), 87
+rules (pysces.PyscesModel.IntegrationDataObj
+rate (pysces.PyscesModel.ReactionObj attribute),
+attribute), 66
+81
+rules (pysces.PyscesModel.ScanDataObj atrate_labels (pysces.PyscesModel.IntegrationDataObj
+tribute), 82
+attribute), 66
+rules (pysces.PyscesModel.StateDataObj atrates (pysces.PyscesModel.IntegrationDataObj
+tribute), 83
+attribute), 66
 rules_labels (pysces.PyscesModel.IntegrationDataObj
+ReactionObj (class in pysces.PyscesModel), 81
+attribute), 66
 readMod2Core()
-attribute), 63
-(pysces.PyscesInterfaces.Core2interfaces rules_labels (pysces.PyscesModel.ScanDataObj
-method), 85
-attribute), 79
-readSBMLToCore()
-rules_labels (pysces.PyscesModel.StateDataObj
+rules_labels (pysces.PyscesModel.ScanDataObj
 (pysces.PyscesInterfaces.Core2interfaces
-attribute), 80
-method), 85
-Run()
+attribute), 82
+method), 89
+rules_labels (pysces.PyscesModel.StateDataObj
+readSBMLToCore()
+attribute), 83
+(pysces.PyscesInterfaces.Core2interfaces Run()
 (pysces.PyscesParScan.ParScanner
-reLoad() (pysces.PyscesModel.PysMod method),
-method), 84
-75
-Run() (pysces.PyscesScan.Scanner method), 82
-ReloadInitFunc()
+method), 89
+method), 88
+reLoad() (pysces.PyscesModel.PysMod method), Run() (pysces.PyscesScan.Scanner method), 85
+78
 RunAgain()
 (pysces.PyscesScan.Scanner
-(pysces.PyscesModel.PysMod method),
-method), 82
-68
-runContinuation()
-ReloadUserFunc()
+ReloadInitFunc()
+method), 86
+(pysces.PyscesModel.PysMod method), runContinuation()
+71
 (pysces.PyscesScan.PITCONScanUtils
-(pysces.PyscesModel.PysMod method),
-method), 81
-68
-RunScatter() (pysces.PyscesParScan.ParScanner
+ReloadUserFunc()
+method), 85
+(pysces.PyscesModel.PysMod method), RunScatter() (pysces.PyscesParScan.ParScanner
+71
+method), 88
 replot()
 (pysces.PyscesPlot2.GnuPlotUPI
-method), 84
-method), 51
+method), 53
+S
 replot()
-(pysces.PyscesPlot2.PyscesUPI S
-method), 58
-save()
+(pysces.PyscesPlot2.PyscesUPI save()
 (pysces.PyscesPlot2.GnuPlotUPI
+method), 61
+method), 53
 replotAndWait()
-method), 51
-(pysces.PyscesPlot2.GnuPlotUPI
 save()
 (pysces.PyscesPlot2.MatplotlibUPI
-method), 51
-method), 54
-res_eigen (pysces.PyscesScan.PITCONScanUtils save() (pysces.PyscesPlot2.PlotBase method), 56
-attribute), 81
-save() (pysces.PyscesPlot2.PyscesUPI method),
+(pysces.PyscesPlot2.GnuPlotUPI
+method), 56
+method), 53
+save() (pysces.PyscesPlot2.PlotBase method), 58
+res_eigen (pysces.PyscesScan.PITCONScanUtils save() (pysces.PyscesPlot2.PyscesUPI method),
+attribute), 84
+61
+res_flux (pysces.PyscesScan.PITCONScanUtils sbml (pysces.PyscesInterfaces.Core2interfaces atattribute), 84
+tribute), 89
+res_idx (pysces.PyscesScan.PITCONScanUtils sbml (pysces.PyscesLink.SBWLayoutWebLink atattribute), 84
 
-module, 84
-pysces.PyscesPlot2
-module, 49
 pysces.PyscesScan
-module, 80
+module, 84
 pysces.PyscesStoich
-module, 86
+module, 90
 pysces.PyscesUtils
-module, 47
-PyscesUPI (class in pysces.PyscesPlot2), 57
-PysMod (class in pysces.PyscesModel), 64
+module, 49
+PyscesUPI (class in pysces.PyscesPlot2), 60
+PysMod (class in pysces.PyscesModel), 67
 
-104
+112
 
 Index
 
-PySCeS User Guide, Release 1.0.0
-51
-59
-(pysces.PyscesModel.Function
-sbml (pysces.PyscesInterfaces.Core2interfaces at- setArg()
-method), 62
-tribute), 85
-sbml (pysces.PyscesLink.SBWLayoutWebLink at- setAssignment() (pysces.PyscesModel.Event
-method), 61
-tribute), 92
+PySCeS User Guide, Release 1.1.0
+method), 63
+tribute), 99
 sbml2core (pysces.PyscesInterfaces.Core2interfacessetAxisLabel()
 (pysces.PyscesPlot2.GnuPlotUPI
-attribute), 85
-method), 51
+attribute), 89
+method), 53
 sbml_level (pysces.PyscesInterfaces.Core2interfaces
 setAxisLabel()
-attribute), 85
+attribute), 89
 (pysces.PyscesPlot2.MatplotlibUPI
 sbml_version (pysces.PyscesInterfaces.Core2interfaces
-method), 54
-attribute), 85
+method), 57
+attribute), 89
 sbmllayout (pysces.PyscesLink.SBWLayoutWebLinksetAxisLabel() (pysces.PyscesPlot2.PlotBase
-method), 56
-attribute), 92
+method), 58
+attribute), 99
 setAxisLabel() (pysces.PyscesPlot2.PyscesUPI
-sbw (pysces.PyscesLink.SBWlink attribute), 92
-method), 59
+sbw (pysces.PyscesLink.SBWlink attribute), 99
+method), 61
 SBW_exposeAll() (pysces.PyscesLink.SBWlink
 setByIdx() (pysces.PyscesStoich.StructMatrix
-method), 92
-method), 91
+method), 99
+method), 97
 SBW_getActiveModules()
-(pysces.PyscesLink.SBWlink method), 92 setByName() (pysces.PyscesStoich.StructMatrix
-method), 91
+(pysces.PyscesLink.SBWlink method), 99 setByName() (pysces.PyscesStoich.StructMatrix
+method), 97
 SBW_loadModule() (pysces.PyscesLink.SBWlink
 setCol()
 (pysces.PyscesStoich.StructMatrix
-method), 92
-method), 91
+method), 99
+method), 97
 sbwhost (pysces.PyscesLink.SBWLayoutWebLink
 setDataFileNumberFormat()
-attribute), 92
+attribute), 99
 (pysces.PyscesPlot2.GnuPlotUPI
 SBWLayoutWebLink (class in pysces.PyscesLink),
-method), 51
-91
+method), 54
+98
 setFluxes() (pysces.PyscesModel.StateDataObj
-SBWlink (class in pysces.PyscesLink), 92
-method), 80
+SBWlink (class in pysces.PyscesLink), 99
+method), 83
 sbwModuleProxy (pysces.PyscesLink.SBWlink atsetFormula() (pysces.PyscesModel.EventAssignment
-tribute), 92
-method), 61
+tribute), 99
+method), 64
 ScaleKL()
 (pysces.PyscesModel.PysMod
 setGraphTitle()
-method), 68
+method), 71
 (pysces.PyscesPlot2.GnuPlotUPI
 ScalePivots()
 (pysces.PyscesStoich.Stoich
-method), 51
-method), 90
-scan (pysces.PyscesModel.PysMod property), 75 setGraphTitle()
+method), 54
+method), 93
+scan (pysces.PyscesModel.PysMod property), 78 setGraphTitle()
 (pysces.PyscesPlot2.MatplotlibUPI
 Scan1() (pysces.PyscesModel.PysMod method),
-method), 54
-68
+method), 57
+71
 Scan1Plot()
 (pysces.PyscesModel.PysMod setGraphTitle() (pysces.PyscesPlot2.PlotBase
-method), 56
-method), 69
+method), 58
+method), 72
 Scan2D() (pysces.PyscesModel.PysMod method), setGraphTitle()
 (pysces.PyscesPlot2.PyscesUPI method),
-69
-59
+72
+61
 Scan2DPlot()
 (pysces.PyscesModel.PysMod
 setGrid()
 (pysces.PyscesPlot2.GnuPlotUPI
-method), 69
-method), 52
-ScanDataObj (class in pysces.PyscesModel), 78
+method), 72
+method), 54
+ScanDataObj (class in pysces.PyscesModel), 81
 setGrid() (pysces.PyscesPlot2.MatplotlibUPI
-Scanner (class in pysces.PyscesScan), 82
-method), 55
+Scanner (class in pysces.PyscesScan), 85
+method), 57
 scans_per_run (pysces.PyscesParScan.ParScanner
 setGrid()
 (pysces.PyscesPlot2.PlotBase
-attribute), 85
-method), 56
+attribute), 88
+method), 58
 select()
 (pysces.PyscesModel.BagOfStuff
 setGrid()
 (pysces.PyscesPlot2.PyscesUPI
-method), 60
-method), 59
+method), 63
+method), 61
 SerialDecode() (pysces.PyscesModel.PysMod
 setKey()
 (pysces.PyscesPlot2.GnuPlotUPI
-method), 69
-method), 52
+method), 72
+method), 54
 SerialEncode() (pysces.PyscesModel.PysMod
 setKey()
 (pysces.PyscesPlot2.MatplotlibUPI
-method), 69
-method), 55
+method), 72
+method), 57
 set() (pysces.PyscesPlot2.GnuPlotUPI method),
+setKey() (pysces.PyscesPlot2.PlotBase method),
+53
+59
+setArg()
+(pysces.PyscesModel.Function
+setKey()
+(pysces.PyscesPlot2.PyscesUPI
+method), 64
+method), 61
+setAssignment() (pysces.PyscesModel.Event
 
 Index
 
-105
+113
 
-PySCeS User Guide, Release 1.0.0
-method), 52
-setKey() (pysces.PyscesPlot2.PlotBase method),
-setRange() (pysces.PyscesPlot2.MatplotlibUPI
-56
-method), 55
-setKey()
-(pysces.PyscesPlot2.PyscesUPI
-setRange()
-(pysces.PyscesPlot2.PlotBase
-method), 59
+PySCeS User Guide, Release 1.1.0
 method), 57
 setKineticLaw()
 setRange()
-(pysces.PyscesPlot2.PyscesUPI
+(pysces.PyscesPlot2.PlotBase
 (pysces.PyscesModel.ReactionObj
 method), 59
-method), 78
-setRates() (pysces.PyscesModel.IntegrationDataObj
+method), 81
+setRange()
+(pysces.PyscesPlot2.PyscesUPI
 setLabels() (pysces.PyscesModel.IntegrationDataObj
-method), 63
-method), 63
+method), 62
+method), 66
+setLabels() (pysces.PyscesModel.ScanDataObj setRates() (pysces.PyscesModel.IntegrationDataObj
+method), 66
+method), 82
+setRow()
 (pysces.PyscesStoich.StructMatrix
-setLabels() (pysces.PyscesModel.ScanDataObj setRow()
-method), 91
-method), 79
-setRules() (pysces.PyscesModel.IntegrationDataObj
 setLineWidth()
-method), 63
+method), 98
 (pysces.PyscesPlot2.MatplotlibUPI
-setRules() (pysces.PyscesModel.StateDataObj
-method), 55
-method), 80
+setRules() (pysces.PyscesModel.IntegrationDataObj
+method), 57
+method), 66
 setLogScale() (pysces.PyscesPlot2.GnuPlotUPI
-setSize()
-(pysces.PyscesPlot2.GnuPlotUPI
-method), 52
-method), 52
+setRules() (pysces.PyscesModel.StateDataObj
+method), 54
+method), 83
 setLogScale() (pysces.PyscesPlot2.MatplotlibUPI
-setSizeAndOrigin()
-method), 55
-(pysces.PyscesPlot2.GnuPlotUPI
+setSequence() (pysces.PyscesModel.EventsProblem
+method), 57
+method), 64
 setLogScale()
 (pysces.PyscesPlot2.PlotBase
-method), 52
-method), 56
-setLogScale() (pysces.PyscesPlot2.PyscesUPI setSpecies() (pysces.PyscesModel.IntegrationDataObj
-method), 63
+setSize()
+(pysces.PyscesPlot2.GnuPlotUPI
 method), 59
+method), 54
+setLogScale() (pysces.PyscesPlot2.PyscesUPI
+setSizeAndOrigin()
+method), 61
+(pysces.PyscesPlot2.GnuPlotUPI
 SetLoud()
-(pysces.PyscesModel.PysMod setSpecies() (pysces.PyscesModel.StateDataObj
-method), 80
-method), 70
+(pysces.PyscesModel.PysMod
+method), 54
+method), 72
 setModValue()
 (in
-module SetStateSymb() (pysces.PyscesModel.PysMod
-method), 70
-pysces.PyscesParScan), 85
+module setSpecies() (pysces.PyscesModel.IntegrationDataObj
+method), 66
+pysces.PyscesParScan), 88
 setModValue()
-(pysces.PyscesScan.Scanner setTerminal() (pysces.PyscesPlot2.GnuPlotUPI
-method), 53
-method), 84
-setTime() (pysces.PyscesModel.IntegrationDataObj
+(pysces.PyscesScan.Scanner setSpecies() (pysces.PyscesModel.StateDataObj
+method), 83
+method), 87
+SetStateSymb() (pysces.PyscesModel.PysMod
 setMultiplot()
-method), 63
+method), 73
+(pysces.PyscesPlot2.GnuPlotUPI
+setTerminal() (pysces.PyscesPlot2.GnuPlotUPI
+method), 54
+method), 55
+setNoLogScale()
+setTime() (pysces.PyscesModel.IntegrationDataObj
 (pysces.PyscesPlot2.GnuPlotUPI
+method), 66
+method), 54
 setTrigger()
 (pysces.PyscesModel.Event
-method), 52
-method), 61
-setName() (pysces.PyscesModel.NewCoreBase
-setUserOuput()
+setNoLogScale()
 method), 63
+(pysces.PyscesPlot2.MatplotlibUPI
+setUserOuput()
+method), 57
 (pysces.PyscesScan.PITCONScanUtils
-setNoLogScale()
-method), 82
-(pysces.PyscesPlot2.GnuPlotUPI
-setValue() (pysces.PyscesModel.NumberBase
-method), 52
-method), 64
-setNoLogScale()
+setNoLogScale() (pysces.PyscesPlot2.PlotBase
+method), 85
+method), 59
 setVariable() (pysces.PyscesModel.EventAssignment
-(pysces.PyscesPlot2.MatplotlibUPI
-method), 61
-method), 55
-setNoLogScale() (pysces.PyscesPlot2.PlotBase setXData() (pysces.PyscesModel.IntegrationDataObj
-method), 63
-method), 56
-setXData() (pysces.PyscesModel.StateDataObj
 setNoLogScale()
-method), 80
+method), 64
 (pysces.PyscesPlot2.PyscesUPI method),
-shape (pysces.PyscesStoich.StructMatrix at59
-tribute), 91
+setXData() (pysces.PyscesModel.IntegrationDataObj
+61
+method), 66
 setOrigin() (pysces.PyscesPlot2.GnuPlotUPI
+setXData() (pysces.PyscesModel.StateDataObj
+method), 54
+method), 83
+setPersistent() (pysces.PyscesModel.Event
+shape (pysces.PyscesStoich.StructMatrix atmethod), 63
+tribute), 98
+setPriority()
+(pysces.PyscesModel.Event
 showCC() (pysces.PyscesModel.PysMod method),
-method), 52
-75
+method), 63
+78
 setProxy() (pysces.PyscesLink.SBWLayoutWebLink
 showConserved() (pysces.PyscesModel.PysMod
-method), 92
-method), 75
+method), 99
+method), 78
 SetQuiet()
 (pysces.PyscesModel.PysMod
 showEigen()
 (pysces.PyscesModel.PysMod
-method), 70
-method), 75
+method), 73
+method), 78
 setRange()
 (pysces.PyscesPlot2.GnuPlotUPI
+showElas()
+(pysces.PyscesModel.PysMod
+method), 54
+method), 78
+setRange() (pysces.PyscesPlot2.MatplotlibUPI
 
-106
+114
 
 Index
 
-PySCeS User Guide, Release 1.0.0
-showElas()
-(pysces.PyscesModel.PysMod species (pysces.PyscesModel.StateDataObj attribute), 80
-method), 75
-showEModes() (pysces.PyscesLink.METATOOLlink species_labels
-(pysces.PyscesModel.IntegrationDataObj
-method), 91
-attribute), 63
+PySCeS User Guide, Release 1.1.0
+tribute), 82
+showEModes() (pysces.PyscesLink.METATOOLlink
+species (pysces.PyscesModel.StateDataObj atmethod), 98
+tribute), 83
 showEpar()
 (pysces.PyscesModel.PysMod
 species_labels
-method), 75
-(pysces.PyscesModel.ScanDataObj
+method), 79
+(pysces.PyscesModel.IntegrationDataObj
 showEvar()
 (pysces.PyscesModel.PysMod
-attribute), 79
-method), 76
+attribute), 66
+method), 79
 species_labels
 showFluxRelationships()
-(pysces.PyscesModel.StateDataObj
+(pysces.PyscesModel.ScanDataObj
 (pysces.PyscesModel.PysMod method),
-attribute), 80
-76
-showK() (pysces.PyscesModel.PysMod method), SplitLU() (pysces.PyscesStoich.Stoich method),
-90
-76
-(pysces.PyscesPlot2.GnuPlotUPI
-showL() (pysces.PyscesModel.PysMod method), splot()
-method), 53
-76
+attribute), 82
+79
+showK() (pysces.PyscesModel.PysMod method), species_labels
+(pysces.PyscesModel.StateDataObj
+79
+attribute), 83
+showL() (pysces.PyscesModel.PysMod method),
+SplitLU() (pysces.PyscesStoich.Stoich method),
+79
+94
 showModel()
-(pysces.PyscesModel.PysMod splot() (pysces.PyscesPlot2.PlotBase method),
-57
-method), 76
-showModifiers() (pysces.PyscesModel.PysMod splot() (pysces.PyscesPlot2.PyscesUPI method),
-59
-method), 76
-showN() (pysces.PyscesModel.PysMod method), splotSurfaces()
+(pysces.PyscesModel.PysMod
+splot()
 (pysces.PyscesPlot2.GnuPlotUPI
-76
-method), 53
+method), 79
+method), 55
+showModifiers() (pysces.PyscesModel.PysMod
+splot() (pysces.PyscesPlot2.PlotBase method),
+method), 79
+59
+showN() (pysces.PyscesModel.PysMod method),
+splot() (pysces.PyscesPlot2.PyscesUPI method),
+79
+62
 showNr() (pysces.PyscesModel.PysMod method),
-splotSurfaces() (pysces.PyscesPlot2.PlotBase
-77
-method), 57
+splotSurfaces()
+80
+(pysces.PyscesPlot2.GnuPlotUPI
 showODE()
 (pysces.PyscesModel.PysMod
-splotSurfaces()
-method), 77
-(pysces.PyscesPlot2.PyscesUPI method),
+method), 55
+method), 80
 showODEr()
-(pysces.PyscesModel.PysMod
-60
-method), 77
+(pysces.PyscesModel.PysMod splotSurfaces() (pysces.PyscesPlot2.PlotBase
+method), 59
+method), 80
 showPar()
-(pysces.PyscesModel.PysMod state (pysces.PyscesModel.Event attribute), 61
-State() (pysces.PyscesModel.PysMod method),
-method), 77
-71
+(pysces.PyscesModel.PysMod splotSurfaces()
+(pysces.PyscesPlot2.PyscesUPI method),
+method), 80
+62
 showRate()
 (pysces.PyscesModel.PysMod
-state0 (pysces.PyscesModel.Event attribute), 61
-method), 77
+state (pysces.PyscesModel.Event attribute), 63
+method), 80
 showRateEq()
-(pysces.PyscesModel.PysMod state_events()
+(pysces.PyscesModel.PysMod State() (pysces.PyscesModel.PysMod method),
+74
+method), 80
+showSpecies() (pysces.PyscesModel.PysMod state0 (pysces.PyscesModel.Event attribute), 63
+state_events()
+method), 80
 (pysces.PyscesModel.EventsProblem
-method), 77
-method), 61
-showSpecies() (pysces.PyscesModel.PysMod
-StateDataObj (class in pysces.PyscesModel), 79
-method), 77
-step_timer()
-(pysces.PyscesUtils.TimerBox
 showSpeciesFixed()
-method), 47
+method), 64
 (pysces.PyscesModel.PysMod method),
-stepGen() (pysces.PyscesScan.Scanner method),
-77
-84
-showSpeciesI() (pysces.PyscesModel.PysMod
-Stoich (class in pysces.PyscesStoich), 88
-method), 77
+StateDataObj (class in pysces.PyscesModel), 82
+80
+(pysces.PyscesUtils.TimerBox
+showSpeciesI() (pysces.PyscesModel.PysMod step_timer()
+method), 49
+method), 80
 showState()
-(pysces.PyscesModel.PysMod Stoich_nmatrix_SetValue()
-(pysces.PyscesModel.PysMod method),
-method), 78
-71
-sim (pysces.PyscesModel.PysMod property), 78
+(pysces.PyscesModel.PysMod stepGen() (pysces.PyscesScan.Scanner method),
+87
+method), 81
+Stoich (class in pysces.PyscesStoich), 92
+sim (pysces.PyscesModel.PysMod property), 81
 SimPlot()
-(pysces.PyscesModel.PysMod Stoichiometry_Analyse()
+(pysces.PyscesModel.PysMod Stoich.finfo (class in pysces.PyscesStoich), 94
+Stoich_nmatrix_SetValue()
+method), 73
 (pysces.PyscesModel.PysMod method),
-method), 70
-71
 Simulate()
 (pysces.PyscesModel.PysMod
-Stoichiometry_Init()
-method), 70
+74
+method), 73
+Stoichiometry_Analyse()
+smallest_normal
 (pysces.PyscesModel.PysMod method),
-species (pysces.PyscesModel.IntegrationDataObj
-71
-attribute), 63
-species (pysces.PyscesModel.ScanDataObj at- Stoichiometry_Load_Serial()
+(pysces.PyscesStoich.Stoich.finfo prop74
+erty), 96
+species (pysces.PyscesModel.IntegrationDataObj Stoichiometry_Init()
 (pysces.PyscesModel.PysMod method),
-tribute), 79
+attribute), 66
+74
+species (pysces.PyscesModel.ScanDataObj at-
 
 Index
 
-107
+115
 
-PySCeS User Guide, Release 1.0.0
-71
+PySCeS User Guide, Release 1.1.0
+
+Stoichiometry_Load_Serial()
+(pysces.PyscesModel.PysMod method),
+74
 Stoichiometry_ReAnalyse()
 (pysces.PyscesModel.PysMod method),
-72
+75
 Stoichiometry_Save_Serial()
 (pysces.PyscesModel.PysMod method),
-72
-stop() (pysces.PyscesUtils.TimerBox method), 47
+75
+stop() (pysces.PyscesUtils.TimerBox method), 49
 StoreData() (pysces.PyscesParScan.ParScanner
-method), 84
+method), 88
 StoreData()
 (pysces.PyscesScan.Scanner
-method), 82
-str2bool() (in module pysces.PyscesUtils), 49
-StructMatrix (class in pysces.PyscesStoich), 90
+method), 86
+str2bool() (in module pysces.PyscesUtils), 51
+StructMatrix (class in pysces.PyscesStoich), 97
 SVD_Rank_Check() (pysces.PyscesStoich.Stoich
-method), 89
-svg (pysces.PyscesLink.SBWLayoutWebLink attribute), 92
+method), 93
+svg (pysces.PyscesLink.SBWLayoutWebLink attribute), 99
 SwapCol() (pysces.PyscesStoich.MathArrayFunc
-method), 87
+method), 90
 SwapCold() (pysces.PyscesStoich.MathArrayFunc
-method), 87
+method), 90
 SwapColz() (pysces.PyscesStoich.MathArrayFunc
-method), 87
+method), 90
 SwapElem() (pysces.PyscesStoich.MathArrayFunc
-method), 87
+method), 91
 SwapRow() (pysces.PyscesStoich.MathArrayFunc
-method), 87
+method), 91
 SwapRowd() (pysces.PyscesStoich.MathArrayFunc
-method), 87
+method), 91
 SwapRowz() (pysces.PyscesStoich.MathArrayFunc
-method), 87
-symbols (pysces.PyscesModel.Event attribute), 61
+method), 91
+symbols (pysces.PyscesModel.Event attribute), 63
 symbols (pysces.PyscesModel.EventAssignment
-attribute), 61
+attribute), 64
 symbols
 (pysces.PyscesModel.Function
-attribute), 62
+attribute), 65
 symbols
 (pysces.PyscesModel.ReactionObj
-attribute), 78
+attribute), 81
 
-timer (pysces.PyscesScan.PITCONScanUtils attribute), 82
-TimerBox (class in pysces.PyscesUtils), 47
-trigger (pysces.PyscesModel.Event attribute), 61
+time_label (pysces.PyscesModel.IntegrationDataObj
+attribute), 66
+timer (pysces.PyscesScan.PITCONScanUtils attribute), 85
+TimerBox (class in pysces.PyscesUtils), 49
+tiny (pysces.PyscesStoich.Stoich.finfo property),
+96
+trigger (pysces.PyscesModel.Event attribute), 63
 TYPE_INFO (pysces.PyscesModel.IntegrationDataObj
-attribute), 62
+attribute), 65
 
 U
 unset()
 (pysces.PyscesPlot2.GnuPlotUPI
-method), 53
+method), 55
 unsetMultiplot()
 (pysces.PyscesPlot2.GnuPlotUPI
-method), 53
+method), 55
 urlGET() (pysces.PyscesLink.SBWLayoutWebLink
-method), 92
+method), 99
 urlPOST() (pysces.PyscesLink.SBWLayoutWebLink
-method), 92
-USE_QR (pysces.PyscesStoich.Stoich attribute), 90
+method), 99
+USE_QR (pysces.PyscesStoich.Stoich attribute), 94
 User_Function() (pysces.PyscesModel.PysMod
-method), 72
+method), 75
 user_output (pysces.PyscesScan.PITCONScanUtils
-attribute), 82
+attribute), 85
 
 V
 value (pysces.PyscesModel.Function attribute),
-62
-value (pysces.PyscesModel.NumberBase attribute), 64
+65
 value (pysces.PyscesModel.PieceWise attribute),
-64
-value_initial (pysces.PyscesModel.NumberBase
-attribute), 64
+67
 variable (pysces.PyscesModel.EventAssignment
-attribute), 61
+attribute), 64
 VersionCheck() (in module pysces.PyscesUtils),
-48
+50
 
 W
 
-wait() (pysces.PyscesPlot2.PlotBase method), 57
+wait() (pysces.PyscesPlot2.PlotBase method), 59
 WasteManagement (class in pysces.PyscesModel),
-80
+83
+Write_array() (pysces.PyscesModel.PysMod
+method), 75
 T
-Write_array()
-(pysces.PyscesModel.PysMod
-Terminals (pysces.PyscesPlot2.GnuPlotUPI atmethod),
-72
-tribute), 50
-Write_array_html()
-testInputParameter()
+Terminals (pysces.PyscesPlot2.GnuPlotUPI at- Write_array_html()
 (pysces.PyscesModel.PysMod method),
-(pysces.PyscesScan.Scanner method), 84
-72
-TestSimState() (pysces.PyscesModel.PysMod
+tribute), 52
+75
+testInputParameter()
 Write_array_latex()
-method), 72
+(pysces.PyscesScan.Scanner method), 87
 (pysces.PyscesModel.PysMod method),
-time (pysces.PyscesModel.IntegrationDataObj at72
-tribute), 63
+TestSimState() (pysces.PyscesModel.PysMod
+75
+method), 75
 writeCore2PSC()
-time_label (pysces.PyscesModel.IntegrationDataObj
-(pysces.PyscesInterfaces.Core2interfaces
-attribute), 63
-method), 85
+time (pysces.PyscesModel.IntegrationDataObj at(pysces.PyscesInterfaces.Core2interfaces
+tribute), 66
+method), 89
 
-108
+116
 
 Index
 
-PySCeS User Guide, Release 1.0.0
+PySCeS User Guide, Release 1.1.0
 
 writeCore2SBML()
 (pysces.PyscesInterfaces.Core2interfaces
-method), 86
+method), 89
 writeMod2PSC()
 (pysces.PyscesInterfaces.Core2interfaces
-method), 86
+method), 89
 writeMod2SBML()
 (pysces.PyscesInterfaces.Core2interfaces
-method), 86
-WriteOutput (class in pysces.PyscesUtils), 48
+method), 89
+WriteOutput (class in pysces.PyscesUtils), 50
 
 X
-xcode (pysces.PyscesModel.Event attribute), 61
-xcode (pysces.PyscesModel.EventAssignment attribute), 61
+xcode (pysces.PyscesModel.Event attribute), 63
+xcode (pysces.PyscesModel.EventAssignment attribute), 64
 xcode (pysces.PyscesModel.Function attribute),
-62
+65
 xcode (pysces.PyscesModel.PieceWise attribute),
-64
-xcode (pysces.PyscesModel.ReactionObj attribute), 78
+67
+xcode (pysces.PyscesModel.ReactionObj attribute), 81
 xdata (pysces.PyscesModel.IntegrationDataObj
-attribute), 63
-xdata (pysces.PyscesModel.ScanDataObj attribute), 79
-xdata (pysces.PyscesModel.StateDataObj attribute), 80
+attribute), 66
+xdata (pysces.PyscesModel.ScanDataObj attribute), 82
+xdata (pysces.PyscesModel.StateDataObj attribute), 83
 xdata_labels (pysces.PyscesModel.IntegrationDataObj
-attribute), 63
+attribute), 66
 xdata_labels (pysces.PyscesModel.ScanDataObj
-attribute), 79
+attribute), 82
 xdata_labels (pysces.PyscesModel.StateDataObj
-attribute), 80
+attribute), 83
 
 Index
 
-109
+117
```

### Comparing `pysces-1.0.3/pysces/examples/benchmark.ipy` & `pysces-1.1.0/pysces/examples/benchmark.ipy`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/examples/parallelscan.ipy` & `pysces-1.1.0/pysces/examples/parallelscan.ipy`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/examples/pysces_stochpy.py` & `pysces-1.1.0/pysces/examples/pysces_stochpy.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/examples/testRunScatter.py` & `pysces-1.1.0/pysces/examples/testRunScatter.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/examples/testinvalidstate.py` & `pysces-1.1.0/pysces/examples/testinvalidstate.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/examples/testparscanner.py` & `pysces-1.1.0/pysces/examples/testparscanner.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/examples/testratechar.py` & `pysces-1.1.0/pysces/examples/testratechar.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/kraken/Kraken.py` & `pysces-1.1.0/pysces/kraken/Kraken.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/kraken/KrakenDataTools.py` & `pysces-1.1.0/pysces/kraken/KrakenDataTools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/kraken/KrakenNET.py` & `pysces-1.1.0/pysces/kraken/KrakenNET.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/kraken/KrakenServer.py` & `pysces-1.1.0/pysces/kraken/KrakenServer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/kraken/__init__.py` & `pysces-1.1.0/pysces/kraken/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/kraken/controllers/kraken_continuation.py` & `pysces-1.1.0/pysces/kraken/controllers/kraken_continuation.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/kraken/controllers/kraken_continuation_eigen.py` & `pysces-1.1.0/pysces/kraken/controllers/kraken_continuation_eigen.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/kraken/controllers/kraken_continuation_eigen2.py` & `pysces-1.1.0/pysces/kraken/controllers/kraken_continuation_eigen2.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/kraken/controllers/kraken_intersect.py` & `pysces-1.1.0/pysces/kraken/controllers/kraken_intersect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/kraken/controllers/kraken_scanner2.py` & `pysces-1.1.0/pysces/kraken/controllers/kraken_scanner2.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/kraken/startup.py` & `pysces-1.1.0/pysces/kraken/startup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/lib/FirstDerivatives.py` & `pysces-1.1.0/pysces/lib/FirstDerivatives.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/lib/__init__.py` & `pysces-1.1.0/pysces/lib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/lib/lex.py` & `pysces-1.1.0/pysces/lib/lex.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/lib/miriamids.py` & `pysces-1.1.0/pysces/lib/miriamids.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/lib/pyparsing.py` & `pysces-1.1.0/pysces/lib/pyparsing.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/lib/yacc.py` & `pysces-1.1.0/pysces/lib/yacc.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/metatool/__init__.py` & `pysces-1.1.0/pysces/metatool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/nleq2/CMakeLists.txt` & `pysces-1.1.0/pysces/nleq2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/nleq2/__init__.py` & `pysces-1.1.0/pysces/nleq2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces/nleq2/linalg_nleq2.f` & `pysces-1.1.0/pysces/nleq2/linalg_nleq2.f`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/nleq2/nleq2-4.3.tar.gz` & `pysces-1.1.0/pysces/nleq2/nleq2-4.3.tar.gz`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/nleq2/nleq2.f` & `pysces-1.1.0/pysces/nleq2/nleq2.f`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/nleq2/nleq2.pyf` & `pysces-1.1.0/pysces/nleq2/nleq2.pyf`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/nleq2/nleq2_readme.txt` & `pysces-1.1.0/pysces/nleq2/nleq2_readme.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/nleq2/readme` & `pysces-1.1.0/pysces/nleq2/readme`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/nleq2/readme.txt` & `pysces-1.1.0/pysces/nleq2/readme.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/nleq2/wnorm.f` & `pysces-1.1.0/pysces/nleq2/wnorm.f`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/nleq2/zibconst.f` & `pysces-1.1.0/pysces/nleq2/zibconst.f`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/nleq2/zibmon.f` & `pysces-1.1.0/pysces/nleq2/zibmon.f`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/nleq2/zibsec.f` & `pysces-1.1.0/pysces/nleq2/zibsec.f`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/pitcon/CMakeLists.txt` & `pysces-1.1.0/pysces/pitcon/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/pitcon/dpcon61.f` & `pysces-1.1.0/pysces/pitcon/dpcon61.f`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/pitcon/dpcon61w.f` & `pysces-1.1.0/pysces/pitcon/dpcon61w.f`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/pitcon/pcon61subd.f` & `pysces-1.1.0/pysces/pitcon/pcon61subd.f`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/pitcon/pitcon.pyf` & `pysces-1.1.0/pysces/pitcon/pitcon.pyf`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/pitcon/readme.txt` & `pysces-1.1.0/pysces/pitcon/readme.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/pscmodels/Burstmodel.psc` & `pysces-1.1.0/pysces/pscmodels/Burstmodel.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/pscmodels/isola2a.psc` & `pysces-1.1.0/pysces/pscmodels/isola2a.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/pscmodels/lin5_hill.psc` & `pysces-1.1.0/pysces/pscmodels/lin5_hill.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/pscmodels/pysces_test_branch1.psc` & `pysces-1.1.0/pysces/pscmodels/pysces_test_branch1.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/pscmodels/pysces_test_moiety1.psc` & `pysces-1.1.0/pysces/pscmodels/pysces_test_moiety1.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/pscmodels/pysces_test_pitcon.psc` & `pysces-1.1.0/pysces/pscmodels/pysces_test_pitcon.psc`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/sandbox/Intersect.py` & `pysces-1.1.0/pysces/sandbox/Intersect.py`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/pysces/tests/__init__.py` & `pysces-1.1.0/pysces/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa.
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license. See LICENSE.txt that came with
```

### Comparing `pysces-1.0.3/pysces.egg-info/PKG-INFO` & `pysces-1.1.0/pysces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysces
-Version: 1.0.3
+Version: 1.1.0
 Summary: The Python Simulator for Cellular Systems - simulation and analysis tools for modelling biological systems
 Home-page: http://pysces.sourceforge.net
 Download-URL: https://pypi.org/project/pysces/#files
 Author: Brett G. Olivier and Johann M. Rohwer
 Author-email: pysces@googlegroups.com
 Maintainer: Brett G. Olivier and Johann M. Rohwer
 Maintainer-email: pysces@googlegroups.com
```

### Comparing `pysces-1.0.3/pysces.egg-info/SOURCES.txt` & `pysces-1.1.0/pysces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysces-1.0.3/setup.py` & `pysces-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 """
 PySCeS - Python Simulator for Cellular Systems (http://pysces.sourceforge.net)
 
-Copyright (C) 2004-2022 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
+Copyright (C) 2004-2023 B.G. Olivier, J.M. Rohwer, J.-H.S Hofmeyr all rights reserved,
 
 Brett G. Olivier (bgoli@users.sourceforge.net)
 Triple-J Group for Molecular Cell Physiology
 Stellenbosch University, South Africa
 
 Permission to use, modify, and distribute this software is given under the
 terms of the PySceS (BSD style) license.  See LICENSE.txt that came with
```


# Comparing `tmp/nemreader-0.8.2.tar.gz` & `tmp/nemreader-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemreader-0.8.2.tar", last modified: Tue Apr  4 20:04:43 2023, max compression
+gzip compressed data, was "nemreader-0.8.3.tar", last modified: Wed Apr 19 10:11:59 2023, max compression
```

## Comparing `nemreader-0.8.2.tar` & `nemreader-0.8.3.tar`

### file list

```diff
@@ -1,218 +1,222 @@
--rwxr-xr-x   0        0        0      135 2022-11-03 05:28:29.076363 nemreader-0.8.2/.flake8
--rwxr-xr-x   0        0        0     1220 2023-02-14 09:16:32.284457 nemreader-0.8.2/.github/workflows/pythonpackage.yml
--rw-r--r--   0        0        0     1185 2023-02-14 09:12:50.910658 nemreader-0.8.2/.gitignore
--rw-r--r--   0        0        0     1074 2022-10-22 23:26:41.875203 nemreader-0.8.2/LICENSE
--rw-r--r--   0        0        0       26 2022-10-22 23:26:41.875203 nemreader-0.8.2/MANIFEST.in
--rw-r--r--   0        0        0     1004 2023-02-14 09:16:46.737509 nemreader-0.8.2/README.md
--rw-r--r--   0        0        0   101291 2022-10-22 23:26:41.875203 nemreader-0.8.2/docs/_static/img/nmi-suffixes.jpg
--rw-r--r--   0        0        0    38420 2022-10-22 23:26:41.879203 nemreader-0.8.2/docs/_static/img/nmi-suffixes2.png
--rw-r--r--   0        0        0    10717 2022-10-22 23:26:41.879203 nemreader-0.8.2/docs/_static/img/plot_cal.png
--rw-r--r--   0        0        0    14205 2022-10-22 23:26:41.879203 nemreader-0.8.2/docs/_static/img/plot_profile.png
--rwxr-xr-x   0        0        0     5363 2022-10-22 23:37:45.243073 nemreader-0.8.2/docs/file-format.md
--rwxr-xr-x   0        0        0      664 2022-10-22 23:41:58.135351 nemreader-0.8.2/docs/gen_ref_pages.py
--rwxr-xr-x   0        0        0      469 2022-10-19 19:12:36.373067 nemreader-0.8.2/docs/index.md
--rwxr-xr-x   0        0        0      164 2022-11-03 10:18:21.085359 nemreader-0.8.2/docs/installation.md
--rwxr-xr-x   0        0        0     5141 2023-02-14 09:12:50.918658 nemreader-0.8.2/docs/quickstart.md
--rw-r--r--   0        0        0       60 2022-10-22 23:53:10.163094 nemreader-0.8.2/docs/requirements.txt
--rw-r--r--   0        0        0    29436 2023-02-14 09:12:50.918658 nemreader-0.8.2/examples/Example_NEM12_ManyNMIs.zip
--rw-r--r--   0        0        0      288 2023-04-04 20:03:11.422958 nemreader-0.8.2/examples/invalid/Example_NEM12_15min_200_30min_300.csv
--rw-r--r--   0        0        0      480 2023-04-04 20:03:11.422958 nemreader-0.8.2/examples/invalid/Example_NEM12_15min_200_30min_400.csv
--rw-r--r--   0        0        0      480 2023-04-04 20:03:11.422958 nemreader-0.8.2/examples/invalid/Example_NEM12_30min_200_15min_300.csv
--rw-r--r--   0        0        0      480 2023-04-04 20:03:11.422958 nemreader-0.8.2/examples/invalid/Example_NEM12_30min_200_15min_400.csv
--rw-r--r--   0        0        0     1147 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/invalid/Example_NEM12_incomplete_interval.csv
--rw-r--r--   0        0        0      759 2022-10-28 17:58:36.467564 nemreader-0.8.2/examples/invalid/Example_NEM12_missing_header.csv
--rw-r--r--   0        0        0     1505 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/invalid/Example_NEM12_powercor.csv
--rw-r--r--   0        0        0      316 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/invalid/Example_NEM12_powercor.csv.zip
--rw-r--r--   0        0        0     1409 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/invalid/Example_NEM12_powercor_missing_fields.csv
--rw-r--r--   0        0        0     1424 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#000000000000001#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0     2190 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#000000000000002#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1016 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#000000000000003#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      534 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#000000000000004#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      861 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#000000000000005#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      836 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#000000000000006#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      769 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#000000000000007#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      513 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#000000000000008#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1325 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#000000000000009#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      525 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#000000000000010#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1614 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#01010_05030502#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0     1272 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#02030_05030501#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0     1066 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#03050_05031001#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      702 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#05090_05031401#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      893 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#06110_05021206#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      867 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#07130_05021202#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      688 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#08150_05031502#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      650 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#10190_05031401#WBAYM#NEMMCO.zip
--rw-r--r--   0        0        0      330 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#NEM1201005Scenario1#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      432 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#NEM1202025Scenario2#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      358 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#NEM1203045Scenario3#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      355 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#NEM1205085Scenario5#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      278 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#NEM1205085bScenario5#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      346 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#NEM1206105Scenario6#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      349 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#NEM1206105bScenario7#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      497 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#NEM1208145Scenario8#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      391 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#NEM1209165Scenario9#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      331 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#NEM1210185Scenario10#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      477 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#NEM1210185Scenario10v4#GLOBALM#NEMMCO.ZIP
--rw-r--r--   0        0        0      882 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO1#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      751 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO10#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0     1101 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO1005032705#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0     1508 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO105032701#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      956 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO2#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0     1635 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO205032701#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      892 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO3#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0     1652 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO305032701#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      552 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO4#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      725 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO5#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      934 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO505033001#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      862 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO6#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      949 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO605033001#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      788 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO7#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      901 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO705033001#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      380 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO8#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      632 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO805040401#ENERGEXM#NEMMCO.zip
--rw-r--r--   0        0        0      796 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#SCENARIO9#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      759 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#Scenario01#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      761 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#Scenario01#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      361 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#Scenario04#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      364 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#Scenario04#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      332 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#Scenario05#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      336 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#Scenario05#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1368 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#Scenario06#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1371 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#Scenario06#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1315 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#Scenario07#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1320 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#Scenario07#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      583 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#Scenario08#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      586 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#Scenario08#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      384 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#Scenario09#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      387 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#Scenario09#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      705 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#Scenario10#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      700 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#Scenario10#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0     1125 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#mdffl0000000001#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      500 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#mdffl0000000004#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      490 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/NEM12#mdffl0000000008#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      320 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#S01#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      388 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#S02#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      304 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#S03#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      324 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#S04#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      280 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#S05#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      308 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#S06#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      307 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#S07#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      329 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#S08#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      351 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#S09#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      305 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#S10#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      898 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO01#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1170 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO01NEM1201003#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      951 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO02#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     2136 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO02NEM1202023#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      883 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO03#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1972 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO03NEM1203043#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      550 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO04#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      553 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO05#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1017 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO05NEM1205083#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      851 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO06#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1488 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO06NEM1206103#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      771 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO07#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1450 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO07NEM1206103#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      352 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO08#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      961 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO08NEM1208143#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      717 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO09#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      693 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO10#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0     1070 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem12/nem12#SCENARIO10NEM1210183#ELECTDSM#NEMMCO.zip
--rw-r--r--   0        0        0      287 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#000000000000011#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      291 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#000000000000012#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      290 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#000000000000013#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      294 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#000000000000014#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      366 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#000000000000015#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      343 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#000000000000016#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      299 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#000000000000017#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      400 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#000000000000018#CNRGYMDP#NEMMCO.zip
--rw-r--r--   0        0        0      280 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#SEN1311003#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      287 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#SEN1312023#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      278 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#SEN1313043#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      337 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#SEN1315083#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      345 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#SEN1316103#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      291 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#SEN1317123#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      334 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#SEN1318143#AGILITY#NEMMCO.zip
--rw-r--r--   0        0        0      276 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#Scenario11#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      280 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#Scenario11#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      283 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#Scenario11#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      290 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#Scenario12#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      293 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#Scenario12#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      295 2022-10-22 23:26:41.879203 nemreader-0.8.2/examples/nem13/NEM13#Scenario12#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      274 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario13#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      279 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario13#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      291 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario13#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      283 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario14#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      285 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario14#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      292 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario14#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      313 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario15#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      315 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario15#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      307 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario15#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      320 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario16#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      323 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario16#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      334 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario16#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      291 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario17#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      295 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario17#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      292 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario17#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      327 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario18#ETSAMDP#NEMMCO.zip
--rw-r--r--   0        0        0      330 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario18#POWERMDP#NEMMCO.zip
--rw-r--r--   0        0        0      310 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#Scenario18#UNITEDDP#NEMMCO.zip
--rw-r--r--   0        0        0      282 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#mdffl0000000013#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      285 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#mdffl000000016A#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      283 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#mdffl000000016B#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      285 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#mdffl000000016C#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      288 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#mdffl000000018E#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      287 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/NEM13#mdffl000000018S#ACTEWM#NEMMCO.zip
--rw-r--r--   0        0        0      295 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/nem13#11#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      427 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/nem13#12#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      276 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/nem13#13#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      282 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/nem13#14#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      308 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/nem13#15#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      309 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/nem13#16#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      285 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/nem13#17#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      427 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/nem13#18#INTEGM#NEMMCO.zip
--rw-r--r--   0        0        0      284 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/nem13#SCENARIO11#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      292 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/nem13#SCENARIO12#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      280 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/nem13#SCENARIO13#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      284 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/nem13#SCENARIO14#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      315 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/nem13#SCENARIO15#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      340 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/nem13#SCENARIO16#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      294 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/nem13#SCENARIO17#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      308 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/nem13/nem13#SCENARIO18#TCAUSTM#NEMMCO.zip
--rw-r--r--   0        0        0      791 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/unzipped/Example_NEM12_actual_interval.csv
--rw-r--r--   0        0        0     1373 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/unzipped/Example_NEM12_different_interval_length.csv
--rw-r--r--   0        0        0     4497 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/unzipped/Example_NEM12_multiple_meters.csv
--rw-r--r--   0        0        0      521 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/unzipped/Example_NEM12_multiple_quality.csv
--rw-r--r--   0        0        0      337 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/unzipped/Example_NEM12_no_scheduled_read.csv
--rw-r--r--   0        0        0      887 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/unzipped/Example_NEM12_substituted_interval.csv
--rw-r--r--   0        0        0      791 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/unzipped/Example_NEM12_upper_case_units.csv
--rw-r--r--   0        0        0      185 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/unzipped/Example_NEM13_consumption_data.csv
--rw-r--r--   0        0        0      345 2022-10-22 23:26:41.883204 nemreader-0.8.2/examples/unzipped/Example_NEM13_forward_estimate.csv
--rwxr-xr-x   0        0        0      594 2022-10-22 23:45:00.094390 nemreader-0.8.2/mkdocs.yml
--rw-r--r--   0        0        0      710 2022-10-28 17:58:36.467564 nemreader-0.8.2/nemreader/__init__.py
--rw-r--r--   0        0        0       28 2022-10-22 23:26:41.883204 nemreader-0.8.2/nemreader/__main__.py
--rw-r--r--   0        0        0     3482 2022-12-29 05:11:02.878653 nemreader-0.8.2/nemreader/cli.py
--rw-r--r--   0        0        0     3510 2023-02-14 09:12:50.914658 nemreader-0.8.2/nemreader/nem_objects.py
--rw-r--r--   0        0        0    21272 2023-04-04 20:03:11.422958 nemreader-0.8.2/nemreader/nem_reader.py
--rw-r--r--   0        0        0     8672 2022-12-30 02:48:01.983692 nemreader-0.8.2/nemreader/outputs.py
--rw-r--r--   0        0        0        0 2022-10-22 23:26:41.883204 nemreader-0.8.2/nemreader/py.typed
--rw-r--r--   0        0        0     5596 2022-12-29 05:11:02.878653 nemreader-0.8.2/nemreader/split_days.py
--rw-r--r--   0        0        0       22 2023-04-04 20:03:40.030570 nemreader-0.8.2/nemreader/version.py
--rwxr-xr-x   0        0        0     1368 2023-02-14 09:12:50.914658 nemreader-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     1956 2023-02-14 09:12:50.914658 nemreader-0.8.2/requirements.txt
--rw-r--r--   0        0        0        0 2022-10-22 23:26:41.883204 nemreader-0.8.2/tests/__init__.py
--rw-r--r--   0        0        0     1157 2022-10-25 19:12:53.653131 nemreader-0.8.2/tests/test_actual_interval.py
--rw-r--r--   0        0        0      924 2022-10-25 19:12:58.373208 nemreader-0.8.2/tests/test_cli.py
--rw-r--r--   0        0        0      471 2023-02-14 09:12:50.918658 nemreader-0.8.2/tests/test_consumption_data.py
--rw-r--r--   0        0        0      816 2023-02-14 09:12:50.918658 nemreader-0.8.2/tests/test_day_split.py
--rw-r--r--   0        0        0     2059 2023-01-26 21:27:00.374407 nemreader-0.8.2/tests/test_file_outputs.py
--rw-r--r--   0        0        0      359 2022-10-28 17:58:36.471564 nemreader-0.8.2/tests/test_header_datestamp.py
--rw-r--r--   0        0        0     1746 2022-10-25 19:12:58.409208 nemreader-0.8.2/tests/test_incomplete_files.py
--rw-r--r--   0        0        0      904 2023-04-04 20:03:11.422958 nemreader-0.8.2/tests/test_invalid_interval_mixing.py
--rw-r--r--   0        0        0      284 2022-11-30 03:41:57.431559 nemreader-0.8.2/tests/test_legacy.py
--rw-r--r--   0        0        0      252 2023-02-14 09:12:50.918658 nemreader-0.8.2/tests/test_many_nmis.py
--rw-r--r--   0        0        0     1034 2022-10-25 19:12:58.393208 nemreader-0.8.2/tests/test_multiple_quality.py
--rw-r--r--   0        0        0     1488 2022-10-25 19:10:30.098582 nemreader-0.8.2/tests/test_open_examples.py
--rw-r--r--   0        0        0      268 2022-10-25 19:10:50.070968 nemreader-0.8.2/tests/test_optional_columns.py
--rw-r--r--   0        0        0     1309 2022-12-30 02:47:14.370981 nemreader-0.8.2/tests/test_unit_capitalisation.py
--rw-r--r--   0        0        0     2158 1970-01-01 00:00:00.000000 nemreader-0.8.2/PKG-INFO
+-rwxr-xr-x   0        0        0      135 2022-11-03 05:28:29.076363 nemreader-0.8.3/.flake8
+-rwxr-xr-x   0        0        0     1220 2023-02-14 09:16:32.284457 nemreader-0.8.3/.github/workflows/pythonpackage.yml
+-rw-r--r--   0        0        0     1185 2023-02-14 09:12:50.910658 nemreader-0.8.3/.gitignore
+-rw-r--r--   0        0        0     1074 2022-10-22 23:26:41.875203 nemreader-0.8.3/LICENSE
+-rw-r--r--   0        0        0       26 2022-10-22 23:26:41.875203 nemreader-0.8.3/MANIFEST.in
+-rw-r--r--   0        0        0     1004 2023-02-14 09:16:46.737509 nemreader-0.8.3/README.md
+-rw-r--r--   0        0        0   101291 2022-10-22 23:26:41.875203 nemreader-0.8.3/docs/_static/img/nmi-suffixes.jpg
+-rw-r--r--   0        0        0    38420 2022-10-22 23:26:41.879203 nemreader-0.8.3/docs/_static/img/nmi-suffixes2.png
+-rw-r--r--   0        0        0    10717 2022-10-22 23:26:41.879203 nemreader-0.8.3/docs/_static/img/plot_cal.png
+-rw-r--r--   0        0        0    14205 2022-10-22 23:26:41.879203 nemreader-0.8.3/docs/_static/img/plot_profile.png
+-rwxr-xr-x   0        0        0     5363 2022-10-22 23:37:45.243073 nemreader-0.8.3/docs/file-format.md
+-rwxr-xr-x   0        0        0      658 2023-04-18 15:51:04.038645 nemreader-0.8.3/docs/gen_ref_pages.py
+-rwxr-xr-x   0        0        0      469 2022-10-19 19:12:36.373067 nemreader-0.8.3/docs/index.md
+-rwxr-xr-x   0        0        0      164 2022-11-03 10:18:21.085359 nemreader-0.8.3/docs/installation.md
+-rwxr-xr-x   0        0        0     5141 2023-02-14 09:12:50.918658 nemreader-0.8.3/docs/quickstart.md
+-rw-r--r--   0        0        0       60 2022-10-22 23:53:10.163094 nemreader-0.8.3/docs/requirements.txt
+-rw-r--r--   0        0        0    29436 2023-02-14 09:12:50.918658 nemreader-0.8.3/examples/Example_NEM12_ManyNMIs.zip
+-rw-r--r--   0        0        0      708 2023-04-19 04:17:11.605921 nemreader-0.8.3/examples/Example_different_intervals.zip
+-rw-r--r--   0        0        0      288 2023-04-04 20:03:11.422958 nemreader-0.8.3/examples/invalid/Example_NEM12_15min_200_30min_300.csv
+-rw-r--r--   0        0        0      480 2023-04-04 20:03:11.422958 nemreader-0.8.3/examples/invalid/Example_NEM12_15min_200_30min_400.csv
+-rw-r--r--   0        0        0      480 2023-04-04 20:03:11.422958 nemreader-0.8.3/examples/invalid/Example_NEM12_30min_200_15min_300.csv
+-rw-r--r--   0        0        0      480 2023-04-04 20:03:11.422958 nemreader-0.8.3/examples/invalid/Example_NEM12_30min_200_15min_400.csv
+-rw-r--r--   0        0        0     1147 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/invalid/Example_NEM12_incomplete_interval.csv
+-rw-r--r--   0        0        0      759 2022-10-28 17:58:36.467564 nemreader-0.8.3/examples/invalid/Example_NEM12_missing_header.csv
+-rw-r--r--   0        0        0     1505 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/invalid/Example_NEM12_powercor.csv
+-rw-r--r--   0        0        0      316 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/invalid/Example_NEM12_powercor.csv.zip
+-rw-r--r--   0        0        0     1409 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/invalid/Example_NEM12_powercor_missing_fields.csv
+-rw-r--r--   0        0        0     1424 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#000000000000001#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     2190 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#000000000000002#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1016 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#000000000000003#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      534 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#000000000000004#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      861 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#000000000000005#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      836 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#000000000000006#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      769 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#000000000000007#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      513 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#000000000000008#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1325 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#000000000000009#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      525 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#000000000000010#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1614 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#01010_05030502#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0     1272 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#02030_05030501#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0     1066 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#03050_05031001#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      702 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#05090_05031401#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      893 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#06110_05021206#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      867 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#07130_05021202#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      688 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#08150_05031502#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      650 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#10190_05031401#WBAYM#NEMMCO.zip
+-rw-r--r--   0        0        0      330 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#NEM1201005Scenario1#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      432 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#NEM1202025Scenario2#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      358 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#NEM1203045Scenario3#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      355 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#NEM1205085Scenario5#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      278 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#NEM1205085bScenario5#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      346 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#NEM1206105Scenario6#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      349 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#NEM1206105bScenario7#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      497 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#NEM1208145Scenario8#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      391 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#NEM1209165Scenario9#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      331 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#NEM1210185Scenario10#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      477 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#NEM1210185Scenario10v4#GLOBALM#NEMMCO.ZIP
+-rw-r--r--   0        0        0      882 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO1#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      751 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO10#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1101 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO1005032705#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0     1508 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO105032701#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      956 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO2#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1635 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO205032701#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      892 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO3#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1652 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO305032701#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      552 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO4#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      725 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO5#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      934 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO505033001#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      862 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO6#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      949 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO605033001#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      788 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO7#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      901 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO705033001#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      380 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO8#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      632 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO805040401#ENERGEXM#NEMMCO.zip
+-rw-r--r--   0        0        0      796 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#SCENARIO9#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      759 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#Scenario01#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      761 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#Scenario01#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      361 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#Scenario04#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      364 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#Scenario04#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      332 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#Scenario05#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      336 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#Scenario05#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1368 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#Scenario06#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1371 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#Scenario06#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1315 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#Scenario07#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1320 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#Scenario07#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      583 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#Scenario08#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      586 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#Scenario08#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      384 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#Scenario09#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      387 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#Scenario09#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      705 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#Scenario10#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      700 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#Scenario10#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0     1125 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#mdffl0000000001#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      500 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#mdffl0000000004#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      490 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/NEM12#mdffl0000000008#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      320 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#S01#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      388 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#S02#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      304 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#S03#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      324 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#S04#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      280 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#S05#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      308 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#S06#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      307 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#S07#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      329 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#S08#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      351 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#S09#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      305 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#S10#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      898 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO01#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1170 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO01NEM1201003#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      951 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO02#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     2136 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO02NEM1202023#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      883 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO03#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1972 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO03NEM1203043#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      550 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO04#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      553 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO05#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1017 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO05NEM1205083#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      851 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO06#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1488 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO06NEM1206103#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      771 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO07#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1450 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO07NEM1206103#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      352 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO08#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      961 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO08NEM1208143#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      717 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO09#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      693 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO10#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0     1070 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem12/nem12#SCENARIO10NEM1210183#ELECTDSM#NEMMCO.zip
+-rw-r--r--   0        0        0      287 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#000000000000011#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      291 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#000000000000012#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      290 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#000000000000013#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      294 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#000000000000014#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      366 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#000000000000015#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      343 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#000000000000016#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      299 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#000000000000017#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      400 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#000000000000018#CNRGYMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      280 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#SEN1311003#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      287 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#SEN1312023#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      278 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#SEN1313043#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      337 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#SEN1315083#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      345 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#SEN1316103#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      291 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#SEN1317123#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      334 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#SEN1318143#AGILITY#NEMMCO.zip
+-rw-r--r--   0        0        0      276 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#Scenario11#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      280 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#Scenario11#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      283 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#Scenario11#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      290 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#Scenario12#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      293 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#Scenario12#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      295 2022-10-22 23:26:41.879203 nemreader-0.8.3/examples/nem13/NEM13#Scenario12#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      274 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario13#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      279 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario13#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      291 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario13#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      283 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario14#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      285 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario14#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      292 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario14#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      313 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario15#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      315 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario15#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      307 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario15#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      320 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario16#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      323 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario16#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      334 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario16#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      291 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario17#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      295 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario17#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      292 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario17#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      327 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario18#ETSAMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      330 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario18#POWERMDP#NEMMCO.zip
+-rw-r--r--   0        0        0      310 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#Scenario18#UNITEDDP#NEMMCO.zip
+-rw-r--r--   0        0        0      282 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#mdffl0000000013#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      285 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#mdffl000000016A#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      283 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#mdffl000000016B#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      285 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#mdffl000000016C#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      288 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#mdffl000000018E#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      287 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/NEM13#mdffl000000018S#ACTEWM#NEMMCO.zip
+-rw-r--r--   0        0        0      295 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/nem13#11#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      427 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/nem13#12#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      276 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/nem13#13#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      282 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/nem13#14#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      308 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/nem13#15#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      309 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/nem13#16#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      285 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/nem13#17#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      427 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/nem13#18#INTEGM#NEMMCO.zip
+-rw-r--r--   0        0        0      284 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/nem13#SCENARIO11#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      292 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/nem13#SCENARIO12#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      280 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/nem13#SCENARIO13#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      284 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/nem13#SCENARIO14#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      315 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/nem13#SCENARIO15#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      340 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/nem13#SCENARIO16#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      294 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/nem13#SCENARIO17#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      308 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/nem13/nem13#SCENARIO18#TCAUSTM#NEMMCO.zip
+-rw-r--r--   0        0        0      791 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/unzipped/Example_NEM12_actual_interval.csv
+-rw-r--r--   0        0        0     1373 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/unzipped/Example_NEM12_different_interval_length.csv
+-rw-r--r--   0        0        0     4497 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/unzipped/Example_NEM12_multiple_meters.csv
+-rw-r--r--   0        0        0      521 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/unzipped/Example_NEM12_multiple_quality.csv
+-rw-r--r--   0        0        0      337 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/unzipped/Example_NEM12_no_scheduled_read.csv
+-rw-r--r--   0        0        0      887 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/unzipped/Example_NEM12_substituted_interval.csv
+-rw-r--r--   0        0        0      791 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/unzipped/Example_NEM12_upper_case_units.csv
+-rw-r--r--   0        0        0      185 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/unzipped/Example_NEM13_consumption_data.csv
+-rw-r--r--   0        0        0      345 2022-10-22 23:26:41.883204 nemreader-0.8.3/examples/unzipped/Example_NEM13_forward_estimate.csv
+-rwxr-xr-x   0        0        0      594 2022-10-22 23:45:00.094390 nemreader-0.8.3/mkdocs.yml
+-rw-r--r--   0        0        0      764 2023-04-18 16:37:46.193786 nemreader-0.8.3/nemreader/__init__.py
+-rw-r--r--   0        0        0       28 2022-10-22 23:26:41.883204 nemreader-0.8.3/nemreader/__main__.py
+-rw-r--r--   0        0        0     3754 2023-04-18 16:29:44.284846 nemreader-0.8.3/nemreader/cli.py
+-rw-r--r--   0        0        0     3515 2023-04-18 15:51:04.094646 nemreader-0.8.3/nemreader/nem_objects.py
+-rw-r--r--   0        0        0    22549 2023-04-19 04:22:30.571119 nemreader-0.8.3/nemreader/nem_reader.py
+-rw-r--r--   0        0        0     5604 2023-04-18 16:41:06.005639 nemreader-0.8.3/nemreader/output_db.py
+-rw-r--r--   0        0        0     5139 2023-04-18 16:01:53.042738 nemreader-0.8.3/nemreader/outputs.py
+-rw-r--r--   0        0        0        0 2022-10-22 23:26:41.883204 nemreader-0.8.3/nemreader/py.typed
+-rw-r--r--   0        0        0     5595 2023-04-18 15:51:04.154647 nemreader-0.8.3/nemreader/split_days.py
+-rw-r--r--   0        0        0       22 2023-04-19 04:41:05.966390 nemreader-0.8.3/nemreader/version.py
+-rwxr-xr-x   0        0        0     1381 2023-04-18 16:02:12.775158 nemreader-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     1956 2023-02-14 09:12:50.914658 nemreader-0.8.3/requirements.txt
+-rw-r--r--   0        0        0        0 2022-10-22 23:26:41.883204 nemreader-0.8.3/tests/__init__.py
+-rw-r--r--   0        0        0     1157 2022-10-25 19:12:53.653131 nemreader-0.8.3/tests/test_actual_interval.py
+-rw-r--r--   0        0        0     1572 2023-04-18 16:14:25.860240 nemreader-0.8.3/tests/test_cli.py
+-rw-r--r--   0        0        0      469 2023-04-18 15:51:04.058645 nemreader-0.8.3/tests/test_consumption_data.py
+-rw-r--r--   0        0        0      850 2023-04-19 04:30:06.541878 nemreader-0.8.3/tests/test_dataframe_pivot.py
+-rw-r--r--   0        0        0      814 2023-04-18 15:51:04.062646 nemreader-0.8.3/tests/test_day_split.py
+-rw-r--r--   0        0        0     2099 2023-04-19 04:41:11.878462 nemreader-0.8.3/tests/test_file_outputs.py
+-rw-r--r--   0        0        0      359 2022-10-28 17:58:36.471564 nemreader-0.8.3/tests/test_header_datestamp.py
+-rw-r--r--   0        0        0     1745 2023-04-18 15:51:04.094646 nemreader-0.8.3/tests/test_incomplete_files.py
+-rw-r--r--   0        0        0      995 2023-04-18 15:51:04.086646 nemreader-0.8.3/tests/test_invalid_interval_mixing.py
+-rw-r--r--   0        0        0      284 2022-11-30 03:41:57.431559 nemreader-0.8.3/tests/test_legacy.py
+-rw-r--r--   0        0        0      252 2023-02-14 09:12:50.918658 nemreader-0.8.3/tests/test_many_nmis.py
+-rw-r--r--   0        0        0     1034 2022-10-25 19:12:58.393208 nemreader-0.8.3/tests/test_multiple_quality.py
+-rw-r--r--   0        0        0     1488 2022-10-25 19:10:30.098582 nemreader-0.8.3/tests/test_open_examples.py
+-rw-r--r--   0        0        0      268 2022-10-25 19:10:50.070968 nemreader-0.8.3/tests/test_optional_columns.py
+-rw-r--r--   0        0        0      589 2023-04-18 16:57:08.719527 nemreader-0.8.3/tests/test_output_db.py
+-rw-r--r--   0        0        0     1307 2023-04-18 15:51:04.102646 nemreader-0.8.3/tests/test_unit_capitalisation.py
+-rw-r--r--   0        0        0     2158 1970-01-01 00:00:00.000000 nemreader-0.8.3/PKG-INFO
```

### Comparing `nemreader-0.8.2/.github/workflows/pythonpackage.yml` & `nemreader-0.8.3/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/.gitignore` & `nemreader-0.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/LICENSE` & `nemreader-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/README.md` & `nemreader-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/docs/_static/img/nmi-suffixes.jpg` & `nemreader-0.8.3/docs/_static/img/nmi-suffixes.jpg`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/docs/_static/img/nmi-suffixes2.png` & `nemreader-0.8.3/docs/_static/img/nmi-suffixes2.png`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/docs/_static/img/plot_cal.png` & `nemreader-0.8.3/docs/_static/img/plot_cal.png`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/docs/_static/img/plot_profile.png` & `nemreader-0.8.3/docs/_static/img/plot_profile.png`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/docs/file-format.md` & `nemreader-0.8.3/docs/file-format.md`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/docs/gen_ref_pages.py` & `nemreader-0.8.3/docs/gen_ref_pages.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Generate the code reference pages."""
 
 from pathlib import Path
 
 import mkdocs_gen_files
 
-
 for path in sorted(Path("nemreader").rglob("*.py")):  #
     module_path = path.relative_to("").with_suffix("")  #
     doc_path = path.relative_to("").with_suffix(".md")  #
     full_doc_path = Path("reference", doc_path)  #
 
     parts = list(module_path.parts)
 
-    if parts[-1] in ("__init__", "__main__", 'version'):
+    if parts[-1] in ("__init__", "__main__", "version"):
         continue
-    
+
     with mkdocs_gen_files.open(full_doc_path, "w") as fd:  #
         identifier = ".".join(parts)  #
         print("::: " + identifier, file=fd)  #
 
     mkdocs_gen_files.set_edit_path(full_doc_path, path)  #
```

### Comparing `nemreader-0.8.2/docs/quickstart.md` & `nemreader-0.8.3/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/Example_NEM12_ManyNMIs.zip` & `nemreader-0.8.3/examples/Example_NEM12_ManyNMIs.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/invalid/Example_NEM12_incomplete_interval.csv` & `nemreader-0.8.3/examples/invalid/Example_NEM12_incomplete_interval.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/invalid/Example_NEM12_missing_header.csv` & `nemreader-0.8.3/examples/invalid/Example_NEM12_missing_header.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/invalid/Example_NEM12_powercor.csv` & `nemreader-0.8.3/examples/invalid/Example_NEM12_powercor.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/invalid/Example_NEM12_powercor_missing_fields.csv` & `nemreader-0.8.3/examples/invalid/Example_NEM12_powercor_missing_fields.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#000000000000001#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#000000000000001#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#000000000000002#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#000000000000002#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#000000000000003#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#000000000000003#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#000000000000004#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#000000000000004#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#000000000000005#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#000000000000005#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#000000000000006#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#000000000000006#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#000000000000007#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#000000000000007#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#000000000000008#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#000000000000008#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#000000000000009#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#000000000000009#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#000000000000010#CNRGYMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#000000000000010#CNRGYMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#01010_05030502#WBAYM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#01010_05030502#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#02030_05030501#WBAYM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#02030_05030501#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#03050_05031001#WBAYM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#03050_05031001#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#05090_05031401#WBAYM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#05090_05031401#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#06110_05021206#WBAYM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#06110_05021206#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#07130_05021202#WBAYM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#07130_05021202#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#08150_05031502#WBAYM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#08150_05031502#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#10190_05031401#WBAYM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#10190_05031401#WBAYM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO1#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO1#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO10#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO10#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO1005032705#ENERGEXM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO1005032705#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO105032701#ENERGEXM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO105032701#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO2#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO2#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO205032701#ENERGEXM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO205032701#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO3#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO3#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO305032701#ENERGEXM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO305032701#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO4#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO4#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO5#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO5#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO505033001#ENERGEXM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO505033001#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO6#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO6#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO605033001#ENERGEXM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO605033001#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO7#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO7#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO705033001#ENERGEXM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO705033001#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO805040401#ENERGEXM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO805040401#ENERGEXM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#SCENARIO9#UNITEDDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#SCENARIO9#UNITEDDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#Scenario01#ETSAMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#Scenario01#ETSAMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#Scenario01#POWERMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#Scenario01#POWERMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#Scenario06#ETSAMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#Scenario06#ETSAMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#Scenario06#POWERMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#Scenario06#POWERMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#Scenario07#ETSAMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#Scenario07#ETSAMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#Scenario07#POWERMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#Scenario07#POWERMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#Scenario08#ETSAMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#Scenario08#ETSAMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#Scenario08#POWERMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#Scenario08#POWERMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#Scenario10#ETSAMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#Scenario10#ETSAMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#Scenario10#POWERMDP#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#Scenario10#POWERMDP#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/NEM12#mdffl0000000001#ACTEWM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/NEM12#mdffl0000000001#ACTEWM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO01#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO01#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO01NEM1201003#ELECTDSM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO01NEM1201003#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO02#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO02#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO02NEM1202023#ELECTDSM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO02NEM1202023#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO03#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO03#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO03NEM1203043#ELECTDSM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO03NEM1203043#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO04#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO04#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO05#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO05#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO05NEM1205083#ELECTDSM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO05NEM1205083#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO06#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO06#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO06NEM1206103#ELECTDSM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO06NEM1206103#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO07#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO07#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO07NEM1206103#ELECTDSM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO07NEM1206103#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO08NEM1208143#ELECTDSM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO08NEM1208143#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO09#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO09#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO10#TCAUSTM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO10#TCAUSTM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/nem12/nem12#SCENARIO10NEM1210183#ELECTDSM#NEMMCO.zip` & `nemreader-0.8.3/examples/nem12/nem12#SCENARIO10NEM1210183#ELECTDSM#NEMMCO.zip`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/unzipped/Example_NEM12_actual_interval.csv` & `nemreader-0.8.3/examples/unzipped/Example_NEM12_actual_interval.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/unzipped/Example_NEM12_different_interval_length.csv` & `nemreader-0.8.3/examples/unzipped/Example_NEM12_different_interval_length.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/unzipped/Example_NEM12_multiple_meters.csv` & `nemreader-0.8.3/examples/unzipped/Example_NEM12_multiple_meters.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/unzipped/Example_NEM12_multiple_quality.csv` & `nemreader-0.8.3/examples/unzipped/Example_NEM12_multiple_quality.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/unzipped/Example_NEM12_substituted_interval.csv` & `nemreader-0.8.3/examples/unzipped/Example_NEM12_substituted_interval.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/examples/unzipped/Example_NEM12_upper_case_units.csv` & `nemreader-0.8.3/examples/unzipped/Example_NEM12_upper_case_units.csv`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/mkdocs.yml` & `nemreader-0.8.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/nemreader/__init__.py` & `nemreader-0.8.3/nemreader/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,30 @@
     NEM13 (accumulated metering data) data files
 """
 
 import logging
 from logging import NullHandler
 
 from .nem_reader import NEMFile, read_nem_file
+from .output_db import extend_sqlite, output_as_sqlite
 from .outputs import (
     nmis_in_file,
     output_as_csv,
     output_as_daily_csv,
     output_as_data_frames,
-    output_as_sqlite,
 )
 from .version import __version__
 
 __all__ = [
     "__version__",
     "NEMFile",
     "read_nem_file",
     "nmis_in_file",
     "output_as_csv",
     "output_as_daily_csv",
     "output_as_data_frames",
     "output_as_sqlite",
+    "extend_sqlite",
 ]
 
 # Set default logging handler to avoid "No handler found" warnings.
 logging.getLogger(__name__).addHandler(NullHandler())
```

### Comparing `nemreader-0.8.2/nemreader/cli.py` & `nemreader-0.8.3/nemreader/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 import os
 from pathlib import Path
 from typing import Optional
 
 import typer
 
-from .outputs import nmis_in_file, output_as_csv, output_as_daily_csv, output_as_sqlite
+from .output_db import extend_sqlite, output_as_sqlite
+from .outputs import nmis_in_file, output_as_csv, output_as_daily_csv
 from .version import __version__
 
 LOG_FORMAT = "%(asctime)s %(levelname)-8s %(message)s"
 app = typer.Typer()
 DEFAULT_DIR = Path(".")
 
 
@@ -20,24 +21,26 @@
 
 
 @app.callback()
 def callback(
     version: Optional[bool] = typer.Option(
         None, "--version", callback=version_callback
     ),
-):
+) -> None:
     """nemreader
 
     Parse AEMO NEM12 and NEM13 meter data files
     """
     pass
 
 
 @app.command()
-def list_nmis(nemfile: Path, verbose: bool = typer.Option(False, "--verbose", "-v")):
+def list_nmis(
+    nemfile: Path, verbose: bool = typer.Option(False, "--verbose", "-v")
+) -> None:
     if verbose:
         log_level = "DEBUG"
     else:
         log_level = "WARNING"
     logging.basicConfig(level=log_level, format=LOG_FORMAT)
 
     nmis = list(nmis_in_file(nemfile))
@@ -55,15 +58,15 @@
     outdir: Path = typer.Option(
         DEFAULT_DIR,
         exists=True,
         file_okay=False,
         dir_okay=True,
         writable=True,
     ),
-):
+) -> None:
     """Output NEM file to transposed CSV.
 
     nemfile is the name of the file to parse.
     """
     if verbose:
         log_level = "DEBUG"
     else:
@@ -80,15 +83,15 @@
     outdir: Path = typer.Option(
         DEFAULT_DIR,
         exists=True,
         file_okay=False,
         dir_okay=True,
         writable=True,
     ),
-):
+) -> None:
     """Output NEM file to transposed CSV.
 
     nemfile is the name of the file to parse.
     """
     if verbose:
         log_level = "DEBUG"
     else:
@@ -104,20 +107,21 @@
     outdir: Path = typer.Option(
         DEFAULT_DIR,
         exists=True,
         file_okay=True,
         dir_okay=True,
         writable=True,
     ),
+    output_file: str = "nemdata.db",
+    set_interval: Optional[int] = None,
     verbose: bool = typer.Option(False, "--verbose", "-v"),
-    five_min: bool = typer.Option(False, "--five-min", "-5"),
-):
-    """Output NEM file to transposed CSV.
+) -> None:
+    """Output NEM file to SQLite DB.
 
-    nemfile is the name of the file to parse.
+    nemfile is the name of the file or folder to parse.
     """
     if verbose:
         log_level = "DEBUG"
     else:
         log_level = "WARNING"
     logging.basicConfig(level=log_level, format=LOG_FORMAT)
     if os.path.isdir(nemfile):
@@ -125,11 +129,18 @@
         files = list(nemfile.glob("*.csv"))
         files += list(nemfile.glob("*.zip"))
     else:
         files = [nemfile]
     for fp in files:
         typer.echo(f"Processing {fp}")
         try:
-            output_as_sqlite(fp, output_dir=outdir, make_fivemins=five_min)
+            output_as_sqlite(
+                fp,
+                output_dir=outdir,
+                output_file=output_file,
+                set_interval=set_interval,
+            )
         except Exception:
             typer.echo(f"Not a valid nem file: {fp}")
+    db_path = outdir / output_file
+    extend_sqlite(db_path)
     typer.echo("Finished exporting to DB.")
```

### Comparing `nemreader-0.8.2/nemreader/nem_objects.py` & `nemreader-0.8.3/nemreader/nem_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime
 from typing import Dict, List, NamedTuple, Optional
 
+
 class HeaderRecord(NamedTuple):
     """Header record (100)"""
 
     version_header: str
     creation_date: Optional[datetime]
     from_participant: str
     to_participant: str
@@ -105,26 +106,28 @@
     """B2B details record (550)"""
 
     previous_trans_code: str
     previous_ret_service_order: str
     current_trans_code: str
     current_ret_service_order: str
 
+
 class NEMReadings:
     """Represents a meter reading"""
 
     readings: Dict[str, Dict[str, List[Reading]]]
     transactions: Dict[str, Dict[str, list]]
 
     def __init__(self, readings, transactions):
         self.readings = readings
         self.transactions = transactions
 
     class Config:
-        copy_on_model_validation = 'shallow' # faster
+        copy_on_model_validation = "shallow"  # faster
+
 
 class NEMData:
     """Represents a meter reading"""
 
     header: HeaderRecord
     readings: Dict[str, Dict[str, List[Reading]]]
     transactions: Dict[str, Dict[str, list]]
@@ -135,8 +138,8 @@
         self.transactions = transactions
 
     @property
     def nmis(self) -> List[str]:
         return list(self.transactions.keys())
 
     class Config:
-        copy_on_model_validation = 'shallow' # faster
+        copy_on_model_validation = "shallow"  # faster
```

### Comparing `nemreader-0.8.2/nemreader/nem_reader.py` & `nemreader-0.8.3/nemreader/nem_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 )
 from .split_days import make_set_interval, split_multiday_reads
 
 log = logging.getLogger(__name__)
 
 minutes_per_day = 24 * 60
 
+
 class NEMFile:
     """An NEM file object"""
 
     def __init__(self, file_path: str, strict: bool = False) -> None:
-
         self.file_path = file_path
         self.strict = strict
         self.nmis: set = set()
         self.nmi_channels: dict = {}
 
     def __repr__(self):
         return f"<NEMFile {self.file_path}>"
@@ -152,23 +152,56 @@
         self,
         split_days: bool = False,
         set_interval: Optional[int] = None,
         include_serno: bool = False,
     ) -> pd.DataFrame:
         """Return NEMData as a DataFrame with suffix columns"""
         df = self.get_data_frame(split_days, set_interval)
-        pivot_index = ["nmi", "t_start", "t_end", "quality", "evt_code", "evt_desc"]
+        index_cols = [
+            "nmi",
+            "suffix",
+            "t_start",
+            "t_end",
+        ]
         if include_serno:
-            pivot_index.append("serno")
-        df_pivoted = df.pivot(
-            index=pivot_index,
-            columns="suffix",
-            values="value",
-        ).reset_index()
-        return df_pivoted
+            index_cols.append("serno")
+        else:
+            del df["serno"]
+
+        df.set_index(index_cols, inplace=True)
+        df = df.unstack("suffix")
+        df = df.reset_index()
+        df.columns = df.columns.map("_".join).str.strip("_")
+        quality = 0
+        evt_code = 0
+        evt_desc = 0
+        new_names = {}
+        for col in df.columns:
+            if "value_" in col:
+                new_names[col] = col[6:]
+            if "quality" in col:
+                if not quality:
+                    new_names[col] = "quality"
+                else:
+                    del df[col]
+                quality += 1
+            if "evt_code" in col:
+                if not evt_code:
+                    new_names[col] = "evt_code"
+                else:
+                    del df[col]
+                evt_code += 1
+            if "evt_desc" in col:
+                if not evt_desc:
+                    new_names[col] = "evt_desc"
+                else:
+                    del df[col]
+                evt_desc += 1
+        df.rename(columns=new_names, inplace=True)
+        return df
 
     def get_per_nmi_dfs(
         self,
         split_days: bool = False,
         set_interval: Optional[int] = None,
         include_serno: bool = False,
     ) -> Generator[Tuple[str, pd.DataFrame], None, None]:
@@ -196,15 +229,15 @@
 
     nf = NEMFile(file_path, strict=ignore_missing_header)
     return nf.nem_data()
 
 
 def parse_100_row(row: List[Any], file_name: str) -> HeaderRecord:
     """Parse header record (100)
-    
+
     RecordIndicator,VersionHeader,DateTime,FromParticipant,ToParticipant
     Example: 100,NEM12,200301011534,MDP1,Retailer1
     """
     return HeaderRecord(
         row[1], parse_datetime(row[2]), row[3], row[4], file_name, False
     )
 
@@ -215,27 +248,29 @@
     readings: Dict[str, Dict[str, List[Reading]]] = {}
     # transactions nested by NMI then channel
     trans: Dict[str, Dict[str, list]] = {}
     nmi_d = None  # current NMI details block that readings apply to
 
     observed_900_records = []
 
-    for (row_num, row) in enumerate(nem_list, start=1):
+    for row_num, row in enumerate(nem_list, start=1):
         try:
             if not row:
                 log.debug(f"Skipping empty row at line {row_num}.")
                 continue
 
             record_indicator = int(row[0])
 
             if record_indicator == 900:
                 # Powercor NEM12 files can concatenate multiple files together
                 # try to keep parsing anyway.
                 if observed_900_records:
-                    log.warning(f"Found multiple end of data (900) rows on lines {observed_900_records}")
+                    log.warning(
+                        f"Found multiple end of data (900) rows on lines {observed_900_records}"
+                    )
 
                 observed_900_records.append(row_num)
                 pass
 
             elif record_indicator == 200:
                 try:
                     nmi_details = parse_200_row(row)
@@ -257,15 +292,22 @@
             elif record_indicator == 300:
                 num_intervals = int(minutes_per_day / nmi_d.interval_length)
                 assert len(row) > 1, f"Invalid 300 Row in {file_name} on line {row_num}"
                 if len(row) < num_intervals + 2:
                     record_date = row[1]
                     msg = "Skipping 300 record for %s %s %s on row %d. "
                     msg += "It does not have the expected %s intervals"
-                    log.error(msg, nmi_d.nmi, nmi_d.nmi_suffix, record_date, row_num, num_intervals)
+                    log.error(
+                        msg,
+                        nmi_d.nmi,
+                        nmi_d.nmi_suffix,
+                        record_date,
+                        row_num,
+                        num_intervals,
+                    )
                     continue
                 interval_record = parse_300_row(
                     row, nmi_d.interval_length, nmi_d.uom, nmi_d.meter_serial_number
                 )
                 # don't flatten the list of interval readings at this stage,
                 # as they may need to be adjusted by a 400 row
                 readings[nmi_d.nmi][nmi_d.nmi_suffix].append(
@@ -280,15 +322,17 @@
 
             elif record_indicator == 500:
                 b2b_details = parse_500_row(row)
                 trans[nmi_d.nmi][nmi_d.nmi_suffix].append(b2b_details)
 
             else:
                 log.warning(
-                    "Record indicator %s on line %d not supported and was skipped", record_indicator, row_num
+                    "Record indicator %s on line %d not supported and was skipped",
+                    record_indicator,
+                    row_num,
                 )
         except (KeyError, ValueError, AssertionError, IndexError, TypeError) as e:
             raise ValueError(f"Unable to parse line {row_num}") from e
 
     for nmi in readings:
         for suffix in readings[nmi]:
             readings[nmi][suffix] = flatten_list(readings[nmi][suffix])
@@ -368,15 +412,15 @@
         val_start,
         val_end,
     )
 
 
 def parse_200_row(row: list) -> NmiDetails:
     """Parse NMI data details record (200)
-    
+
     RecordIndicator,NMI,NMIConfiguration,RegisterID,NMISuffix,MDMDataStreamIdentifier,MeterSerialNumber,UOM,IntervalLength,NextScheduledReadDate
     Example: 200,VABD000163,E1Q1,1,E1,N1,METSER123,kWh,30,20040120
     """
 
     next_read = None  # Next scheduled read is an optional field
     if len(row) > 9:
         next_read = parse_datetime(row[9])
@@ -384,21 +428,21 @@
     return NmiDetails(
         row[1], row[2], row[3], row[4], row[5], row[6], row[7], int(row[8]), next_read
     )
 
 
 def parse_250_row(row: list) -> BasicMeterData:
     """Parse basic meter data record (250)
-    
-    RecordIndicator,NMI,NMIConfiguration,RegisterID,NMISuffix,MDMDataStreamIdentifier,MeterSeri
-alNumber,DirectionIndicator,PreviousRegisterRead,PreviousRegisterReadDateTime,PreviousQuali
-tyMethod,PreviousReasonCode,PreviousReasonDescription,CurrentRegisterRead,CurrentRegister
-ReadDateTime,CurrentQualityMethod,CurrentReasonCode,CurrentReasonDescription,Quantity,U
-OM,NextScheduledReadDate,UpdateDateTime,MSATSLoadDateTime
-    Example: 250,1234567890,1141,01,11,11,METSER66,E,000021.2,20031001103230,A,,,000534.5,20040201100030,E64,77,,343.5,kWh,20040509, 20040202125010,20040203000130
+
+        RecordIndicator,NMI,NMIConfiguration,RegisterID,NMISuffix,MDMDataStreamIdentifier,MeterSeri
+    alNumber,DirectionIndicator,PreviousRegisterRead,PreviousRegisterReadDateTime,PreviousQuali
+    tyMethod,PreviousReasonCode,PreviousReasonDescription,CurrentRegisterRead,CurrentRegister
+    ReadDateTime,CurrentQualityMethod,CurrentReasonCode,CurrentReasonDescription,Quantity,U
+    OM,NextScheduledReadDate,UpdateDateTime,MSATSLoadDateTime
+        Example: 250,1234567890,1141,01,11,11,METSER66,E,000021.2,20031001103230,A,,,000534.5,20040201100030,E64,77,,343.5,kWh,20040509, 20040202125010,20040203000130
     """
     return BasicMeterData(
         row[1],
         row[2],
         row[3],
         row[4],
         row[5],
@@ -427,27 +471,31 @@
     return next(islice(iterable, n, None), default)
 
 
 def parse_300_row(
     row: list, interval: int, uom: str, meter_serial_number: str
 ) -> IntervalRecord:
     """Interval data record (300)
-    
+
     RecordIndicator,IntervalDate,IntervalValue1 . . . IntervalValueN,
     QualityMethod,ReasonCode,ReasonDescription,UpdateDateTime,MSATSLoadDateTime
     Example: 300,20030501,50.1, . . . ,21.5,V,,,20030101153445,20030102023012
     """
-    num_non_reading_fields = 7 # count of fields except IntervalValue1 . . . IntervalValueN
+    num_non_reading_fields = (
+        7  # count of fields except IntervalValue1 . . . IntervalValueN
+    )
 
     num_intervals = int(minutes_per_day / interval)
-    
+
     interval_date = parse_datetime(row[1])
     last_interval = 2 + num_intervals
     if len(row) != num_intervals + num_non_reading_fields:
-        raise ValueError(f"Unexpected number of values in 300 row: {len(row)-num_non_reading_fields} readings for {interval}min intervals")
+        raise ValueError(
+            f"Unexpected number of values in 300 row: {len(row)-num_non_reading_fields} readings for {interval}min intervals"
+        )
     quality_method = row[last_interval]
 
     # Optional fields
     reason_code = nth(row, last_interval + 1, "")
     reason_desc = nth(row, last_interval + 2, "")
     update_datetime = parse_datetime(nth(row, last_interval + 3, None))
     msats_load_datatime = parse_datetime(nth(row, last_interval + 4, None))
@@ -512,29 +560,35 @@
     except ValueError:
         log.warning('Reading of "%s" is not a number', val)
         return None  # Not a valid reading
 
 
 def parse_400_row(row: list, interval_length: int) -> tuple:
     """Interval event record (400)
-    
+
     RecordIndicator,StartInterval,EndInterval,QualityMethod,ReasonCode,ReasonDescription
     Example: 400,1,28,S14,32
 
     Note that intervals are indexed from 1 not 0.
     """
     num_intervals = int(minutes_per_day / interval_length)
     start_interval = int(row[1])
     end_interval = int(row[2])
     if end_interval < start_interval:
-        raise ValueError(f"End interval {end_interval} is earlier than start interval {start_interval} in 400 row.")
+        raise ValueError(
+            f"End interval {end_interval} is earlier than start interval {start_interval} in 400 row."
+        )
     if not (0 < start_interval <= num_intervals):
-        raise ValueError(f"Invalid start interval {start_interval} in 400 row. Expecting {num_intervals} intervals.")
+        raise ValueError(
+            f"Invalid start interval {start_interval} in 400 row. Expecting {num_intervals} intervals."
+        )
     if not (0 < end_interval <= num_intervals):
-        raise ValueError(f"Invalid end interval {end_interval} in 400 row. Expecting {num_intervals} intervals.")
+        raise ValueError(
+            f"Invalid end interval {end_interval} in 400 row. Expecting {num_intervals} intervals."
+        )
 
     return EventRecord(int(row[1]), int(row[2]), row[3], row[4], row[5])
 
 
 def update_reading_events(readings, event_record):
     """Updates readings from a 300 row to reflect any events found in a
     subsequent 400 row
@@ -554,24 +608,24 @@
             val_end=readings[i].val_end,
         )
     return readings
 
 
 def parse_500_row(row: list) -> tuple:
     """Parse B2B details record
-    
+
     RecordIndicator,TransCode,RetServiceOrder,ReadDateTime,IndexRead
     Example: 500,S,RETNSRVCEORD1,20031220154500,001123.5
     """
     return B2BDetails12(row[1], row[2], row[3], row[4])
 
 
 def parse_550_row(row: list) -> tuple:
     """Parse B2B details record
-    
+
     RecordIndicator,PreviousTransCode,PreviousRetServiceOrder,CurrentTransCode,CurrentRetServiceOrder
     Example: 550,N,,A,
     """
     return B2BDetails13(row[1], row[2], row[3], row[4])
 
 
 def parse_datetime(record: str) -> Optional[datetime]:
```

### Comparing `nemreader-0.8.2/nemreader/split_days.py` & `nemreader-0.8.3/nemreader/split_days.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,14 @@
             if group_end not in group_records:
                 group_records[group_end] = [r]
             else:
                 group_records[group_end].append(r)
 
     # Output any aggregated grouped values
     for group_end in sorted(group_records.keys()):
-
         start = group_end - delta
         grp_readings = group_records[group_end]
         uom = grp_readings[0].uom
         meter_serial_number = grp_readings[0].meter_serial_number
         quality_methods = list(set([x.quality_method for x in grp_readings]))
         event_codes = list(set([x.event_code for x in grp_readings if x.event_code]))
         event_descs = list(set([x.event_desc for x in grp_readings if x.event_desc]))
```

### Comparing `nemreader-0.8.2/pyproject.toml` & `nemreader-0.8.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "nemreader"
 authors = [{ name = "Alex Guinman", email = "alex@guinman.id.au" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.11",    
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.8",
     "Operating System :: OS Independent",
 ]
 keywords = ["energy", "NEM12", "NEM13"]
 requires-python = ">=3.8"
@@ -35,13 +35,13 @@
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
 addopts = "-ra --failed-first --showlocals --durations=3 --cov=nemreader"
 
 [tool.coverage.run]
-omit = ["*/version.py"]
+omit = ["*/version.py", '*/__main__.py']
 
 [tool.coverage.report]
 show_missing = true
 skip_empty = true
-fail_under = 85
+fail_under = 90
```

### Comparing `nemreader-0.8.2/requirements.txt` & `nemreader-0.8.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/tests/test_actual_interval.py` & `nemreader-0.8.3/tests/test_actual_interval.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/tests/test_cli.py` & `nemreader-0.8.3/tests/test_cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,26 +5,46 @@
 
 
 @pytest.fixture
 def runner():
     return CliRunner()
 
 
+def test_cli_version(runner):
+    result = runner.invoke(app, ["--version"])
+    assert "nemreader version:" in result.stdout
+    assert result.exit_code == 0
+
+
 def test_cli_list_nmis(runner):
     file_name = "examples/unzipped/Example_NEM12_actual_interval.csv"
     result = runner.invoke(app, ["list-nmis", file_name, "--verbose"])
     assert "The following NMI[suffix] exist in this file:" in result.stdout
     assert result.exit_code == 0
 
 
 def test_cli_csv(runner):
     file_name = "examples/invalid/Example_NEM12_missing_header.csv"
     result = runner.invoke(app, ["output-csv", file_name, "--verbose"])
     assert "Created" in result.stdout
     assert result.exit_code == 0
 
 
+def test_cli_csv_daily(runner):
+    file_name = "examples/unzipped/Example_NEM12_actual_interval.csv"
+    result = runner.invoke(app, ["output-csv-daily", file_name, "--verbose"])
+    assert "Created" in result.stdout
+    assert result.exit_code == 0
+
+
 def test_cli_sqlite(runner):
     file_name = "examples/unzipped/Example_NEM12_actual_interval.csv"
     result = runner.invoke(app, ["output-sqlite", file_name, "--verbose"])
     assert "Finished exporting to DB." in result.stdout
     assert result.exit_code == 0
+
+
+def test_cli_sqlite_dir(runner):
+    file_dir = "examples/unzipped/"
+    result = runner.invoke(app, ["output-sqlite", file_dir, "--verbose"])
+    assert "Finished exporting to DB." in result.stdout
+    assert result.exit_code == 0
```

### Comparing `nemreader-0.8.2/tests/test_day_split.py` & `nemreader-0.8.3/tests/test_day_split.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-
 import pandas as pd
 
 from nemreader.outputs import output_as_data_frames
 
 
 def test_split_interval():
     """Create a temporary csv output"""
```

### Comparing `nemreader-0.8.2/tests/test_file_outputs.py` & `nemreader-0.8.3/tests/test_file_outputs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,42 @@
+from pathlib import Path
+
 from nemreader import (
     nmis_in_file,
     output_as_csv,
     output_as_daily_csv,
     output_as_data_frames,
 )
 
 
-def test_nmi_output(tmpdir):
+def test_nmi_output():
     """Check NMIs in file"""
     file_name = "examples/unzipped/Example_NEM12_multiple_meters.csv"
     items = list(nmis_in_file(file_name))
     nmis = [x[0] for x in items]
     assert "NCDE001111" in nmis
     assert "NDDD001888" in nmis
 
     suffixes = [x[1] for x in items]
     assert "E1" in suffixes[0]
     assert "E1" not in suffixes[1]
     assert "B1" in suffixes[1]
 
 
-def test_csv_output(tmpdir):
+def test_csv_output(tmp_path: Path):
     """Create a temporary csv output"""
     file_name = "examples/unzipped/Example_NEM12_actual_interval.csv"
-    output_files = output_as_csv(file_name, output_dir=tmpdir)
+    output_files = output_as_csv(file_name, output_dir=tmp_path)
     assert len(output_files) == 1
 
 
-def test_daily_csv_output(tmpdir):
+def test_daily_csv_output(tmp_path: Path):
     """Create a temporary csv output"""
     file_name = "examples/unzipped/Example_NEM12_actual_interval.csv"
-    output_file = output_as_daily_csv(file_name, output_dir=tmpdir)
+    output_file = output_as_daily_csv(file_name, output_dir=tmp_path)
     assert "Example_NEM12_actual_interval_daily_totals.csv" in str(output_file)
 
 
 def test_data_frame_output():
     """Create a pandas dataframe"""
     file_name = "examples/unzipped/Example_NEM12_actual_interval.csv"
     output_dfs = output_as_data_frames(file_name)
```

### Comparing `nemreader-0.8.2/tests/test_incomplete_files.py` & `nemreader-0.8.3/tests/test_incomplete_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import pytest
 
 from nemreader import NEMFile
 
 
 def test_correct_NMIs():
-
     nf = NEMFile("examples/invalid/Example_NEM12_powercor.csv", strict=False)
     meter_data = nf.nem_data()
     assert len(meter_data.readings) == 1
     assert "VABD000163" in meter_data.readings
 
 
 def test_incomplete_interval_row():
```

### Comparing `nemreader-0.8.2/tests/test_invalid_interval_mixing.py` & `nemreader-0.8.3/tests/test_invalid_interval_mixing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 import pytest
 
 from nemreader import NEMFile
 
 
 def test_30min_200_15min_300():
     with pytest.raises(ValueError):
-        nf = NEMFile("examples/invalid/Example_NEM12_30min_200_15min_300.csv", strict=False)
+        nf = NEMFile(
+            "examples/invalid/Example_NEM12_30min_200_15min_300.csv", strict=False
+        )
         meter_data = nf.nem_data()
 
+
 def test_15min_200_30min_300():
     with pytest.raises(ValueError):
-        nf = NEMFile("examples/invalid/Example_NEM12_15min_200_30min_300.csv", strict=False)
+        nf = NEMFile(
+            "examples/invalid/Example_NEM12_15min_200_30min_300.csv", strict=False
+        )
         meter_data = nf.nem_data()
 
+
 def test_30min_200_15min_400():
     with pytest.raises(ValueError):
-        nf = NEMFile("examples/invalid/Example_NEM12_30min_200_15min_400.csv", strict=False)
+        nf = NEMFile(
+            "examples/invalid/Example_NEM12_30min_200_15min_400.csv", strict=False
+        )
         meter_data = nf.nem_data()
 
+
 @pytest.mark.skip(reason="need to rearchitect parser to detect this")
 def test_15min_200_30min_400():
     with pytest.raises(ValueError):
-        nf = NEMFile("examples/invalid/Example_NEM12_15min_200_30min_400.csv", strict=False)
+        nf = NEMFile(
+            "examples/invalid/Example_NEM12_15min_200_30min_400.csv", strict=False
+        )
         meter_data = nf.nem_data()
```

### Comparing `nemreader-0.8.2/tests/test_multiple_quality.py` & `nemreader-0.8.3/tests/test_multiple_quality.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/tests/test_open_examples.py` & `nemreader-0.8.3/tests/test_open_examples.py`

 * *Files identical despite different names*

### Comparing `nemreader-0.8.2/tests/test_unit_capitalisation.py` & `nemreader-0.8.3/tests/test_unit_capitalisation.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     nf = NEMFile("examples/unzipped/Example_NEM12_upper_case_units.csv", strict=True)
     meter_data = nf.nem_data()
 
     df_15min = nf.get_pivot_data_frame(split_days=True, set_interval=15)
     df_30min = nf.get_pivot_data_frame(split_days=True, set_interval=30)
     df_60min = nf.get_pivot_data_frame(split_days=True, set_interval=60)
 
-    for (nmi, nmi_readings) in meter_data.readings.items():
+    for nmi, nmi_readings in meter_data.readings.items():
         for key in nmi_readings.keys():
             assert nmi_readings[key][0].t_end - nmi_readings[key][
                 0
             ].t_start == pd.Timedelta(minutes=30)
             assert "H" in nmi_readings[key][0].uom
 
         nmi_df_15min = df_15min[(df_15min["nmi"] == nmi)]
```

### Comparing `nemreader-0.8.2/PKG-INFO` & `nemreader-0.8.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nemreader
-Version: 0.8.2
+Version: 0.8.3
 Summary: nemreader
 Keywords: energy,NEM12,NEM13
 Author-email: Alex Guinman <alex@guinman.id.au>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/labscript-suite-3.2.0.tar.gz` & `tmp/labscript-suite-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labscript-suite-3.2.0.tar", last modified: Wed Apr 19 19:59:33 2023, max compression
+gzip compressed data, was "labscript-suite-3.2.0rc1.tar", last modified: Wed Apr 19 19:55:16 2023, max compression
```

## Comparing `labscript-suite-3.2.0.tar` & `labscript-suite-3.2.0rc1.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:59:33.900606 labscript-suite-3.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:59:33.880606 labscript-suite-3.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:59:33.880606 labscript-suite-3.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19044 2023-04-19 19:59:33.900606 labscript-suite-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:59:33.896606 labscript-suite-3.2.0/art/
--rw-r--r--   0 runner    (1001) docker     (123)   104672 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/blacs.ico
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/blacs_128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/blacs_128x128.svg
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/blacs_16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/blacs_16x16.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/blacs_22x22.png
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/blacs_22x22.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/blacs_256x256.png
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/blacs_256x256.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/blacs_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/blacs_32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/blacs_64x64.png
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/blacs_64x64.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-banner_1072x256.png
--rw-r--r--   0 runner    (1001) docker     (123)    17572 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-banner_1072x256.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-banner_134nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-banner_134x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-banner_268x64.png
--rw-r--r--   0 runner    (1001) docker     (123)    17571 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-banner_268x64.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-banner_536x128.png
--rw-r--r--   0 runner    (1001) docker     (123)    17572 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-banner_536x128.svg
--rw-r--r--   0 runner    (1001) docker     (123)    69044 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-dark_1104x560.png
--rw-r--r--   0 runner    (1001) docker     (123)    42277 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-dark_1104x560.svg
--rw-r--r--   0 runner    (1001) docker     (123)    47044 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-dark_138nx70n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-dark_138x70.png
--rw-r--r--   0 runner    (1001) docker     (123)    16177 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-dark_276x140.png
--rw-r--r--   0 runner    (1001) docker     (123)    42275 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-dark_276x140.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33668 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-dark_552x280.png
--rw-r--r--   0 runner    (1001) docker     (123)    42276 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-dark_552x280.svg
--rw-r--r--   0 runner    (1001) docker     (123)    68775 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-transparent_1104x560.png
--rw-r--r--   0 runner    (1001) docker     (123)    41928 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-transparent_1104x560.svg
--rw-r--r--   0 runner    (1001) docker     (123)    46681 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-transparent_138nx70n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-transparent_138x70.png
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-transparent_276x140.png
--rw-r--r--   0 runner    (1001) docker     (123)    41926 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-transparent_276x140.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33442 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-transparent_552x280.png
--rw-r--r--   0 runner    (1001) docker     (123)    41927 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-transparent_552x280.svg
--rw-r--r--   0 runner    (1001) docker     (123)    69605 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-white_1104x560.png
--rw-r--r--   0 runner    (1001) docker     (123)    42455 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-white_1104x560.svg
--rw-r--r--   0 runner    (1001) docker     (123)    46878 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-white_138nx70n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-white_138x70.png
--rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-white_276x140.png
--rw-r--r--   0 runner    (1001) docker     (123)    42453 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-white_276x140.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33692 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-white_552x280.png
--rw-r--r--   0 runner    (1001) docker     (123)    42454 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-rectangular-white_552x280.svg
--rw-r--r--   0 runner    (1001) docker     (123)    73409 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-square-dark_1104x1104.png
--rw-r--r--   0 runner    (1001) docker     (123)    40130 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-square-dark_1104x1104.svg
--rw-r--r--   0 runner    (1001) docker     (123)    44359 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-square-dark_138nx138n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-square-dark_138x138.png
--rw-r--r--   0 runner    (1001) docker     (123)    17056 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-square-dark_276x276.png
--rw-r--r--   0 runner    (1001) docker     (123)    40128 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-square-dark_276x276.svg
--rw-r--r--   0 runner    (1001) docker     (123)    35887 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-square-dark_552x552.png
--rw-r--r--   0 runner    (1001) docker     (123)    40130 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-square-dark_552x552.svg
--rw-r--r--   0 runner    (1001) docker     (123)    73932 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-square-white_1104x1104.png
--rw-r--r--   0 runner    (1001) docker     (123)    41117 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-square-white_1104x1104.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45434 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-square-white_138nx138n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-square-white_138x138.png
--rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-square-white_276x276.png
--rw-r--r--   0 runner    (1001) docker     (123)    41115 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-square-white_276x276.svg
--rw-r--r--   0 runner    (1001) docker     (123)    35917 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-square-white_552x552.png
--rw-r--r--   0 runner    (1001) docker     (123)    41117 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript-suite-square-white_552x552.svg
--rw-r--r--   0 runner    (1001) docker     (123)    98716 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript_128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript_128x128.svg
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript_16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript_16x16.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript_22x2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript_22x22.png
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript_256x256.png
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript_256x256.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript_32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript_64x64.png
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/labscript_64x64.svg
--rw-r--r--   0 runner    (1001) docker     (123)   102420 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/lyse.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/lyse_128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/lyse_128x128.svg
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/lyse_16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/lyse_16x16.svg
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/lyse_22x22.png
--rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/lyse_22x22.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/lyse_256x256.png
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/lyse_256x256.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/lyse_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/lyse_32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/lyse_64x64.png
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/lyse_64x64.svg
--rw-r--r--   0 runner    (1001) docker     (123)   106126 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runmanager.ico
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runmanager_128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runmanager_128x128.svg
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runmanager_16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runmanager_16x16.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runmanager_22x22.png
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runmanager_22x22.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runmanager_256x256.png
--rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runmanager_256x256.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runmanager_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runmanager_32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runmanager_64x64.png
--rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runmanager_64x64.svg
--rw-r--r--   0 runner    (1001) docker     (123)   103187 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runvewer.ico
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runviewer_128x128.png
--rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runviewer_128x128.svg
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runviewer_16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runviewer_16x16.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runviewer_22x22.png
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runviewer_22x22.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runviewer_256x256.png
--rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runviewer_256x256.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runviewer_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runviewer_32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runviewer_64x64.png
--rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/runviewer_64x64.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:59:33.896606 labscript-suite-3.2.0/art/source/
--rw-r--r--   0 runner    (1001) docker     (123)   570664 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/source/labscript-suite-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/art/source/make_scaled_svgs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:59:33.896606 labscript-suite-3.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:59:33.896606 labscript-suite-3.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:59:33.896606 labscript-suite-3.2.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:59:33.896606 labscript-suite-3.2.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/_templates/components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/archive.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:59:33.900606 labscript-suite-3.2.0/docs/source/building_docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/building_docs/docs_build.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/building_docs/docs_comitting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/building_docs/docs_install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/building_docs/docs_minutia.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/building_docs/docs_resources.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/building_docs/docs_writing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/building_docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/changes.md
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/community.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/features.md
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:59:33.900606 labscript-suite-3.2.0/docs/source/installation/
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/installation/developer-anaconda.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/installation/developer-pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/installation/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/installation/regular-anaconda.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/installation/regular-pypi.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/installation/regular-to-developer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/installation/setting-up-an-environment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/main.md
--rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/pyqt5-modified-objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/docs/source/troubleshooting.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:59:33.900606 labscript-suite-3.2.0/labscript_suite/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/labscript_suite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/labscript_suite/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:59:33.900606 labscript-suite-3.2.0/labscript_suite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19044 2023-04-19 19:59:33.000000 labscript-suite-3.2.0/labscript_suite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-19 19:59:33.000000 labscript-suite-3.2.0/labscript_suite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:59:33.000000 labscript-suite-3.2.0/labscript_suite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:59:33.000000 labscript-suite-3.2.0/labscript_suite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-19 19:59:33.000000 labscript-suite-3.2.0/labscript_suite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 19:59:33.000000 labscript-suite-3.2.0/labscript_suite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-19 19:59:33.900606 labscript-suite-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 19:59:23.000000 labscript-suite-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:16.947777 labscript-suite-3.2.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:16.903777 labscript-suite-3.2.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:16.907776 labscript-suite-3.2.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-04-19 19:55:16.947777 labscript-suite-3.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17885 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:16.939777 labscript-suite-3.2.0rc1/art/
+-rw-r--r--   0 runner    (1001) docker     (123)   104672 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/blacs.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/blacs_128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/blacs_128x128.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/blacs_16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/blacs_16x16.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/blacs_22x22.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/blacs_22x22.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/blacs_256x256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/blacs_256x256.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/blacs_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/blacs_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/blacs_64x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/blacs_64x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-banner_1072x256.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17572 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-banner_1072x256.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-banner_134nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-banner_134x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-banner_268x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17571 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-banner_268x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-banner_536x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17572 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-banner_536x128.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    69044 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-dark_1104x560.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42277 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-dark_1104x560.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    47044 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-dark_138nx70n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-dark_138x70.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16177 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-dark_276x140.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42275 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-dark_276x140.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33668 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-dark_552x280.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42276 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-dark_552x280.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    68775 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-transparent_1104x560.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41928 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-transparent_1104x560.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    46681 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-transparent_138nx70n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-transparent_138x70.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-transparent_276x140.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41926 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-transparent_276x140.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33442 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-transparent_552x280.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41927 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-transparent_552x280.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    69605 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-white_1104x560.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42455 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-white_1104x560.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    46878 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-white_138nx70n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-white_138x70.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-white_276x140.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42453 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-white_276x140.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33692 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-white_552x280.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42454 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-white_552x280.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    73409 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-square-dark_1104x1104.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40130 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-square-dark_1104x1104.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    44359 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-square-dark_138nx138n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-square-dark_138x138.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17056 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-square-dark_276x276.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40128 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-square-dark_276x276.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35887 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-square-dark_552x552.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40130 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-square-dark_552x552.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    73932 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-square-white_1104x1104.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41117 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-square-white_1104x1104.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45434 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-square-white_138nx138n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-square-white_138x138.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17034 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-square-white_276x276.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41115 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-square-white_276x276.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    35917 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-square-white_552x552.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41117 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript-suite-square-white_552x552.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    98716 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript_128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript_128x128.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript_16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript_16x16.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript_22x2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript_22x22.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript_256x256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript_256x256.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript_64x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/labscript_64x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   102420 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/lyse.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/lyse_128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/lyse_128x128.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/lyse_16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/lyse_16x16.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/lyse_22x22.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/lyse_22x22.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/lyse_256x256.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/lyse_256x256.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/lyse_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/lyse_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/lyse_64x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/lyse_64x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   106126 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runmanager.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runmanager_128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runmanager_128x128.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runmanager_16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runmanager_16x16.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runmanager_22x22.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runmanager_22x22.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runmanager_256x256.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runmanager_256x256.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runmanager_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runmanager_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runmanager_64x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runmanager_64x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   103187 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runvewer.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runviewer_128x128.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runviewer_128x128.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runviewer_16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runviewer_16x16.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runviewer_22x22.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runviewer_22x22.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runviewer_256x256.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runviewer_256x256.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runviewer_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runviewer_32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runviewer_64x64.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/runviewer_64x64.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:16.939777 labscript-suite-3.2.0rc1/art/source/
+-rw-r--r--   0 runner    (1001) docker     (123)   570664 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/source/labscript-suite-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/art/source/make_scaled_svgs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:16.939777 labscript-suite-3.2.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:16.943777 labscript-suite-3.2.0rc1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:16.943777 labscript-suite-3.2.0rc1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:16.943777 labscript-suite-3.2.0rc1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/_templates/components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/archive.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:16.943777 labscript-suite-3.2.0rc1/docs/source/building_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/building_docs/docs_build.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/building_docs/docs_comitting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/building_docs/docs_install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/building_docs/docs_minutia.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/building_docs/docs_resources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/building_docs/docs_writing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/building_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/changes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/community.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/features.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:16.947777 labscript-suite-3.2.0rc1/docs/source/installation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/installation/developer-anaconda.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/installation/developer-pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/installation/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/installation/regular-anaconda.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/installation/regular-pypi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/installation/regular-to-developer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/installation/setting-up-an-environment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/main.md
+-rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/pyqt5-modified-objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/docs/source/troubleshooting.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:16.947777 labscript-suite-3.2.0rc1/labscript_suite/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/labscript_suite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/labscript_suite/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:16.947777 labscript-suite-3.2.0rc1/labscript_suite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-04-19 19:55:16.000000 labscript-suite-3.2.0rc1/labscript_suite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-19 19:55:16.000000 labscript-suite-3.2.0rc1/labscript_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:55:16.000000 labscript-suite-3.2.0rc1/labscript_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:55:16.000000 labscript-suite-3.2.0rc1/labscript_suite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-19 19:55:16.000000 labscript-suite-3.2.0rc1/labscript_suite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 19:55:16.000000 labscript-suite-3.2.0rc1/labscript_suite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-19 19:55:16.947777 labscript-suite-3.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-19 19:55:01.000000 labscript-suite-3.2.0rc1/setup.py
```

### Comparing `labscript-suite-3.2.0/.github/workflows/release.yml` & `labscript-suite-3.2.0rc1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/.gitignore` & `labscript-suite-3.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/CITATION.cff` & `labscript-suite-3.2.0rc1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/LICENSE.txt` & `labscript-suite-3.2.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/PKG-INFO` & `labscript-suite-3.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labscript-suite
-Version: 3.2.0
+Version: 3.2.0rc1
 Summary: Meta-package for the labscript suite experiment control and automation system
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/labscript-suite
 Project-URL: Download, https://github.com/labscript-suite/labscript-suite/releases
@@ -29,15 +29,15 @@
 
 # the _labscript suite_
 
 <a href="https://github.com/labscript-suite/labscript"><img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/labscript_32nx32n.svg" height="64" alt="the labscript suite – labscript"></a> <a href="https://github.com/labscript-suite/runmanager"><img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/runmanager_32nx32n.svg" height="64" alt="the labscript suite – runmanager"></a> <a href="https://github.com/labscript-suite/blacs"><img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/blacs_32nx32n.svg" height="64" alt="the labscript suite – blacs"></a> <a href="https://github.com/labscript-suite/lyse"><img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/lyse_32nx32n.svg" height="64" alt="the labscript suite – lyse"></a> <a href="https://github.com/labscript-suite/runviewer"><img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/runviewer_32nx32n.svg" height="64" alt="the labscript suite – runviewer"></a>
 
 ### Experiment control and automation system
 
-[![Actions Status](https://github.com/labscript-suite/labscript-suite/workflows/Build%20and%20Release/badge.svg?event=push)](https://github.com/labscript-suite/labscript-suite/actions)
+[![Actions Status](https://github.com/labscript-suite/labscript-suite/workflows/Build%20and%20Release/badge.svg?branch=maintenance%2F3.0.x)](https://github.com/labscript-suite/labscript-suite/actions)
 [![Documentation Status](https://readthedocs.org/projects/labscriptsuite/badge/?version=latest)](https://docs.labscriptsuite.org)
 [![License](https://img.shields.io/pypi/l/labscript-suite.svg)](https://github.com/labscript-suite/labscript-suite/raw/master/LICENSE.txt)
 [![Python Version](https://img.shields.io/pypi/pyversions/labscript-suite.svg)](https://python.org)
 [![PyPI](https://img.shields.io/pypi/v/labscript-suite.svg)](https://pypi.org/project/labscript-suite)
 [![Conda Version](https://img.shields.io/conda/v/labscript-suite/labscript-suite)](https://anaconda.org/labscript-suite/labscript-suite)
 [![Google Group](https://img.shields.io/badge/Google%20Group-labscriptsuite-blue.svg)](https://groups.google.com/forum/#!forum/labscriptsuite)
 [![DOI](https://img.shields.io/badge/DOI-10.1063%2F1.4817213-0F79D0.svg)](https://doi.org/10.1063/1.4817213)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: labscript-suite Version: 3.2.0 Summary: Meta-
+Metadata-Version: 2.1 Name: labscript-suite Version: 3.2.0rc1 Summary: Meta-
 package for the labscript suite experiment control and automation system Home-
 page: http://labscriptsuite.org Author: The labscript suite community Author-
 email: labscriptsuite@googlegroups.com License: BSD Project-URL: Source Code,
 https://github.com/labscript-suite/labscript-suite Project-URL: Download,
 https://github.com/labscript-suite/labscript-suite/releases Project-URL:
 Tracker, https://github.com/labscript-suite/labscript-suite/issues Keywords:
 experiment control automation Classifier: License :: OSI Approved :: BSD
@@ -14,18 +14,18 @@
 Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra: pyqt
 Provides-Extra: spincore Provides-Extra: nidaqmx Provides-Extra: nivision
 Provides-Extra: docs License-File: LICENSE.txt # the _labscript suite_ [the
 labscript_suite_â_labscript] [the_labscript_suite_â_runmanager] [the
 labscript_suite_â_blacs] [the_labscript_suite_â_lyse] [the_labscript_suite
 â_runviewer] ### Experiment control and automation system [![Actions Status]
 (https://github.com/labscript-suite/labscript-suite/workflows/
-Build%20and%20Release/badge.svg?event=push)](https://github.com/labscript-
-suite/labscript-suite/actions) [![Documentation Status](https://
-readthedocs.org/projects/labscriptsuite/badge/?version=latest)](https://
-docs.labscriptsuite.org) [![License](https://img.shields.io/pypi/l/labscript-
+Build%20and%20Release/badge.svg?branch=maintenance%2F3.0.x)](https://
+github.com/labscript-suite/labscript-suite/actions) [![Documentation Status]
+(https://readthedocs.org/projects/labscriptsuite/badge/?version=latest)](https:
+//docs.labscriptsuite.org) [![License](https://img.shields.io/pypi/l/labscript-
 suite.svg)](https://github.com/labscript-suite/labscript-suite/raw/master/
 LICENSE.txt) [![Python Version](https://img.shields.io/pypi/pyversions/
 labscript-suite.svg)](https://python.org) [![PyPI](https://img.shields.io/pypi/
 v/labscript-suite.svg)](https://pypi.org/project/labscript-suite) [![Conda
 Version](https://img.shields.io/conda/v/labscript-suite/labscript-suite)]
 (https://anaconda.org/labscript-suite/labscript-suite) [![Google Group](https:/
 /img.shields.io/badge/Google%20Group-labscriptsuite-blue.svg)](https://
```

### Comparing `labscript-suite-3.2.0/README.md` & `labscript-suite-3.2.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # the _labscript suite_
 
 <a href="https://github.com/labscript-suite/labscript"><img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/labscript_32nx32n.svg" height="64" alt="the labscript suite – labscript"></a> <a href="https://github.com/labscript-suite/runmanager"><img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/runmanager_32nx32n.svg" height="64" alt="the labscript suite – runmanager"></a> <a href="https://github.com/labscript-suite/blacs"><img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/blacs_32nx32n.svg" height="64" alt="the labscript suite – blacs"></a> <a href="https://github.com/labscript-suite/lyse"><img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/lyse_32nx32n.svg" height="64" alt="the labscript suite – lyse"></a> <a href="https://github.com/labscript-suite/runviewer"><img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/runviewer_32nx32n.svg" height="64" alt="the labscript suite – runviewer"></a>
 
 ### Experiment control and automation system
 
-[![Actions Status](https://github.com/labscript-suite/labscript-suite/workflows/Build%20and%20Release/badge.svg?event=push)](https://github.com/labscript-suite/labscript-suite/actions)
+[![Actions Status](https://github.com/labscript-suite/labscript-suite/workflows/Build%20and%20Release/badge.svg?branch=maintenance%2F3.0.x)](https://github.com/labscript-suite/labscript-suite/actions)
 [![Documentation Status](https://readthedocs.org/projects/labscriptsuite/badge/?version=latest)](https://docs.labscriptsuite.org)
 [![License](https://img.shields.io/pypi/l/labscript-suite.svg)](https://github.com/labscript-suite/labscript-suite/raw/master/LICENSE.txt)
 [![Python Version](https://img.shields.io/pypi/pyversions/labscript-suite.svg)](https://python.org)
 [![PyPI](https://img.shields.io/pypi/v/labscript-suite.svg)](https://pypi.org/project/labscript-suite)
 [![Conda Version](https://img.shields.io/conda/v/labscript-suite/labscript-suite)](https://anaconda.org/labscript-suite/labscript-suite)
 [![Google Group](https://img.shields.io/badge/Google%20Group-labscriptsuite-blue.svg)](https://groups.google.com/forum/#!forum/labscriptsuite)
 [![DOI](https://img.shields.io/badge/DOI-10.1063%2F1.4817213-0F79D0.svg)](https://doi.org/10.1063/1.4817213)
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # the _labscript suite_ [the_labscript_suite_â_labscript] [the_labscript
 suite_â_runmanager] [the_labscript_suite_â_blacs] [the_labscript_suite_â
 lyse] [the_labscript_suite_â_runviewer] ### Experiment control and automation
 system [![Actions Status](https://github.com/labscript-suite/labscript-suite/
-workflows/Build%20and%20Release/badge.svg?event=push)](https://github.com/
-labscript-suite/labscript-suite/actions) [![Documentation Status](https://
-readthedocs.org/projects/labscriptsuite/badge/?version=latest)](https://
-docs.labscriptsuite.org) [![License](https://img.shields.io/pypi/l/labscript-
+workflows/Build%20and%20Release/badge.svg?branch=maintenance%2F3.0.x)](https://
+github.com/labscript-suite/labscript-suite/actions) [![Documentation Status]
+(https://readthedocs.org/projects/labscriptsuite/badge/?version=latest)](https:
+//docs.labscriptsuite.org) [![License](https://img.shields.io/pypi/l/labscript-
 suite.svg)](https://github.com/labscript-suite/labscript-suite/raw/master/
 LICENSE.txt) [![Python Version](https://img.shields.io/pypi/pyversions/
 labscript-suite.svg)](https://python.org) [![PyPI](https://img.shields.io/pypi/
 v/labscript-suite.svg)](https://pypi.org/project/labscript-suite) [![Conda
 Version](https://img.shields.io/conda/v/labscript-suite/labscript-suite)]
 (https://anaconda.org/labscript-suite/labscript-suite) [![Google Group](https:/
 /img.shields.io/badge/Google%20Group-labscriptsuite-blue.svg)](https://
```

### Comparing `labscript-suite-3.2.0/art/blacs.ico` & `labscript-suite-3.2.0rc1/art/blacs.ico`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/blacs_128x128.png` & `labscript-suite-3.2.0rc1/art/blacs_128x128.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/blacs_128x128.svg` & `labscript-suite-3.2.0rc1/art/blacs_128x128.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/blacs_16x16.png` & `labscript-suite-3.2.0rc1/art/blacs_16x16.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/blacs_16x16.svg` & `labscript-suite-3.2.0rc1/art/blacs_16x16.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/blacs_22x22.png` & `labscript-suite-3.2.0rc1/art/blacs_22x22.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/blacs_22x22.svg` & `labscript-suite-3.2.0rc1/art/blacs_22x22.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/blacs_256x256.png` & `labscript-suite-3.2.0rc1/art/blacs_256x256.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/blacs_256x256.svg` & `labscript-suite-3.2.0rc1/art/blacs_256x256.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/blacs_32nx32n.svg` & `labscript-suite-3.2.0rc1/art/blacs_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/blacs_32x32.png` & `labscript-suite-3.2.0rc1/art/blacs_32x32.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/blacs_64x64.png` & `labscript-suite-3.2.0rc1/art/blacs_64x64.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/blacs_64x64.svg` & `labscript-suite-3.2.0rc1/art/blacs_64x64.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-banner_1072x256.png` & `labscript-suite-3.2.0rc1/art/labscript-banner_1072x256.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-banner_1072x256.svg` & `labscript-suite-3.2.0rc1/art/labscript-banner_1072x256.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-banner_134nx32n.svg` & `labscript-suite-3.2.0rc1/art/labscript-banner_134nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-banner_134x32.png` & `labscript-suite-3.2.0rc1/art/labscript-banner_134x32.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-banner_268x64.png` & `labscript-suite-3.2.0rc1/art/labscript-banner_268x64.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-banner_268x64.svg` & `labscript-suite-3.2.0rc1/art/labscript-banner_268x64.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-banner_536x128.png` & `labscript-suite-3.2.0rc1/art/labscript-banner_536x128.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-banner_536x128.svg` & `labscript-suite-3.2.0rc1/art/labscript-banner_536x128.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-dark_1104x560.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-dark_1104x560.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-dark_1104x560.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-dark_1104x560.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-dark_138nx70n.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-dark_138nx70n.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-dark_138x70.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-dark_138x70.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-dark_276x140.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-dark_276x140.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-dark_276x140.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-dark_276x140.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-dark_552x280.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-dark_552x280.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-dark_552x280.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-dark_552x280.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-transparent_1104x560.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-transparent_1104x560.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-transparent_1104x560.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-transparent_1104x560.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-transparent_138nx70n.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-transparent_138nx70n.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-transparent_138x70.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-transparent_138x70.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-transparent_276x140.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-transparent_276x140.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-transparent_276x140.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-transparent_276x140.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-transparent_552x280.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-transparent_552x280.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-transparent_552x280.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-transparent_552x280.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-white_1104x560.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-white_1104x560.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-white_1104x560.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-white_1104x560.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-white_138nx70n.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-white_138nx70n.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-white_138x70.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-white_138x70.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-white_276x140.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-white_276x140.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-white_276x140.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-white_276x140.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-white_552x280.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-white_552x280.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-rectangular-white_552x280.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-rectangular-white_552x280.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-square-dark_1104x1104.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-square-dark_1104x1104.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-square-dark_1104x1104.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-square-dark_1104x1104.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-square-dark_138nx138n.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-square-dark_138nx138n.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-square-dark_138x138.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-square-dark_138x138.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-square-dark_276x276.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-square-dark_276x276.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-square-dark_276x276.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-square-dark_276x276.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-square-dark_552x552.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-square-dark_552x552.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-square-dark_552x552.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-square-dark_552x552.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-square-white_1104x1104.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-square-white_1104x1104.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-square-white_1104x1104.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-square-white_1104x1104.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-square-white_138nx138n.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-square-white_138nx138n.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-square-white_138x138.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-square-white_138x138.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-square-white_276x276.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-square-white_276x276.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-square-white_276x276.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-square-white_276x276.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-square-white_552x552.png` & `labscript-suite-3.2.0rc1/art/labscript-suite-square-white_552x552.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript-suite-square-white_552x552.svg` & `labscript-suite-3.2.0rc1/art/labscript-suite-square-white_552x552.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript.ico` & `labscript-suite-3.2.0rc1/art/labscript.ico`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript_128x128.png` & `labscript-suite-3.2.0rc1/art/labscript_128x128.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript_128x128.svg` & `labscript-suite-3.2.0rc1/art/labscript_128x128.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript_16x16.png` & `labscript-suite-3.2.0rc1/art/labscript_16x16.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript_16x16.svg` & `labscript-suite-3.2.0rc1/art/labscript_16x16.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript_22x2.svg` & `labscript-suite-3.2.0rc1/art/labscript_22x2.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript_22x22.png` & `labscript-suite-3.2.0rc1/art/labscript_22x22.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript_256x256.png` & `labscript-suite-3.2.0rc1/art/labscript_256x256.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript_256x256.svg` & `labscript-suite-3.2.0rc1/art/labscript_256x256.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript_32nx32n.svg` & `labscript-suite-3.2.0rc1/art/labscript_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript_32x32.png` & `labscript-suite-3.2.0rc1/art/labscript_32x32.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript_64x64.png` & `labscript-suite-3.2.0rc1/art/labscript_64x64.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/labscript_64x64.svg` & `labscript-suite-3.2.0rc1/art/labscript_64x64.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/lyse.ico` & `labscript-suite-3.2.0rc1/art/lyse.ico`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/lyse_128x128.png` & `labscript-suite-3.2.0rc1/art/lyse_128x128.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/lyse_128x128.svg` & `labscript-suite-3.2.0rc1/art/lyse_128x128.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/lyse_16x16.png` & `labscript-suite-3.2.0rc1/art/lyse_16x16.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/lyse_16x16.svg` & `labscript-suite-3.2.0rc1/art/lyse_16x16.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/lyse_22x22.png` & `labscript-suite-3.2.0rc1/art/lyse_22x22.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/lyse_22x22.svg` & `labscript-suite-3.2.0rc1/art/lyse_22x22.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/lyse_256x256.png` & `labscript-suite-3.2.0rc1/art/lyse_256x256.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/lyse_256x256.svg` & `labscript-suite-3.2.0rc1/art/lyse_256x256.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/lyse_32nx32n.svg` & `labscript-suite-3.2.0rc1/art/lyse_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/lyse_32x32.png` & `labscript-suite-3.2.0rc1/art/lyse_32x32.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/lyse_64x64.png` & `labscript-suite-3.2.0rc1/art/lyse_64x64.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/lyse_64x64.svg` & `labscript-suite-3.2.0rc1/art/lyse_64x64.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runmanager.ico` & `labscript-suite-3.2.0rc1/art/runmanager.ico`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runmanager_128x128.png` & `labscript-suite-3.2.0rc1/art/runmanager_128x128.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runmanager_128x128.svg` & `labscript-suite-3.2.0rc1/art/runmanager_128x128.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runmanager_16x16.png` & `labscript-suite-3.2.0rc1/art/runmanager_16x16.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runmanager_16x16.svg` & `labscript-suite-3.2.0rc1/art/runmanager_16x16.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runmanager_22x22.png` & `labscript-suite-3.2.0rc1/art/runmanager_22x22.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runmanager_22x22.svg` & `labscript-suite-3.2.0rc1/art/runmanager_22x22.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runmanager_256x256.png` & `labscript-suite-3.2.0rc1/art/runmanager_256x256.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runmanager_256x256.svg` & `labscript-suite-3.2.0rc1/art/runmanager_256x256.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runmanager_32nx32n.svg` & `labscript-suite-3.2.0rc1/art/runmanager_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runmanager_32x32.png` & `labscript-suite-3.2.0rc1/art/runmanager_32x32.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runmanager_64x64.png` & `labscript-suite-3.2.0rc1/art/runmanager_64x64.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runmanager_64x64.svg` & `labscript-suite-3.2.0rc1/art/runmanager_64x64.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runvewer.ico` & `labscript-suite-3.2.0rc1/art/runvewer.ico`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runviewer_128x128.png` & `labscript-suite-3.2.0rc1/art/runviewer_128x128.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runviewer_128x128.svg` & `labscript-suite-3.2.0rc1/art/runviewer_128x128.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runviewer_16x16.png` & `labscript-suite-3.2.0rc1/art/runviewer_16x16.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runviewer_16x16.svg` & `labscript-suite-3.2.0rc1/art/runviewer_16x16.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runviewer_22x22.png` & `labscript-suite-3.2.0rc1/art/runviewer_22x22.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runviewer_22x22.svg` & `labscript-suite-3.2.0rc1/art/runviewer_22x22.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runviewer_256x256.png` & `labscript-suite-3.2.0rc1/art/runviewer_256x256.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runviewer_256x256.svg` & `labscript-suite-3.2.0rc1/art/runviewer_256x256.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runviewer_32nx32n.svg` & `labscript-suite-3.2.0rc1/art/runviewer_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runviewer_32x32.png` & `labscript-suite-3.2.0rc1/art/runviewer_32x32.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runviewer_64x64.png` & `labscript-suite-3.2.0rc1/art/runviewer_64x64.png`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/runviewer_64x64.svg` & `labscript-suite-3.2.0rc1/art/runviewer_64x64.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/source/labscript-suite-icons.svg` & `labscript-suite-3.2.0rc1/art/source/labscript-suite-icons.svg`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/art/source/make_scaled_svgs.py` & `labscript-suite-3.2.0rc1/art/source/make_scaled_svgs.py`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/Makefile` & `labscript-suite-3.2.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/make.bat` & `labscript-suite-3.2.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/_static/custom.css` & `labscript-suite-3.2.0rc1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/_templates/components.rst` & `labscript-suite-3.2.0rc1/docs/source/_templates/components.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/archive.md` & `labscript-suite-3.2.0rc1/docs/source/archive.md`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/building_docs/docs_build.rst` & `labscript-suite-3.2.0rc1/docs/source/building_docs/docs_build.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/building_docs/docs_comitting.rst` & `labscript-suite-3.2.0rc1/docs/source/building_docs/docs_comitting.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/building_docs/docs_install.rst` & `labscript-suite-3.2.0rc1/docs/source/building_docs/docs_install.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/building_docs/docs_minutia.rst` & `labscript-suite-3.2.0rc1/docs/source/building_docs/docs_minutia.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/building_docs/docs_resources.rst` & `labscript-suite-3.2.0rc1/docs/source/building_docs/docs_resources.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/building_docs/docs_writing.rst` & `labscript-suite-3.2.0rc1/docs/source/building_docs/docs_writing.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/building_docs.rst` & `labscript-suite-3.2.0rc1/docs/source/building_docs.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/changes.md` & `labscript-suite-3.2.0rc1/docs/source/changes.md`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/community.rst` & `labscript-suite-3.2.0rc1/docs/source/community.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/conf.py` & `labscript-suite-3.2.0rc1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/configuration.rst` & `labscript-suite-3.2.0rc1/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/contributing.md` & `labscript-suite-3.2.0rc1/docs/source/contributing.md`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/features.md` & `labscript-suite-3.2.0rc1/docs/source/features.md`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/index.rst` & `labscript-suite-3.2.0rc1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/installation/developer-anaconda.rst` & `labscript-suite-3.2.0rc1/docs/source/installation/developer-anaconda.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/installation/developer-pypi.rst` & `labscript-suite-3.2.0rc1/docs/source/installation/developer-pypi.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/installation/index.rst` & `labscript-suite-3.2.0rc1/docs/source/installation/index.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/installation/regular-anaconda.rst` & `labscript-suite-3.2.0rc1/docs/source/installation/regular-anaconda.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/installation/regular-pypi.rst` & `labscript-suite-3.2.0rc1/docs/source/installation/regular-pypi.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/installation/setting-up-an-environment.rst` & `labscript-suite-3.2.0rc1/docs/source/installation/setting-up-an-environment.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/main.md` & `labscript-suite-3.2.0rc1/docs/source/main.md`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/pyqt5-modified-objects.inv` & `labscript-suite-3.2.0rc1/docs/source/pyqt5-modified-objects.inv`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/docs/source/troubleshooting.rst` & `labscript-suite-3.2.0rc1/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/labscript_suite.egg-info/PKG-INFO` & `labscript-suite-3.2.0rc1/labscript_suite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labscript-suite
-Version: 3.2.0
+Version: 3.2.0rc1
 Summary: Meta-package for the labscript suite experiment control and automation system
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/labscript-suite
 Project-URL: Download, https://github.com/labscript-suite/labscript-suite/releases
@@ -29,15 +29,15 @@
 
 # the _labscript suite_
 
 <a href="https://github.com/labscript-suite/labscript"><img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/labscript_32nx32n.svg" height="64" alt="the labscript suite – labscript"></a> <a href="https://github.com/labscript-suite/runmanager"><img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/runmanager_32nx32n.svg" height="64" alt="the labscript suite – runmanager"></a> <a href="https://github.com/labscript-suite/blacs"><img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/blacs_32nx32n.svg" height="64" alt="the labscript suite – blacs"></a> <a href="https://github.com/labscript-suite/lyse"><img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/lyse_32nx32n.svg" height="64" alt="the labscript suite – lyse"></a> <a href="https://github.com/labscript-suite/runviewer"><img src="https://raw.githubusercontent.com/labscript-suite/labscript-suite/master/art/runviewer_32nx32n.svg" height="64" alt="the labscript suite – runviewer"></a>
 
 ### Experiment control and automation system
 
-[![Actions Status](https://github.com/labscript-suite/labscript-suite/workflows/Build%20and%20Release/badge.svg?event=push)](https://github.com/labscript-suite/labscript-suite/actions)
+[![Actions Status](https://github.com/labscript-suite/labscript-suite/workflows/Build%20and%20Release/badge.svg?branch=maintenance%2F3.0.x)](https://github.com/labscript-suite/labscript-suite/actions)
 [![Documentation Status](https://readthedocs.org/projects/labscriptsuite/badge/?version=latest)](https://docs.labscriptsuite.org)
 [![License](https://img.shields.io/pypi/l/labscript-suite.svg)](https://github.com/labscript-suite/labscript-suite/raw/master/LICENSE.txt)
 [![Python Version](https://img.shields.io/pypi/pyversions/labscript-suite.svg)](https://python.org)
 [![PyPI](https://img.shields.io/pypi/v/labscript-suite.svg)](https://pypi.org/project/labscript-suite)
 [![Conda Version](https://img.shields.io/conda/v/labscript-suite/labscript-suite)](https://anaconda.org/labscript-suite/labscript-suite)
 [![Google Group](https://img.shields.io/badge/Google%20Group-labscriptsuite-blue.svg)](https://groups.google.com/forum/#!forum/labscriptsuite)
 [![DOI](https://img.shields.io/badge/DOI-10.1063%2F1.4817213-0F79D0.svg)](https://doi.org/10.1063/1.4817213)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: labscript-suite Version: 3.2.0 Summary: Meta-
+Metadata-Version: 2.1 Name: labscript-suite Version: 3.2.0rc1 Summary: Meta-
 package for the labscript suite experiment control and automation system Home-
 page: http://labscriptsuite.org Author: The labscript suite community Author-
 email: labscriptsuite@googlegroups.com License: BSD Project-URL: Source Code,
 https://github.com/labscript-suite/labscript-suite Project-URL: Download,
 https://github.com/labscript-suite/labscript-suite/releases Project-URL:
 Tracker, https://github.com/labscript-suite/labscript-suite/issues Keywords:
 experiment control automation Classifier: License :: OSI Approved :: BSD
@@ -14,18 +14,18 @@
 Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra: pyqt
 Provides-Extra: spincore Provides-Extra: nidaqmx Provides-Extra: nivision
 Provides-Extra: docs License-File: LICENSE.txt # the _labscript suite_ [the
 labscript_suite_â_labscript] [the_labscript_suite_â_runmanager] [the
 labscript_suite_â_blacs] [the_labscript_suite_â_lyse] [the_labscript_suite
 â_runviewer] ### Experiment control and automation system [![Actions Status]
 (https://github.com/labscript-suite/labscript-suite/workflows/
-Build%20and%20Release/badge.svg?event=push)](https://github.com/labscript-
-suite/labscript-suite/actions) [![Documentation Status](https://
-readthedocs.org/projects/labscriptsuite/badge/?version=latest)](https://
-docs.labscriptsuite.org) [![License](https://img.shields.io/pypi/l/labscript-
+Build%20and%20Release/badge.svg?branch=maintenance%2F3.0.x)](https://
+github.com/labscript-suite/labscript-suite/actions) [![Documentation Status]
+(https://readthedocs.org/projects/labscriptsuite/badge/?version=latest)](https:
+//docs.labscriptsuite.org) [![License](https://img.shields.io/pypi/l/labscript-
 suite.svg)](https://github.com/labscript-suite/labscript-suite/raw/master/
 LICENSE.txt) [![Python Version](https://img.shields.io/pypi/pyversions/
 labscript-suite.svg)](https://python.org) [![PyPI](https://img.shields.io/pypi/
 v/labscript-suite.svg)](https://pypi.org/project/labscript-suite) [![Conda
 Version](https://img.shields.io/conda/v/labscript-suite/labscript-suite)]
 (https://anaconda.org/labscript-suite/labscript-suite) [![Google Group](https:/
 /img.shields.io/badge/Google%20Group-labscriptsuite-blue.svg)](https://
```

### Comparing `labscript-suite-3.2.0/labscript_suite.egg-info/SOURCES.txt` & `labscript-suite-3.2.0rc1/labscript_suite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/readthedocs.yaml` & `labscript-suite-3.2.0rc1/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `labscript-suite-3.2.0/setup.cfg` & `labscript-suite-3.2.0rc1/setup.cfg`

 * *Files identical despite different names*


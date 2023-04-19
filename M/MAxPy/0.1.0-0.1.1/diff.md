# Comparing `tmp/MAxPy-0.1.0.tar.gz` & `tmp/MAxPy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MAxPy-0.1.0.tar", last modified: Fri Apr 14 04:16:43 2023, max compression
+gzip compressed data, was "MAxPy-0.1.1.tar", last modified: Wed Apr 19 01:19:27 2023, max compression
```

## Comparing `MAxPy-0.1.0.tar` & `MAxPy-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,60 @@
-drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-14 04:16:43.488294 MAxPy-0.1.0/
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)     1070 2023-04-14 02:22:18.000000 MAxPy-0.1.0/LICENSE
--rw-r--r--   0 ysba      (1000) ysba      (1000)     2316 2023-04-14 04:16:43.488294 MAxPy-0.1.0/PKG-INFO
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)     1774 2023-04-14 04:09:13.000000 MAxPy-0.1.0/README.md
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)       94 2023-04-14 03:59:12.000000 MAxPy-0.1.0/pyproject.toml
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)      805 2023-04-14 04:16:43.488294 MAxPy-0.1.0/setup.cfg
-drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-14 04:16:43.484961 MAxPy-0.1.0/src/
-drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-14 04:16:43.484961 MAxPy-0.1.0/src/MAxPy/
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)       30 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/__init__.py
--rw-r--r--   0 ysba      (1000) ysba      (1000)      706 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/check.py
--rw-r--r--   0 ysba      (1000) ysba      (1000)     3985 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/compile.py
--rw-r--r--   0 ysba      (1000) ysba      (1000)     3658 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/estimations.py
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)    12802 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/maxpy.py
--rw-r--r--   0 ysba      (1000) ysba      (1000)      547 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/pareto.py
-drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-14 04:16:43.488294 MAxPy-0.1.0/src/MAxPy/pdk/
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)  2345732 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/pdk/NanGate15nm.lib
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)    25021 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/pdk/NanGate15nm.v
--rw-r--r--   0 ysba      (1000) ysba      (1000)     9156 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/probprun.py
--rw-r--r--   0 ysba      (1000) ysba      (1000)     1909 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/resources.py
--rw-r--r--   0 ysba      (1000) ysba      (1000)     1447 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/results.py
--rw-r--r--   0 ysba      (1000) ysba      (1000)     4591 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/synth.py
-drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-14 04:16:43.484961 MAxPy-0.1.0/src/MAxPy/tcl/
-drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-14 04:16:43.488294 MAxPy-0.1.0/src/MAxPy/tcl/Genus/
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)     1006 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/tcl/Genus/constraints.sdc
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)     1083 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/tcl/Genus/qor_saif.tcl
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)      931 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/tcl/Genus/qor_sta.tcl
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)      149 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/tcl/Genus/sdf_cmd_file.base
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)     1545 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/tcl/Genus/sta.tcl
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)     1702 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/tcl/Genus/synth.tcl
-drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-14 04:16:43.488294 MAxPy-0.1.0/src/MAxPy/tcl/Incisive/
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)      116 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/tcl/Incisive/tcf_cmd.tcl
-drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-14 04:16:43.488294 MAxPy-0.1.0/src/MAxPy/tcl/OpenSTA/
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)      222 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/tcl/OpenSTA/cmd_file.sta
-drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-14 04:16:43.488294 MAxPy-0.1.0/src/MAxPy/tcl/Verilator/
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)      315 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/tcl/Verilator/verilator_config.vlt
-drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-14 04:16:43.488294 MAxPy-0.1.0/src/MAxPy/tcl/Yosys/
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)      226 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/tcl/Yosys/synth.ys
-drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-14 04:16:43.488294 MAxPy-0.1.0/src/MAxPy/templates/
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)      365 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/templates/cmake_pybind.txt
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)      172 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/templates/instance_source.cpp
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)     7606 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/templates/verilator_pybind_wrapper.cpp
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)     2702 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/templates/verilator_pybind_wrapper.h
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)     1649 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/utility.py
--rw-r--r--   0 ysba      (1000) ysba      (1000)     2693 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/verilate.py
--rw-r--r--   0 ysba      (1000) ysba      (1000)    23679 2023-03-27 22:55:42.000000 MAxPy-0.1.0/src/MAxPy/wrapper.py
-drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-14 04:16:43.488294 MAxPy-0.1.0/src/MAxPy.egg-info/
--rw-r--r--   0 ysba      (1000) ysba      (1000)     2316 2023-04-14 04:16:43.000000 MAxPy-0.1.0/src/MAxPy.egg-info/PKG-INFO
--rw-r--r--   0 ysba      (1000) ysba      (1000)     1040 2023-04-14 04:16:43.000000 MAxPy-0.1.0/src/MAxPy.egg-info/SOURCES.txt
--rw-r--r--   0 ysba      (1000) ysba      (1000)        1 2023-04-14 04:16:43.000000 MAxPy-0.1.0/src/MAxPy.egg-info/dependency_links.txt
--rw-r--r--   0 ysba      (1000) ysba      (1000)        6 2023-04-14 04:16:43.000000 MAxPy-0.1.0/src/MAxPy.egg-info/top_level.txt
-drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-14 04:16:43.488294 MAxPy-0.1.0/tests/
--rwxr-xr-x   0 ysba      (1000) ysba      (1000)      990 2023-03-27 22:55:42.000000 MAxPy-0.1.0/tests/testbench.py
+drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-19 01:19:27.051917 MAxPy-0.1.1/
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)     1070 2023-04-14 02:22:18.000000 MAxPy-0.1.1/LICENSE
+-rw-r--r--   0 ysba      (1000) ysba      (1000)     2316 2023-04-19 01:19:27.051917 MAxPy-0.1.1/PKG-INFO
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)     1774 2023-04-14 04:09:13.000000 MAxPy-0.1.1/README.md
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)       94 2023-04-14 03:59:12.000000 MAxPy-0.1.1/pyproject.toml
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)      805 2023-04-19 01:19:27.051917 MAxPy-0.1.1/setup.cfg
+drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-19 01:19:27.045250 MAxPy-0.1.1/src/
+drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-19 01:19:27.048583 MAxPy-0.1.1/src/MAxPy/
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)       30 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/__init__.py
+-rw-r--r--   0 ysba      (1000) ysba      (1000)      706 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/check.py
+-rw-r--r--   0 ysba      (1000) ysba      (1000)     3985 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/compile.py
+-rw-r--r--   0 ysba      (1000) ysba      (1000)     3658 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/estimations.py
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)    12802 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/maxpy.py
+-rw-r--r--   0 ysba      (1000) ysba      (1000)      547 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/pareto.py
+drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-19 01:19:27.048583 MAxPy-0.1.1/src/MAxPy/pdk/
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)  2345732 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/pdk/NanGate15nm.lib
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)    25021 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/pdk/NanGate15nm.v
+-rw-r--r--   0 ysba      (1000) ysba      (1000)     9156 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/probprun.py
+-rw-r--r--   0 ysba      (1000) ysba      (1000)     1909 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/resources.py
+-rw-r--r--   0 ysba      (1000) ysba      (1000)     1447 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/results.py
+-rw-r--r--   0 ysba      (1000) ysba      (1000)     4591 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/synth.py
+drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-19 01:19:27.045250 MAxPy-0.1.1/src/MAxPy/tcl/
+drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-19 01:19:27.051917 MAxPy-0.1.1/src/MAxPy/tcl/Genus/
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)     1006 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/tcl/Genus/constraints.sdc
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)     1083 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/tcl/Genus/qor_saif.tcl
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)      931 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/tcl/Genus/qor_sta.tcl
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)      149 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/tcl/Genus/sdf_cmd_file.base
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)     1545 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/tcl/Genus/sta.tcl
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)     1702 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/tcl/Genus/synth.tcl
+drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-19 01:19:27.051917 MAxPy-0.1.1/src/MAxPy/tcl/Incisive/
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)      116 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/tcl/Incisive/tcf_cmd.tcl
+drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-19 01:19:27.051917 MAxPy-0.1.1/src/MAxPy/tcl/OpenSTA/
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)      222 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/tcl/OpenSTA/cmd_file.sta
+drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-19 01:19:27.051917 MAxPy-0.1.1/src/MAxPy/tcl/Verilator/
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)      315 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/tcl/Verilator/verilator_config.vlt
+drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-19 01:19:27.051917 MAxPy-0.1.1/src/MAxPy/tcl/Yosys/
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)      226 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/tcl/Yosys/synth.ys
+drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-19 01:19:27.051917 MAxPy-0.1.1/src/MAxPy/templates/
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)      365 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/templates/cmake_pybind.txt
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)      172 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/templates/instance_source.cpp
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)     7606 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/templates/verilator_pybind_wrapper.cpp
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)     2702 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/templates/verilator_pybind_wrapper.h
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)     1649 2023-04-19 01:12:01.000000 MAxPy-0.1.1/src/MAxPy/utility.py
+-rw-r--r--   0 ysba      (1000) ysba      (1000)     2693 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/verilate.py
+drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-19 01:19:27.045250 MAxPy-0.1.1/src/MAxPy/vlib/
+drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-19 01:19:27.051917 MAxPy-0.1.1/src/MAxPy/vlib/AxArith/
+-rw-r--r--   0 ysba      (1000) ysba      (1000)      183 2023-04-19 01:13:40.000000 MAxPy-0.1.1/src/MAxPy/vlib/AxArith/README.md
+drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-19 01:19:27.051917 MAxPy-0.1.1/src/MAxPy/vlib/AxArith/adders/
+-rw-r--r--   0 ysba      (1000) ysba      (1000)      681 2023-04-19 01:13:40.000000 MAxPy-0.1.1/src/MAxPy/vlib/AxArith/adders/copy.v
+-rw-r--r--   0 ysba      (1000) ysba      (1000)      724 2023-04-19 01:13:40.000000 MAxPy-0.1.1/src/MAxPy/vlib/AxArith/adders/eta1.v
+-rw-r--r--   0 ysba      (1000) ysba      (1000)      359 2023-04-19 01:13:40.000000 MAxPy-0.1.1/src/MAxPy/vlib/AxArith/adders/loa.v
+-rw-r--r--   0 ysba      (1000) ysba      (1000)      716 2023-04-19 01:13:40.000000 MAxPy-0.1.1/src/MAxPy/vlib/AxArith/adders/trunc.v
+-rw-r--r--   0 ysba      (1000) ysba      (1000)    23679 2023-03-27 22:55:42.000000 MAxPy-0.1.1/src/MAxPy/wrapper.py
+drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-19 01:19:27.048583 MAxPy-0.1.1/src/MAxPy.egg-info/
+-rw-r--r--   0 ysba      (1000) ysba      (1000)     2316 2023-04-19 01:19:27.000000 MAxPy-0.1.1/src/MAxPy.egg-info/PKG-INFO
+-rw-r--r--   0 ysba      (1000) ysba      (1000)     1221 2023-04-19 01:19:27.000000 MAxPy-0.1.1/src/MAxPy.egg-info/SOURCES.txt
+-rw-r--r--   0 ysba      (1000) ysba      (1000)        1 2023-04-19 01:19:27.000000 MAxPy-0.1.1/src/MAxPy.egg-info/dependency_links.txt
+-rw-r--r--   0 ysba      (1000) ysba      (1000)        6 2023-04-19 01:19:27.000000 MAxPy-0.1.1/src/MAxPy.egg-info/top_level.txt
+drwxr-xr-x   0 ysba      (1000) ysba      (1000)        0 2023-04-19 01:19:27.051917 MAxPy-0.1.1/tests/
+-rwxr-xr-x   0 ysba      (1000) ysba      (1000)      990 2023-03-27 22:55:42.000000 MAxPy-0.1.1/tests/testbench.py
```

### Comparing `MAxPy-0.1.0/LICENSE` & `MAxPy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/PKG-INFO` & `MAxPy-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MAxPy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Multi-layer Approximate Computing Python Framework
 Home-page: https://maxpy-project.github.io/MAxPy/
 Author: Yuri Arbeletche <ysba000@gmail.com>, Guilherme Paim <gppaim@ieee.org>
 Project-URL: Bug Tracker, https://github.com/MAxPy-Project/MAxPy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MAxPy Version: 0.1.0 Summary: Multi-layer
+Metadata-Version: 2.1 Name: MAxPy Version: 0.1.1 Summary: Multi-layer
 Approximate Computing Python Framework Home-page: https://maxpy-
 project.github.io/MAxPy/ Author: Yuri Arbeletche
 gmail.com>, Guilherme Paim
 ieee.org> Project-URL: Bug Tracker, https://github.com/MAxPy-Project/MAxPy/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `MAxPy-0.1.0/README.md` & `MAxPy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/setup.cfg` & `MAxPy-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = MAxPy
-version = 0.1.0
+version = 0.1.1
 author = Yuri Arbeletche <ysba000@gmail.com>, Guilherme Paim <gppaim@ieee.org>
 description = Multi-layer Approximate Computing Python Framework
 long_description = file: README.md
 long_description_content = text/markdown
 long_description_content_type = text/markdown
 url = https://maxpy-project.github.io/MAxPy/
 project_urls =
```

### Comparing `MAxPy-0.1.0/src/MAxPy/check.py` & `MAxPy-0.1.1/src/MAxPy/check.py`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/compile.py` & `MAxPy-0.1.1/src/MAxPy/compile.py`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/estimations.py` & `MAxPy-0.1.1/src/MAxPy/estimations.py`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/maxpy.py` & `MAxPy-0.1.1/src/MAxPy/maxpy.py`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/pareto.py` & `MAxPy-0.1.1/src/MAxPy/pareto.py`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/pdk/NanGate15nm.lib` & `MAxPy-0.1.1/src/MAxPy/pdk/NanGate15nm.lib`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/pdk/NanGate15nm.v` & `MAxPy-0.1.1/src/MAxPy/pdk/NanGate15nm.v`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/probprun.py` & `MAxPy-0.1.1/src/MAxPy/probprun.py`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/resources.py` & `MAxPy-0.1.1/src/MAxPy/resources.py`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/results.py` & `MAxPy-0.1.1/src/MAxPy/results.py`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/synth.py` & `MAxPy-0.1.1/src/MAxPy/synth.py`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/tcl/Genus/constraints.sdc` & `MAxPy-0.1.1/src/MAxPy/tcl/Genus/constraints.sdc`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/tcl/Genus/qor_saif.tcl` & `MAxPy-0.1.1/src/MAxPy/tcl/Genus/qor_saif.tcl`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/tcl/Genus/qor_sta.tcl` & `MAxPy-0.1.1/src/MAxPy/tcl/Genus/qor_sta.tcl`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/tcl/Genus/sta.tcl` & `MAxPy-0.1.1/src/MAxPy/tcl/Genus/sta.tcl`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/tcl/Genus/synth.tcl` & `MAxPy-0.1.1/src/MAxPy/tcl/Genus/synth.tcl`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/templates/verilator_pybind_wrapper.cpp` & `MAxPy-0.1.1/src/MAxPy/templates/verilator_pybind_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/templates/verilator_pybind_wrapper.h` & `MAxPy-0.1.1/src/MAxPy/templates/verilator_pybind_wrapper.h`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/utility.py` & `MAxPy-0.1.1/src/MAxPy/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import enum
 import datetime
 
 
-version = '0.0.1'
+version = '0.1.1'
 
 
 class MainLoopFsm(enum.Enum):
 	INIT = enum.auto()
 	PREPARE_PATHS = enum.auto()
 	SYNTH = enum.auto()
 	VERI2C = enum.auto()
```

### Comparing `MAxPy-0.1.0/src/MAxPy/verilate.py` & `MAxPy-0.1.1/src/MAxPy/verilate.py`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy/wrapper.py` & `MAxPy-0.1.1/src/MAxPy/wrapper.py`

 * *Files identical despite different names*

### Comparing `MAxPy-0.1.0/src/MAxPy.egg-info/PKG-INFO` & `MAxPy-0.1.1/src/MAxPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MAxPy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Multi-layer Approximate Computing Python Framework
 Home-page: https://maxpy-project.github.io/MAxPy/
 Author: Yuri Arbeletche <ysba000@gmail.com>, Guilherme Paim <gppaim@ieee.org>
 Project-URL: Bug Tracker, https://github.com/MAxPy-Project/MAxPy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MAxPy Version: 0.1.0 Summary: Multi-layer
+Metadata-Version: 2.1 Name: MAxPy Version: 0.1.1 Summary: Multi-layer
 Approximate Computing Python Framework Home-page: https://maxpy-
 project.github.io/MAxPy/ Author: Yuri Arbeletche
 gmail.com>, Guilherme Paim
 ieee.org> Project-URL: Bug Tracker, https://github.com/MAxPy-Project/MAxPy/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
```

### Comparing `MAxPy-0.1.0/src/MAxPy.egg-info/SOURCES.txt` & `MAxPy-0.1.1/src/MAxPy.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -31,8 +31,13 @@
 src/MAxPy/tcl/OpenSTA/cmd_file.sta
 src/MAxPy/tcl/Verilator/verilator_config.vlt
 src/MAxPy/tcl/Yosys/synth.ys
 src/MAxPy/templates/cmake_pybind.txt
 src/MAxPy/templates/instance_source.cpp
 src/MAxPy/templates/verilator_pybind_wrapper.cpp
 src/MAxPy/templates/verilator_pybind_wrapper.h
+src/MAxPy/vlib/AxArith/README.md
+src/MAxPy/vlib/AxArith/adders/copy.v
+src/MAxPy/vlib/AxArith/adders/eta1.v
+src/MAxPy/vlib/AxArith/adders/loa.v
+src/MAxPy/vlib/AxArith/adders/trunc.v
 tests/testbench.py
```

### Comparing `MAxPy-0.1.0/tests/testbench.py` & `MAxPy-0.1.1/tests/testbench.py`

 * *Files identical despite different names*


# Comparing `tmp/ansys-meshing-prime-0.4.0.dev3.tar.gz` & `tmp/ansys-meshing-prime-0.4.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-meshing-prime-0.4.0.dev3.tar", last modified: Mon Feb 27 16:12:39 2023, max compression
+gzip compressed data, was "ansys-meshing-prime-0.4.0.dev6.tar", last modified: Wed Apr 19 19:50:42 2023, max compression
```

## Comparing `ansys-meshing-prime-0.4.0.dev3.tar` & `ansys-meshing-prime-0.4.0.dev6.tar`

### file list

```diff
@@ -1,109 +1,117 @@
--rw-r--r--   0        0        0     1090 2023-02-27 16:12:21.226009 ansys-meshing-prime-0.4.0.dev3/LICENSE
--rw-r--r--   0        0        0     2865 2023-02-27 16:12:21.226009 ansys-meshing-prime-0.4.0.dev3/README.md
--rw-r--r--   0        0        0     2054 2023-02-27 16:12:21.298011 ansys-meshing-prime-0.4.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     5451 2023-02-27 16:12:21.298011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/__init__.py
--rw-r--r--   0        0        0     2328 2023-02-27 16:12:21.298011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/automesh.py
--rw-r--r--   0        0        0    32375 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/automeshstructs.py
--rw-r--r--   0        0        0     5059 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py
--rw-r--r--   0        0        0     3038 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/collapsetool.py
--rw-r--r--   0        0        0    14701 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/collapsetoolstructs.py
--rw-r--r--   0        0        0    15524 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/commonstructs.py
--rw-r--r--   0        0        0     3875 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/commontypes.py
--rw-r--r--   0        0        0     9797 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/connect.py
--rw-r--r--   0        0        0    54150 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/connectstructs.py
--rw-r--r--   0        0        0     8792 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/controldata.py
--rw-r--r--   0        0        0    55335 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/controlstructs.py
--rw-r--r--   0        0        0      714 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/coreobject.py
--rw-r--r--   0        0        0     2922 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/deletetool.py
--rw-r--r--   0        0        0    13990 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/deletetoolstructs.py
--rw-r--r--   0        0        0     4502 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/featureextraction.py
--rw-r--r--   0        0        0    33896 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/featureextractionstructs.py
--rw-r--r--   0        0        0    18729 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/fileio.py
--rw-r--r--   0        0        0   109006 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/fileiostructs.py
--rw-r--r--   0        0        0    36760 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/igastructs.py
--rw-r--r--   0        0        0     3460 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/materialpointmanager.py
--rw-r--r--   0        0        0    16296 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py
--rw-r--r--   0        0        0     4164 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/meshinfo.py
--rw-r--r--   0        0        0    60035 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/meshinfostructs.py
--rw-r--r--   0        0        0    14200 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/model.py
--rw-r--r--   0        0        0    27227 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/modelstructs.py
--rw-r--r--   0        0        0    44837 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/part.py
--rw-r--r--   0        0        0   164498 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/partstructs.py
--rw-r--r--   0        0        0     6804 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/periodiccontrol.py
--rw-r--r--   0        0        0    13315 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py
--rw-r--r--   0        0        0    24366 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/primeconfig.py
--rw-r--r--   0        0        0     5167 2023-02-27 16:12:21.302011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/prismcontrol.py
--rw-r--r--   0        0        0    14563 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/prismcontrolstructs.py
--rw-r--r--   0        0        0     5904 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/scaffolder.py
--rw-r--r--   0        0        0    29265 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/scaffolderstructs.py
--rw-r--r--   0        0        0    16884 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/sizecontrol.py
--rw-r--r--   0        0        0    52720 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/sizecontrolstructs.py
--rw-r--r--   0        0        0     2375 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/sizefield.py
--rw-r--r--   0        0        0    18893 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/sizefieldstructs.py
--rw-r--r--   0        0        0     4241 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/splittoolstructs.py
--rw-r--r--   0        0        0    13393 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/surfacesearch.py
--rw-r--r--   0        0        0   106092 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/surfacesearchstructs.py
--rw-r--r--   0        0        0    15337 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/surfaceutilities.py
--rw-r--r--   0        0        0   139711 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py
--rw-r--r--   0        0        0     5852 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/surfer.py
--rw-r--r--   0        0        0    38754 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/surferstructs.py
--rw-r--r--   0        0        0     1157 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/thinvolumecontrol.py
--rw-r--r--   0        0        0     3245 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py
--rw-r--r--   0        0        0     2820 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/topodata.py
--rw-r--r--   0        0        0     2313 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/topoutilities.py
--rw-r--r--   0        0        0    13167 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/topoutilitystructs.py
--rw-r--r--   0        0        0     2495 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/transform.py
--rw-r--r--   0        0        0     8727 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/transformstructs.py
--rw-r--r--   0        0        0     5480 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/volumecontrol.py
--rw-r--r--   0        0        0     4712 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/volumecontrolstructs.py
--rw-r--r--   0        0        0     3929 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/volumemeshtool.py
--rw-r--r--   0        0        0    29508 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py
--rw-r--r--   0        0        0     2575 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/volumesearch.py
--rw-r--r--   0        0        0    25492 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/volumesearchstructs.py
--rw-r--r--   0        0        0     4438 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/wrapper.py
--rw-r--r--   0        0        0     9549 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/wrappercontrol.py
--rw-r--r--   0        0        0    61895 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/wrapperstructs.py
--rw-r--r--   0        0        0    11623 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/controldata.py
--rw-r--r--   0        0        0    16869 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/fileio.py
--rw-r--r--   0        0        0     9978 2023-02-27 16:12:21.306011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/model.py
--rw-r--r--   0        0        0     3982 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/part.py
--rw-r--r--   0        0        0     1761 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/periodiccontrol.py
--rw-r--r--   0        0        0     1676 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/sizecontrol.py
--rw-r--r--   0        0        0     3799 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/surfaceutilities.py
--rw-r--r--   0        0        0     4400 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/surfer.py
--rw-r--r--   0        0        0     1703 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/volumecontrol.py
--rw-r--r--   0        0        0     5692 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/wrapper.py
--rw-r--r--   0        0        0     1608 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/wrappercontrol.py
--rw-r--r--   0        0        0    14733 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/examples/__init__.py
--rw-r--r--   0        0        0     2049 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/examples/download.py
--rw-r--r--   0        0        0       59 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/graphics/__init__.py
--rw-r--r--   0        0        0    34726 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/graphics/graphics.py
--rw-r--r--   0        0        0     2234 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/graphics/images/bin.png
--rw-r--r--   0        0        0     1708 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/graphics/images/invert_visibility.png
--rw-r--r--   0        0        0     2510 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/graphics/images/parts.png
--rw-r--r--   0        0        0     1297 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/graphics/images/selectioninfo.png
--rw-r--r--   0        0        0     2440 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/graphics/images/show_edges.png
--rw-r--r--   0        0        0      203 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/graphics/images/show_ruler.png
--rw-r--r--   0        0        0     1547 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/graphics/images/surface_body.png
--rw-r--r--   0        0        0     4484 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/client.py
--rw-r--r--   0        0        0      238 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/comm_manager.py
--rw-r--r--   0        0        0      506 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/communicator.py
--rw-r--r--   0        0        0     2960 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/config.py
--rw-r--r--   0        0        0     3077 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/defaults.py
--rw-r--r--   0        0        0    30504 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/error_handling.py
--rw-r--r--   0        0        0     6130 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/grpc_communicator.py
--rw-r--r--   0        0        0      492 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/grpc_utils.py
--rw-r--r--   0        0        0     1444 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/json_utils.py
--rw-r--r--   0        0        0     8029 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/launcher.py
--rw-r--r--   0        0        0     1720 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/prime_communicator.py
--rw-r--r--   0        0        0     7634 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/utils.py
--rw-r--r--   0        0        0      143 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/lucid/__init__.py
--rw-r--r--   0        0        0    68592 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/lucid/mesh_util.py
--rw-r--r--   0        0        0     7399 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/lucid/scope.py
--rw-r--r--   0        0        0      991 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/lucid/utils.py
--rw-r--r--   0        0        0     1812 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/params/primestructs.py
--rw-r--r--   0        0        0     4345 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/relaxed_json/__init__.py
--rw-r--r--   0        0        0    10039 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/relaxed_json/decoder.py
--rw-r--r--   0        0        0    12256 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/relaxed_json/encoder.py
--rw-r--r--   0        0        0     2623 2023-02-27 16:12:21.310011 ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/relaxed_json/scanner.py
--rw-r--r--   0        0        0     4764 1970-01-01 00:00:00.000000 ansys-meshing-prime-0.4.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-19 19:50:28.381177 ansys-meshing-prime-0.4.0.dev6/LICENSE
+-rw-r--r--   0        0        0     2983 2023-04-19 19:50:28.381177 ansys-meshing-prime-0.4.0.dev6/README.md
+-rw-r--r--   0        0        0     2054 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0     6098 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/__init__.py
+-rw-r--r--   0        0        0     2650 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/automesh.py
+-rw-r--r--   0        0        0    59522 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/automeshstructs.py
+-rw-r--r--   0        0        0     6111 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py
+-rw-r--r--   0        0        0     3847 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/collapsetool.py
+-rw-r--r--   0        0        0    14701 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/collapsetoolstructs.py
+-rw-r--r--   0        0        0    15524 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/commonstructs.py
+-rw-r--r--   0        0        0     3875 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/commontypes.py
+-rw-r--r--   0        0        0    12295 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/connect.py
+-rw-r--r--   0        0        0    54150 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/connectstructs.py
+-rw-r--r--   0        0        0    10456 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/controldata.py
+-rw-r--r--   0        0        0    55335 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/controlstructs.py
+-rw-r--r--   0        0        0      714 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/coreobject.py
+-rw-r--r--   0        0        0     3427 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/deletetool.py
+-rw-r--r--   0        0        0    13990 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/deletetoolstructs.py
+-rw-r--r--   0        0        0     5573 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/featureextraction.py
+-rw-r--r--   0        0        0    33896 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/featureextractionstructs.py
+-rw-r--r--   0        0        0    29402 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/fileio.py
+-rw-r--r--   0        0        0   126575 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/fileiostructs.py
+-rw-r--r--   0        0        0    60431 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/igastructs.py
+-rw-r--r--   0        0        0     4093 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/materialpointmanager.py
+-rw-r--r--   0        0        0    16296 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py
+-rw-r--r--   0        0        0     4858 2023-04-19 19:50:28.441179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/meshinfo.py
+-rw-r--r--   0        0        0    60035 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/meshinfostructs.py
+-rw-r--r--   0        0        0    16491 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/model.py
+-rw-r--r--   0        0        0    27227 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/modelstructs.py
+-rw-r--r--   0        0        0     3793 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/morpher.py
+-rw-r--r--   0        0        0     7831 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/morpherbcsstructs.py
+-rw-r--r--   0        0        0    25161 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/morpherstructs.py
+-rw-r--r--   0        0        0    58131 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/part.py
+-rw-r--r--   0        0        0   167481 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/partstructs.py
+-rw-r--r--   0        0        0     7502 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/periodiccontrol.py
+-rw-r--r--   0        0        0    13315 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py
+-rw-r--r--   0        0        0    27640 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/primeconfig.py
+-rw-r--r--   0        0        0     5727 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/prismcontrol.py
+-rw-r--r--   0        0        0    14563 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/prismcontrolstructs.py
+-rw-r--r--   0        0        0     3773 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/quadtospline.py
+-rw-r--r--   0        0        0     7237 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/scaffolder.py
+-rw-r--r--   0        0        0    29265 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/scaffolderstructs.py
+-rw-r--r--   0        0        0    18382 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/sizecontrol.py
+-rw-r--r--   0        0        0    52720 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/sizecontrolstructs.py
+-rw-r--r--   0        0        0     2790 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/sizefield.py
+-rw-r--r--   0        0        0    18893 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/sizefieldstructs.py
+-rw-r--r--   0        0        0     4241 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/splittoolstructs.py
+-rw-r--r--   0        0        0    19710 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfacesearch.py
+-rw-r--r--   0        0        0   117867 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfacesearchstructs.py
+-rw-r--r--   0        0        0    22036 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfaceutilities.py
+-rw-r--r--   0        0        0   144419 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py
+-rw-r--r--   0        0        0     7182 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfer.py
+-rw-r--r--   0        0        0    42738 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surferstructs.py
+-rw-r--r--   0        0        0     4432 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/thinvolumecontrol.py
+-rw-r--r--   0        0        0     6689 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/thinvolumecontrolstructs.py
+-rw-r--r--   0        0        0     8477 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/topodata.py
+-rw-r--r--   0        0        0     2646 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/topoutilities.py
+-rw-r--r--   0        0        0    13167 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/topoutilitystructs.py
+-rw-r--r--   0        0        0     2960 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/transform.py
+-rw-r--r--   0        0        0     8727 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/transformstructs.py
+-rw-r--r--   0        0        0     5980 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumecontrol.py
+-rw-r--r--   0        0        0     6259 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumecontrolstructs.py
+-rw-r--r--   0        0        0     4893 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumemeshtool.py
+-rw-r--r--   0        0        0    29508 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py
+-rw-r--r--   0        0        0     2761 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumesearch.py
+-rw-r--r--   0        0        0    25492 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumesearchstructs.py
+-rw-r--r--   0        0        0     4886 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumesweeper.py
+-rw-r--r--   0        0        0    25535 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumesweeperstructs.py
+-rw-r--r--   0        0        0     5426 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/wrapper.py
+-rw-r--r--   0        0        0    10816 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/wrappercontrol.py
+-rw-r--r--   0        0        0    61895 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/wrapperstructs.py
+-rw-r--r--   0        0        0    13848 2023-04-19 19:50:28.445179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/controldata.py
+-rw-r--r--   0        0        0    17032 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/fileio.py
+-rw-r--r--   0        0        0    10734 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/model.py
+-rw-r--r--   0        0        0     4207 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/part.py
+-rw-r--r--   0        0        0     2314 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/periodiccontrol.py
+-rw-r--r--   0        0        0     2193 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/sizecontrol.py
+-rw-r--r--   0        0        0     4091 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/surfaceutilities.py
+-rw-r--r--   0        0        0     4400 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/surfer.py
+-rw-r--r--   0        0        0     2308 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/volumecontrol.py
+-rw-r--r--   0        0        0     2823 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/volumesweeper.py
+-rw-r--r--   0        0        0     5692 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/wrapper.py
+-rw-r--r--   0        0        0     2141 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/wrappercontrol.py
+-rw-r--r--   0        0        0      347 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/examples/__init__.py
+-rw-r--r--   0        0        0     2049 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/examples/download_utilities.py
+-rw-r--r--   0        0        0    15180 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/examples/examples.py
+-rw-r--r--   0        0        0       59 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/__init__.py
+-rw-r--r--   0        0        0    34726 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/graphics.py
+-rw-r--r--   0        0        0     2234 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/bin.png
+-rw-r--r--   0        0        0     1708 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/invert_visibility.png
+-rw-r--r--   0        0        0     2510 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/parts.png
+-rw-r--r--   0        0        0     1297 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/selectioninfo.png
+-rw-r--r--   0        0        0     2440 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/show_edges.png
+-rw-r--r--   0        0        0      203 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/show_ruler.png
+-rw-r--r--   0        0        0     1547 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/surface_body.png
+-rw-r--r--   0        0        0     4484 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/client.py
+-rw-r--r--   0        0        0      238 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/comm_manager.py
+-rw-r--r--   0        0        0      506 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/communicator.py
+-rw-r--r--   0        0        0     2960 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/config.py
+-rw-r--r--   0        0        0     3077 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/defaults.py
+-rw-r--r--   0        0        0    33288 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/error_handling.py
+-rw-r--r--   0        0        0     6130 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/grpc_communicator.py
+-rw-r--r--   0        0        0      492 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/grpc_utils.py
+-rw-r--r--   0        0        0     1444 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/json_utils.py
+-rw-r--r--   0        0        0     8029 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/launcher.py
+-rw-r--r--   0        0        0     1720 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/prime_communicator.py
+-rw-r--r--   0        0        0     7634 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/utils.py
+-rw-r--r--   0        0        0      143 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/lucid/__init__.py
+-rw-r--r--   0        0        0    68592 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/lucid/mesh_util.py
+-rw-r--r--   0        0        0     7399 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/lucid/scope.py
+-rw-r--r--   0        0        0     1649 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/lucid/utils.py
+-rw-r--r--   0        0        0     2059 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/params/primestructs.py
+-rw-r--r--   0        0        0     4345 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/relaxed_json/__init__.py
+-rw-r--r--   0        0        0    10039 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/relaxed_json/decoder.py
+-rw-r--r--   0        0        0    12256 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/relaxed_json/encoder.py
+-rw-r--r--   0        0        0     2623 2023-04-19 19:50:28.449179 ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/relaxed_json/scanner.py
+-rw-r--r--   0        0        0     4882 1970-01-01 00:00:00.000000 ansys-meshing-prime-0.4.0.dev6/PKG-INFO
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/LICENSE` & `ansys-meshing-prime-0.4.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/README.md` & `ansys-meshing-prime-0.4.0.dev6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 ```bash
 pip install -e .
 ```
 
 ## Dependencies
 
-You must have a licensed copy of the latest version of Ansys 2023 R1 locally.
+You must have Ansys 2023 R1 or newer versions installed for Ansys Prime Server (optionally, CAD readers can be configured).  Ansys Prime Server requires a Preppost or CFD Preppost license to run.
 
 ## Get Started
 
 ### Launching PyPrimeMesh
 
 To launch PyPrimeMesh:
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/pyproject.toml` & `ansys-meshing-prime-0.4.0.dev6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-meshing-prime"
-version = "0.4.0.dev3"
+version = "0.4.0.dev6"
 description = "PyPrimeMesh provides a python client to Ansys Prime Server. Ansys Prime Server delivers core Ansys meshing technology."
 readme = "README.md"
 requires-python = ">=3.7,<4"
 license = {file = "LICENSE"}
 authors = [{name = "ANSYS, Inc.", email = "pyansys.support@ansys.com"}]
 maintainers = [{name = "PyAnsys developers", email = "pyansys.maintainers@ansys.com"}]
 classifiers = [
@@ -30,26 +30,26 @@
 ]
 
 [project.optional-dependencies]
 graphics = [
   "pyvista>=0.32.0",
 ]
 tests = [
-  "pytest==7.2.1",
+  "pytest==7.3.1",
   "pytest-cov==4.0.0",
 ]
 doc = [
-  "ansys-sphinx-theme==0.9.3",
+  "ansys-sphinx-theme==0.9.7",
   "jupyter-sphinx==0.4.0",
   "numpydoc==1.5.0",
-  "pyvista==0.38.2",
+  "pyvista==0.38.5",
   "Sphinx==5.3.0",
   "sphinx-autodoc-typehints==1.22",
   "sphinx-copybutton==0.5.1",
-  "sphinx-gallery==0.11.1",
+  "sphinx-gallery==0.12.2",
   "sphinx-notfound-page==0.8.3",
   "sphinxemoji==0.2.0",
 ]
 all = [
   "pyvista>=0.32.0",
 ]
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/__init__.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 '''PyPrimeMesh Client library
 '''
 # isort: skip_file
 from ansys.meshing.prime.core.model import Model
 from ansys.meshing.prime.core.part import Part
 from ansys.meshing.prime.core.fileio import FileIO
 from ansys.meshing.prime.core.surfer import Surfer
+from ansys.meshing.prime.core.volumesweeper import VolumeSweeper
 from ansys.meshing.prime.autogen.surfacesearch import SurfaceSearch
 from ansys.meshing.prime.autogen.volumesearch import VolumeSearch
 from ansys.meshing.prime.core.wrappercontrol import WrapperControl
 from ansys.meshing.prime.core.controldata import ControlData
 from ansys.meshing.prime.core.wrapper import Wrapper
 from ansys.meshing.prime.core.surfaceutilities import SurfaceUtilities
 from ansys.meshing.prime.core.sizecontrol import SizeControl
 from ansys.meshing.prime.core.volumecontrol import VolumeControl
 
 from ansys.meshing.prime.autogen.surfaceutilitystructs import *
 from ansys.meshing.prime.autogen.wrapperstructs import *
 from ansys.meshing.prime.autogen.scaffolder import Scaffolder
 from ansys.meshing.prime.autogen.automesh import AutoMesh
 from ansys.meshing.prime.autogen.boundaryfittednurbs import BoundaryFittedSpline
+from ansys.meshing.prime.autogen.quadtospline import QuadToSpline
 from ansys.meshing.prime.autogen.sizefield import SizeField
 from ansys.meshing.prime.autogen.meshinfo import MeshInfo
 from ansys.meshing.prime.autogen.transform import Transform
 from ansys.meshing.prime.autogen.connect import Connect
 from ansys.meshing.prime.autogen.deletetool import DeleteTool
 from ansys.meshing.prime.autogen.collapsetool import CollapseTool
 from ansys.meshing.prime.autogen.volumemeshtool import VolumeMeshTool
 from ansys.meshing.prime.autogen.topoutilities import TopoUtilities
+from ansys.meshing.prime.autogen.morpher import Morpher
 from ansys.meshing.prime.autogen.commontypes import *
 from ansys.meshing.prime.autogen.commonstructs import *
 from ansys.meshing.prime.autogen.modelstructs import *
 from ansys.meshing.prime.autogen.fileiostructs import *
 from ansys.meshing.prime.autogen.partstructs import *
 from ansys.meshing.prime.autogen.surferstructs import *
 from ansys.meshing.prime.autogen.scaffolderstructs import *
@@ -42,25 +45,32 @@
 from ansys.meshing.prime.autogen.materialpointmanager import MaterialPointManager
 from ansys.meshing.prime.autogen.controlstructs import *
 from ansys.meshing.prime.autogen.sizecontrolstructs import *
 from ansys.meshing.prime.autogen.sizefieldstructs import *
 from ansys.meshing.prime.autogen.meshinfostructs import *
 from ansys.meshing.prime.autogen.prismcontrolstructs import *
 from ansys.meshing.prime.autogen.prismcontrol import PrismControl
+from ansys.meshing.prime.autogen.thinvolumecontrol import ThinVolumeControl
 from ansys.meshing.prime.autogen.connectstructs import *
 from ansys.meshing.prime.autogen.surfaceutilitystructs import *
 from ansys.meshing.prime.autogen.transformstructs import *
 from ansys.meshing.prime.autogen.deletetoolstructs import *
 from ansys.meshing.prime.autogen.splittoolstructs import *
 from ansys.meshing.prime.autogen.collapsetoolstructs import *
 from ansys.meshing.prime.autogen.volumecontrolstructs import *
+from ansys.meshing.prime.autogen.periodiccontrol import PeriodicControl
+from ansys.meshing.prime.autogen.periodiccontrolstructs import *
 from ansys.meshing.prime.autogen.featureextractionstructs import *
 from ansys.meshing.prime.autogen.featureextraction import *
+from ansys.meshing.prime.autogen.thinvolumecontrolstructs import *
 from ansys.meshing.prime.autogen.volumemeshtoolstructs import *
+from ansys.meshing.prime.autogen.volumesweeperstructs import *
 from ansys.meshing.prime.autogen.topoutilitystructs import *
+from ansys.meshing.prime.autogen.morpherstructs import *
+from ansys.meshing.prime.autogen.morpherbcsstructs import *
 
 from ansys.meshing.prime.internals.error_handling import PrimeRuntimeError, PrimeRuntimeWarning
 from ansys.meshing.prime.internals.client import Client
 from ansys.meshing.prime.internals.launcher import *
 from ansys.meshing.prime.internals.config import (
     is_optimizing_numpy_arrays,
     enable_optimizing_numpy_arrays,
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/automeshstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/featureextractionstructs.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,729 +4,741 @@
 from ansys.meshing.prime.internals.comm_manager import CommunicationManager
 from ansys.meshing.prime.internals import utils
 from ansys.meshing.prime.autogen.coreobject import *
 import numpy as np
 
 from ansys.meshing.prime.params.primestructs import *
 
-class VolumeFillType(enum.IntEnum):
-    """Types of volume fill options.
-    """
-    TET = 0
-    """Volume fill using tetrahedral cells."""
-    POLY = 1
-    """Volume fill using polyhedral cells."""
-    HEXCORETET = 2
-    """Volume fill using hexahedral cells in the core and tetrahedral cells near the boundary."""
-    HEXCOREPOLY = 3
-    """Volume fill using hexahedral cells in the core and polyhedral cells near the boundary."""
-
-class AutoMeshResults(CoreObject):
-    """Results of volume meshing.
+class ExtractFeatureParams(CoreObject):
+    """Parameter to control feature edge extraction.
     """
     _default_params = {}
 
     def __initialize(
             self,
-            error_code: ErrorCode,
-            warning_codes: List[WarningCode],
-            error_locations: Iterable[float]):
-        self._error_code = ErrorCode(error_code)
-        self._warning_codes = warning_codes
-        self._error_locations = error_locations if isinstance(error_locations, np.ndarray) else np.array(error_locations, dtype=np.double) if error_locations is not None else None
+            replace: bool,
+            feature_angle: float,
+            separate_features: bool,
+            separation_angle: float,
+            disconnect_with_faces: bool,
+            label_name: str):
+        self._replace = replace
+        self._feature_angle = feature_angle
+        self._separate_features = separate_features
+        self._separation_angle = separation_angle
+        self._disconnect_with_faces = disconnect_with_faces
+        self._label_name = label_name
 
     def __init__(
             self,
             model: CommunicationManager=None,
-            error_code: ErrorCode = None,
-            warning_codes: List[WarningCode] = None,
-            error_locations: Iterable[float] = None,
+            replace: bool = None,
+            feature_angle: float = None,
+            separate_features: bool = None,
+            separation_angle: float = None,
+            disconnect_with_faces: bool = None,
+            label_name: str = None,
             json_data : dict = None,
              **kwargs):
-        """Initializes the AutoMeshResults.
+        """Initializes the ExtractFeatureParams.
 
         Parameters
         ----------
         model: Model
-            Model to create a AutoMeshResults object with default parameters.
-        error_code: ErrorCode, optional
-            Provides error message when automesh fails.
-        warning_codes: List[WarningCode], optional
-            Warning codes associated with the operation.
-        error_locations: Iterable[float], optional
-            Error location coordinates returned when automesh fails.
+            Model to create a ExtractFeatureParams object with default parameters.
+        replace: bool, optional
+            Option to replace existing edge zonelets with new extracted edge zonelets.
+        feature_angle: float, optional
+            Angle used to capture face features to be  extracted as edges.
+        separate_features: bool, optional
+            Option to separate extracted features.
+        separation_angle: float, optional
+            Angle used to separate extracted features.
+        disconnect_with_faces: bool, optional
+            Option to disconnect edges from faces. If false, edges remain connected to faces by sharing nodes.
+        label_name: str, optional
+            Label name to be assigned to extracted features.
         json_data: dict, optional
-            JSON dictionary to create a AutoMeshResults object with provided parameters.
+            JSON dictionary to create a ExtractFeatureParams object with provided parameters.
 
         Examples
         --------
-        >>> auto_mesh_results = prime.AutoMeshResults(model = model)
+        >>> extract_feature_params = prime.ExtractFeatureParams(model = model)
         """
         if json_data:
             self.__initialize(
-                ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None),
-                [WarningCode(data) for data in json_data["warningCodes"]] if "warningCodes" in json_data else None,
-                json_data["errorLocations"] if "errorLocations" in json_data else None)
+                json_data["replace"] if "replace" in json_data else None,
+                json_data["featureAngle"] if "featureAngle" in json_data else None,
+                json_data["separateFeatures"] if "separateFeatures" in json_data else None,
+                json_data["separationAngle"] if "separationAngle" in json_data else None,
+                json_data["disconnectWithFaces"] if "disconnectWithFaces" in json_data else None,
+                json_data["labelName"] if "labelName" in json_data else None)
         else:
-            all_field_specified = all(arg is not None for arg in [error_code, warning_codes, error_locations])
+            all_field_specified = all(arg is not None for arg in [replace, feature_angle, separate_features, separation_angle, disconnect_with_faces, label_name])
             if all_field_specified:
                 self.__initialize(
-                    error_code,
-                    warning_codes,
-                    error_locations)
+                    replace,
+                    feature_angle,
+                    separate_features,
+                    separation_angle,
+                    disconnect_with_faces,
+                    label_name)
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
-                    param_json = model._communicator.initialize_params(model, "AutoMeshResults")
-                    json_data = param_json["AutoMeshResults"] if "AutoMeshResults" in param_json else {}
+                    param_json = model._communicator.initialize_params(model, "ExtractFeatureParams")
+                    json_data = param_json["ExtractFeatureParams"] if "ExtractFeatureParams" in param_json else {}
                     self.__initialize(
-                        error_code if error_code is not None else ( AutoMeshResults._default_params["error_code"] if "error_code" in AutoMeshResults._default_params else ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None)),
-                        warning_codes if warning_codes is not None else ( AutoMeshResults._default_params["warning_codes"] if "warning_codes" in AutoMeshResults._default_params else [WarningCode(data) for data in (json_data["warningCodes"] if "warningCodes" in json_data else None)]),
-                        error_locations if error_locations is not None else ( AutoMeshResults._default_params["error_locations"] if "error_locations" in AutoMeshResults._default_params else (json_data["errorLocations"] if "errorLocations" in json_data else None)))
+                        replace if replace is not None else ( ExtractFeatureParams._default_params["replace"] if "replace" in ExtractFeatureParams._default_params else (json_data["replace"] if "replace" in json_data else None)),
+                        feature_angle if feature_angle is not None else ( ExtractFeatureParams._default_params["feature_angle"] if "feature_angle" in ExtractFeatureParams._default_params else (json_data["featureAngle"] if "featureAngle" in json_data else None)),
+                        separate_features if separate_features is not None else ( ExtractFeatureParams._default_params["separate_features"] if "separate_features" in ExtractFeatureParams._default_params else (json_data["separateFeatures"] if "separateFeatures" in json_data else None)),
+                        separation_angle if separation_angle is not None else ( ExtractFeatureParams._default_params["separation_angle"] if "separation_angle" in ExtractFeatureParams._default_params else (json_data["separationAngle"] if "separationAngle" in json_data else None)),
+                        disconnect_with_faces if disconnect_with_faces is not None else ( ExtractFeatureParams._default_params["disconnect_with_faces"] if "disconnect_with_faces" in ExtractFeatureParams._default_params else (json_data["disconnectWithFaces"] if "disconnectWithFaces" in json_data else None)),
+                        label_name if label_name is not None else ( ExtractFeatureParams._default_params["label_name"] if "label_name" in ExtractFeatureParams._default_params else (json_data["labelName"] if "labelName" in json_data else None)))
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
     def set_default(
-            error_code: ErrorCode = None,
-            warning_codes: List[WarningCode] = None,
-            error_locations: Iterable[float] = None):
-        """Set the default values of AutoMeshResults.
+            replace: bool = None,
+            feature_angle: float = None,
+            separate_features: bool = None,
+            separation_angle: float = None,
+            disconnect_with_faces: bool = None,
+            label_name: str = None):
+        """Set the default values of ExtractFeatureParams.
 
         Parameters
         ----------
-        error_code: ErrorCode, optional
-            Provides error message when automesh fails.
-        warning_codes: List[WarningCode], optional
-            Warning codes associated with the operation.
-        error_locations: Iterable[float], optional
-            Error location coordinates returned when automesh fails.
+        replace: bool, optional
+            Option to replace existing edge zonelets with new extracted edge zonelets.
+        feature_angle: float, optional
+            Angle used to capture face features to be  extracted as edges.
+        separate_features: bool, optional
+            Option to separate extracted features.
+        separation_angle: float, optional
+            Angle used to separate extracted features.
+        disconnect_with_faces: bool, optional
+            Option to disconnect edges from faces. If false, edges remain connected to faces by sharing nodes.
+        label_name: str, optional
+            Label name to be assigned to extracted features.
         """
         args = locals()
-        [AutoMeshResults._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+        [ExtractFeatureParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
     def print_default():
-        """Print the default values of AutoMeshResults.
+        """Print the default values of ExtractFeatureParams.
 
         Examples
         --------
-        >>> AutoMeshResults.print_default()
+        >>> ExtractFeatureParams.print_default()
         """
         message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in AutoMeshResults._default_params.items())
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in ExtractFeatureParams._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
-        if self._error_code is not None:
-            json_data["errorCode"] = self._error_code
-        if self._warning_codes is not None:
-            json_data["warningCodes"] = [data for data in self._warning_codes]
-        if self._error_locations is not None:
-            json_data["errorLocations"] = self._error_locations
+        if self._replace is not None:
+            json_data["replace"] = self._replace
+        if self._feature_angle is not None:
+            json_data["featureAngle"] = self._feature_angle
+        if self._separate_features is not None:
+            json_data["separateFeatures"] = self._separate_features
+        if self._separation_angle is not None:
+            json_data["separationAngle"] = self._separation_angle
+        if self._disconnect_with_faces is not None:
+            json_data["disconnectWithFaces"] = self._disconnect_with_faces
+        if self._label_name is not None:
+            json_data["labelName"] = self._label_name
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "error_code :  %s\nwarning_codes :  %s\nerror_locations :  %s" % (self._error_code, '[' + ''.join('\n' + str(data) for data in self._warning_codes) + ']', self._error_locations)
+        message = "replace :  %s\nfeature_angle :  %s\nseparate_features :  %s\nseparation_angle :  %s\ndisconnect_with_faces :  %s\nlabel_name :  %s" % (self._replace, self._feature_angle, self._separate_features, self._separation_angle, self._disconnect_with_faces, self._label_name)
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
     @property
-    def error_code(self) -> ErrorCode:
-        """Provides error message when automesh fails.
+    def replace(self) -> bool:
+        """Option to replace existing edge zonelets with new extracted edge zonelets.
         """
-        return self._error_code
+        return self._replace
 
-    @error_code.setter
-    def error_code(self, value: ErrorCode):
-        self._error_code = value
+    @replace.setter
+    def replace(self, value: bool):
+        self._replace = value
+
+    @property
+    def feature_angle(self) -> float:
+        """Angle used to capture face features to be  extracted as edges.
+        """
+        return self._feature_angle
+
+    @feature_angle.setter
+    def feature_angle(self, value: float):
+        self._feature_angle = value
+
+    @property
+    def separate_features(self) -> bool:
+        """Option to separate extracted features.
+        """
+        return self._separate_features
+
+    @separate_features.setter
+    def separate_features(self, value: bool):
+        self._separate_features = value
 
     @property
-    def warning_codes(self) -> List[WarningCode]:
-        """Warning codes associated with the operation.
+    def separation_angle(self) -> float:
+        """Angle used to separate extracted features.
         """
-        return self._warning_codes
+        return self._separation_angle
 
-    @warning_codes.setter
-    def warning_codes(self, value: List[WarningCode]):
-        self._warning_codes = value
+    @separation_angle.setter
+    def separation_angle(self, value: float):
+        self._separation_angle = value
 
     @property
-    def error_locations(self) -> Iterable[float]:
-        """Error location coordinates returned when automesh fails.
+    def disconnect_with_faces(self) -> bool:
+        """Option to disconnect edges from faces. If false, edges remain connected to faces by sharing nodes.
         """
-        return self._error_locations
+        return self._disconnect_with_faces
 
-    @error_locations.setter
-    def error_locations(self, value: Iterable[float]):
-        self._error_locations = value
+    @disconnect_with_faces.setter
+    def disconnect_with_faces(self, value: bool):
+        self._disconnect_with_faces = value
 
-class PrismStairStep(CoreObject):
-    """Parameters to control prism stairsteping.
+    @property
+    def label_name(self) -> str:
+        """Label name to be assigned to extracted features.
+        """
+        return self._label_name
+
+    @label_name.setter
+    def label_name(self, value: str):
+        self._label_name = value
+
+class ExtractFeatureResults(CoreObject):
+    """Result of edge zonelet extraction by angle.
     """
     _default_params = {}
 
     def __initialize(
-            self):
-        pass
+            self,
+            processing_time: float,
+            error_code: ErrorCode,
+            new_edge_zonelets: Iterable[int]):
+        self._processing_time = processing_time
+        self._error_code = ErrorCode(error_code)
+        self._new_edge_zonelets = new_edge_zonelets if isinstance(new_edge_zonelets, np.ndarray) else np.array(new_edge_zonelets, dtype=np.int32) if new_edge_zonelets is not None else None
 
     def __init__(
             self,
             model: CommunicationManager=None,
+            processing_time: float = None,
+            error_code: ErrorCode = None,
+            new_edge_zonelets: Iterable[int] = None,
             json_data : dict = None,
              **kwargs):
-        """Initializes the PrismStairStep.
+        """Initializes the ExtractFeatureResults.
 
         Parameters
         ----------
         model: Model
-            Model to create a PrismStairStep object with default parameters.
+            Model to create a ExtractFeatureResults object with default parameters.
+        processing_time: float, optional
+            Time taken for edge extraction.
+        error_code: ErrorCode, optional
+            Error code returned by edge extraction function.
+        new_edge_zonelets: Iterable[int], optional
+            Ids of new edge zonelets extracted.
         json_data: dict, optional
-            JSON dictionary to create a PrismStairStep object with provided parameters.
+            JSON dictionary to create a ExtractFeatureResults object with provided parameters.
 
         Examples
         --------
-        >>> prism_stair_step = prime.PrismStairStep(model = model)
+        >>> extract_feature_results = prime.ExtractFeatureResults(model = model)
         """
         if json_data:
-            self.__initialize()
+            self.__initialize(
+                json_data["processingTime"] if "processingTime" in json_data else None,
+                ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None),
+                json_data["newEdgeZonelets"] if "newEdgeZonelets" in json_data else None)
         else:
-            all_field_specified = all(arg is not None for arg in [])
+            all_field_specified = all(arg is not None for arg in [processing_time, error_code, new_edge_zonelets])
             if all_field_specified:
-                self.__initialize()
+                self.__initialize(
+                    processing_time,
+                    error_code,
+                    new_edge_zonelets)
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
-                    param_json = model._communicator.initialize_params(model, "PrismStairStep")
-                    json_data = param_json["PrismStairStep"] if "PrismStairStep" in param_json else {}
-                    self.__initialize()
+                    param_json = model._communicator.initialize_params(model, "ExtractFeatureResults")
+                    json_data = param_json["ExtractFeatureResults"] if "ExtractFeatureResults" in param_json else {}
+                    self.__initialize(
+                        processing_time if processing_time is not None else ( ExtractFeatureResults._default_params["processing_time"] if "processing_time" in ExtractFeatureResults._default_params else (json_data["processingTime"] if "processingTime" in json_data else None)),
+                        error_code if error_code is not None else ( ExtractFeatureResults._default_params["error_code"] if "error_code" in ExtractFeatureResults._default_params else ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None)),
+                        new_edge_zonelets if new_edge_zonelets is not None else ( ExtractFeatureResults._default_params["new_edge_zonelets"] if "new_edge_zonelets" in ExtractFeatureResults._default_params else (json_data["newEdgeZonelets"] if "newEdgeZonelets" in json_data else None)))
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
-    def set_default():
-        """Set the default values of PrismStairStep.
+    def set_default(
+            processing_time: float = None,
+            error_code: ErrorCode = None,
+            new_edge_zonelets: Iterable[int] = None):
+        """Set the default values of ExtractFeatureResults.
 
+        Parameters
+        ----------
+        processing_time: float, optional
+            Time taken for edge extraction.
+        error_code: ErrorCode, optional
+            Error code returned by edge extraction function.
+        new_edge_zonelets: Iterable[int], optional
+            Ids of new edge zonelets extracted.
         """
         args = locals()
-        [PrismStairStep._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+        [ExtractFeatureResults._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
     def print_default():
-        """Print the default values of PrismStairStep.
+        """Print the default values of ExtractFeatureResults.
 
         Examples
         --------
-        >>> PrismStairStep.print_default()
+        >>> ExtractFeatureResults.print_default()
         """
         message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in PrismStairStep._default_params.items())
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in ExtractFeatureResults._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
+        if self._processing_time is not None:
+            json_data["processingTime"] = self._processing_time
+        if self._error_code is not None:
+            json_data["errorCode"] = self._error_code
+        if self._new_edge_zonelets is not None:
+            json_data["newEdgeZonelets"] = self._new_edge_zonelets
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "" % ()
+        message = "processing_time :  %s\nerror_code :  %s\nnew_edge_zonelets :  %s" % (self._processing_time, self._error_code, self._new_edge_zonelets)
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
-class PrismParams(CoreObject):
-    """Parameters to control prism mesh generation.
+    @property
+    def processing_time(self) -> float:
+        """Time taken for edge extraction.
+        """
+        return self._processing_time
+
+    @processing_time.setter
+    def processing_time(self, value: float):
+        self._processing_time = value
+
+    @property
+    def error_code(self) -> ErrorCode:
+        """Error code returned by edge extraction function.
+        """
+        return self._error_code
+
+    @error_code.setter
+    def error_code(self, value: ErrorCode):
+        self._error_code = value
+
+    @property
+    def new_edge_zonelets(self) -> Iterable[int]:
+        """Ids of new edge zonelets extracted.
+        """
+        return self._new_edge_zonelets
+
+    @new_edge_zonelets.setter
+    def new_edge_zonelets(self, value: Iterable[int]):
+        self._new_edge_zonelets = value
+
+class ExtractedFeatureIds(CoreObject):
+    """Contains ids of the features extracted.
     """
     _default_params = {}
 
     def __initialize(
             self,
-            stair_step: PrismStairStep,
-            no_imprint_zonelets: Iterable[int]):
-        self._stair_step = stair_step
-        self._no_imprint_zonelets = no_imprint_zonelets if isinstance(no_imprint_zonelets, np.ndarray) else np.array(no_imprint_zonelets, dtype=np.int32) if no_imprint_zonelets is not None else None
+            part_id: int,
+            new_edge_zonelets: Iterable[int]):
+        self._part_id = part_id
+        self._new_edge_zonelets = new_edge_zonelets if isinstance(new_edge_zonelets, np.ndarray) else np.array(new_edge_zonelets, dtype=np.int32) if new_edge_zonelets is not None else None
 
     def __init__(
             self,
             model: CommunicationManager=None,
-            stair_step: PrismStairStep = None,
-            no_imprint_zonelets: Iterable[int] = None,
+            part_id: int = None,
+            new_edge_zonelets: Iterable[int] = None,
             json_data : dict = None,
              **kwargs):
-        """Initializes the PrismParams.
+        """Initializes the ExtractedFeatureIds.
 
         Parameters
         ----------
         model: Model
-            Model to create a PrismParams object with default parameters.
-        stair_step: PrismStairStep, optional
-            Prism stairstep parameters.
-        no_imprint_zonelets: Iterable[int], optional
-            Option to specify zonelets to skip prism imprint.
+            Model to create a ExtractedFeatureIds object with default parameters.
+        part_id: int, optional
+            Id of the part from which edge zonelets are extracted.
+        new_edge_zonelets: Iterable[int], optional
+            Ids of new edge zonelets extracted.
         json_data: dict, optional
-            JSON dictionary to create a PrismParams object with provided parameters.
+            JSON dictionary to create a ExtractedFeatureIds object with provided parameters.
 
         Examples
         --------
-        >>> prism_params = prime.PrismParams(model = model)
+        >>> extracted_feature_ids = prime.ExtractedFeatureIds(model = model)
         """
         if json_data:
             self.__initialize(
-                PrismStairStep(model = model, json_data = json_data["stairStep"] if "stairStep" in json_data else None),
-                json_data["noImprintZonelets"] if "noImprintZonelets" in json_data else None)
+                json_data["partId"] if "partId" in json_data else None,
+                json_data["newEdgeZonelets"] if "newEdgeZonelets" in json_data else None)
         else:
-            all_field_specified = all(arg is not None for arg in [stair_step, no_imprint_zonelets])
+            all_field_specified = all(arg is not None for arg in [part_id, new_edge_zonelets])
             if all_field_specified:
                 self.__initialize(
-                    stair_step,
-                    no_imprint_zonelets)
+                    part_id,
+                    new_edge_zonelets)
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
-                    param_json = model._communicator.initialize_params(model, "PrismParams")
-                    json_data = param_json["PrismParams"] if "PrismParams" in param_json else {}
+                    param_json = model._communicator.initialize_params(model, "ExtractedFeatureIds")
+                    json_data = param_json["ExtractedFeatureIds"] if "ExtractedFeatureIds" in param_json else {}
                     self.__initialize(
-                        stair_step if stair_step is not None else ( PrismParams._default_params["stair_step"] if "stair_step" in PrismParams._default_params else PrismStairStep(model = model, json_data = (json_data["stairStep"] if "stairStep" in json_data else None))),
-                        no_imprint_zonelets if no_imprint_zonelets is not None else ( PrismParams._default_params["no_imprint_zonelets"] if "no_imprint_zonelets" in PrismParams._default_params else (json_data["noImprintZonelets"] if "noImprintZonelets" in json_data else None)))
+                        part_id if part_id is not None else ( ExtractedFeatureIds._default_params["part_id"] if "part_id" in ExtractedFeatureIds._default_params else (json_data["partId"] if "partId" in json_data else None)),
+                        new_edge_zonelets if new_edge_zonelets is not None else ( ExtractedFeatureIds._default_params["new_edge_zonelets"] if "new_edge_zonelets" in ExtractedFeatureIds._default_params else (json_data["newEdgeZonelets"] if "newEdgeZonelets" in json_data else None)))
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
     def set_default(
-            stair_step: PrismStairStep = None,
-            no_imprint_zonelets: Iterable[int] = None):
-        """Set the default values of PrismParams.
+            part_id: int = None,
+            new_edge_zonelets: Iterable[int] = None):
+        """Set the default values of ExtractedFeatureIds.
 
         Parameters
         ----------
-        stair_step: PrismStairStep, optional
-            Prism stairstep parameters.
-        no_imprint_zonelets: Iterable[int], optional
-            Option to specify zonelets to skip prism imprint.
+        part_id: int, optional
+            Id of the part from which edge zonelets are extracted.
+        new_edge_zonelets: Iterable[int], optional
+            Ids of new edge zonelets extracted.
         """
         args = locals()
-        [PrismParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+        [ExtractedFeatureIds._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
     def print_default():
-        """Print the default values of PrismParams.
+        """Print the default values of ExtractedFeatureIds.
 
         Examples
         --------
-        >>> PrismParams.print_default()
+        >>> ExtractedFeatureIds.print_default()
         """
         message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in PrismParams._default_params.items())
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in ExtractedFeatureIds._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
-        if self._stair_step is not None:
-            json_data["stairStep"] = self._stair_step._jsonify()
-        if self._no_imprint_zonelets is not None:
-            json_data["noImprintZonelets"] = self._no_imprint_zonelets
+        if self._part_id is not None:
+            json_data["partId"] = self._part_id
+        if self._new_edge_zonelets is not None:
+            json_data["newEdgeZonelets"] = self._new_edge_zonelets
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "stair_step :  %s\nno_imprint_zonelets :  %s" % ('{ ' + str(self._stair_step) + ' }', self._no_imprint_zonelets)
+        message = "part_id :  %s\nnew_edge_zonelets :  %s" % (self._part_id, self._new_edge_zonelets)
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
     @property
-    def stair_step(self) -> PrismStairStep:
-        """Prism stairstep parameters.
+    def part_id(self) -> int:
+        """Id of the part from which edge zonelets are extracted.
         """
-        return self._stair_step
+        return self._part_id
 
-    @stair_step.setter
-    def stair_step(self, value: PrismStairStep):
-        self._stair_step = value
+    @part_id.setter
+    def part_id(self, value: int):
+        self._part_id = value
 
     @property
-    def no_imprint_zonelets(self) -> Iterable[int]:
-        """Option to specify zonelets to skip prism imprint.
+    def new_edge_zonelets(self) -> Iterable[int]:
+        """Ids of new edge zonelets extracted.
         """
-        return self._no_imprint_zonelets
+        return self._new_edge_zonelets
 
-    @no_imprint_zonelets.setter
-    def no_imprint_zonelets(self, value: Iterable[int]):
-        self._no_imprint_zonelets = value
+    @new_edge_zonelets.setter
+    def new_edge_zonelets(self, value: Iterable[int]):
+        self._new_edge_zonelets = value
 
-class TetParams(CoreObject):
-    """Parameters to control tetrahedral mesh generation.
+class CreateIntersectionEdgeLoopsParams(CoreObject):
+    """Parameters used to calculate edge loops created by intersection of two groups of face zonelets.
     """
     _default_params = {}
 
     def __initialize(
             self,
-            quadratic: bool):
-        self._quadratic = quadratic
+            label_name: str):
+        self._label_name = label_name
 
     def __init__(
             self,
             model: CommunicationManager=None,
-            quadratic: bool = None,
+            label_name: str = None,
             json_data : dict = None,
              **kwargs):
-        """Initializes the TetParams.
+        """Initializes the CreateIntersectionEdgeLoopsParams.
 
         Parameters
         ----------
         model: Model
-            Model to create a TetParams object with default parameters.
-        quadratic: bool, optional
-            Option to generate quadratic tetrahedral mesh. It is not supported with parallel meshing. It is only supported with pure tetrahedral mesh.
+            Model to create a CreateIntersectionEdgeLoopsParams object with default parameters.
+        label_name: str, optional
+            Label name to be assigned to extracted features.
         json_data: dict, optional
-            JSON dictionary to create a TetParams object with provided parameters.
+            JSON dictionary to create a CreateIntersectionEdgeLoopsParams object with provided parameters.
 
         Examples
         --------
-        >>> tet_params = prime.TetParams(model = model)
+        >>> create_intersection_edge_loops_params = prime.CreateIntersectionEdgeLoopsParams(model = model)
         """
         if json_data:
             self.__initialize(
-                json_data["quadratic"] if "quadratic" in json_data else None)
+                json_data["labelName"] if "labelName" in json_data else None)
         else:
-            all_field_specified = all(arg is not None for arg in [quadratic])
+            all_field_specified = all(arg is not None for arg in [label_name])
             if all_field_specified:
                 self.__initialize(
-                    quadratic)
+                    label_name)
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
-                    param_json = model._communicator.initialize_params(model, "TetParams")
-                    json_data = param_json["TetParams"] if "TetParams" in param_json else {}
+                    param_json = model._communicator.initialize_params(model, "CreateIntersectionEdgeLoopsParams")
+                    json_data = param_json["CreateIntersectionEdgeLoopsParams"] if "CreateIntersectionEdgeLoopsParams" in param_json else {}
                     self.__initialize(
-                        quadratic if quadratic is not None else ( TetParams._default_params["quadratic"] if "quadratic" in TetParams._default_params else (json_data["quadratic"] if "quadratic" in json_data else None)))
+                        label_name if label_name is not None else ( CreateIntersectionEdgeLoopsParams._default_params["label_name"] if "label_name" in CreateIntersectionEdgeLoopsParams._default_params else (json_data["labelName"] if "labelName" in json_data else None)))
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
     def set_default(
-            quadratic: bool = None):
-        """Set the default values of TetParams.
+            label_name: str = None):
+        """Set the default values of CreateIntersectionEdgeLoopsParams.
 
         Parameters
         ----------
-        quadratic: bool, optional
-            Option to generate quadratic tetrahedral mesh. It is not supported with parallel meshing. It is only supported with pure tetrahedral mesh.
+        label_name: str, optional
+            Label name to be assigned to extracted features.
         """
         args = locals()
-        [TetParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+        [CreateIntersectionEdgeLoopsParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
     def print_default():
-        """Print the default values of TetParams.
+        """Print the default values of CreateIntersectionEdgeLoopsParams.
 
         Examples
         --------
-        >>> TetParams.print_default()
+        >>> CreateIntersectionEdgeLoopsParams.print_default()
         """
         message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in TetParams._default_params.items())
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in CreateIntersectionEdgeLoopsParams._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
-        if self._quadratic is not None:
-            json_data["quadratic"] = self._quadratic
+        if self._label_name is not None:
+            json_data["labelName"] = self._label_name
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "quadratic :  %s" % (self._quadratic)
+        message = "label_name :  %s" % (self._label_name)
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
     @property
-    def quadratic(self) -> bool:
-        """Option to generate quadratic tetrahedral mesh. It is not supported with parallel meshing. It is only supported with pure tetrahedral mesh.
+    def label_name(self) -> str:
+        """Label name to be assigned to extracted features.
         """
-        return self._quadratic
+        return self._label_name
 
-    @quadratic.setter
-    def quadratic(self, value: bool):
-        self._quadratic = value
+    @label_name.setter
+    def label_name(self, value: str):
+        self._label_name = value
 
-class AutoMeshParams(CoreObject):
-    """Parameters for volume meshing.
+class CreateIntersectionEdgeLoopsResults(CoreObject):
+    """Results for the edge loops created by intersection of two groups of face zonelets.
     """
     _default_params = {}
 
     def __initialize(
             self,
-            size_field_type: SizeFieldType,
-            max_size: float,
-            prism_control_ids: Iterable[int],
-            volume_fill_type: VolumeFillType,
-            prism: PrismParams,
-            tet: TetParams,
-            volume_control_ids: Iterable[int],
-            periodic_control_ids: Iterable[int]):
-        self._size_field_type = SizeFieldType(size_field_type)
-        self._max_size = max_size
-        self._prism_control_ids = prism_control_ids if isinstance(prism_control_ids, np.ndarray) else np.array(prism_control_ids, dtype=np.int32) if prism_control_ids is not None else None
-        self._volume_fill_type = VolumeFillType(volume_fill_type)
-        self._prism = prism
-        self._tet = tet
-        self._volume_control_ids = volume_control_ids if isinstance(volume_control_ids, np.ndarray) else np.array(volume_control_ids, dtype=np.int32) if volume_control_ids is not None else None
-        self._periodic_control_ids = periodic_control_ids if isinstance(periodic_control_ids, np.ndarray) else np.array(periodic_control_ids, dtype=np.int32) if periodic_control_ids is not None else None
+            processing_time: float,
+            error_code: ErrorCode,
+            extracted_ids: List[ExtractedFeatureIds]):
+        self._processing_time = processing_time
+        self._error_code = ErrorCode(error_code)
+        self._extracted_ids = extracted_ids
 
     def __init__(
             self,
             model: CommunicationManager=None,
-            size_field_type: SizeFieldType = None,
-            max_size: float = None,
-            prism_control_ids: Iterable[int] = None,
-            volume_fill_type: VolumeFillType = None,
-            prism: PrismParams = None,
-            tet: TetParams = None,
-            volume_control_ids: Iterable[int] = None,
-            periodic_control_ids: Iterable[int] = None,
+            processing_time: float = None,
+            error_code: ErrorCode = None,
+            extracted_ids: List[ExtractedFeatureIds] = None,
             json_data : dict = None,
              **kwargs):
-        """Initializes the AutoMeshParams.
+        """Initializes the CreateIntersectionEdgeLoopsResults.
 
         Parameters
         ----------
         model: Model
-            Model to create a AutoMeshParams object with default parameters.
-        size_field_type: SizeFieldType, optional
-            Type of sizing to be used to generate volume mesh.
-        max_size: float, optional
-            Maximum cell size.
-        prism_control_ids: Iterable[int], optional
-            Set prism control ids.
-        volume_fill_type: VolumeFillType, optional
-            Option to fill volume.
-        prism: PrismParams, optional
-            Prism control parameters.
-        tet: TetParams, optional
-            Parameters to control tetrahedral mesh generation.
-        volume_control_ids: Iterable[int], optional
-            Ids of the volume controls.
-        periodic_control_ids: Iterable[int], optional
-            Ids of the periodic controls.
+            Model to create a CreateIntersectionEdgeLoopsResults object with default parameters.
+        processing_time: float, optional
+            Time taken to extract edges formed by intersecting faces.
+        error_code: ErrorCode, optional
+            Error code returned by edge extraction function.
+        extracted_ids: List[ExtractedFeatureIds], optional
+            List of ExtractedFeatureIds that contains ids of extracted edges.
         json_data: dict, optional
-            JSON dictionary to create a AutoMeshParams object with provided parameters.
+            JSON dictionary to create a CreateIntersectionEdgeLoopsResults object with provided parameters.
 
         Examples
         --------
-        >>> auto_mesh_params = prime.AutoMeshParams(model = model)
+        >>> create_intersection_edge_loops_results = prime.CreateIntersectionEdgeLoopsResults(model = model)
         """
         if json_data:
             self.__initialize(
-                SizeFieldType(json_data["sizeFieldType"] if "sizeFieldType" in json_data else None),
-                json_data["maxSize"] if "maxSize" in json_data else None,
-                json_data["prismControlIds"] if "prismControlIds" in json_data else None,
-                VolumeFillType(json_data["volumeFillType"] if "volumeFillType" in json_data else None),
-                PrismParams(model = model, json_data = json_data["prism"] if "prism" in json_data else None),
-                TetParams(model = model, json_data = json_data["tet"] if "tet" in json_data else None),
-                json_data["volumeControlIds"] if "volumeControlIds" in json_data else None,
-                json_data["periodicControlIds"] if "periodicControlIds" in json_data else None)
+                json_data["processingTime"] if "processingTime" in json_data else None,
+                ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None),
+                [ExtractedFeatureIds(model = model, json_data = data) for data in json_data["extractedIds"]] if "extractedIds" in json_data else None)
         else:
-            all_field_specified = all(arg is not None for arg in [size_field_type, max_size, prism_control_ids, volume_fill_type, prism, tet, volume_control_ids, periodic_control_ids])
+            all_field_specified = all(arg is not None for arg in [processing_time, error_code, extracted_ids])
             if all_field_specified:
                 self.__initialize(
-                    size_field_type,
-                    max_size,
-                    prism_control_ids,
-                    volume_fill_type,
-                    prism,
-                    tet,
-                    volume_control_ids,
-                    periodic_control_ids)
+                    processing_time,
+                    error_code,
+                    extracted_ids)
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
-                    param_json = model._communicator.initialize_params(model, "AutoMeshParams")
-                    json_data = param_json["AutoMeshParams"] if "AutoMeshParams" in param_json else {}
+                    param_json = model._communicator.initialize_params(model, "CreateIntersectionEdgeLoopsResults")
+                    json_data = param_json["CreateIntersectionEdgeLoopsResults"] if "CreateIntersectionEdgeLoopsResults" in param_json else {}
                     self.__initialize(
-                        size_field_type if size_field_type is not None else ( AutoMeshParams._default_params["size_field_type"] if "size_field_type" in AutoMeshParams._default_params else SizeFieldType(json_data["sizeFieldType"] if "sizeFieldType" in json_data else None)),
-                        max_size if max_size is not None else ( AutoMeshParams._default_params["max_size"] if "max_size" in AutoMeshParams._default_params else (json_data["maxSize"] if "maxSize" in json_data else None)),
-                        prism_control_ids if prism_control_ids is not None else ( AutoMeshParams._default_params["prism_control_ids"] if "prism_control_ids" in AutoMeshParams._default_params else (json_data["prismControlIds"] if "prismControlIds" in json_data else None)),
-                        volume_fill_type if volume_fill_type is not None else ( AutoMeshParams._default_params["volume_fill_type"] if "volume_fill_type" in AutoMeshParams._default_params else VolumeFillType(json_data["volumeFillType"] if "volumeFillType" in json_data else None)),
-                        prism if prism is not None else ( AutoMeshParams._default_params["prism"] if "prism" in AutoMeshParams._default_params else PrismParams(model = model, json_data = (json_data["prism"] if "prism" in json_data else None))),
-                        tet if tet is not None else ( AutoMeshParams._default_params["tet"] if "tet" in AutoMeshParams._default_params else TetParams(model = model, json_data = (json_data["tet"] if "tet" in json_data else None))),
-                        volume_control_ids if volume_control_ids is not None else ( AutoMeshParams._default_params["volume_control_ids"] if "volume_control_ids" in AutoMeshParams._default_params else (json_data["volumeControlIds"] if "volumeControlIds" in json_data else None)),
-                        periodic_control_ids if periodic_control_ids is not None else ( AutoMeshParams._default_params["periodic_control_ids"] if "periodic_control_ids" in AutoMeshParams._default_params else (json_data["periodicControlIds"] if "periodicControlIds" in json_data else None)))
+                        processing_time if processing_time is not None else ( CreateIntersectionEdgeLoopsResults._default_params["processing_time"] if "processing_time" in CreateIntersectionEdgeLoopsResults._default_params else (json_data["processingTime"] if "processingTime" in json_data else None)),
+                        error_code if error_code is not None else ( CreateIntersectionEdgeLoopsResults._default_params["error_code"] if "error_code" in CreateIntersectionEdgeLoopsResults._default_params else ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None)),
+                        extracted_ids if extracted_ids is not None else ( CreateIntersectionEdgeLoopsResults._default_params["extracted_ids"] if "extracted_ids" in CreateIntersectionEdgeLoopsResults._default_params else [ExtractedFeatureIds(model = model, json_data = data) for data in (json_data["extractedIds"] if "extractedIds" in json_data else None)]))
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
     def set_default(
-            size_field_type: SizeFieldType = None,
-            max_size: float = None,
-            prism_control_ids: Iterable[int] = None,
-            volume_fill_type: VolumeFillType = None,
-            prism: PrismParams = None,
-            tet: TetParams = None,
-            volume_control_ids: Iterable[int] = None,
-            periodic_control_ids: Iterable[int] = None):
-        """Set the default values of AutoMeshParams.
+            processing_time: float = None,
+            error_code: ErrorCode = None,
+            extracted_ids: List[ExtractedFeatureIds] = None):
+        """Set the default values of CreateIntersectionEdgeLoopsResults.
 
         Parameters
         ----------
-        size_field_type: SizeFieldType, optional
-            Type of sizing to be used to generate volume mesh.
-        max_size: float, optional
-            Maximum cell size.
-        prism_control_ids: Iterable[int], optional
-            Set prism control ids.
-        volume_fill_type: VolumeFillType, optional
-            Option to fill volume.
-        prism: PrismParams, optional
-            Prism control parameters.
-        tet: TetParams, optional
-            Parameters to control tetrahedral mesh generation.
-        volume_control_ids: Iterable[int], optional
-            Ids of the volume controls.
-        periodic_control_ids: Iterable[int], optional
-            Ids of the periodic controls.
+        processing_time: float, optional
+            Time taken to extract edges formed by intersecting faces.
+        error_code: ErrorCode, optional
+            Error code returned by edge extraction function.
+        extracted_ids: List[ExtractedFeatureIds], optional
+            List of ExtractedFeatureIds that contains ids of extracted edges.
         """
         args = locals()
-        [AutoMeshParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+        [CreateIntersectionEdgeLoopsResults._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
     def print_default():
-        """Print the default values of AutoMeshParams.
+        """Print the default values of CreateIntersectionEdgeLoopsResults.
 
         Examples
         --------
-        >>> AutoMeshParams.print_default()
+        >>> CreateIntersectionEdgeLoopsResults.print_default()
         """
         message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in AutoMeshParams._default_params.items())
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in CreateIntersectionEdgeLoopsResults._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
-        if self._size_field_type is not None:
-            json_data["sizeFieldType"] = self._size_field_type
-        if self._max_size is not None:
-            json_data["maxSize"] = self._max_size
-        if self._prism_control_ids is not None:
-            json_data["prismControlIds"] = self._prism_control_ids
-        if self._volume_fill_type is not None:
-            json_data["volumeFillType"] = self._volume_fill_type
-        if self._prism is not None:
-            json_data["prism"] = self._prism._jsonify()
-        if self._tet is not None:
-            json_data["tet"] = self._tet._jsonify()
-        if self._volume_control_ids is not None:
-            json_data["volumeControlIds"] = self._volume_control_ids
-        if self._periodic_control_ids is not None:
-            json_data["periodicControlIds"] = self._periodic_control_ids
+        if self._processing_time is not None:
+            json_data["processingTime"] = self._processing_time
+        if self._error_code is not None:
+            json_data["errorCode"] = self._error_code
+        if self._extracted_ids is not None:
+            json_data["extractedIds"] = [data._jsonify() for data in self._extracted_ids]
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "size_field_type :  %s\nmax_size :  %s\nprism_control_ids :  %s\nvolume_fill_type :  %s\nprism :  %s\ntet :  %s\nvolume_control_ids :  %s\nperiodic_control_ids :  %s" % (self._size_field_type, self._max_size, self._prism_control_ids, self._volume_fill_type, '{ ' + str(self._prism) + ' }', '{ ' + str(self._tet) + ' }', self._volume_control_ids, self._periodic_control_ids)
+        message = "processing_time :  %s\nerror_code :  %s\nextracted_ids :  %s" % (self._processing_time, self._error_code, '[' + ''.join('\n' + str(data) for data in self._extracted_ids) + ']')
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
     @property
-    def size_field_type(self) -> SizeFieldType:
-        """Type of sizing to be used to generate volume mesh.
+    def processing_time(self) -> float:
+        """Time taken to extract edges formed by intersecting faces.
         """
-        return self._size_field_type
+        return self._processing_time
 
-    @size_field_type.setter
-    def size_field_type(self, value: SizeFieldType):
-        self._size_field_type = value
+    @processing_time.setter
+    def processing_time(self, value: float):
+        self._processing_time = value
 
     @property
-    def max_size(self) -> float:
-        """Maximum cell size.
-        """
-        return self._max_size
-
-    @max_size.setter
-    def max_size(self, value: float):
-        self._max_size = value
-
-    @property
-    def prism_control_ids(self) -> Iterable[int]:
-        """Set prism control ids.
-        """
-        return self._prism_control_ids
-
-    @prism_control_ids.setter
-    def prism_control_ids(self, value: Iterable[int]):
-        self._prism_control_ids = value
-
-    @property
-    def volume_fill_type(self) -> VolumeFillType:
-        """Option to fill volume.
-        """
-        return self._volume_fill_type
-
-    @volume_fill_type.setter
-    def volume_fill_type(self, value: VolumeFillType):
-        self._volume_fill_type = value
-
-    @property
-    def prism(self) -> PrismParams:
-        """Prism control parameters.
-        """
-        return self._prism
-
-    @prism.setter
-    def prism(self, value: PrismParams):
-        self._prism = value
-
-    @property
-    def tet(self) -> TetParams:
-        """Parameters to control tetrahedral mesh generation.
-        """
-        return self._tet
-
-    @tet.setter
-    def tet(self, value: TetParams):
-        self._tet = value
-
-    @property
-    def volume_control_ids(self) -> Iterable[int]:
-        """Ids of the volume controls.
+    def error_code(self) -> ErrorCode:
+        """Error code returned by edge extraction function.
         """
-        return self._volume_control_ids
+        return self._error_code
 
-    @volume_control_ids.setter
-    def volume_control_ids(self, value: Iterable[int]):
-        self._volume_control_ids = value
+    @error_code.setter
+    def error_code(self, value: ErrorCode):
+        self._error_code = value
 
     @property
-    def periodic_control_ids(self) -> Iterable[int]:
-        """Ids of the periodic controls.
+    def extracted_ids(self) -> List[ExtractedFeatureIds]:
+        """List of ExtractedFeatureIds that contains ids of extracted edges.
         """
-        return self._periodic_control_ids
+        return self._extracted_ids
 
-    @periodic_control_ids.setter
-    def periodic_control_ids(self, value: Iterable[int]):
-        self._periodic_control_ids = value
+    @extracted_ids.setter
+    def extracted_ids(self, value: List[ExtractedFeatureIds]):
+        self._extracted_ids = value
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/boundaryfittednurbs.py`

 * *Files 24% similar despite different names*

```diff
@@ -58,14 +58,20 @@
         >>> #connect client to server and get model from it
         >>> client = Client(ip="localhost", port=50060)
         >>> model = client.model
         >>> boundary_fitted_spline = BoundaryFittedSpline(model = model)
         >>> results = boundary_fitted_spline.create_boundary_fitted_spline(part_id, cell_zonelet_ids, boundary_fitted_spline_params)
 
         """
+        if not isinstance(part_id, int):
+            raise TypeError("Invalid argument type passed for part_id, valid argument type is int.")
+        if not isinstance(cell_zonelet_ids, Iterable):
+            raise TypeError("Invalid argument type passed for cell_zonelet_ids, valid argument type is Iterable[int].")
+        if not isinstance(boundary_fitted_spline_params, BoundaryFittedSplineParams):
+            raise TypeError("Invalid argument type passed for boundary_fitted_spline_params, valid argument type is BoundaryFittedSplineParams.")
         args = {"part_id" : part_id,
         "cell_zonelet_ids" : cell_zonelet_ids,
         "boundary_fitted_spline_params" : boundary_fitted_spline_params._jsonify()}
         command_name = "PrimeMesh::BoundaryFittedSpline/CreateBoundaryFittedSpline"
         self._model._print_logs_before_command("create_boundary_fitted_spline", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("create_boundary_fitted_spline", IGAResults(model = self._model, json_data = result))
@@ -98,14 +104,20 @@
         >>> #connect client to server and get model from it
         >>> client = Client(ip="localhost", port=50060)
         >>> model = client.model
         >>> boundary_fitted_spline = BoundaryFittedSpline(model = model)
         >>> results = boundary_fitted_spline.refine_spline(part_id, spline_ids, refine_spline_params)
 
         """
+        if not isinstance(part_id, int):
+            raise TypeError("Invalid argument type passed for part_id, valid argument type is int.")
+        if not isinstance(spline_ids, Iterable):
+            raise TypeError("Invalid argument type passed for spline_ids, valid argument type is Iterable[int].")
+        if not isinstance(refine_spline_params, RefineSplineParams):
+            raise TypeError("Invalid argument type passed for refine_spline_params, valid argument type is RefineSplineParams.")
         args = {"part_id" : part_id,
         "spline_ids" : spline_ids,
         "refine_spline_params" : refine_spline_params._jsonify()}
         command_name = "PrimeMesh::BoundaryFittedSpline/RefineSpline"
         self._model._print_logs_before_command("refine_spline", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("refine_spline", IGAResults(model = self._model, json_data = result))
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/collapsetoolstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/collapsetoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/commonstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/commonstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/commontypes.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/commontypes.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/connect.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/connect.py`

 * *Files 24% similar despite different names*

```diff
@@ -58,14 +58,22 @@
 
         Examples
         --------
         >>> connect = Connect(model = model)
         >>> results = connect.intersect_face_zonelets (part_id, face_zonelet_ids, with_face_zonelet_ids, params)
 
         """
+        if not isinstance(part_id, int):
+            raise TypeError("Invalid argument type passed for part_id, valid argument type is int.")
+        if not isinstance(face_zonelet_ids, Iterable):
+            raise TypeError("Invalid argument type passed for face_zonelet_ids, valid argument type is Iterable[int].")
+        if not isinstance(with_face_zonelet_ids, Iterable):
+            raise TypeError("Invalid argument type passed for with_face_zonelet_ids, valid argument type is Iterable[int].")
+        if not isinstance(params, IntersectParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is IntersectParams.")
         args = {"part_id" : part_id,
         "face_zonelet_ids" : face_zonelet_ids,
         "with_face_zonelet_ids" : with_face_zonelet_ids,
         "params" : params._jsonify()}
         command_name = "PrimeMesh::Connect/IntersectFaceZonelets"
         self._model._print_logs_before_command("intersect_face_zonelets", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
@@ -95,14 +103,22 @@
 
         Examples
         --------
         >>> connect = Connect(model = model)
         >>> results = connect.join_face_zonelets (part_id, face_zonelet_ids, with_face_zonelet_ids, params)
 
         """
+        if not isinstance(part_id, int):
+            raise TypeError("Invalid argument type passed for part_id, valid argument type is int.")
+        if not isinstance(face_zonelet_ids, Iterable):
+            raise TypeError("Invalid argument type passed for face_zonelet_ids, valid argument type is Iterable[int].")
+        if not isinstance(with_face_zonelet_ids, Iterable):
+            raise TypeError("Invalid argument type passed for with_face_zonelet_ids, valid argument type is Iterable[int].")
+        if not isinstance(params, JoinParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is JoinParams.")
         args = {"part_id" : part_id,
         "face_zonelet_ids" : face_zonelet_ids,
         "with_face_zonelet_ids" : with_face_zonelet_ids,
         "params" : params._jsonify()}
         command_name = "PrimeMesh::Connect/JoinFaceZonelets"
         self._model._print_logs_before_command("join_face_zonelets", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
@@ -131,14 +147,22 @@
 
 
         Examples
         --------
         >>> results = connect.subtract_volumes(part_id, target_volumes, cutter_volumes, params)
 
         """
+        if not isinstance(part_id, int):
+            raise TypeError("Invalid argument type passed for part_id, valid argument type is int.")
+        if not isinstance(target_volumes, Iterable):
+            raise TypeError("Invalid argument type passed for target_volumes, valid argument type is Iterable[int].")
+        if not isinstance(cutter_volumes, Iterable):
+            raise TypeError("Invalid argument type passed for cutter_volumes, valid argument type is Iterable[int].")
+        if not isinstance(params, SubtractVolumesParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is SubtractVolumesParams.")
         args = {"part_id" : part_id,
         "target_volumes" : target_volumes,
         "cutter_volumes" : cutter_volumes,
         "params" : params._jsonify()}
         command_name = "PrimeMesh::Connect/SubtractVolumes"
         self._model._print_logs_before_command("subtract_volumes", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
@@ -168,46 +192,32 @@
 
         Examples
         --------
         >>> connect = Connect(model = model)
         >>> results = connect.stitch_face_zonelets (part_id, face_zonelet_ids, with_face_zonelet_ids, stitch_params)
 
         """
+        if not isinstance(part_id, int):
+            raise TypeError("Invalid argument type passed for part_id, valid argument type is int.")
+        if not isinstance(face_zonelet_ids, Iterable):
+            raise TypeError("Invalid argument type passed for face_zonelet_ids, valid argument type is Iterable[int].")
+        if not isinstance(with_face_zonelet_ids, Iterable):
+            raise TypeError("Invalid argument type passed for with_face_zonelet_ids, valid argument type is Iterable[int].")
+        if not isinstance(params, StitchParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is StitchParams.")
         args = {"part_id" : part_id,
         "face_zonelet_ids" : face_zonelet_ids,
         "with_face_zonelet_ids" : with_face_zonelet_ids,
         "params" : params._jsonify()}
         command_name = "PrimeMesh::Connect/StitchFaceZonelets"
         self._model._print_logs_before_command("stitch_face_zonelets", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("stitch_face_zonelets", ConnectResults(model = self._model, json_data = result))
         return ConnectResults(model = self._model, json_data = result)
 
-    def initialize_mesh_match_params(self) -> MeshMatchParams:
-        """ Initialize mesh match parameters with default values.
-
-
-        Returns
-        -------
-        MeshMatchParams
-            Returns the MeshMatchParams structure.
-
-
-        Examples
-        --------
-        >>> params = connect.InitializeMeshMatchParams()
-
-        """
-        args = {}
-        command_name = "PrimeMesh::Connect/InitializeMeshMatchParams"
-        self._model._print_logs_before_command("initialize_mesh_match_params", args)
-        result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("initialize_mesh_match_params", MeshMatchParams(model = self._model, json_data = result))
-        return MeshMatchParams(model = self._model, json_data = result)
-
     def mesh_match_within_part_face_zonelets(self, part_id : int, source_face_zonelet_ids : Iterable[int], target_face_zonelet_ids : Iterable[int], params : MeshMatchParams) -> MeshMatchResults:
         """ Perform mesh matching between overlapping face zonelets within a single part. Matched mesh can then be colocated, merged or removed as directed.
 
 
         Parameters
         ----------
         part_id : int
@@ -223,18 +233,26 @@
         -------
         MeshMatchResults
             Returns the MeshMatchResults.
 
 
         Examples
         --------
-        >>> connect = Connect(model = model)
-        >>> results = connect.MeshMatchWithinPartFaceZonelets(part_id, source_face_zonelet_ids, target_face_zonelet_ids, match_mesh_params)
+        connect = Connect(model = model)
+        connect.mesh_match_within_part_face_zonelets(part.id, source_face_zonelet_ids, target_face_zonelet_ids, match_mesh_params)
 
         """
+        if not isinstance(part_id, int):
+            raise TypeError("Invalid argument type passed for part_id, valid argument type is int.")
+        if not isinstance(source_face_zonelet_ids, Iterable):
+            raise TypeError("Invalid argument type passed for source_face_zonelet_ids, valid argument type is Iterable[int].")
+        if not isinstance(target_face_zonelet_ids, Iterable):
+            raise TypeError("Invalid argument type passed for target_face_zonelet_ids, valid argument type is Iterable[int].")
+        if not isinstance(params, MeshMatchParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is MeshMatchParams.")
         args = {"part_id" : part_id,
         "source_face_zonelet_ids" : source_face_zonelet_ids,
         "target_face_zonelet_ids" : target_face_zonelet_ids,
         "params" : params._jsonify()}
         command_name = "PrimeMesh::Connect/MeshMatchWithinPartFaceZonelets"
         self._model._print_logs_before_command("mesh_match_within_part_face_zonelets", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/connectstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/connectstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/controldata.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/controldata.py`

 * *Files 23% similar despite different names*

```diff
@@ -63,14 +63,16 @@
         An empty size control is created on calling this API.
 
         Examples
         --------
         >>> size_control = model.control_data.create_size_control(SizingType.CURVATURE)
 
         """
+        if not isinstance(type, SizingType):
+            raise TypeError("Invalid argument type passed for type, valid argument type is SizingType.")
         args = {"type" : type}
         command_name = "PrimeMesh::ControlData/CreateSizeControl"
         self._model._print_logs_before_command("create_size_control", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("create_size_control")
         return result
 
@@ -92,14 +94,36 @@
         args = {}
         command_name = "PrimeMesh::ControlData/CreatePrismControl"
         self._model._print_logs_before_command("create_prism_control", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("create_prism_control")
         return result
 
+    def create_thin_volume_control(self) -> List[Any]:
+        """ Creates the ThinVolumeControl.
+
+
+        Returns
+        -------
+        ThinVolumeControl
+            Returns the ThinVolumeControl.
+
+
+        Examples
+        --------
+        >>> thin_volume_control = model.control_data.create_thin_volume_control()
+
+        """
+        args = {}
+        command_name = "PrimeMesh::ControlData/CreateThinVolumeControl"
+        self._model._print_logs_before_command("create_thin_volume_control", args)
+        result = self._comm.serve(self._model, command_name, self._object_id, args=args)
+        self._model._print_logs_after_command("create_thin_volume_control")
+        return result
+
     def create_volume_control(self) -> List[Any]:
         """ Creates the volume control.
 
 
         Returns
         -------
         VolumeControl
@@ -153,14 +177,16 @@
             Returns the DeleteResults.
 
         Examples
         --------
         >>> results = model.control_data.delete_controls([size_control.id, volume_control.id])
 
         """
+        if not isinstance(control_ids, Iterable):
+            raise TypeError("Invalid argument type passed for control_ids, valid argument type is Iterable[int].")
         args = {"control_ids" : control_ids}
         command_name = "PrimeMesh::ControlData/DeleteControls"
         self._model._print_logs_before_command("delete_controls", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("delete_controls", DeleteResults(model = self._model, json_data = result))
         return DeleteResults(model = self._model, json_data = result)
 
@@ -185,14 +211,18 @@
         >>> face_zonelets = model.control_data.get_scope_face_zonelets(
         >>>                 prime.ScopeDefinition(model = model,
         >>>                 entity_type = prime.ScopeEntity.FACEZONELETS,
         >>>                 part_expression = "*"),
         >>>                 prime.ScopeZoneletParams(model =model))
 
         """
+        if not isinstance(scope, ScopeDefinition):
+            raise TypeError("Invalid argument type passed for scope, valid argument type is ScopeDefinition.")
+        if not isinstance(params, ScopeZoneletParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is ScopeZoneletParams.")
         args = {"scope" : scope._jsonify(),
         "params" : params._jsonify()}
         command_name = "PrimeMesh::ControlData/GetScopeFaceZonelets"
         self._model._print_logs_before_command("get_scope_face_zonelets", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("get_scope_face_zonelets")
         return result
@@ -215,14 +245,16 @@
         --------
         >>> part_ids = model.control_data.get_scope_parts(
         >>>                 prime.ScopeDefinition(model = model,
         >>>                 part_expression = "*"),
         >>>                 prime.ScopeZoneletParams(model =model))
 
         """
+        if not isinstance(scope, ScopeDefinition):
+            raise TypeError("Invalid argument type passed for scope, valid argument type is ScopeDefinition.")
         args = {"scope" : scope._jsonify()}
         command_name = "PrimeMesh::ControlData/GetScopeParts"
         self._model._print_logs_before_command("get_scope_parts", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("get_scope_parts")
         return result
 
@@ -242,14 +274,16 @@
 
 
         Examples
         --------
         >>> results = control_data.get_part_zonelets(scope)
 
         """
+        if not isinstance(scope, ScopeDefinition):
+            raise TypeError("Invalid argument type passed for scope, valid argument type is ScopeDefinition.")
         args = {"scope" : scope._jsonify()}
         command_name = "PrimeMesh::ControlData/GetPartZonelets"
         self._model._print_logs_before_command("get_part_zonelets", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("get_part_zonelets", [PartZonelets(model = self._model, json_data = data) for data in result])
         return [PartZonelets(model = self._model, json_data = data) for data in result]
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/controlstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/controlstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/coreobject.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/coreobject.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/deletetool.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/deletetool.py`

 * *Files 17% similar despite different names*

```diff
@@ -53,14 +53,20 @@
         >>> results = delete_tool.delete_fringes_and_overlaps_on_zonelets(
         >>>                                    part.id,
         >>>                                    part.get_face_zonelets(),
         >>>                                    prime.DeleteFringesAndOverlapsParams(
         >>>                                       model=model))
 
         """
+        if not isinstance(part_id, int):
+            raise TypeError("Invalid argument type passed for part_id, valid argument type is int.")
+        if not isinstance(face_zonelets, Iterable):
+            raise TypeError("Invalid argument type passed for face_zonelets, valid argument type is Iterable[int].")
+        if not isinstance(params, DeleteFringesAndOverlapsParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is DeleteFringesAndOverlapsParams.")
         args = {"part_id" : part_id,
         "face_zonelets" : face_zonelets,
         "params" : params._jsonify()}
         command_name = "PrimeMesh::DeleteTool/DeleteFringesAndOverlapsOnZonelets"
         self._model._print_logs_before_command("delete_fringes_and_overlaps_on_zonelets", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("delete_fringes_and_overlaps_on_zonelets", DeleteFringesAndOverlapsResults(model = self._model, json_data = result))
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/deletetoolstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/deletetoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/featureextraction.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/featureextraction.py`

 * *Files 23% similar despite different names*

```diff
@@ -49,14 +49,20 @@
 
 
         Examples
         --------
         >>> results = feature_extraction.extract_features_on_face_zonelets(part_id, face_zonelets, params)
 
         """
+        if not isinstance(part_id, int):
+            raise TypeError("Invalid argument type passed for part_id, valid argument type is int.")
+        if not isinstance(face_zonelets, Iterable):
+            raise TypeError("Invalid argument type passed for face_zonelets, valid argument type is Iterable[int].")
+        if not isinstance(params, ExtractFeatureParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is ExtractFeatureParams.")
         args = {"part_id" : part_id,
         "face_zonelets" : face_zonelets,
         "params" : params._jsonify()}
         command_name = "PrimeMesh::FeatureExtraction/ExtractFeaturesOnFaceZonelets"
         self._model._print_logs_before_command("extract_features_on_face_zonelets", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("extract_features_on_face_zonelets", ExtractFeatureResults(model = self._model, json_data = result))
@@ -82,14 +88,20 @@
 
 
         Examples
         --------
         >>> results = feature_extraction.create_intersection_edge_loops(part_face_zonelets, intersecting_part_face_zonelets, params)
 
         """
+        if not isinstance(part_face_zonelets, List):
+            raise TypeError("Invalid argument type passed for part_face_zonelets, valid argument type is List[PartZonelets].")
+        if not isinstance(intersecting_part_face_zonelets, List):
+            raise TypeError("Invalid argument type passed for intersecting_part_face_zonelets, valid argument type is List[PartZonelets].")
+        if not isinstance(params, CreateIntersectionEdgeLoopsParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is CreateIntersectionEdgeLoopsParams.")
         args = {"part_face_zonelets" : [p._jsonify() for p in part_face_zonelets],
         "intersecting_part_face_zonelets" : [p._jsonify() for p in intersecting_part_face_zonelets],
         "params" : params._jsonify()}
         command_name = "PrimeMesh::FeatureExtraction/CreateIntersectionEdgeLoops"
         self._model._print_logs_before_command("create_intersection_edge_loops", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("create_intersection_edge_loops", CreateIntersectionEdgeLoopsResults(model = self._model, json_data = result))
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/featureextractionstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumemeshtoolstructs.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,741 +4,616 @@
 from ansys.meshing.prime.internals.comm_manager import CommunicationManager
 from ansys.meshing.prime.internals import utils
 from ansys.meshing.prime.autogen.coreobject import *
 import numpy as np
 
 from ansys.meshing.prime.params.primestructs import *
 
-class ExtractFeatureParams(CoreObject):
-    """Parameter to control feature edge extraction.
+class AutoNodeMoveParams(CoreObject):
+    """Parameters used to improve volume mesh by auto node move.
     """
     _default_params = {}
 
     def __initialize(
             self,
-            replace: bool,
-            feature_angle: float,
-            separate_features: bool,
-            separation_angle: float,
-            disconnect_with_faces: bool,
-            label_name: str):
-        self._replace = replace
-        self._feature_angle = feature_angle
-        self._separate_features = separate_features
-        self._separation_angle = separation_angle
-        self._disconnect_with_faces = disconnect_with_faces
-        self._label_name = label_name
+            quality_measure: CellQualityMeasure,
+            target_quality: float,
+            dihedral_angle: float,
+            n_iterations_per_node: int,
+            restrict_boundary_nodes_along_surface: bool,
+            n_attempts: int):
+        self._quality_measure = CellQualityMeasure(quality_measure)
+        self._target_quality = target_quality
+        self._dihedral_angle = dihedral_angle
+        self._n_iterations_per_node = n_iterations_per_node
+        self._restrict_boundary_nodes_along_surface = restrict_boundary_nodes_along_surface
+        self._n_attempts = n_attempts
 
     def __init__(
             self,
             model: CommunicationManager=None,
-            replace: bool = None,
-            feature_angle: float = None,
-            separate_features: bool = None,
-            separation_angle: float = None,
-            disconnect_with_faces: bool = None,
-            label_name: str = None,
+            quality_measure: CellQualityMeasure = None,
+            target_quality: float = None,
+            dihedral_angle: float = None,
+            n_iterations_per_node: int = None,
+            restrict_boundary_nodes_along_surface: bool = None,
+            n_attempts: int = None,
             json_data : dict = None,
              **kwargs):
-        """Initializes the ExtractFeatureParams.
+        """Initializes the AutoNodeMoveParams.
 
         Parameters
         ----------
         model: Model
-            Model to create a ExtractFeatureParams object with default parameters.
-        replace: bool, optional
-            Option to replace existing edge zonelets with new extracted edge zonelets.
-        feature_angle: float, optional
-            Angle used to capture face features to be  extracted as edges.
-        separate_features: bool, optional
-            Option to separate extracted features.
-        separation_angle: float, optional
-            Angle used to separate extracted features.
-        disconnect_with_faces: bool, optional
-            Option to disconnect edges from faces. If false, edges remain connected to faces by sharing nodes.
-        label_name: str, optional
-            Label name to be assigned to extracted features.
+            Model to create a AutoNodeMoveParams object with default parameters.
+        quality_measure: CellQualityMeasure, optional
+            Specify cell quality measure to be used for volume mesh improvement. The default value for cell quality measure is skewness.
+        target_quality: float, optional
+            Specify target quality used for the mesh improvement based on specified quality measure.
+        dihedral_angle: float, optional
+            Dihedral angle used to mantain features of boundary face zonelets.
+        n_iterations_per_node: int, optional
+            Number of iterations per node to be moved.
+        restrict_boundary_nodes_along_surface: bool, optional
+            Option to restrict the movement of the boundary node to the plane containing the boundary faces sharing the boundary node.
+        n_attempts: int, optional
+            Number of attempts to improve specified quality measure by node movement.
         json_data: dict, optional
-            JSON dictionary to create a ExtractFeatureParams object with provided parameters.
+            JSON dictionary to create a AutoNodeMoveParams object with provided parameters.
 
         Examples
         --------
-        >>> extract_feature_params = prime.ExtractFeatureParams(model = model)
+        >>> auto_node_move_params = prime.AutoNodeMoveParams(model = model)
         """
         if json_data:
             self.__initialize(
-                json_data["replace"] if "replace" in json_data else None,
-                json_data["featureAngle"] if "featureAngle" in json_data else None,
-                json_data["separateFeatures"] if "separateFeatures" in json_data else None,
-                json_data["separationAngle"] if "separationAngle" in json_data else None,
-                json_data["disconnectWithFaces"] if "disconnectWithFaces" in json_data else None,
-                json_data["labelName"] if "labelName" in json_data else None)
+                CellQualityMeasure(json_data["qualityMeasure"] if "qualityMeasure" in json_data else None),
+                json_data["targetQuality"] if "targetQuality" in json_data else None,
+                json_data["dihedralAngle"] if "dihedralAngle" in json_data else None,
+                json_data["nIterationsPerNode"] if "nIterationsPerNode" in json_data else None,
+                json_data["restrictBoundaryNodesAlongSurface"] if "restrictBoundaryNodesAlongSurface" in json_data else None,
+                json_data["nAttempts"] if "nAttempts" in json_data else None)
         else:
-            all_field_specified = all(arg is not None for arg in [replace, feature_angle, separate_features, separation_angle, disconnect_with_faces, label_name])
+            all_field_specified = all(arg is not None for arg in [quality_measure, target_quality, dihedral_angle, n_iterations_per_node, restrict_boundary_nodes_along_surface, n_attempts])
             if all_field_specified:
                 self.__initialize(
-                    replace,
-                    feature_angle,
-                    separate_features,
-                    separation_angle,
-                    disconnect_with_faces,
-                    label_name)
+                    quality_measure,
+                    target_quality,
+                    dihedral_angle,
+                    n_iterations_per_node,
+                    restrict_boundary_nodes_along_surface,
+                    n_attempts)
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
-                    param_json = model._communicator.initialize_params(model, "ExtractFeatureParams")
-                    json_data = param_json["ExtractFeatureParams"] if "ExtractFeatureParams" in param_json else {}
+                    param_json = model._communicator.initialize_params(model, "AutoNodeMoveParams")
+                    json_data = param_json["AutoNodeMoveParams"] if "AutoNodeMoveParams" in param_json else {}
                     self.__initialize(
-                        replace if replace is not None else ( ExtractFeatureParams._default_params["replace"] if "replace" in ExtractFeatureParams._default_params else (json_data["replace"] if "replace" in json_data else None)),
-                        feature_angle if feature_angle is not None else ( ExtractFeatureParams._default_params["feature_angle"] if "feature_angle" in ExtractFeatureParams._default_params else (json_data["featureAngle"] if "featureAngle" in json_data else None)),
-                        separate_features if separate_features is not None else ( ExtractFeatureParams._default_params["separate_features"] if "separate_features" in ExtractFeatureParams._default_params else (json_data["separateFeatures"] if "separateFeatures" in json_data else None)),
-                        separation_angle if separation_angle is not None else ( ExtractFeatureParams._default_params["separation_angle"] if "separation_angle" in ExtractFeatureParams._default_params else (json_data["separationAngle"] if "separationAngle" in json_data else None)),
-                        disconnect_with_faces if disconnect_with_faces is not None else ( ExtractFeatureParams._default_params["disconnect_with_faces"] if "disconnect_with_faces" in ExtractFeatureParams._default_params else (json_data["disconnectWithFaces"] if "disconnectWithFaces" in json_data else None)),
-                        label_name if label_name is not None else ( ExtractFeatureParams._default_params["label_name"] if "label_name" in ExtractFeatureParams._default_params else (json_data["labelName"] if "labelName" in json_data else None)))
+                        quality_measure if quality_measure is not None else ( AutoNodeMoveParams._default_params["quality_measure"] if "quality_measure" in AutoNodeMoveParams._default_params else CellQualityMeasure(json_data["qualityMeasure"] if "qualityMeasure" in json_data else None)),
+                        target_quality if target_quality is not None else ( AutoNodeMoveParams._default_params["target_quality"] if "target_quality" in AutoNodeMoveParams._default_params else (json_data["targetQuality"] if "targetQuality" in json_data else None)),
+                        dihedral_angle if dihedral_angle is not None else ( AutoNodeMoveParams._default_params["dihedral_angle"] if "dihedral_angle" in AutoNodeMoveParams._default_params else (json_data["dihedralAngle"] if "dihedralAngle" in json_data else None)),
+                        n_iterations_per_node if n_iterations_per_node is not None else ( AutoNodeMoveParams._default_params["n_iterations_per_node"] if "n_iterations_per_node" in AutoNodeMoveParams._default_params else (json_data["nIterationsPerNode"] if "nIterationsPerNode" in json_data else None)),
+                        restrict_boundary_nodes_along_surface if restrict_boundary_nodes_along_surface is not None else ( AutoNodeMoveParams._default_params["restrict_boundary_nodes_along_surface"] if "restrict_boundary_nodes_along_surface" in AutoNodeMoveParams._default_params else (json_data["restrictBoundaryNodesAlongSurface"] if "restrictBoundaryNodesAlongSurface" in json_data else None)),
+                        n_attempts if n_attempts is not None else ( AutoNodeMoveParams._default_params["n_attempts"] if "n_attempts" in AutoNodeMoveParams._default_params else (json_data["nAttempts"] if "nAttempts" in json_data else None)))
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
     def set_default(
-            replace: bool = None,
-            feature_angle: float = None,
-            separate_features: bool = None,
-            separation_angle: float = None,
-            disconnect_with_faces: bool = None,
-            label_name: str = None):
-        """Set the default values of ExtractFeatureParams.
+            quality_measure: CellQualityMeasure = None,
+            target_quality: float = None,
+            dihedral_angle: float = None,
+            n_iterations_per_node: int = None,
+            restrict_boundary_nodes_along_surface: bool = None,
+            n_attempts: int = None):
+        """Set the default values of AutoNodeMoveParams.
 
         Parameters
         ----------
-        replace: bool, optional
-            Option to replace existing edge zonelets with new extracted edge zonelets.
-        feature_angle: float, optional
-            Angle used to capture face features to be  extracted as edges.
-        separate_features: bool, optional
-            Option to separate extracted features.
-        separation_angle: float, optional
-            Angle used to separate extracted features.
-        disconnect_with_faces: bool, optional
-            Option to disconnect edges from faces. If false, edges remain connected to faces by sharing nodes.
-        label_name: str, optional
-            Label name to be assigned to extracted features.
+        quality_measure: CellQualityMeasure, optional
+            Specify cell quality measure to be used for volume mesh improvement. The default value for cell quality measure is skewness.
+        target_quality: float, optional
+            Specify target quality used for the mesh improvement based on specified quality measure.
+        dihedral_angle: float, optional
+            Dihedral angle used to mantain features of boundary face zonelets.
+        n_iterations_per_node: int, optional
+            Number of iterations per node to be moved.
+        restrict_boundary_nodes_along_surface: bool, optional
+            Option to restrict the movement of the boundary node to the plane containing the boundary faces sharing the boundary node.
+        n_attempts: int, optional
+            Number of attempts to improve specified quality measure by node movement.
         """
         args = locals()
-        [ExtractFeatureParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+        [AutoNodeMoveParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
     def print_default():
-        """Print the default values of ExtractFeatureParams.
+        """Print the default values of AutoNodeMoveParams.
 
         Examples
         --------
-        >>> ExtractFeatureParams.print_default()
+        >>> AutoNodeMoveParams.print_default()
         """
         message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in ExtractFeatureParams._default_params.items())
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in AutoNodeMoveParams._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
-        if self._replace is not None:
-            json_data["replace"] = self._replace
-        if self._feature_angle is not None:
-            json_data["featureAngle"] = self._feature_angle
-        if self._separate_features is not None:
-            json_data["separateFeatures"] = self._separate_features
-        if self._separation_angle is not None:
-            json_data["separationAngle"] = self._separation_angle
-        if self._disconnect_with_faces is not None:
-            json_data["disconnectWithFaces"] = self._disconnect_with_faces
-        if self._label_name is not None:
-            json_data["labelName"] = self._label_name
+        if self._quality_measure is not None:
+            json_data["qualityMeasure"] = self._quality_measure
+        if self._target_quality is not None:
+            json_data["targetQuality"] = self._target_quality
+        if self._dihedral_angle is not None:
+            json_data["dihedralAngle"] = self._dihedral_angle
+        if self._n_iterations_per_node is not None:
+            json_data["nIterationsPerNode"] = self._n_iterations_per_node
+        if self._restrict_boundary_nodes_along_surface is not None:
+            json_data["restrictBoundaryNodesAlongSurface"] = self._restrict_boundary_nodes_along_surface
+        if self._n_attempts is not None:
+            json_data["nAttempts"] = self._n_attempts
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "replace :  %s\nfeature_angle :  %s\nseparate_features :  %s\nseparation_angle :  %s\ndisconnect_with_faces :  %s\nlabel_name :  %s" % (self._replace, self._feature_angle, self._separate_features, self._separation_angle, self._disconnect_with_faces, self._label_name)
+        message = "quality_measure :  %s\ntarget_quality :  %s\ndihedral_angle :  %s\nn_iterations_per_node :  %s\nrestrict_boundary_nodes_along_surface :  %s\nn_attempts :  %s" % (self._quality_measure, self._target_quality, self._dihedral_angle, self._n_iterations_per_node, self._restrict_boundary_nodes_along_surface, self._n_attempts)
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
     @property
-    def replace(self) -> bool:
-        """Option to replace existing edge zonelets with new extracted edge zonelets.
+    def quality_measure(self) -> CellQualityMeasure:
+        """Specify cell quality measure to be used for volume mesh improvement. The default value for cell quality measure is skewness.
         """
-        return self._replace
+        return self._quality_measure
 
-    @replace.setter
-    def replace(self, value: bool):
-        self._replace = value
+    @quality_measure.setter
+    def quality_measure(self, value: CellQualityMeasure):
+        self._quality_measure = value
 
     @property
-    def feature_angle(self) -> float:
-        """Angle used to capture face features to be  extracted as edges.
+    def target_quality(self) -> float:
+        """Specify target quality used for the mesh improvement based on specified quality measure.
         """
-        return self._feature_angle
+        return self._target_quality
 
-    @feature_angle.setter
-    def feature_angle(self, value: float):
-        self._feature_angle = value
+    @target_quality.setter
+    def target_quality(self, value: float):
+        self._target_quality = value
 
     @property
-    def separate_features(self) -> bool:
-        """Option to separate extracted features.
+    def dihedral_angle(self) -> float:
+        """Dihedral angle used to mantain features of boundary face zonelets.
         """
-        return self._separate_features
+        return self._dihedral_angle
 
-    @separate_features.setter
-    def separate_features(self, value: bool):
-        self._separate_features = value
+    @dihedral_angle.setter
+    def dihedral_angle(self, value: float):
+        self._dihedral_angle = value
 
     @property
-    def separation_angle(self) -> float:
-        """Angle used to separate extracted features.
+    def n_iterations_per_node(self) -> int:
+        """Number of iterations per node to be moved.
         """
-        return self._separation_angle
+        return self._n_iterations_per_node
 
-    @separation_angle.setter
-    def separation_angle(self, value: float):
-        self._separation_angle = value
+    @n_iterations_per_node.setter
+    def n_iterations_per_node(self, value: int):
+        self._n_iterations_per_node = value
 
     @property
-    def disconnect_with_faces(self) -> bool:
-        """Option to disconnect edges from faces. If false, edges remain connected to faces by sharing nodes.
+    def restrict_boundary_nodes_along_surface(self) -> bool:
+        """Option to restrict the movement of the boundary node to the plane containing the boundary faces sharing the boundary node.
         """
-        return self._disconnect_with_faces
+        return self._restrict_boundary_nodes_along_surface
 
-    @disconnect_with_faces.setter
-    def disconnect_with_faces(self, value: bool):
-        self._disconnect_with_faces = value
+    @restrict_boundary_nodes_along_surface.setter
+    def restrict_boundary_nodes_along_surface(self, value: bool):
+        self._restrict_boundary_nodes_along_surface = value
 
     @property
-    def label_name(self) -> str:
-        """Label name to be assigned to extracted features.
+    def n_attempts(self) -> int:
+        """Number of attempts to improve specified quality measure by node movement.
         """
-        return self._label_name
+        return self._n_attempts
 
-    @label_name.setter
-    def label_name(self, value: str):
-        self._label_name = value
+    @n_attempts.setter
+    def n_attempts(self, value: int):
+        self._n_attempts = value
 
-class ExtractFeatureResults(CoreObject):
-    """Result of edge zonelet extraction by angle.
+class CheckMeshParams(CoreObject):
+    """Parameters used to check mesh.
     """
     _default_params = {}
 
     def __initialize(
-            self,
-            processing_time: float,
-            error_code: ErrorCode,
-            new_edge_zonelets: Iterable[int]):
-        self._processing_time = processing_time
-        self._error_code = ErrorCode(error_code)
-        self._new_edge_zonelets = new_edge_zonelets if isinstance(new_edge_zonelets, np.ndarray) else np.array(new_edge_zonelets, dtype=np.int32) if new_edge_zonelets is not None else None
+            self):
+        pass
 
     def __init__(
             self,
             model: CommunicationManager=None,
-            processing_time: float = None,
-            error_code: ErrorCode = None,
-            new_edge_zonelets: Iterable[int] = None,
             json_data : dict = None,
              **kwargs):
-        """Initializes the ExtractFeatureResults.
+        """Initializes the CheckMeshParams.
 
         Parameters
         ----------
         model: Model
-            Model to create a ExtractFeatureResults object with default parameters.
-        processing_time: float, optional
-            Time taken for edge extraction.
-        error_code: ErrorCode, optional
-            Error code returned by edge extraction function.
-        new_edge_zonelets: Iterable[int], optional
-            Ids of new edge zonelets extracted.
+            Model to create a CheckMeshParams object with default parameters.
         json_data: dict, optional
-            JSON dictionary to create a ExtractFeatureResults object with provided parameters.
+            JSON dictionary to create a CheckMeshParams object with provided parameters.
 
         Examples
         --------
-        >>> extract_feature_results = prime.ExtractFeatureResults(model = model)
+        >>> check_mesh_params = prime.CheckMeshParams(model = model)
         """
         if json_data:
-            self.__initialize(
-                json_data["processingTime"] if "processingTime" in json_data else None,
-                ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None),
-                json_data["newEdgeZonelets"] if "newEdgeZonelets" in json_data else None)
+            self.__initialize()
         else:
-            all_field_specified = all(arg is not None for arg in [processing_time, error_code, new_edge_zonelets])
+            all_field_specified = all(arg is not None for arg in [])
             if all_field_specified:
-                self.__initialize(
-                    processing_time,
-                    error_code,
-                    new_edge_zonelets)
+                self.__initialize()
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
-                    param_json = model._communicator.initialize_params(model, "ExtractFeatureResults")
-                    json_data = param_json["ExtractFeatureResults"] if "ExtractFeatureResults" in param_json else {}
-                    self.__initialize(
-                        processing_time if processing_time is not None else ( ExtractFeatureResults._default_params["processing_time"] if "processing_time" in ExtractFeatureResults._default_params else (json_data["processingTime"] if "processingTime" in json_data else None)),
-                        error_code if error_code is not None else ( ExtractFeatureResults._default_params["error_code"] if "error_code" in ExtractFeatureResults._default_params else ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None)),
-                        new_edge_zonelets if new_edge_zonelets is not None else ( ExtractFeatureResults._default_params["new_edge_zonelets"] if "new_edge_zonelets" in ExtractFeatureResults._default_params else (json_data["newEdgeZonelets"] if "newEdgeZonelets" in json_data else None)))
+                    param_json = model._communicator.initialize_params(model, "CheckMeshParams")
+                    json_data = param_json["CheckMeshParams"] if "CheckMeshParams" in param_json else {}
+                    self.__initialize()
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
-    def set_default(
-            processing_time: float = None,
-            error_code: ErrorCode = None,
-            new_edge_zonelets: Iterable[int] = None):
-        """Set the default values of ExtractFeatureResults.
+    def set_default():
+        """Set the default values of CheckMeshParams.
 
-        Parameters
-        ----------
-        processing_time: float, optional
-            Time taken for edge extraction.
-        error_code: ErrorCode, optional
-            Error code returned by edge extraction function.
-        new_edge_zonelets: Iterable[int], optional
-            Ids of new edge zonelets extracted.
         """
         args = locals()
-        [ExtractFeatureResults._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+        [CheckMeshParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
     def print_default():
-        """Print the default values of ExtractFeatureResults.
+        """Print the default values of CheckMeshParams.
 
         Examples
         --------
-        >>> ExtractFeatureResults.print_default()
+        >>> CheckMeshParams.print_default()
         """
         message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in ExtractFeatureResults._default_params.items())
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in CheckMeshParams._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
-        if self._processing_time is not None:
-            json_data["processingTime"] = self._processing_time
-        if self._error_code is not None:
-            json_data["errorCode"] = self._error_code
-        if self._new_edge_zonelets is not None:
-            json_data["newEdgeZonelets"] = self._new_edge_zonelets
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "processing_time :  %s\nerror_code :  %s\nnew_edge_zonelets :  %s" % (self._processing_time, self._error_code, self._new_edge_zonelets)
+        message = "" % ()
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
-    @property
-    def processing_time(self) -> float:
-        """Time taken for edge extraction.
-        """
-        return self._processing_time
-
-    @processing_time.setter
-    def processing_time(self, value: float):
-        self._processing_time = value
-
-    @property
-    def error_code(self) -> ErrorCode:
-        """Error code returned by edge extraction function.
-        """
-        return self._error_code
-
-    @error_code.setter
-    def error_code(self, value: ErrorCode):
-        self._error_code = value
-
-    @property
-    def new_edge_zonelets(self) -> Iterable[int]:
-        """Ids of new edge zonelets extracted.
-        """
-        return self._new_edge_zonelets
-
-    @new_edge_zonelets.setter
-    def new_edge_zonelets(self, value: Iterable[int]):
-        self._new_edge_zonelets = value
-
-class ExtractedFeatureIds(CoreObject):
-    """Contains ids of the features extracted.
+class VolumeMeshToolResults(CoreObject):
+    """Result associated with the volume mesh tool operation.
     """
     _default_params = {}
 
     def __initialize(
             self,
-            part_id: int,
-            new_edge_zonelets: Iterable[int]):
-        self._part_id = part_id
-        self._new_edge_zonelets = new_edge_zonelets if isinstance(new_edge_zonelets, np.ndarray) else np.array(new_edge_zonelets, dtype=np.int32) if new_edge_zonelets is not None else None
-
-    def __init__(
-            self,
-            model: CommunicationManager=None,
-            part_id: int = None,
-            new_edge_zonelets: Iterable[int] = None,
-            json_data : dict = None,
-             **kwargs):
-        """Initializes the ExtractedFeatureIds.
-
-        Parameters
-        ----------
-        model: Model
-            Model to create a ExtractedFeatureIds object with default parameters.
-        part_id: int, optional
-            Id of the part from which edge zonelets are extracted.
-        new_edge_zonelets: Iterable[int], optional
-            Ids of new edge zonelets extracted.
-        json_data: dict, optional
-            JSON dictionary to create a ExtractedFeatureIds object with provided parameters.
-
-        Examples
-        --------
-        >>> extracted_feature_ids = prime.ExtractedFeatureIds(model = model)
-        """
-        if json_data:
-            self.__initialize(
-                json_data["partId"] if "partId" in json_data else None,
-                json_data["newEdgeZonelets"] if "newEdgeZonelets" in json_data else None)
-        else:
-            all_field_specified = all(arg is not None for arg in [part_id, new_edge_zonelets])
-            if all_field_specified:
-                self.__initialize(
-                    part_id,
-                    new_edge_zonelets)
-            else:
-                if model is None:
-                    raise ValueError("Invalid assignment. Either pass model or specify all properties")
-                else:
-                    param_json = model._communicator.initialize_params(model, "ExtractedFeatureIds")
-                    json_data = param_json["ExtractedFeatureIds"] if "ExtractedFeatureIds" in param_json else {}
-                    self.__initialize(
-                        part_id if part_id is not None else ( ExtractedFeatureIds._default_params["part_id"] if "part_id" in ExtractedFeatureIds._default_params else (json_data["partId"] if "partId" in json_data else None)),
-                        new_edge_zonelets if new_edge_zonelets is not None else ( ExtractedFeatureIds._default_params["new_edge_zonelets"] if "new_edge_zonelets" in ExtractedFeatureIds._default_params else (json_data["newEdgeZonelets"] if "newEdgeZonelets" in json_data else None)))
-        self._custom_params = kwargs
-        if model is not None:
-            [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
-        [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
-        lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
-        self._freeze()
-
-    @staticmethod
-    def set_default(
-            part_id: int = None,
-            new_edge_zonelets: Iterable[int] = None):
-        """Set the default values of ExtractedFeatureIds.
-
-        Parameters
-        ----------
-        part_id: int, optional
-            Id of the part from which edge zonelets are extracted.
-        new_edge_zonelets: Iterable[int], optional
-            Ids of new edge zonelets extracted.
-        """
-        args = locals()
-        [ExtractedFeatureIds._default_params.update({ key: value }) for key, value in args.items() if value is not None]
-
-    @staticmethod
-    def print_default():
-        """Print the default values of ExtractedFeatureIds.
-
-        Examples
-        --------
-        >>> ExtractedFeatureIds.print_default()
-        """
-        message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in ExtractedFeatureIds._default_params.items())
-        print(message)
-
-    def _jsonify(self) -> Dict[str, Any]:
-        json_data = {}
-        if self._part_id is not None:
-            json_data["partId"] = self._part_id
-        if self._new_edge_zonelets is not None:
-            json_data["newEdgeZonelets"] = self._new_edge_zonelets
-        [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
-        return json_data
-
-    def __str__(self) -> str:
-        message = "part_id :  %s\nnew_edge_zonelets :  %s" % (self._part_id, self._new_edge_zonelets)
-        message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
-        return message
-
-    @property
-    def part_id(self) -> int:
-        """Id of the part from which edge zonelets are extracted.
-        """
-        return self._part_id
-
-    @part_id.setter
-    def part_id(self, value: int):
-        self._part_id = value
-
-    @property
-    def new_edge_zonelets(self) -> Iterable[int]:
-        """Ids of new edge zonelets extracted.
-        """
-        return self._new_edge_zonelets
-
-    @new_edge_zonelets.setter
-    def new_edge_zonelets(self, value: Iterable[int]):
-        self._new_edge_zonelets = value
-
-class CreateIntersectionEdgeLoopsParams(CoreObject):
-    """Parameters used to calculate edge loops created by intersection of two groups of face zonelets.
-    """
-    _default_params = {}
-
-    def __initialize(
-            self,
-            label_name: str):
-        self._label_name = label_name
+            error_code: ErrorCode):
+        self._error_code = ErrorCode(error_code)
 
     def __init__(
             self,
             model: CommunicationManager=None,
-            label_name: str = None,
+            error_code: ErrorCode = None,
             json_data : dict = None,
              **kwargs):
-        """Initializes the CreateIntersectionEdgeLoopsParams.
+        """Initializes the VolumeMeshToolResults.
 
         Parameters
         ----------
         model: Model
-            Model to create a CreateIntersectionEdgeLoopsParams object with default parameters.
-        label_name: str, optional
-            Label name to be assigned to extracted features.
+            Model to create a VolumeMeshToolResults object with default parameters.
+        error_code: ErrorCode, optional
+            Error code associated with the volume mesh tool operation.
         json_data: dict, optional
-            JSON dictionary to create a CreateIntersectionEdgeLoopsParams object with provided parameters.
+            JSON dictionary to create a VolumeMeshToolResults object with provided parameters.
 
         Examples
         --------
-        >>> create_intersection_edge_loops_params = prime.CreateIntersectionEdgeLoopsParams(model = model)
+        >>> volume_mesh_tool_results = prime.VolumeMeshToolResults(model = model)
         """
         if json_data:
             self.__initialize(
-                json_data["labelName"] if "labelName" in json_data else None)
+                ErrorCode(json_data["error_code"] if "error_code" in json_data else None))
         else:
-            all_field_specified = all(arg is not None for arg in [label_name])
+            all_field_specified = all(arg is not None for arg in [error_code])
             if all_field_specified:
                 self.__initialize(
-                    label_name)
+                    error_code)
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
-                    param_json = model._communicator.initialize_params(model, "CreateIntersectionEdgeLoopsParams")
-                    json_data = param_json["CreateIntersectionEdgeLoopsParams"] if "CreateIntersectionEdgeLoopsParams" in param_json else {}
+                    param_json = model._communicator.initialize_params(model, "VolumeMeshToolResults")
+                    json_data = param_json["VolumeMeshToolResults"] if "VolumeMeshToolResults" in param_json else {}
                     self.__initialize(
-                        label_name if label_name is not None else ( CreateIntersectionEdgeLoopsParams._default_params["label_name"] if "label_name" in CreateIntersectionEdgeLoopsParams._default_params else (json_data["labelName"] if "labelName" in json_data else None)))
+                        error_code if error_code is not None else ( VolumeMeshToolResults._default_params["error_code"] if "error_code" in VolumeMeshToolResults._default_params else ErrorCode(json_data["error_code"] if "error_code" in json_data else None)))
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
     def set_default(
-            label_name: str = None):
-        """Set the default values of CreateIntersectionEdgeLoopsParams.
+            error_code: ErrorCode = None):
+        """Set the default values of VolumeMeshToolResults.
 
         Parameters
         ----------
-        label_name: str, optional
-            Label name to be assigned to extracted features.
+        error_code: ErrorCode, optional
+            Error code associated with the volume mesh tool operation.
         """
         args = locals()
-        [CreateIntersectionEdgeLoopsParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+        [VolumeMeshToolResults._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
     def print_default():
-        """Print the default values of CreateIntersectionEdgeLoopsParams.
+        """Print the default values of VolumeMeshToolResults.
 
         Examples
         --------
-        >>> CreateIntersectionEdgeLoopsParams.print_default()
+        >>> VolumeMeshToolResults.print_default()
         """
         message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in CreateIntersectionEdgeLoopsParams._default_params.items())
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in VolumeMeshToolResults._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
-        if self._label_name is not None:
-            json_data["labelName"] = self._label_name
+        if self._error_code is not None:
+            json_data["error_code"] = self._error_code
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "label_name :  %s" % (self._label_name)
+        message = "error_code :  %s" % (self._error_code)
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
     @property
-    def label_name(self) -> str:
-        """Label name to be assigned to extracted features.
+    def error_code(self) -> ErrorCode:
+        """Error code associated with the volume mesh tool operation.
         """
-        return self._label_name
+        return self._error_code
 
-    @label_name.setter
-    def label_name(self, value: str):
-        self._label_name = value
+    @error_code.setter
+    def error_code(self, value: ErrorCode):
+        self._error_code = value
 
-class CreateIntersectionEdgeLoopsResults(CoreObject):
-    """Results for the edge loops created by intersection of two groups of face zonelets.
+class CheckMeshResults(CoreObject):
+    """Result associated with the check mesh operation.
     """
     _default_params = {}
 
     def __initialize(
             self,
-            processing_time: float,
+            has_non_positive_volumes: bool,
+            has_non_positive_areas: bool,
+            has_invalid_shape: bool,
+            has_left_handed_faces: bool,
             error_code: ErrorCode,
-            extracted_ids: List[ExtractedFeatureIds]):
-        self._processing_time = processing_time
+            warning_codes: List[WarningCode]):
+        self._has_non_positive_volumes = has_non_positive_volumes
+        self._has_non_positive_areas = has_non_positive_areas
+        self._has_invalid_shape = has_invalid_shape
+        self._has_left_handed_faces = has_left_handed_faces
         self._error_code = ErrorCode(error_code)
-        self._extracted_ids = extracted_ids
+        self._warning_codes = warning_codes
 
     def __init__(
             self,
             model: CommunicationManager=None,
-            processing_time: float = None,
+            has_non_positive_volumes: bool = None,
+            has_non_positive_areas: bool = None,
+            has_invalid_shape: bool = None,
+            has_left_handed_faces: bool = None,
             error_code: ErrorCode = None,
-            extracted_ids: List[ExtractedFeatureIds] = None,
+            warning_codes: List[WarningCode] = None,
             json_data : dict = None,
              **kwargs):
-        """Initializes the CreateIntersectionEdgeLoopsResults.
+        """Initializes the CheckMeshResults.
 
         Parameters
         ----------
         model: Model
-            Model to create a CreateIntersectionEdgeLoopsResults object with default parameters.
-        processing_time: float, optional
-            Time taken to extract edges formed by intersecting faces.
+            Model to create a CheckMeshResults object with default parameters.
+        has_non_positive_volumes: bool, optional
+            Indicates whether mesh has non positive volumes.
+        has_non_positive_areas: bool, optional
+            Indicates whether mesh has non positive areas.
+        has_invalid_shape: bool, optional
+            Indicates whether mesh has invalid shape.
+        has_left_handed_faces: bool, optional
+            Indicates whether mesh has left handed faces.
         error_code: ErrorCode, optional
-            Error code returned by edge extraction function.
-        extracted_ids: List[ExtractedFeatureIds], optional
-            List of ExtractedFeatureIds that contains ids of extracted edges.
+            Error code associated with the check grid operation.
+        warning_codes: List[WarningCode], optional
+            Warning codes associated with the check grid operation.
         json_data: dict, optional
-            JSON dictionary to create a CreateIntersectionEdgeLoopsResults object with provided parameters.
+            JSON dictionary to create a CheckMeshResults object with provided parameters.
 
         Examples
         --------
-        >>> create_intersection_edge_loops_results = prime.CreateIntersectionEdgeLoopsResults(model = model)
+        >>> check_mesh_results = prime.CheckMeshResults(model = model)
         """
         if json_data:
             self.__initialize(
-                json_data["processingTime"] if "processingTime" in json_data else None,
+                json_data["hasNonPositiveVolumes"] if "hasNonPositiveVolumes" in json_data else None,
+                json_data["hasNonPositiveAreas"] if "hasNonPositiveAreas" in json_data else None,
+                json_data["hasInvalidShape"] if "hasInvalidShape" in json_data else None,
+                json_data["hasLeftHandedFaces"] if "hasLeftHandedFaces" in json_data else None,
                 ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None),
-                [ExtractedFeatureIds(model = model, json_data = data) for data in json_data["extractedIds"]] if "extractedIds" in json_data else None)
+                [WarningCode(data) for data in json_data["warningCodes"]] if "warningCodes" in json_data else None)
         else:
-            all_field_specified = all(arg is not None for arg in [processing_time, error_code, extracted_ids])
+            all_field_specified = all(arg is not None for arg in [has_non_positive_volumes, has_non_positive_areas, has_invalid_shape, has_left_handed_faces, error_code, warning_codes])
             if all_field_specified:
                 self.__initialize(
-                    processing_time,
+                    has_non_positive_volumes,
+                    has_non_positive_areas,
+                    has_invalid_shape,
+                    has_left_handed_faces,
                     error_code,
-                    extracted_ids)
+                    warning_codes)
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
-                    param_json = model._communicator.initialize_params(model, "CreateIntersectionEdgeLoopsResults")
-                    json_data = param_json["CreateIntersectionEdgeLoopsResults"] if "CreateIntersectionEdgeLoopsResults" in param_json else {}
+                    param_json = model._communicator.initialize_params(model, "CheckMeshResults")
+                    json_data = param_json["CheckMeshResults"] if "CheckMeshResults" in param_json else {}
                     self.__initialize(
-                        processing_time if processing_time is not None else ( CreateIntersectionEdgeLoopsResults._default_params["processing_time"] if "processing_time" in CreateIntersectionEdgeLoopsResults._default_params else (json_data["processingTime"] if "processingTime" in json_data else None)),
-                        error_code if error_code is not None else ( CreateIntersectionEdgeLoopsResults._default_params["error_code"] if "error_code" in CreateIntersectionEdgeLoopsResults._default_params else ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None)),
-                        extracted_ids if extracted_ids is not None else ( CreateIntersectionEdgeLoopsResults._default_params["extracted_ids"] if "extracted_ids" in CreateIntersectionEdgeLoopsResults._default_params else [ExtractedFeatureIds(model = model, json_data = data) for data in (json_data["extractedIds"] if "extractedIds" in json_data else None)]))
+                        has_non_positive_volumes if has_non_positive_volumes is not None else ( CheckMeshResults._default_params["has_non_positive_volumes"] if "has_non_positive_volumes" in CheckMeshResults._default_params else (json_data["hasNonPositiveVolumes"] if "hasNonPositiveVolumes" in json_data else None)),
+                        has_non_positive_areas if has_non_positive_areas is not None else ( CheckMeshResults._default_params["has_non_positive_areas"] if "has_non_positive_areas" in CheckMeshResults._default_params else (json_data["hasNonPositiveAreas"] if "hasNonPositiveAreas" in json_data else None)),
+                        has_invalid_shape if has_invalid_shape is not None else ( CheckMeshResults._default_params["has_invalid_shape"] if "has_invalid_shape" in CheckMeshResults._default_params else (json_data["hasInvalidShape"] if "hasInvalidShape" in json_data else None)),
+                        has_left_handed_faces if has_left_handed_faces is not None else ( CheckMeshResults._default_params["has_left_handed_faces"] if "has_left_handed_faces" in CheckMeshResults._default_params else (json_data["hasLeftHandedFaces"] if "hasLeftHandedFaces" in json_data else None)),
+                        error_code if error_code is not None else ( CheckMeshResults._default_params["error_code"] if "error_code" in CheckMeshResults._default_params else ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None)),
+                        warning_codes if warning_codes is not None else ( CheckMeshResults._default_params["warning_codes"] if "warning_codes" in CheckMeshResults._default_params else [WarningCode(data) for data in (json_data["warningCodes"] if "warningCodes" in json_data else None)]))
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
     def set_default(
-            processing_time: float = None,
+            has_non_positive_volumes: bool = None,
+            has_non_positive_areas: bool = None,
+            has_invalid_shape: bool = None,
+            has_left_handed_faces: bool = None,
             error_code: ErrorCode = None,
-            extracted_ids: List[ExtractedFeatureIds] = None):
-        """Set the default values of CreateIntersectionEdgeLoopsResults.
+            warning_codes: List[WarningCode] = None):
+        """Set the default values of CheckMeshResults.
 
         Parameters
         ----------
-        processing_time: float, optional
-            Time taken to extract edges formed by intersecting faces.
+        has_non_positive_volumes: bool, optional
+            Indicates whether mesh has non positive volumes.
+        has_non_positive_areas: bool, optional
+            Indicates whether mesh has non positive areas.
+        has_invalid_shape: bool, optional
+            Indicates whether mesh has invalid shape.
+        has_left_handed_faces: bool, optional
+            Indicates whether mesh has left handed faces.
         error_code: ErrorCode, optional
-            Error code returned by edge extraction function.
-        extracted_ids: List[ExtractedFeatureIds], optional
-            List of ExtractedFeatureIds that contains ids of extracted edges.
+            Error code associated with the check grid operation.
+        warning_codes: List[WarningCode], optional
+            Warning codes associated with the check grid operation.
         """
         args = locals()
-        [CreateIntersectionEdgeLoopsResults._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+        [CheckMeshResults._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
     def print_default():
-        """Print the default values of CreateIntersectionEdgeLoopsResults.
+        """Print the default values of CheckMeshResults.
 
         Examples
         --------
-        >>> CreateIntersectionEdgeLoopsResults.print_default()
+        >>> CheckMeshResults.print_default()
         """
         message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in CreateIntersectionEdgeLoopsResults._default_params.items())
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in CheckMeshResults._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
-        if self._processing_time is not None:
-            json_data["processingTime"] = self._processing_time
+        if self._has_non_positive_volumes is not None:
+            json_data["hasNonPositiveVolumes"] = self._has_non_positive_volumes
+        if self._has_non_positive_areas is not None:
+            json_data["hasNonPositiveAreas"] = self._has_non_positive_areas
+        if self._has_invalid_shape is not None:
+            json_data["hasInvalidShape"] = self._has_invalid_shape
+        if self._has_left_handed_faces is not None:
+            json_data["hasLeftHandedFaces"] = self._has_left_handed_faces
         if self._error_code is not None:
             json_data["errorCode"] = self._error_code
-        if self._extracted_ids is not None:
-            json_data["extractedIds"] = [data._jsonify() for data in self._extracted_ids]
+        if self._warning_codes is not None:
+            json_data["warningCodes"] = [data for data in self._warning_codes]
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "processing_time :  %s\nerror_code :  %s\nextracted_ids :  %s" % (self._processing_time, self._error_code, '[' + ''.join('\n' + str(data) for data in self._extracted_ids) + ']')
+        message = "has_non_positive_volumes :  %s\nhas_non_positive_areas :  %s\nhas_invalid_shape :  %s\nhas_left_handed_faces :  %s\nerror_code :  %s\nwarning_codes :  %s" % (self._has_non_positive_volumes, self._has_non_positive_areas, self._has_invalid_shape, self._has_left_handed_faces, self._error_code, '[' + ''.join('\n' + str(data) for data in self._warning_codes) + ']')
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
     @property
-    def processing_time(self) -> float:
-        """Time taken to extract edges formed by intersecting faces.
+    def has_non_positive_volumes(self) -> bool:
+        """Indicates whether mesh has non positive volumes.
+        """
+        return self._has_non_positive_volumes
+
+    @has_non_positive_volumes.setter
+    def has_non_positive_volumes(self, value: bool):
+        self._has_non_positive_volumes = value
+
+    @property
+    def has_non_positive_areas(self) -> bool:
+        """Indicates whether mesh has non positive areas.
+        """
+        return self._has_non_positive_areas
+
+    @has_non_positive_areas.setter
+    def has_non_positive_areas(self, value: bool):
+        self._has_non_positive_areas = value
+
+    @property
+    def has_invalid_shape(self) -> bool:
+        """Indicates whether mesh has invalid shape.
+        """
+        return self._has_invalid_shape
+
+    @has_invalid_shape.setter
+    def has_invalid_shape(self, value: bool):
+        self._has_invalid_shape = value
+
+    @property
+    def has_left_handed_faces(self) -> bool:
+        """Indicates whether mesh has left handed faces.
         """
-        return self._processing_time
+        return self._has_left_handed_faces
 
-    @processing_time.setter
-    def processing_time(self, value: float):
-        self._processing_time = value
+    @has_left_handed_faces.setter
+    def has_left_handed_faces(self, value: bool):
+        self._has_left_handed_faces = value
 
     @property
     def error_code(self) -> ErrorCode:
-        """Error code returned by edge extraction function.
+        """Error code associated with the check grid operation.
         """
         return self._error_code
 
     @error_code.setter
     def error_code(self, value: ErrorCode):
         self._error_code = value
 
     @property
-    def extracted_ids(self) -> List[ExtractedFeatureIds]:
-        """List of ExtractedFeatureIds that contains ids of extracted edges.
+    def warning_codes(self) -> List[WarningCode]:
+        """Warning codes associated with the check grid operation.
         """
-        return self._extracted_ids
+        return self._warning_codes
 
-    @extracted_ids.setter
-    def extracted_ids(self, value: List[ExtractedFeatureIds]):
-        self._extracted_ids = value
+    @warning_codes.setter
+    def warning_codes(self, value: List[WarningCode]):
+        self._warning_codes = value
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/fileio.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/sizecontrol.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,487 +1,463 @@
 """ Auto-generated file. DO NOT MODIFY """
 from __future__ import annotations
 from ansys.meshing.prime.internals.comm_manager import CommunicationManager
 from ansys.meshing.prime.params.primestructs import *
 from ansys.meshing.prime.autogen.coreobject import *
 from typing import List, Any, Union
 
-class FileIO(CoreObject):
-    """Handles reading or writing files from the disk.
+class SizeControl(CoreObject):
+    """Size control is used to compute the size field.
 
+    The size field is computed based on the size control defined.
+    Different type of size controls provide control over how the mesh size is distributed on a surface or within the volume.
     """
 
-    def __init__(self, model: CommunicationManager):
-        """ Initialize FileIO """
+    def __init__(self, model: CommunicationManager, id: int, object_id: int, name: str):
+        """ Initialize SizeControl """
         self._model = model
         self._comm = model._communicator
-        command_name = "PrimeMesh::FileIO/Construct"
-        args = {"ModelID" : model._object_id , "MaxID" : -1 }
-        result = self._comm.serve(model, command_name, args=args)
-        self._object_id = result["ObjectIndex"]
+        self._id = id
+        self._object_id = object_id
+        self._name = name
         self._freeze()
 
-    def __enter__(self):
-        """ Enter context for FileIO. """
-        return self
-
-    def __exit__(self, type, value, traceback) :
-        """ Exit context for FileIO. """
-        command_name = "PrimeMesh::FileIO/Destruct"
-        self._comm.serve(self._model, command_name, self._object_id, args={})
+    def set_curvature_sizing_params(self, params : CurvatureSizingParams) -> SetSizingResults:
+        """ Set the curvature sizing parameters to compute volumetric size field.
 
-    def read_pmdat(self, file_name : str, file_read_params : FileReadParams) -> FileReadResults:
-        """ Function that reads PRIME's database file.
-
-        PRIME's database files have pmdat extension.
 
         Parameters
         ----------
-        file_name : str
-            Path to file on disk.
-        file_read_params : FileReadParams
-            Parameter to read a file.
+        params : CurvatureSizingParams
+            Parameters that enables you to set the normal angle as the maximum allowable angle at which one element edge may span.
 
         Returns
         -------
-        FileReadResults
-            Returns FileReadResults.
-
+        SetSizingResults
+            Return the SetSizingResults.
 
-        Notes
-        -----
-        This API does not support Unicode paths now.
 
         Examples
         --------
-        >>> import ansys.meshing.prime as prime
-        >>> #connect client to server and get model from it
-        >>> client = prime.Client(ip="localhost", port=50060)
-        >>> model = client.model
-        >>> file_io = prime.FileIO(model = model)
-        >>> file_read_params = prime.FileReadParams(model = model)
-        >>> results = file_io.read_pmdat("/tmp/file.pmdat", file_read_params)
+        >>> size_control.set_curvature_sizing_params(
+        >>>                  prime.CurvatureSizingParams(model=model,
+        >>>                  min = 0.1, max = 1.0, growth_rate = 1.2,
+        >>>                  normal_angle = 18))
 
         """
-        args = {"file_name" : file_name,
-        "file_read_params" : file_read_params._jsonify()}
-        command_name = "PrimeMesh::FileIO/ReadPMDAT"
-        self._model._print_logs_before_command("read_pmdat", args)
+        if not isinstance(params, CurvatureSizingParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is CurvatureSizingParams.")
+        args = {"params" : params._jsonify()}
+        command_name = "PrimeMesh::SizeControl/SetCurvatureSizingParams"
+        self._model._print_logs_before_command("set_curvature_sizing_params", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("read_pmdat", FileReadResults(model = self._model, json_data = result))
-        return FileReadResults(model = self._model, json_data = result)
+        self._model._print_logs_after_command("set_curvature_sizing_params", SetSizingResults(model = self._model, json_data = result))
+        return SetSizingResults(model = self._model, json_data = result)
 
-    def write_pmdat(self, file_name : str, file_write_params : FileWriteParams) -> FileWriteResults:
-        """ Writes Prime mesh data file. Prime mesh data files have .pmdat extension.
+    def set_soft_sizing_params(self, params : SoftSizingParams) -> SetSizingResults:
+        """ Set the soft sizing parameters to compute volumetric size field.
 
 
         Parameters
         ----------
-        file_name : str
-            Path to write file on disk.
-        file_write_params : FileWriteParams
-            Parameters to write Prime mesh data file.
+        params : SoftSizingParams
+            Parameters that enables you to set the maximum size on scoped face zonelets.
 
         Returns
         -------
-        FileWriteResults
-            Returns the FileWriteResults structure.
+        SetSizingResults
+            Return the SetSizingResults.
 
 
         Examples
         --------
-        >>> results = file_io.write_pmdat("/tmp/prime_mesh_data.pmdat", prime.FileWriteParams(model = model))
+        >>> size_control.set_soft_sizing_params(
+        >>>                  prime.SoftSizingParams(model=model,
+        >>>                  max = 1.0, growth_rate = 1.2))
 
         """
-        args = {"file_name" : file_name,
-        "file_write_params" : file_write_params._jsonify()}
-        command_name = "PrimeMesh::FileIO/WritePMDAT"
-        self._model._print_logs_before_command("write_pmdat", args)
+        if not isinstance(params, SoftSizingParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is SoftSizingParams.")
+        args = {"params" : params._jsonify()}
+        command_name = "PrimeMesh::SizeControl/SetSoftSizingParams"
+        self._model._print_logs_before_command("set_soft_sizing_params", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("write_pmdat", FileWriteResults(model = self._model, json_data = result))
-        return FileWriteResults(model = self._model, json_data = result)
+        self._model._print_logs_after_command("set_soft_sizing_params", SetSizingResults(model = self._model, json_data = result))
+        return SetSizingResults(model = self._model, json_data = result)
 
-    def import_fluent_meshing_size_field(self, file_name : str) -> SizeFieldFileReadResults:
-        """ Import Fluent-Meshing's sizefield file from disk.
+    def set_proximity_sizing_params(self, params : ProximitySizingParams) -> SetSizingResults:
+        """ Set the proximity sizing parameters to compute volumetric size field.
 
-        Fluent-Meshing's sizefield files have sf and sf.gz extension.
 
         Parameters
         ----------
-        file_name : str
-            Path to file on disk
+        params : ProximitySizingParams
+            Parameters that enables you to specify number of elements in the gaps.
 
         Returns
         -------
-        SizeFieldFileReadResults
-            Return the SizeFieldFileReadResults.
+        SetSizingResults
+            Return the SetSizingResults.
 
 
-        Notes
-        -----
-        This API does not support Unicode paths now.
-
         Examples
         --------
-        >>> file_io = prime.FileIO(model = model)
-        >>> results = file_io.import_fluent_meshing_size_field("/tmp/my_sizefield.sf")
+        >>> size_control.set_proximity_sizing_params(
+        >>>                  prime.ProximitySizingParams(model=model,
+        >>>                  min = 0.1, max = 1.0, growth_rate = 1.2))
 
         """
-        args = {"file_name" : file_name}
-        command_name = "PrimeMesh::FileIO/ImportFluentMeshingSizeField"
-        self._model._print_logs_before_command("import_fluent_meshing_size_field", args)
+        if not isinstance(params, ProximitySizingParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is ProximitySizingParams.")
+        args = {"params" : params._jsonify()}
+        command_name = "PrimeMesh::SizeControl/SetProximitySizingParams"
+        self._model._print_logs_before_command("set_proximity_sizing_params", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("import_fluent_meshing_size_field", SizeFieldFileReadResults(model = self._model, json_data = result))
-        return SizeFieldFileReadResults(model = self._model, json_data = result)
+        self._model._print_logs_after_command("set_proximity_sizing_params", SetSizingResults(model = self._model, json_data = result))
+        return SetSizingResults(model = self._model, json_data = result)
 
-    def read_size_field(self, file_name : str, params : ReadSizeFieldParams) -> SizeFieldFileReadResults:
-        """ Read PRIME's sizefield file from disk.
+    def set_hard_sizing_params(self, params : HardSizingParams) -> SetSizingResults:
+        """ Set the hard sizing parameters to compute volumetric size field.
 
-        PRIME's sizefield files have psf and psf.gz extension.
 
         Parameters
         ----------
-        file_name : str
-            Path to file on disk.
-        params : ReadSizeFieldParams
-            Parameters to read size field file.
+        params : HardSizingParams
+            Parameters that enables you to set uniform size based on the specified size.
 
         Returns
         -------
-        SizeFieldFileReadResults
-            Return the SizeFieldFileReadResults.
-
+        SetSizingResults
+            Return the SetSizingResults.
 
-        Notes
-        -----
-        This API does not support Unicode paths now.
 
         Examples
         --------
-        >>> file_io = prime.FileIO(model = model)
-        >>> params = prime.ReadSizeFieldParams(model = model)
-        >>> results = file_io.read_size_field("/tmp/my_prime_sizefield.psf", params)
+        >>> size_control.set_hard_sizing_params(
+        >>>                  prime.HardSizingParams(model=model,
+        >>>                  min = 0.1, growth_rate = 1.2))
 
         """
-        args = {"file_name" : file_name,
-        "params" : params._jsonify()}
-        command_name = "PrimeMesh::FileIO/ReadSizeField"
-        self._model._print_logs_before_command("read_size_field", args)
+        if not isinstance(params, HardSizingParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is HardSizingParams.")
+        args = {"params" : params._jsonify()}
+        command_name = "PrimeMesh::SizeControl/SetHardSizingParams"
+        self._model._print_logs_before_command("set_hard_sizing_params", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("read_size_field", SizeFieldFileReadResults(model = self._model, json_data = result))
-        return SizeFieldFileReadResults(model = self._model, json_data = result)
+        self._model._print_logs_after_command("set_hard_sizing_params", SetSizingResults(model = self._model, json_data = result))
+        return SetSizingResults(model = self._model, json_data = result)
 
-    def write_size_field(self, file_name : str, params : WriteSizeFieldParams) -> FileWriteResults:
-        """ Write PRIME's sizefield (.psf) to file.
+    def set_meshed_sizing_params(self, params : MeshedSizingParams) -> SetSizingResults:
+        """ Set the meshed sizing parameters to compute volumetric size field.
 
 
         Parameters
         ----------
-        file_name : str
-            Path to file on disk.
-        params : WriteSizeFieldParams
-            Parameters to write size field file.
+        params : MeshedSizingParams
+            Parameters that enables you to set the sizes based on existing sizes.
 
         Returns
         -------
-        FileWriteResults
-            Return the FileWriteResults.
+        SetSizingResults
+            Return the SetSizingResults.
 
 
-        Notes
-        -----
-        This API does not support Unicode paths now.
-
         Examples
         --------
-        >>> file_io = prime.FileIO(model = model)
-        >>> params = prime.WriteSizeFieldParams(model = model)
-        >>> results = file_io.write_size_field("/tmp/my_prime_sizefield.psf", params)
+        >>> size_control.set_meshed_sizing_params(
+        >>>                  prime.MeshedSizingParams(model=model,
+        >>>                  growth_rate = 1.2))
 
         """
-        args = {"file_name" : file_name,
-        "params" : params._jsonify()}
-        command_name = "PrimeMesh::FileIO/WriteSizeField"
-        self._model._print_logs_before_command("write_size_field", args)
+        if not isinstance(params, MeshedSizingParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is MeshedSizingParams.")
+        args = {"params" : params._jsonify()}
+        command_name = "PrimeMesh::SizeControl/SetMeshedSizingParams"
+        self._model._print_logs_before_command("set_meshed_sizing_params", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("write_size_field", FileWriteResults(model = self._model, json_data = result))
-        return FileWriteResults(model = self._model, json_data = result)
+        self._model._print_logs_after_command("set_meshed_sizing_params", SetSizingResults(model = self._model, json_data = result))
+        return SetSizingResults(model = self._model, json_data = result)
 
-    def import_mapdl_cdb(self, file_name : str, params : ImportMapdlCdbParams) -> ImportMapdlCdbResults:
-        """ Function that imports MAPDL CDB file(cdb).
+    def set_boi_sizing_params(self, params : BoiSizingParams) -> SetSizingResults:
+        """ Set the body of influence sizing parameters to compute volumetric size field.
 
 
         Parameters
         ----------
-        file_name : str
-            Path to file on disk.
-        params : ImportMapdlCdbParams
-            Parameter to import a CDB file.
+        params : BoiSizingParams
+            Parameters that enables you to set sizing on the body of influence region.
 
         Returns
         -------
-        ImportMapdlCdbResults
-            Returns ImportMapdlCdbResults.
-
+        SetSizingResults
+            Return the SetSizingResults.
 
-        Notes
-        -----
-        This API does not support Unicode paths now.
 
         Examples
         --------
-        >>> import ansys.meshing.prime as prime
-        >>> #connect client to server and get model from it
-        >>> client = prime.Client(ip="localhost", port=50060)
-        >>> model = client.model
-        >>> file_io = prime.FileIO(model = model)
-        >>> params = prime.ImportMapdlCdbParams(model = model)
-        >>> results = file_io.import_mapdl_cdb("/tmp/file.cdb", params)
+        >>> size_control.set_boi_sizing_params(
+        >>>                  prime.BoiSizingParams(model=model,
+        >>>                  max = 0.1, growth_rate = 1.2))
 
         """
-        args = {"file_name" : file_name,
-        "params" : params._jsonify()}
-        command_name = "PrimeMesh::FileIO/ImportMapdlCdb"
-        self._model._print_logs_before_command("import_mapdl_cdb", args)
+        if not isinstance(params, BoiSizingParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is BoiSizingParams.")
+        args = {"params" : params._jsonify()}
+        command_name = "PrimeMesh::SizeControl/SetBoiSizingParams"
+        self._model._print_logs_before_command("set_boi_sizing_params", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("import_mapdl_cdb", ImportMapdlCdbResults(model = self._model, json_data = result))
-        return ImportMapdlCdbResults(model = self._model, json_data = result)
-
-    def export_mapdl_cdb(self, file_name : str, params : ExportMapdlCdbParams) -> ExportMapdlCdbResults:
-        """ Function that exports MAPDL CDB file(cdb).
+        self._model._print_logs_after_command("set_boi_sizing_params", SetSizingResults(model = self._model, json_data = result))
+        return SetSizingResults(model = self._model, json_data = result)
 
+    def get_curvature_sizing_params(self) -> CurvatureSizingParams:
+        """ Get the curvature sizing parameters of size control.
 
-        Parameters
-        ----------
-        file_name : str
-            Path to file on disk.
-        params : ExportMapdlCdbParams
-            Parameter to export a CDB file.
 
         Returns
         -------
-        ExportMapdlCdbResults
-            Returns ExportMapdlCdbResults.
+        CurvatureSizingParams
+            Return the CurvatureSizingParams.
 
 
-        Notes
-        -----
-        This API does not support Unicode paths now.
-
         Examples
         --------
-        >>> import ansys.meshing.prime as prime
-        >>> #connect client to server and get model from it
-        >>> client = prime.Client(ip="localhost", port=50060)
-        >>> model = client.model
-        >>> file_io = prime.FileIO(model = model)
-        >>> params = prime.ExportMapdlCdbParams(model = model)
-        >>> results = file_io.export_mapdl_cdb("/tmp/file.cdb", params)
+        >>> params = size_control.get_curvature_sizing_params()
 
         """
-        args = {"file_name" : file_name,
-        "params" : params._jsonify()}
-        command_name = "PrimeMesh::FileIO/ExportMapdlCdb"
-        self._model._print_logs_before_command("export_mapdl_cdb", args)
+        args = {}
+        command_name = "PrimeMesh::SizeControl/GetCurvatureSizingParams"
+        self._model._print_logs_before_command("get_curvature_sizing_params", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("export_mapdl_cdb", ExportMapdlCdbResults(model = self._model, json_data = result))
-        return ExportMapdlCdbResults(model = self._model, json_data = result)
+        self._model._print_logs_after_command("get_curvature_sizing_params", CurvatureSizingParams(model = self._model, json_data = result))
+        return CurvatureSizingParams(model = self._model, json_data = result)
 
-    def import_fluent_meshing_meshes(self, file_names : List[str], import_fluent_meshing_mesh_params : ImportFluentMeshingMeshParams) -> ImportFluentMeshingMeshResults:
-        """ Imports fluent meshing meshes of given files on disk.
+    def get_soft_sizing_params(self) -> SoftSizingParams:
+        """ Get the soft sizing parameters of size control.
 
-        Fluent Meshing mesh files have msh and msh.gz extension.
-
-        Parameters
-        ----------
-        file_names : List[str]
-            Full path of files to be imported.
-        import_fluent_meshing_mesh_params : ImportFluentMeshingMeshParams
-            Parameters to import fluent meshing mesh.
 
         Returns
         -------
-        ImportFluentMeshingMeshResults
-            Returns the FileReadResults.
+        SoftSizingParams
+            Return the SoftSizingParams.
+
+
+        Examples
+        --------
+        >>> params = size_control.get_soft_sizing_params()
+
+        """
+        args = {}
+        command_name = "PrimeMesh::SizeControl/GetSoftSizingParams"
+        self._model._print_logs_before_command("get_soft_sizing_params", args)
+        result = self._comm.serve(self._model, command_name, self._object_id, args=args)
+        self._model._print_logs_after_command("get_soft_sizing_params", SoftSizingParams(model = self._model, json_data = result))
+        return SoftSizingParams(model = self._model, json_data = result)
+
+    def get_proximity_sizing_params(self) -> ProximitySizingParams:
+        """ Get the proximity sizing parameters of size control.
 
 
-        Notes
-        -----
-        This API does not support Unicode paths now.
+        Returns
+        -------
+        ProximitySizingParams
+            Return the ProximitySizingParams.
+
 
         Examples
         --------
-        >>> file_io = prime.FileIO(model = model)
-        >>> params = prime.ImportFluentMeshingMeshParams(model = model)
-        >>> results = file_io.import_fluent_meshing_meshes(["/tmp/mesh.msh", "/tmp/mesh1.msh"], params)
+        >>> params = size_control.get_proximity_sizing_params()
 
         """
-        args = {"file_names" : file_names,
-        "import_fluent_meshing_mesh_params" : import_fluent_meshing_mesh_params._jsonify()}
-        command_name = "PrimeMesh::FileIO/ImportFluentMeshingMeshes"
-        self._model._print_logs_before_command("import_fluent_meshing_meshes", args)
+        args = {}
+        command_name = "PrimeMesh::SizeControl/GetProximitySizingParams"
+        self._model._print_logs_before_command("get_proximity_sizing_params", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("import_fluent_meshing_meshes", ImportFluentMeshingMeshResults(model = self._model, json_data = result))
-        return ImportFluentMeshingMeshResults(model = self._model, json_data = result)
+        self._model._print_logs_after_command("get_proximity_sizing_params", ProximitySizingParams(model = self._model, json_data = result))
+        return ProximitySizingParams(model = self._model, json_data = result)
 
-    def import_fluent_case(self, file_name : str, import_fluent_case_params : ImportFluentCaseParams) -> ImportFluentCaseResults:
-        """ Imports fluent case file on disk.
+    def get_hard_sizing_params(self) -> HardSizingParams:
+        """ Get the hard sizing parameters of size control.
 
-        Fluent case files have cas extension.
 
-        Parameters
-        ----------
-        file_name : str
-            Path to file on disk.
-        import_fluent_case_params : ImportFluentCaseParams
-            Parameters to import fluent case file.
+        Returns
+        -------
+        HardSizingParams
+            Return the HardSizingParams.
+
+
+        Examples
+        --------
+        >>> params = size_control.get_hard_sizing_params()
+
+        """
+        args = {}
+        command_name = "PrimeMesh::SizeControl/GetHardSizingParams"
+        self._model._print_logs_before_command("get_hard_sizing_params", args)
+        result = self._comm.serve(self._model, command_name, self._object_id, args=args)
+        self._model._print_logs_after_command("get_hard_sizing_params", HardSizingParams(model = self._model, json_data = result))
+        return HardSizingParams(model = self._model, json_data = result)
+
+    def get_meshed_sizing_params(self) -> MeshedSizingParams:
+        """ Get the meshed sizing parameters of size control.
+
 
         Returns
         -------
-        ImportFluentCaseResults
-            Returns the ImportFluentCaseResults.
+        MeshedSizingParams
+            Return the MeshedSizingParams.
+
+
+        Examples
+        --------
+        >>> params = size_control.get_meshed_sizing_params()
+
+        """
+        args = {}
+        command_name = "PrimeMesh::SizeControl/GetMeshedSizingParams"
+        self._model._print_logs_before_command("get_meshed_sizing_params", args)
+        result = self._comm.serve(self._model, command_name, self._object_id, args=args)
+        self._model._print_logs_after_command("get_meshed_sizing_params", MeshedSizingParams(model = self._model, json_data = result))
+        return MeshedSizingParams(model = self._model, json_data = result)
 
+    def get_boi_sizing_params(self) -> BoiSizingParams:
+        """ Get the body of influence sizing parameters of size control.
+
+
+        Returns
+        -------
+        BoiSizingParams
+            Return the BoiSizingParams.
 
-        Notes
-        -----
-        This API does not support unicode paths now.
 
         Examples
         --------
-        >>> file_io = prime.FileIO(model = model)
-        >>> params = prime.ImportFluentCaseParams(model = model)
-        >>> results = file_io.import_fluent_case("/tmp/fluent.cas", params)
+        >>> params = size_control.get_boi_sizing_params()
 
         """
-        args = {"file_name" : file_name,
-        "import_fluent_case_params" : import_fluent_case_params._jsonify()}
-        command_name = "PrimeMesh::FileIO/ImportFluentCase"
-        self._model._print_logs_before_command("import_fluent_case", args)
+        args = {}
+        command_name = "PrimeMesh::SizeControl/GetBoiSizingParams"
+        self._model._print_logs_before_command("get_boi_sizing_params", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("import_fluent_case", ImportFluentCaseResults(model = self._model, json_data = result))
-        return ImportFluentCaseResults(model = self._model, json_data = result)
+        self._model._print_logs_after_command("get_boi_sizing_params", BoiSizingParams(model = self._model, json_data = result))
+        return BoiSizingParams(model = self._model, json_data = result)
 
-    def export_fluent_case(self, file_name : str, export_fluent_case_params : ExportFluentCaseParams) -> FileWriteResults:
-        """ Exports Fluent case file. Fluent case files have cas extension.
+    def set_suggested_name(self, name : str) -> SetNameResults:
+        """ Set the unique name for the size control based on the given suggested name.
 
 
         Parameters
         ----------
-        file_name : str
-            Path to file on disk.
-        export_fluent_case_params : ExportFluentCaseParams
-            Parameters to export fluent case file.
+        name : str
+            Suggested name for the size control.
 
         Returns
         -------
-        FileWriteResults
-            Returns the FileWriteResults structure.
+        SetNameResults
+            Return a name of the size control.
 
 
         Examples
         --------
-        >>> file_io = FileIO(model = model)
-        >>> results = file_io.export_fluent_case("/tmp/fluent.cas", prime.ExportFluentCaseParams(model = model))
+        >>> size_control.set_suggested_name("control1")
 
         """
-        args = {"file_name" : file_name,
-        "export_fluent_case_params" : export_fluent_case_params._jsonify()}
-        command_name = "PrimeMesh::FileIO/ExportFluentCase"
-        self._model._print_logs_before_command("export_fluent_case", args)
+        if not isinstance(name, str):
+            raise TypeError("Invalid argument type passed for name, valid argument type is str.")
+        args = {"name" : name}
+        command_name = "PrimeMesh::SizeControl/SetSuggestedName"
+        self._model._print_logs_before_command("set_suggested_name", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("export_fluent_case", FileWriteResults(model = self._model, json_data = result))
-        return FileWriteResults(model = self._model, json_data = result)
+        self._model._print_logs_after_command("set_suggested_name", SetNameResults(model = self._model, json_data = result))
+        return SetNameResults(model = self._model, json_data = result)
 
-    def export_fluent_meshing_mesh(self, file_name : str, export_fluent_mesh_params : ExportFluentMeshingMeshParams) -> FileWriteResults:
-        """ Export Fluent Meshing mesh file. Fluent Meshing mesh files have .msh extension.
+    def set_scope(self, scope : ScopeDefinition) -> SetScopeResults:
+        """ Set the scope for size control to evaluate.
 
+        Size control uses scope to evaluate entities for which size field needs to be computed.
 
         Parameters
         ----------
-        file_name : str
-            Path to file on disk.
-        export_fluent_mesh_params : ExportFluentMeshingMeshParams
-            Parameters to export Fluent Meshing mesh file.
+        scope : ScopeDefinition
+            ScopeDefinition to scope entities for size field computation.
 
         Returns
         -------
-        FileWriteResults
-            Returns the FileWriteResults structure.
+        SetScopeResults
+            Return a SetScopeResults.
 
 
         Examples
         --------
-        >>> results = file_io.export_fluent_meshing_mesh("/tmp/fluent_meshing.msh", ExportFluentMeshingMeshParams(model = model))
+        >>> size_control.set_scope(prime.ScopeDefinition(model=model,
+        >>>                        entity_type = ScopeEntity.FACEZONELETS,
+        >>>                        evaluation_type = ScopeEvaluationType.LABELS,
+        >>>                        label_expression = "inlet"))
 
         """
-        args = {"file_name" : file_name,
-        "export_fluent_mesh_params" : export_fluent_mesh_params._jsonify()}
-        command_name = "PrimeMesh::FileIO/ExportFluentMeshingMesh"
-        self._model._print_logs_before_command("export_fluent_meshing_mesh", args)
+        if not isinstance(scope, ScopeDefinition):
+            raise TypeError("Invalid argument type passed for scope, valid argument type is ScopeDefinition.")
+        args = {"scope" : scope._jsonify()}
+        command_name = "PrimeMesh::SizeControl/SetScope"
+        self._model._print_logs_before_command("set_scope", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("export_fluent_meshing_mesh", FileWriteResults(model = self._model, json_data = result))
-        return FileWriteResults(model = self._model, json_data = result)
-
-    def export_boundary_fitted_spline_kfile(self, file_name : str, export_params : ExportBoundaryFittedSplineParams) -> FileWriteResults:
-        """ Export IGA LS-DYNA Keyword file for boundary fitted spline.
+        self._model._print_logs_after_command("set_scope", SetScopeResults(model = self._model, json_data = result))
+        return SetScopeResults(model = self._model, json_data = result)
 
+    def get_scope(self) -> ScopeDefinition:
+        """ Get the scope used by size control to evaluate entities.
 
-        Parameters
-        ----------
-        file_name : str
-            Name of the file.
-        export_params : ExportBoundaryFittedSplineParams
-            Parameters for IGA LS-DYNA Keyword file export.
 
         Returns
         -------
-        FileWriteResults
-            Returns FileWriteResults.
+        ScopeDefinition
+            Return the ScopeDefinition.
+
 
         Examples
         --------
-        >>> results = file_io.export_boundary_fitted_spline_k_file(file_name, ExportBoundaryFittedSplineParams(model = model))
+        >>> scope = size_control.get_scope()
 
         """
-        args = {"file_name" : file_name,
-        "export_params" : export_params._jsonify()}
-        command_name = "PrimeMesh::FileIO/ExportBoundaryFittedSplineKFile"
-        self._model._print_logs_before_command("export_boundary_fitted_spline_kfile", args)
+        args = {}
+        command_name = "PrimeMesh::SizeControl/GetScope"
+        self._model._print_logs_before_command("get_scope", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("export_boundary_fitted_spline_kfile", FileWriteResults(model = self._model, json_data = result))
-        return FileWriteResults(model = self._model, json_data = result)
+        self._model._print_logs_after_command("get_scope", ScopeDefinition(model = self._model, json_data = result))
+        return ScopeDefinition(model = self._model, json_data = result)
 
-    def import_cad(self, file_name : str, import_cad_params : ImportCadParams) -> ImportCadResults:
-        """ Imports CAD file from disk.
+    def get_summary(self, params : SizeControlSummaryParams) -> SizeControlSummaryResult:
+        """ Get the size control summary along with the evaluated scope for the provided parameters..
 
 
         Parameters
         ----------
-        file_name : str
-            Path to file on disk.
-        import_cad_params : ImportCadParams
-            Parameters to control CAD import options.
+        params : SizeControlSummaryParams
+            Size control summary parameters.
 
         Returns
         -------
-        ImportCadResults
-            Returns the ImportCadResults.
-
-
-        Notes
-        -----
-        This API does not support Unicode paths now.
+        SizeControlSummaryResult
+            Return the SizeControlSummaryResult.
 
         Examples
         --------
-        >>> file_io = prime.FileIO(model = model)
-        >>> params = prime.ImportCadParams(model = model)
-        >>> results = file_io.import_cad(file_name="/tmp/my_cad.x_t", import_cad_params=params)
+        >>> results = size_control.get_summary(prime.SizeControlSummaryParams(model=model))
 
         """
-        args = {"file_name" : file_name,
-        "import_cad_params" : import_cad_params._jsonify()}
-        command_name = "PrimeMesh::FileIO/ImportCAD"
-        self._model._print_logs_before_command("import_cad", args)
+        if not isinstance(params, SizeControlSummaryParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is SizeControlSummaryParams.")
+        args = {"params" : params._jsonify()}
+        command_name = "PrimeMesh::SizeControl/GetSummary"
+        self._model._print_logs_before_command("get_summary", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("import_cad", ImportCadResults(model = self._model, json_data = result))
-        return ImportCadResults(model = self._model, json_data = result)
+        self._model._print_logs_after_command("get_summary", SizeControlSummaryResult(model = self._model, json_data = result))
+        return SizeControlSummaryResult(model = self._model, json_data = result)
+
+    @property
+    def id(self):
+        """ Get the id of SizeControl."""
+        return self._id
+
+    @property
+    def name(self):
+        """ Get the name of SizeControl."""
+        return self._name
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/fileiostructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/fileiostructs.py`

 * *Files 6% similar despite different names*

```diff
@@ -936,14 +936,115 @@
         return json_data
 
     def __str__(self) -> str:
         message = "" % ()
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
+class ExportSTLParams(CoreObject):
+    """Parameters to export STL file.
+    """
+    _default_params = {}
+
+    def __initialize(
+            self,
+            part_ids: Iterable[int]):
+        self._part_ids = part_ids if isinstance(part_ids, np.ndarray) else np.array(part_ids, dtype=np.int32) if part_ids is not None else None
+
+    def __init__(
+            self,
+            model: CommunicationManager=None,
+            part_ids: Iterable[int] = None,
+            json_data : dict = None,
+             **kwargs):
+        """Initializes the ExportSTLParams.
+
+        Parameters
+        ----------
+        model: Model
+            Model to create a ExportSTLParams object with default parameters.
+        part_ids: Iterable[int], optional
+            Ids of parts to export.
+        json_data: dict, optional
+            JSON dictionary to create a ExportSTLParams object with provided parameters.
+
+        Examples
+        --------
+        >>> export_stlparams = prime.ExportSTLParams(model = model)
+        """
+        if json_data:
+            self.__initialize(
+                json_data["partIds"] if "partIds" in json_data else None)
+        else:
+            all_field_specified = all(arg is not None for arg in [part_ids])
+            if all_field_specified:
+                self.__initialize(
+                    part_ids)
+            else:
+                if model is None:
+                    raise ValueError("Invalid assignment. Either pass model or specify all properties")
+                else:
+                    param_json = model._communicator.initialize_params(model, "ExportSTLParams")
+                    json_data = param_json["ExportSTLParams"] if "ExportSTLParams" in param_json else {}
+                    self.__initialize(
+                        part_ids if part_ids is not None else ( ExportSTLParams._default_params["part_ids"] if "part_ids" in ExportSTLParams._default_params else (json_data["partIds"] if "partIds" in json_data else None)))
+        self._custom_params = kwargs
+        if model is not None:
+            [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
+        [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
+        lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
+        self._freeze()
+
+    @staticmethod
+    def set_default(
+            part_ids: Iterable[int] = None):
+        """Set the default values of ExportSTLParams.
+
+        Parameters
+        ----------
+        part_ids: Iterable[int], optional
+            Ids of parts to export.
+        """
+        args = locals()
+        [ExportSTLParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+
+    @staticmethod
+    def print_default():
+        """Print the default values of ExportSTLParams.
+
+        Examples
+        --------
+        >>> ExportSTLParams.print_default()
+        """
+        message = ""
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in ExportSTLParams._default_params.items())
+        print(message)
+
+    def _jsonify(self) -> Dict[str, Any]:
+        json_data = {}
+        if self._part_ids is not None:
+            json_data["partIds"] = self._part_ids
+        [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
+        return json_data
+
+    def __str__(self) -> str:
+        message = "part_ids :  %s" % (self._part_ids)
+        message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
+        return message
+
+    @property
+    def part_ids(self) -> Iterable[int]:
+        """Ids of parts to export.
+        """
+        return self._part_ids
+
+    @part_ids.setter
+    def part_ids(self, value: Iterable[int]):
+        self._part_ids = value
+
 class CadRefacetingParams(CoreObject):
     """Parameters to refacet CAD during import.
     """
     _default_params = {}
 
     def __initialize(
             self,
@@ -2412,14 +2513,339 @@
         """
         return self._error_code
 
     @error_code.setter
     def error_code(self, value: ErrorCode):
         self._error_code = value
 
+class ImportLSDynaKeywordFileParams(CoreObject):
+    """Parameters to control LS-DYNA keyword file import settings.
+    """
+    _default_params = {}
+
+    def __initialize(
+            self,
+            drop_mid_nodes: bool,
+            append: bool):
+        self._drop_mid_nodes = drop_mid_nodes
+        self._append = append
+
+    def __init__(
+            self,
+            model: CommunicationManager=None,
+            drop_mid_nodes: bool = None,
+            append: bool = None,
+            json_data : dict = None,
+             **kwargs):
+        """Initializes the ImportLSDynaKeywordFileParams.
+
+        Parameters
+        ----------
+        model: Model
+            Model to create a ImportLSDynaKeywordFileParams object with default parameters.
+        drop_mid_nodes: bool, optional
+            Option to import quadratic mesh elements as linear skipping the mid nodes.
+        append: bool, optional
+            Option to append imported k file into existing model.
+        json_data: dict, optional
+            JSON dictionary to create a ImportLSDynaKeywordFileParams object with provided parameters.
+
+        Examples
+        --------
+        >>> import_lsdyna_keyword_file_params = prime.ImportLSDynaKeywordFileParams(model = model)
+        """
+        if json_data:
+            self.__initialize(
+                json_data["dropMidNodes"] if "dropMidNodes" in json_data else None,
+                json_data["append"] if "append" in json_data else None)
+        else:
+            all_field_specified = all(arg is not None for arg in [drop_mid_nodes, append])
+            if all_field_specified:
+                self.__initialize(
+                    drop_mid_nodes,
+                    append)
+            else:
+                if model is None:
+                    raise ValueError("Invalid assignment. Either pass model or specify all properties")
+                else:
+                    param_json = model._communicator.initialize_params(model, "ImportLSDynaKeywordFileParams")
+                    json_data = param_json["ImportLSDynaKeywordFileParams"] if "ImportLSDynaKeywordFileParams" in param_json else {}
+                    self.__initialize(
+                        drop_mid_nodes if drop_mid_nodes is not None else ( ImportLSDynaKeywordFileParams._default_params["drop_mid_nodes"] if "drop_mid_nodes" in ImportLSDynaKeywordFileParams._default_params else (json_data["dropMidNodes"] if "dropMidNodes" in json_data else None)),
+                        append if append is not None else ( ImportLSDynaKeywordFileParams._default_params["append"] if "append" in ImportLSDynaKeywordFileParams._default_params else (json_data["append"] if "append" in json_data else None)))
+        self._custom_params = kwargs
+        if model is not None:
+            [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
+        [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
+        lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
+        self._freeze()
+
+    @staticmethod
+    def set_default(
+            drop_mid_nodes: bool = None,
+            append: bool = None):
+        """Set the default values of ImportLSDynaKeywordFileParams.
+
+        Parameters
+        ----------
+        drop_mid_nodes: bool, optional
+            Option to import quadratic mesh elements as linear skipping the mid nodes.
+        append: bool, optional
+            Option to append imported k file into existing model.
+        """
+        args = locals()
+        [ImportLSDynaKeywordFileParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+
+    @staticmethod
+    def print_default():
+        """Print the default values of ImportLSDynaKeywordFileParams.
+
+        Examples
+        --------
+        >>> ImportLSDynaKeywordFileParams.print_default()
+        """
+        message = ""
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in ImportLSDynaKeywordFileParams._default_params.items())
+        print(message)
+
+    def _jsonify(self) -> Dict[str, Any]:
+        json_data = {}
+        if self._drop_mid_nodes is not None:
+            json_data["dropMidNodes"] = self._drop_mid_nodes
+        if self._append is not None:
+            json_data["append"] = self._append
+        [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
+        return json_data
+
+    def __str__(self) -> str:
+        message = "drop_mid_nodes :  %s\nappend :  %s" % (self._drop_mid_nodes, self._append)
+        message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
+        return message
+
+    @property
+    def drop_mid_nodes(self) -> bool:
+        """Option to import quadratic mesh elements as linear skipping the mid nodes.
+        """
+        return self._drop_mid_nodes
+
+    @drop_mid_nodes.setter
+    def drop_mid_nodes(self, value: bool):
+        self._drop_mid_nodes = value
+
+    @property
+    def append(self) -> bool:
+        """Option to append imported k file into existing model.
+        """
+        return self._append
+
+    @append.setter
+    def append(self, value: bool):
+        self._append = value
+
+class ExportLSDynaKeywordFileParams(CoreObject):
+    """Parameters to control LS-DYNA keyword file export settings.
+    """
+    _default_params = {}
+
+    def __initialize(
+            self,
+            part_ids: Iterable[int]):
+        self._part_ids = part_ids if isinstance(part_ids, np.ndarray) else np.array(part_ids, dtype=np.int32) if part_ids is not None else None
+
+    def __init__(
+            self,
+            model: CommunicationManager=None,
+            part_ids: Iterable[int] = None,
+            json_data : dict = None,
+             **kwargs):
+        """Initializes the ExportLSDynaKeywordFileParams.
+
+        Parameters
+        ----------
+        model: Model
+            Model to create a ExportLSDynaKeywordFileParams object with default parameters.
+        part_ids: Iterable[int], optional
+            Option to export only specified parts.
+        json_data: dict, optional
+            JSON dictionary to create a ExportLSDynaKeywordFileParams object with provided parameters.
+
+        Examples
+        --------
+        >>> export_lsdyna_keyword_file_params = prime.ExportLSDynaKeywordFileParams(model = model)
+        """
+        if json_data:
+            self.__initialize(
+                json_data["partIds"] if "partIds" in json_data else None)
+        else:
+            all_field_specified = all(arg is not None for arg in [part_ids])
+            if all_field_specified:
+                self.__initialize(
+                    part_ids)
+            else:
+                if model is None:
+                    raise ValueError("Invalid assignment. Either pass model or specify all properties")
+                else:
+                    param_json = model._communicator.initialize_params(model, "ExportLSDynaKeywordFileParams")
+                    json_data = param_json["ExportLSDynaKeywordFileParams"] if "ExportLSDynaKeywordFileParams" in param_json else {}
+                    self.__initialize(
+                        part_ids if part_ids is not None else ( ExportLSDynaKeywordFileParams._default_params["part_ids"] if "part_ids" in ExportLSDynaKeywordFileParams._default_params else (json_data["partIds"] if "partIds" in json_data else None)))
+        self._custom_params = kwargs
+        if model is not None:
+            [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
+        [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
+        lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
+        self._freeze()
+
+    @staticmethod
+    def set_default(
+            part_ids: Iterable[int] = None):
+        """Set the default values of ExportLSDynaKeywordFileParams.
+
+        Parameters
+        ----------
+        part_ids: Iterable[int], optional
+            Option to export only specified parts.
+        """
+        args = locals()
+        [ExportLSDynaKeywordFileParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+
+    @staticmethod
+    def print_default():
+        """Print the default values of ExportLSDynaKeywordFileParams.
+
+        Examples
+        --------
+        >>> ExportLSDynaKeywordFileParams.print_default()
+        """
+        message = ""
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in ExportLSDynaKeywordFileParams._default_params.items())
+        print(message)
+
+    def _jsonify(self) -> Dict[str, Any]:
+        json_data = {}
+        if self._part_ids is not None:
+            json_data["partIds"] = self._part_ids
+        [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
+        return json_data
+
+    def __str__(self) -> str:
+        message = "part_ids :  %s" % (self._part_ids)
+        message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
+        return message
+
+    @property
+    def part_ids(self) -> Iterable[int]:
+        """Option to export only specified parts.
+        """
+        return self._part_ids
+
+    @part_ids.setter
+    def part_ids(self, value: Iterable[int]):
+        self._part_ids = value
+
+class ExportLSDynaIgaKeywordFileParams(CoreObject):
+    """Parameters for exporting LS-Dyna IGA keyword file.
+    """
+    _default_params = {}
+
+    def __initialize(
+            self,
+            part_ids: Iterable[int]):
+        self._part_ids = part_ids if isinstance(part_ids, np.ndarray) else np.array(part_ids, dtype=np.int32) if part_ids is not None else None
+
+    def __init__(
+            self,
+            model: CommunicationManager=None,
+            part_ids: Iterable[int] = None,
+            json_data : dict = None,
+             **kwargs):
+        """Initializes the ExportLSDynaIgaKeywordFileParams.
+
+        Parameters
+        ----------
+        model: Model
+            Model to create a ExportLSDynaIgaKeywordFileParams object with default parameters.
+        part_ids: Iterable[int], optional
+        json_data: dict, optional
+            JSON dictionary to create a ExportLSDynaIgaKeywordFileParams object with provided parameters.
+
+        Examples
+        --------
+        >>> export_lsdyna_iga_keyword_file_params = prime.ExportLSDynaIgaKeywordFileParams(model = model)
+        """
+        if json_data:
+            self.__initialize(
+                json_data["partIds"] if "partIds" in json_data else None)
+        else:
+            all_field_specified = all(arg is not None for arg in [part_ids])
+            if all_field_specified:
+                self.__initialize(
+                    part_ids)
+            else:
+                if model is None:
+                    raise ValueError("Invalid assignment. Either pass model or specify all properties")
+                else:
+                    param_json = model._communicator.initialize_params(model, "ExportLSDynaIgaKeywordFileParams")
+                    json_data = param_json["ExportLSDynaIgaKeywordFileParams"] if "ExportLSDynaIgaKeywordFileParams" in param_json else {}
+                    self.__initialize(
+                        part_ids if part_ids is not None else ( ExportLSDynaIgaKeywordFileParams._default_params["part_ids"] if "part_ids" in ExportLSDynaIgaKeywordFileParams._default_params else (json_data["partIds"] if "partIds" in json_data else None)))
+        self._custom_params = kwargs
+        if model is not None:
+            [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
+        [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
+        lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
+        self._freeze()
+
+    @staticmethod
+    def set_default(
+            part_ids: Iterable[int] = None):
+        """Set the default values of ExportLSDynaIgaKeywordFileParams.
+
+        Parameters
+        ----------
+        part_ids: Iterable[int], optional
+        """
+        args = locals()
+        [ExportLSDynaIgaKeywordFileParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+
+    @staticmethod
+    def print_default():
+        """Print the default values of ExportLSDynaIgaKeywordFileParams.
+
+        Examples
+        --------
+        >>> ExportLSDynaIgaKeywordFileParams.print_default()
+        """
+        message = ""
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in ExportLSDynaIgaKeywordFileParams._default_params.items())
+        print(message)
+
+    def _jsonify(self) -> Dict[str, Any]:
+        json_data = {}
+        if self._part_ids is not None:
+            json_data["partIds"] = self._part_ids
+        [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
+        return json_data
+
+    def __str__(self) -> str:
+        message = "part_ids :  %s" % (self._part_ids)
+        message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
+        return message
+
+    @property
+    def part_ids(self) -> Iterable[int]:
+        """
+        Option to export only specified parts.
+        """
+        return self._part_ids
+
+    @part_ids.setter
+    def part_ids(self, value: Iterable[int]):
+        self._part_ids = value
+
 class ExportBoundaryFittedSplineParams(CoreObject):
     """Parameters for exporting boundary fitted splines.
     """
     _default_params = {}
 
     def __initialize(
             self,
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/materialpointmanager.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/materialpointmanager.py`

 * *Files 24% similar despite different names*

```diff
@@ -42,14 +42,20 @@
         A material point is created on calling this API.
 
         Examples
         --------
         >>> material_point_results = model.control_data.create_material_point("Fluid", [1.0,2,0,3.0], params)
 
         """
+        if not isinstance(suggested_name, str):
+            raise TypeError("Invalid argument type passed for suggested_name, valid argument type is str.")
+        if not isinstance(coords, Iterable):
+            raise TypeError("Invalid argument type passed for coords, valid argument type is Iterable[float].")
+        if not isinstance(params, CreateMaterialPointParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is CreateMaterialPointParams.")
         args = {"suggested_name" : suggested_name,
         "coords" : coords,
         "params" : params._jsonify()}
         command_name = "PrimeMesh::MaterialPointManager/CreateMaterialPoint"
         self._model._print_logs_before_command("create_material_point", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("create_material_point", CreateMaterialPointResults(model = self._model, json_data = result))
@@ -72,14 +78,16 @@
 
         Examples
         --------
         >>> model = prime.local_model()
         >>> results = model.material_point_data.delete_material_point("fluid")
 
         """
+        if not isinstance(name, str):
+            raise TypeError("Invalid argument type passed for name, valid argument type is str.")
         args = {"name" : name}
         command_name = "PrimeMesh::MaterialPointManager/DeleteMaterialPoint"
         self._model._print_logs_before_command("delete_material_point", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("delete_material_point", DeleteMaterialPointResults(model = self._model, json_data = result))
         return DeleteMaterialPointResults(model = self._model, json_data = result)
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/materialpointmanagerstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/meshinfo.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/meshinfo.py`

 * *Files 18% similar despite different names*

```diff
@@ -52,14 +52,18 @@
         --------
         >>> mesh_info = prime.MeshInfo(model)
         >>> part_ids = [part.id for part in model.parts]
         >>> result = mesh_info.get_face_and_edge_connectivity(part_ids,
         >>>                  prime.FaceAndEdgeConnectivityParams(model =model))
 
         """
+        if not isinstance(part_ids, Iterable):
+            raise TypeError("Invalid argument type passed for part_ids, valid argument type is Iterable[int].")
+        if not isinstance(params, FaceAndEdgeConnectivityParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is FaceAndEdgeConnectivityParams.")
         args = {"part_ids" : part_ids,
         "params" : params._jsonify()}
         command_name = "PrimeMesh::MeshInfo/GetFaceAndEdgeConnectivity"
         self._model._print_logs_before_command("get_face_and_edge_connectivity", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("get_face_and_edge_connectivity", FaceAndEdgeConnectivityResults(model = self._model, json_data = result))
         return FaceAndEdgeConnectivityResults(model = self._model, json_data = result)
@@ -85,14 +89,18 @@
         --------
         >>> mesh_info = prime.MeshInfo(model)
         >>> part = model.get_part_by_name("part_name")
         >>> result = mesh_info.get_statistics_of_cell_zonelets(part.get_cell_zonelets(),
         >>>                  prime.CellStatisticsParams(model=model))
 
         """
+        if not isinstance(cell_zonelets, Iterable):
+            raise TypeError("Invalid argument type passed for cell_zonelets, valid argument type is Iterable[int].")
+        if not isinstance(params, CellStatisticsParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is CellStatisticsParams.")
         args = {"cell_zonelets" : cell_zonelets,
         "params" : params._jsonify()}
         command_name = "PrimeMesh::MeshInfo/GetStatisticsOfCellZonelets"
         self._model._print_logs_before_command("get_statistics_of_cell_zonelets", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("get_statistics_of_cell_zonelets", CellStatisticsResults(model = self._model, json_data = result))
         return CellStatisticsResults(model = self._model, json_data = result)
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/meshinfostructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/meshinfostructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/model.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 
 
         Examples
         --------
         >>> results = model.delete_parts(part_ids)
 
         """
+        if not isinstance(part_ids, Iterable):
+            raise TypeError("Invalid argument type passed for part_ids, valid argument type is Iterable[int].")
         args = {"part_ids" : part_ids}
         command_name = "PrimeMesh::Model/DeleteParts"
         self._print_logs_before_command("delete_parts", args)
         result = self._comm.serve(self, command_name, self._object_id, args=args)
         self._print_logs_after_command("delete_parts", DeleteResults(model = self, json_data = result))
         return DeleteResults(model = self, json_data = result)
 
@@ -75,14 +77,18 @@
 
         Examples
         --------
         >>> params = prime.MergePartsParams(model = model)
         >>> results = model.merge_parts(part_ids, params)
 
         """
+        if not isinstance(part_ids, Iterable):
+            raise TypeError("Invalid argument type passed for part_ids, valid argument type is Iterable[int].")
+        if not isinstance(params, MergePartsParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is MergePartsParams.")
         args = {"part_ids" : part_ids,
         "params" : params._jsonify()}
         command_name = "PrimeMesh::Model/MergeParts"
         self._print_logs_before_command("merge_parts", args)
         result = self._comm.serve(self, command_name, self._object_id, args=args)
         self._print_logs_after_command("merge_parts", MergePartsResults(model = self, json_data = result))
         return MergePartsResults(model = self, json_data = result)
@@ -100,14 +106,16 @@
         --------
         >>> model = client.model
         >>> model.set_global_sizing_params(
         >>>           prime.GlobalSizingParams(model=model,
         >>>           min = 0.1, max = 1.0, growth_rate = 1.2))
 
         """
+        if not isinstance(params, GlobalSizingParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is GlobalSizingParams.")
         args = {"params" : params._jsonify()}
         command_name = "PrimeMesh::Model/SetGlobalSizingParams"
         self._print_logs_before_command("set_global_sizing_params", args)
         result = self._comm.serve(self, command_name, self._object_id, args=args)
         self._print_logs_after_command("set_global_sizing_params", SetSizingResults(model = self, json_data = result))
         return SetSizingResults(model = self, json_data = result)
 
@@ -168,14 +176,16 @@
 
         Examples
         --------
         >>> model = client.model
         >>> model.activate_volumetric_size_fields(size_field_ids)
 
         """
+        if not isinstance(size_field_ids, Iterable):
+            raise TypeError("Invalid argument type passed for size_field_ids, valid argument type is Iterable[int].")
         args = {"size_field_ids" : size_field_ids}
         command_name = "PrimeMesh::Model/ActivateVolumetricSizeFields"
         self._print_logs_before_command("activate_volumetric_size_fields", args)
         self._comm.serve(self, command_name, self._object_id, args=args)
         self._print_logs_after_command("activate_volumetric_size_fields")
 
     def deactivate_volumetric_size_fields(self, size_field_ids : Iterable[int]):
@@ -189,14 +199,16 @@
 
         Examples
         --------
         >>> model = client.model
         >>> model.deactivate_volumetric_size_fields(size_field_ids)
 
         """
+        if not isinstance(size_field_ids, Iterable):
+            raise TypeError("Invalid argument type passed for size_field_ids, valid argument type is Iterable[int].")
         args = {"size_field_ids" : size_field_ids}
         command_name = "PrimeMesh::Model/DeactivateVolumetricSizeFields"
         self._print_logs_before_command("deactivate_volumetric_size_fields", args)
         self._comm.serve(self, command_name, self._object_id, args=args)
         self._print_logs_after_command("deactivate_volumetric_size_fields")
 
     def delete_volumetric_size_fields(self, size_field_ids : Iterable[int]):
@@ -210,14 +222,16 @@
 
         Examples
         --------
         >>> model = client.model
         >>> model.delete_volumetric_size_fields(size_field_ids)
 
         """
+        if not isinstance(size_field_ids, Iterable):
+            raise TypeError("Invalid argument type passed for size_field_ids, valid argument type is Iterable[int].")
         args = {"size_field_ids" : size_field_ids}
         command_name = "PrimeMesh::Model/DeleteVolumetricSizeFields"
         self._print_logs_before_command("delete_volumetric_size_fields", args)
         self._comm.serve(self, command_name, self._object_id, args=args)
         self._print_logs_after_command("delete_volumetric_size_fields")
 
     def set_num_threads(self, num : int):
@@ -231,14 +245,16 @@
 
         Examples
         --------
         >>> model = client.model
         >>> model.set_num_threads(4)
 
         """
+        if not isinstance(num, int):
+            raise TypeError("Invalid argument type passed for num, valid argument type is int.")
         args = {"num" : num}
         command_name = "PrimeMesh::Model/SetNumThreads"
         self._print_logs_before_command("set_num_threads", args)
         self._comm.serve(self, command_name, self._object_id, args=args)
         self._print_logs_after_command("set_num_threads")
 
     def get_num_threads(self) -> int:
@@ -299,14 +315,18 @@
 
         Examples
         --------
         >>> model = prime.local_model()
         >>> results = model.create_zone("wall", prime.ZoneType.FACE)
 
         """
+        if not isinstance(suggested_name, str):
+            raise TypeError("Invalid argument type passed for suggested_name, valid argument type is str.")
+        if not isinstance(type, ZoneType):
+            raise TypeError("Invalid argument type passed for type, valid argument type is ZoneType.")
         args = {"suggested_name" : suggested_name,
         "type" : type}
         command_name = "PrimeMesh::Model/CreateZone"
         self._print_logs_before_command("create_zone", args)
         result = self._comm.serve(self, command_name, self._object_id, args=args)
         self._print_logs_after_command("create_zone", CreateZoneResults(model = self, json_data = result))
         return CreateZoneResults(model = self, json_data = result)
@@ -328,14 +348,16 @@
 
         Examples
         --------
         >>> model = prime.local_model()
         >>> results = model.delete_zone(1)
 
         """
+        if not isinstance(zone_id, int):
+            raise TypeError("Invalid argument type passed for zone_id, valid argument type is int.")
         args = {"zone_id" : zone_id}
         command_name = "PrimeMesh::Model/DeleteZone"
         self._print_logs_before_command("delete_zone", args)
         result = self._comm.serve(self, command_name, self._object_id, args=args)
         self._print_logs_after_command("delete_zone", DeleteZoneResults(model = self, json_data = result))
         return DeleteZoneResults(model = self, json_data = result)
 
@@ -356,14 +378,16 @@
 
         Examples
         --------
         >>> model = prime.local_model()
         >>> zone_id = model.get_zone_by_name("inlet")
 
         """
+        if not isinstance(zone_name, str):
+            raise TypeError("Invalid argument type passed for zone_name, valid argument type is str.")
         args = {"zone_name" : zone_name}
         command_name = "PrimeMesh::Model/GetZoneByName"
         self._print_logs_before_command("get_zone_by_name", args)
         result = self._comm.serve(self, command_name, self._object_id, args=args)
         self._print_logs_after_command("get_zone_by_name")
         return result
 
@@ -384,14 +408,16 @@
 
         Examples
         --------
         >>> model = prime.local_model()
         >>> name = model.get_zone_name(id)
 
         """
+        if not isinstance(id, int):
+            raise TypeError("Invalid argument type passed for id, valid argument type is int.")
         args = {"id" : id}
         command_name = "PrimeMesh::Model/GetZoneName"
         self._print_logs_before_command("get_zone_name", args)
         result = self._comm.serve(self, command_name, self._object_id, args=args)
         self._print_logs_after_command("get_zone_name")
         return result
 
@@ -414,14 +440,18 @@
 
         Examples
         --------
         >>> model = prime.local_model()
         >>> results = model.set_suggested_zone_name(id = 5, name = "zone1")
 
         """
+        if not isinstance(id, int):
+            raise TypeError("Invalid argument type passed for id, valid argument type is int.")
+        if not isinstance(name, str):
+            raise TypeError("Invalid argument type passed for name, valid argument type is str.")
         args = {"id" : id,
         "name" : name}
         command_name = "PrimeMesh::Model/SetSuggestedZoneName"
         self._print_logs_before_command("set_suggested_zone_name", args)
         result = self._comm.serve(self, command_name, self._object_id, args=args)
         self._print_logs_after_command("set_suggested_zone_name", SetNameResults(model = self, json_data = result))
         return SetNameResults(model = self, json_data = result)
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/modelstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/modelstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/partstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/partstructs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9770,513 +9770,699 @@
 00026290: 654f 626a 6563 7429 3a0a 2020 2020 2222  eObject):.    ""
 000262a0: 2250 6172 616d 6574 6572 7320 746f 206d  "Parameters to m
 000262b0: 6572 6765 2076 6f6c 756d 6573 2e0a 2020  erge volumes..  
 000262c0: 2020 2222 220a 2020 2020 5f64 6566 6175    """.    _defau
 000262d0: 6c74 5f70 6172 616d 7320 3d20 7b7d 0a0a  lt_params = {}..
 000262e0: 2020 2020 6465 6620 5f5f 696e 6974 6961      def __initia
 000262f0: 6c69 7a65 280a 2020 2020 2020 2020 2020  lize(.          
-00026300: 2020 7365 6c66 293a 0a20 2020 2020 2020    self):.       
-00026310: 2070 6173 730a 0a20 2020 2064 6566 205f   pass..    def _
-00026320: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00026330: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00026340: 2020 2020 2020 206d 6f64 656c 3a20 436f         model: Co
-00026350: 6d6d 756e 6963 6174 696f 6e4d 616e 6167  mmunicationManag
-00026360: 6572 3d4e 6f6e 652c 0a20 2020 2020 2020  er=None,.       
-00026370: 2020 2020 206a 736f 6e5f 6461 7461 203a       json_data :
-00026380: 2064 6963 7420 3d20 4e6f 6e65 2c0a 2020   dict = None,.  
-00026390: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
-000263a0: 7267 7329 3a0a 2020 2020 2020 2020 2222  rgs):.        ""
-000263b0: 2249 6e69 7469 616c 697a 6573 2074 6865  "Initializes the
-000263c0: 204d 6572 6765 566f 6c75 6d65 7350 6172   MergeVolumesPar
-000263d0: 616d 732e 0a0a 2020 2020 2020 2020 5061  ams...        Pa
-000263e0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-000263f0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00026400: 2020 2020 6d6f 6465 6c3a 204d 6f64 656c      model: Model
-00026410: 0a20 2020 2020 2020 2020 2020 204d 6f64  .            Mod
-00026420: 656c 2074 6f20 6372 6561 7465 2061 204d  el to create a M
-00026430: 6572 6765 566f 6c75 6d65 7350 6172 616d  ergeVolumesParam
-00026440: 7320 6f62 6a65 6374 2077 6974 6820 6465  s object with de
-00026450: 6661 756c 7420 7061 7261 6d65 7465 7273  fault parameters
-00026460: 2e0a 2020 2020 2020 2020 6a73 6f6e 5f64  ..        json_d
-00026470: 6174 613a 2064 6963 742c 206f 7074 696f  ata: dict, optio
-00026480: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-00026490: 4a53 4f4e 2064 6963 7469 6f6e 6172 7920  JSON dictionary 
-000264a0: 746f 2063 7265 6174 6520 6120 4d65 7267  to create a Merg
-000264b0: 6556 6f6c 756d 6573 5061 7261 6d73 206f  eVolumesParams o
-000264c0: 626a 6563 7420 7769 7468 2070 726f 7669  bject with provi
-000264d0: 6465 6420 7061 7261 6d65 7465 7273 2e0a  ded parameters..
-000264e0: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-000264f0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00026500: 2d2d 0a20 2020 2020 2020 203e 3e3e 206d  --.        >>> m
-00026510: 6572 6765 5f76 6f6c 756d 6573 5f70 6172  erge_volumes_par
-00026520: 616d 7320 3d20 7072 696d 652e 4d65 7267  ams = prime.Merg
-00026530: 6556 6f6c 756d 6573 5061 7261 6d73 286d  eVolumesParams(m
-00026540: 6f64 656c 203d 206d 6f64 656c 290a 2020  odel = model).  
-00026550: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00026560: 2020 6966 206a 736f 6e5f 6461 7461 3a0a    if json_data:.
-00026570: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00026580: 2e5f 5f69 6e69 7469 616c 697a 6528 290a  .__initialize().
-00026590: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000265a0: 2020 2020 2020 2020 2020 616c 6c5f 6669            all_fi
-000265b0: 656c 645f 7370 6563 6966 6965 6420 3d20  eld_specified = 
-000265c0: 616c 6c28 6172 6720 6973 206e 6f74 204e  all(arg is not N
-000265d0: 6f6e 6520 666f 7220 6172 6720 696e 205b  one for arg in [
-000265e0: 5d29 0a20 2020 2020 2020 2020 2020 2069  ]).            i
-000265f0: 6620 616c 6c5f 6669 656c 645f 7370 6563  f all_field_spec
-00026600: 6966 6965 643a 0a20 2020 2020 2020 2020  ified:.         
-00026610: 2020 2020 2020 2073 656c 662e 5f5f 696e         self.__in
-00026620: 6974 6961 6c69 7a65 2829 0a20 2020 2020  itialize().     
-00026630: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00026640: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00026650: 6d6f 6465 6c20 6973 204e 6f6e 653a 0a20  model is None:. 
-00026660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026670: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00026680: 726f 7228 2249 6e76 616c 6964 2061 7373  ror("Invalid ass
-00026690: 6967 6e6d 656e 742e 2045 6974 6865 7220  ignment. Either 
-000266a0: 7061 7373 206d 6f64 656c 206f 7220 7370  pass model or sp
-000266b0: 6563 6966 7920 616c 6c20 7072 6f70 6572  ecify all proper
-000266c0: 7469 6573 2229 0a20 2020 2020 2020 2020  ties").         
-000266d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000266e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000266f0: 2070 6172 616d 5f6a 736f 6e20 3d20 6d6f   param_json = mo
-00026700: 6465 6c2e 5f63 6f6d 6d75 6e69 6361 746f  del._communicato
-00026710: 722e 696e 6974 6961 6c69 7a65 5f70 6172  r.initialize_par
-00026720: 616d 7328 6d6f 6465 6c2c 2022 4d65 7267  ams(model, "Merg
-00026730: 6556 6f6c 756d 6573 5061 7261 6d73 2229  eVolumesParams")
-00026740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00026750: 2020 2020 206a 736f 6e5f 6461 7461 203d       json_data =
-00026760: 2070 6172 616d 5f6a 736f 6e5b 224d 6572   param_json["Mer
-00026770: 6765 566f 6c75 6d65 7350 6172 616d 7322  geVolumesParams"
-00026780: 5d20 6966 2022 4d65 7267 6556 6f6c 756d  ] if "MergeVolum
-00026790: 6573 5061 7261 6d73 2220 696e 2070 6172  esParams" in par
-000267a0: 616d 5f6a 736f 6e20 656c 7365 207b 7d0a  am_json else {}.
-000267b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000267c0: 2020 2020 7365 6c66 2e5f 5f69 6e69 7469      self.__initi
-000267d0: 616c 697a 6528 290a 2020 2020 2020 2020  alize().        
-000267e0: 7365 6c66 2e5f 6375 7374 6f6d 5f70 6172  self._custom_par
-000267f0: 616d 7320 3d20 6b77 6172 6773 0a20 2020  ams = kwargs.   
-00026800: 2020 2020 2069 6620 6d6f 6465 6c20 6973       if model is
-00026810: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00026820: 2020 2020 2020 205b 206d 6f64 656c 2e5f         [ model._
-00026830: 6c6f 6767 6572 2e77 6172 6e69 6e67 2866  logger.warning(f
-00026840: 2755 6e73 7570 706f 7274 6564 2061 7267  'Unsupported arg
-00026850: 756d 656e 7420 3a20 7b6b 6579 7d27 2920  ument : {key}') 
-00026860: 666f 7220 6b65 7920 696e 206b 7761 7267  for key in kwarg
-00026870: 7320 5d0a 2020 2020 2020 2020 5b73 6574  s ].        [set
-00026880: 6174 7472 2874 7970 6528 7365 6c66 292c  attr(type(self),
-00026890: 206b 6579 2c20 7072 6f70 6572 7479 286c   key, property(l
-000268a0: 616d 6264 6120 7365 6c66 2c20 6b65 7920  ambda self, key 
-000268b0: 3d20 6b65 793a 2020 7365 6c66 2e5f 6375  = key:  self._cu
-000268c0: 7374 6f6d 5f70 6172 616d 735b 6b65 795d  stom_params[key]
-000268d0: 2069 6620 6b65 7920 696e 2073 656c 662e   if key in self.
-000268e0: 5f63 7573 746f 6d5f 7061 7261 6d73 2065  _custom_params e
-000268f0: 6c73 6520 4e6f 6e65 2c0a 2020 2020 2020  lse None,.      
-00026900: 2020 6c61 6d62 6461 2073 656c 662c 2076    lambda self, v
-00026910: 616c 7565 2c20 6b65 7920 3d20 6b65 7920  alue, key = key 
-00026920: 3a20 7365 6c66 2e5f 6375 7374 6f6d 5f70  : self._custom_p
-00026930: 6172 616d 732e 7570 6461 7465 287b 206b  arams.update({ k
-00026940: 6579 3a20 7661 6c75 6520 7d29 2929 2066  ey: value }))) f
-00026950: 6f72 206b 6579 2069 6e20 6b77 6172 6773  or key in kwargs
-00026960: 5d0a 2020 2020 2020 2020 7365 6c66 2e5f  ].        self._
-00026970: 6672 6565 7a65 2829 0a0a 2020 2020 4073  freeze()..    @s
-00026980: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
-00026990: 6465 6620 7365 745f 6465 6661 756c 7428  def set_default(
-000269a0: 293a 0a20 2020 2020 2020 2022 2222 5365  ):.        """Se
-000269b0: 7420 7468 6520 6465 6661 756c 7420 7661  t the default va
-000269c0: 6c75 6573 206f 6620 4d65 7267 6556 6f6c  lues of MergeVol
-000269d0: 756d 6573 5061 7261 6d73 2e0a 0a20 2020  umesParams...   
-000269e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000269f0: 2061 7267 7320 3d20 6c6f 6361 6c73 2829   args = locals()
-00026a00: 0a20 2020 2020 2020 205b 4d65 7267 6556  .        [MergeV
-00026a10: 6f6c 756d 6573 5061 7261 6d73 2e5f 6465  olumesParams._de
-00026a20: 6661 756c 745f 7061 7261 6d73 2e75 7064  fault_params.upd
-00026a30: 6174 6528 7b20 6b65 793a 2076 616c 7565  ate({ key: value
-00026a40: 207d 2920 666f 7220 6b65 792c 2076 616c   }) for key, val
-00026a50: 7565 2069 6e20 6172 6773 2e69 7465 6d73  ue in args.items
-00026a60: 2829 2069 6620 7661 6c75 6520 6973 206e  () if value is n
-00026a70: 6f74 204e 6f6e 655d 0a0a 2020 2020 4073  ot None]..    @s
-00026a80: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
-00026a90: 6465 6620 7072 696e 745f 6465 6661 756c  def print_defaul
-00026aa0: 7428 293a 0a20 2020 2020 2020 2022 2222  t():.        """
-00026ab0: 5072 696e 7420 7468 6520 6465 6661 756c  Print the defaul
-00026ac0: 7420 7661 6c75 6573 206f 6620 4d65 7267  t values of Merg
-00026ad0: 6556 6f6c 756d 6573 5061 7261 6d73 2e0a  eVolumesParams..
-00026ae0: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-00026af0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00026b00: 2d2d 0a20 2020 2020 2020 203e 3e3e 204d  --.        >>> M
+00026300: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00026310: 2020 2020 6d65 7267 655f 746f 5f6e 6569      merge_to_nei
+00026320: 6768 626f 725f 766f 6c75 6d65 3a20 626f  ghbor_volume: bo
+00026330: 6f6c 2c0a 2020 2020 2020 2020 2020 2020  ol,.            
+00026340: 6e65 6967 6862 6f72 5f76 6f6c 756d 6573  neighbor_volumes
+00026350: 3a20 4974 6572 6162 6c65 5b69 6e74 5d29  : Iterable[int])
+00026360: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00026370: 6d65 7267 655f 746f 5f6e 6569 6768 626f  merge_to_neighbo
+00026380: 725f 766f 6c75 6d65 203d 206d 6572 6765  r_volume = merge
+00026390: 5f74 6f5f 6e65 6967 6862 6f72 5f76 6f6c  _to_neighbor_vol
+000263a0: 756d 650a 2020 2020 2020 2020 7365 6c66  ume.        self
+000263b0: 2e5f 6e65 6967 6862 6f72 5f76 6f6c 756d  ._neighbor_volum
+000263c0: 6573 203d 206e 6569 6768 626f 725f 766f  es = neighbor_vo
+000263d0: 6c75 6d65 7320 6966 2069 7369 6e73 7461  lumes if isinsta
+000263e0: 6e63 6528 6e65 6967 6862 6f72 5f76 6f6c  nce(neighbor_vol
+000263f0: 756d 6573 2c20 6e70 2e6e 6461 7272 6179  umes, np.ndarray
+00026400: 2920 656c 7365 206e 702e 6172 7261 7928  ) else np.array(
+00026410: 6e65 6967 6862 6f72 5f76 6f6c 756d 6573  neighbor_volumes
+00026420: 2c20 6474 7970 653d 6e70 2e69 6e74 3332  , dtype=np.int32
+00026430: 2920 6966 206e 6569 6768 626f 725f 766f  ) if neighbor_vo
+00026440: 6c75 6d65 7320 6973 206e 6f74 204e 6f6e  lumes is not Non
+00026450: 6520 656c 7365 204e 6f6e 650a 0a20 2020  e else None..   
+00026460: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00026470: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+00026480: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
+00026490: 656c 3a20 436f 6d6d 756e 6963 6174 696f  el: Communicatio
+000264a0: 6e4d 616e 6167 6572 3d4e 6f6e 652c 0a20  nManager=None,. 
+000264b0: 2020 2020 2020 2020 2020 206d 6572 6765             merge
+000264c0: 5f74 6f5f 6e65 6967 6862 6f72 5f76 6f6c  _to_neighbor_vol
+000264d0: 756d 653a 2062 6f6f 6c20 3d20 4e6f 6e65  ume: bool = None
+000264e0: 2c0a 2020 2020 2020 2020 2020 2020 6e65  ,.            ne
+000264f0: 6967 6862 6f72 5f76 6f6c 756d 6573 3a20  ighbor_volumes: 
+00026500: 4974 6572 6162 6c65 5b69 6e74 5d20 3d20  Iterable[int] = 
+00026510: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00026520: 2020 6a73 6f6e 5f64 6174 6120 3a20 6469    json_data : di
+00026530: 6374 203d 204e 6f6e 652c 0a20 2020 2020  ct = None,.     
+00026540: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+00026550: 293a 0a20 2020 2020 2020 2022 2222 496e  ):.        """In
+00026560: 6974 6961 6c69 7a65 7320 7468 6520 4d65  itializes the Me
+00026570: 7267 6556 6f6c 756d 6573 5061 7261 6d73  rgeVolumesParams
+00026580: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00026590: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+000265a0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+000265b0: 206d 6f64 656c 3a20 4d6f 6465 6c0a 2020   model: Model.  
+000265c0: 2020 2020 2020 2020 2020 4d6f 6465 6c20            Model 
+000265d0: 746f 2063 7265 6174 6520 6120 4d65 7267  to create a Merg
+000265e0: 6556 6f6c 756d 6573 5061 7261 6d73 206f  eVolumesParams o
+000265f0: 626a 6563 7420 7769 7468 2064 6566 6175  bject with defau
+00026600: 6c74 2070 6172 616d 6574 6572 732e 0a20  lt parameters.. 
+00026610: 2020 2020 2020 206d 6572 6765 5f74 6f5f         merge_to_
+00026620: 6e65 6967 6862 6f72 5f76 6f6c 756d 653a  neighbor_volume:
+00026630: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0a   bool, optional.
+00026640: 2020 2020 2020 2020 2020 2020 4f70 7469              Opti
+00026650: 6f6e 2074 6f20 6d65 7267 6520 6769 7665  on to merge give
+00026660: 6e20 766f 6c75 6d65 7320 746f 2074 6865  n volumes to the
+00026670: 6972 206e 6569 6768 626f 7220 766f 6c75  ir neighbor volu
+00026680: 6d65 2e0a 2020 2020 2020 2020 6e65 6967  me..        neig
+00026690: 6862 6f72 5f76 6f6c 756d 6573 3a20 4974  hbor_volumes: It
+000266a0: 6572 6162 6c65 5b69 6e74 5d2c 206f 7074  erable[int], opt
+000266b0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+000266c0: 2020 4964 73c2 a06f 66c2 a076 6f6c 756d    Ids..of..volum
+000266d0: 6520 7468 6174 2061 7265 c2a0 6e65 6967  e that are..neig
+000266e0: 6862 6f72 73c2 a074 6fc2 a067 6976 656e  hbors..to..given
+000266f0: c2a0 766f 6c75 6d65 73c2 a066 6f72 c2a0  ..volumes..for..
+00026700: 6d65 7267 696e 672e 0a20 2020 2020 2020  merging..       
+00026710: 206a 736f 6e5f 6461 7461 3a20 6469 6374   json_data: dict
+00026720: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00026730: 2020 2020 2020 204a 534f 4e20 6469 6374         JSON dict
+00026740: 696f 6e61 7279 2074 6f20 6372 6561 7465  ionary to create
+00026750: 2061 204d 6572 6765 566f 6c75 6d65 7350   a MergeVolumesP
+00026760: 6172 616d 7320 6f62 6a65 6374 2077 6974  arams object wit
+00026770: 6820 7072 6f76 6964 6564 2070 6172 616d  h provided param
+00026780: 6574 6572 732e 0a0a 2020 2020 2020 2020  eters...        
+00026790: 4578 616d 706c 6573 0a20 2020 2020 2020  Examples.       
+000267a0: 202d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020   --------.      
+000267b0: 2020 3e3e 3e20 6d65 7267 655f 766f 6c75    >>> merge_volu
+000267c0: 6d65 735f 7061 7261 6d73 203d 2070 7269  mes_params = pri
+000267d0: 6d65 2e4d 6572 6765 566f 6c75 6d65 7350  me.MergeVolumesP
+000267e0: 6172 616d 7328 6d6f 6465 6c20 3d20 6d6f  arams(model = mo
+000267f0: 6465 6c29 0a20 2020 2020 2020 2022 2222  del).        """
+00026800: 0a20 2020 2020 2020 2069 6620 6a73 6f6e  .        if json
+00026810: 5f64 6174 613a 0a20 2020 2020 2020 2020  _data:.         
+00026820: 2020 2073 656c 662e 5f5f 696e 6974 6961     self.__initia
+00026830: 6c69 7a65 280a 2020 2020 2020 2020 2020  lize(.          
+00026840: 2020 2020 2020 6a73 6f6e 5f64 6174 615b        json_data[
+00026850: 226d 6572 6765 546f 4e65 6967 6862 6f72  "mergeToNeighbor
+00026860: 566f 6c75 6d65 225d 2069 6620 226d 6572  Volume"] if "mer
+00026870: 6765 546f 4e65 6967 6862 6f72 566f 6c75  geToNeighborVolu
+00026880: 6d65 2220 696e 206a 736f 6e5f 6461 7461  me" in json_data
+00026890: 2065 6c73 6520 4e6f 6e65 2c0a 2020 2020   else None,.    
+000268a0: 2020 2020 2020 2020 2020 2020 6a73 6f6e              json
+000268b0: 5f64 6174 615b 226e 6569 6768 626f 7256  _data["neighborV
+000268c0: 6f6c 756d 6573 225d 2069 6620 226e 6569  olumes"] if "nei
+000268d0: 6768 626f 7256 6f6c 756d 6573 2220 696e  ghborVolumes" in
+000268e0: 206a 736f 6e5f 6461 7461 2065 6c73 6520   json_data else 
+000268f0: 4e6f 6e65 290a 2020 2020 2020 2020 656c  None).        el
+00026900: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00026910: 616c 6c5f 6669 656c 645f 7370 6563 6966  all_field_specif
+00026920: 6965 6420 3d20 616c 6c28 6172 6720 6973  ied = all(arg is
+00026930: 206e 6f74 204e 6f6e 6520 666f 7220 6172   not None for ar
+00026940: 6720 696e 205b 6d65 7267 655f 746f 5f6e  g in [merge_to_n
+00026950: 6569 6768 626f 725f 766f 6c75 6d65 2c20  eighbor_volume, 
+00026960: 6e65 6967 6862 6f72 5f76 6f6c 756d 6573  neighbor_volumes
+00026970: 5d29 0a20 2020 2020 2020 2020 2020 2069  ]).            i
+00026980: 6620 616c 6c5f 6669 656c 645f 7370 6563  f all_field_spec
+00026990: 6966 6965 643a 0a20 2020 2020 2020 2020  ified:.         
+000269a0: 2020 2020 2020 2073 656c 662e 5f5f 696e         self.__in
+000269b0: 6974 6961 6c69 7a65 280a 2020 2020 2020  itialize(.      
+000269c0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+000269d0: 7267 655f 746f 5f6e 6569 6768 626f 725f  rge_to_neighbor_
+000269e0: 766f 6c75 6d65 2c0a 2020 2020 2020 2020  volume,.        
+000269f0: 2020 2020 2020 2020 2020 2020 6e65 6967              neig
+00026a00: 6862 6f72 5f76 6f6c 756d 6573 290a 2020  hbor_volumes).  
+00026a10: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00026a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026a30: 6966 206d 6f64 656c 2069 7320 4e6f 6e65  if model is None
+00026a40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00026a50: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00026a60: 6545 7272 6f72 2822 496e 7661 6c69 6420  eError("Invalid 
+00026a70: 6173 7369 676e 6d65 6e74 2e20 4569 7468  assignment. Eith
+00026a80: 6572 2070 6173 7320 6d6f 6465 6c20 6f72  er pass model or
+00026a90: 2073 7065 6369 6679 2061 6c6c 2070 726f   specify all pro
+00026aa0: 7065 7274 6965 7322 290a 2020 2020 2020  perties").      
+00026ab0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00026ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026ad0: 2020 2020 7061 7261 6d5f 6a73 6f6e 203d      param_json =
+00026ae0: 206d 6f64 656c 2e5f 636f 6d6d 756e 6963   model._communic
+00026af0: 6174 6f72 2e69 6e69 7469 616c 697a 655f  ator.initialize_
+00026b00: 7061 7261 6d73 286d 6f64 656c 2c20 224d  params(model, "M
 00026b10: 6572 6765 566f 6c75 6d65 7350 6172 616d  ergeVolumesParam
-00026b20: 732e 7072 696e 745f 6465 6661 756c 7428  s.print_default(
-00026b30: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
-00026b40: 2020 2020 2020 6d65 7373 6167 6520 3d20        message = 
-00026b50: 2222 0a20 2020 2020 2020 206d 6573 7361  "".        messa
-00026b60: 6765 202b 3d20 2727 2e6a 6f69 6e28 7374  ge += ''.join(st
-00026b70: 7228 6b65 7929 202b 2027 203a 2027 202b  r(key) + ' : ' +
-00026b80: 2073 7472 2876 616c 7565 2920 2b20 275c   str(value) + '\
-00026b90: 6e27 2066 6f72 206b 6579 2c20 7661 6c75  n' for key, valu
-00026ba0: 6520 696e 204d 6572 6765 566f 6c75 6d65  e in MergeVolume
-00026bb0: 7350 6172 616d 732e 5f64 6566 6175 6c74  sParams._default
-00026bc0: 5f70 6172 616d 732e 6974 656d 7328 2929  _params.items())
-00026bd0: 0a20 2020 2020 2020 2070 7269 6e74 286d  .        print(m
-00026be0: 6573 7361 6765 290a 0a20 2020 2064 6566  essage)..    def
-00026bf0: 205f 6a73 6f6e 6966 7928 7365 6c66 2920   _jsonify(self) 
-00026c00: 2d3e 2044 6963 745b 7374 722c 2041 6e79  -> Dict[str, Any
-00026c10: 5d3a 0a20 2020 2020 2020 206a 736f 6e5f  ]:.        json_
-00026c20: 6461 7461 203d 207b 7d0a 2020 2020 2020  data = {}.      
-00026c30: 2020 5b20 6a73 6f6e 5f64 6174 612e 7570    [ json_data.up
-00026c40: 6461 7465 287b 2075 7469 6c73 2e74 6f5f  date({ utils.to_
-00026c50: 6361 6d65 6c5f 6361 7365 286b 6579 2920  camel_case(key) 
-00026c60: 3a20 7661 6c75 6520 7d29 2066 6f72 206b  : value }) for k
-00026c70: 6579 2c20 7661 6c75 6520 696e 2073 656c  ey, value in sel
-00026c80: 662e 5f63 7573 746f 6d5f 7061 7261 6d73  f._custom_params
-00026c90: 2e69 7465 6d73 2829 5d0a 2020 2020 2020  .items()].      
-00026ca0: 2020 7265 7475 726e 206a 736f 6e5f 6461    return json_da
-00026cb0: 7461 0a0a 2020 2020 6465 6620 5f5f 7374  ta..    def __st
-00026cc0: 725f 5f28 7365 6c66 2920 2d3e 2073 7472  r__(self) -> str
-00026cd0: 3a0a 2020 2020 2020 2020 6d65 7373 6167  :.        messag
-00026ce0: 6520 3d20 2222 2025 2028 290a 2020 2020  e = "" % ().    
-00026cf0: 2020 2020 6d65 7373 6167 6520 2b3d 2027      message += '
-00026d00: 272e 6a6f 696e 2827 5c6e 2720 2b20 7374  '.join('\n' + st
-00026d10: 7228 6b65 7929 202b 2027 203a 2027 202b  r(key) + ' : ' +
-00026d20: 2073 7472 2876 616c 7565 2920 666f 7220   str(value) for 
-00026d30: 6b65 792c 2076 616c 7565 2069 6e20 7365  key, value in se
-00026d40: 6c66 2e5f 6375 7374 6f6d 5f70 6172 616d  lf._custom_param
-00026d50: 732e 6974 656d 7328 2929 0a20 2020 2020  s.items()).     
-00026d60: 2020 2072 6574 7572 6e20 6d65 7373 6167     return messag
-00026d70: 650a 0a63 6c61 7373 204d 6572 6765 566f  e..class MergeVo
-00026d80: 6c75 6d65 7352 6573 756c 7473 2843 6f72  lumesResults(Cor
-00026d90: 654f 626a 6563 7429 3a0a 2020 2020 2222  eObject):.    ""
-00026da0: 2252 6573 756c 7473 2061 7373 6f63 6961  "Results associa
-00026db0: 7465 6420 7769 7468 206d 6572 6765 2076  ted with merge v
-00026dc0: 6f6c 756d 6573 206f 7065 7261 7469 6f6e  olumes operation
-00026dd0: 2e0a 2020 2020 2222 220a 2020 2020 5f64  ..    """.    _d
-00026de0: 6566 6175 6c74 5f70 6172 616d 7320 3d20  efault_params = 
-00026df0: 7b7d 0a0a 2020 2020 6465 6620 5f5f 696e  {}..    def __in
-00026e00: 6974 6961 6c69 7a65 280a 2020 2020 2020  itialize(.      
-00026e10: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00026e20: 2020 2020 2020 2020 6d65 7267 6564 5f76          merged_v
-00026e30: 6f6c 756d 6573 3a20 4974 6572 6162 6c65  olumes: Iterable
-00026e40: 5b69 6e74 5d2c 0a20 2020 2020 2020 2020  [int],.         
-00026e50: 2020 2065 7272 6f72 5f63 6f64 653a 2045     error_code: E
-00026e60: 7272 6f72 436f 6465 293a 0a20 2020 2020  rrorCode):.     
-00026e70: 2020 2073 656c 662e 5f6d 6572 6765 645f     self._merged_
-00026e80: 766f 6c75 6d65 7320 3d20 6d65 7267 6564  volumes = merged
-00026e90: 5f76 6f6c 756d 6573 2069 6620 6973 696e  _volumes if isin
-00026ea0: 7374 616e 6365 286d 6572 6765 645f 766f  stance(merged_vo
-00026eb0: 6c75 6d65 732c 206e 702e 6e64 6172 7261  lumes, np.ndarra
-00026ec0: 7929 2065 6c73 6520 6e70 2e61 7272 6179  y) else np.array
-00026ed0: 286d 6572 6765 645f 766f 6c75 6d65 732c  (merged_volumes,
-00026ee0: 2064 7479 7065 3d6e 702e 696e 7433 3229   dtype=np.int32)
-00026ef0: 2069 6620 6d65 7267 6564 5f76 6f6c 756d   if merged_volum
-00026f00: 6573 2069 7320 6e6f 7420 4e6f 6e65 2065  es is not None e
-00026f10: 6c73 6520 4e6f 6e65 0a20 2020 2020 2020  lse None.       
-00026f20: 2073 656c 662e 5f65 7272 6f72 5f63 6f64   self._error_cod
-00026f30: 6520 3d20 4572 726f 7243 6f64 6528 6572  e = ErrorCode(er
-00026f40: 726f 725f 636f 6465 290a 0a20 2020 2064  ror_code)..    d
-00026f50: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00026f60: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
-00026f70: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-00026f80: 3a20 436f 6d6d 756e 6963 6174 696f 6e4d  : CommunicationM
-00026f90: 616e 6167 6572 3d4e 6f6e 652c 0a20 2020  anager=None,.   
-00026fa0: 2020 2020 2020 2020 206d 6572 6765 645f           merged_
-00026fb0: 766f 6c75 6d65 733a 2049 7465 7261 626c  volumes: Iterabl
-00026fc0: 655b 696e 745d 203d 204e 6f6e 652c 0a20  e[int] = None,. 
-00026fd0: 2020 2020 2020 2020 2020 2065 7272 6f72             error
-00026fe0: 5f63 6f64 653a 2045 7272 6f72 436f 6465  _code: ErrorCode
-00026ff0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00027000: 2020 2020 206a 736f 6e5f 6461 7461 203a       json_data :
-00027010: 2064 6963 7420 3d20 4e6f 6e65 2c0a 2020   dict = None,.  
-00027020: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
-00027030: 7267 7329 3a0a 2020 2020 2020 2020 2222  rgs):.        ""
-00027040: 2249 6e69 7469 616c 697a 6573 2074 6865  "Initializes the
-00027050: 204d 6572 6765 566f 6c75 6d65 7352 6573   MergeVolumesRes
-00027060: 756c 7473 2e0a 0a20 2020 2020 2020 2050  ults...        P
-00027070: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00027080: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00027090: 2020 2020 206d 6f64 656c 3a20 4d6f 6465       model: Mode
-000270a0: 6c0a 2020 2020 2020 2020 2020 2020 4d6f  l.            Mo
-000270b0: 6465 6c20 746f 2063 7265 6174 6520 6120  del to create a 
-000270c0: 4d65 7267 6556 6f6c 756d 6573 5265 7375  MergeVolumesResu
-000270d0: 6c74 7320 6f62 6a65 6374 2077 6974 6820  lts object with 
-000270e0: 6465 6661 756c 7420 7061 7261 6d65 7465  default paramete
-000270f0: 7273 2e0a 2020 2020 2020 2020 6d65 7267  rs..        merg
-00027100: 6564 5f76 6f6c 756d 6573 3a20 4974 6572  ed_volumes: Iter
-00027110: 6162 6c65 5b69 6e74 5d2c 206f 7074 696f  able[int], optio
-00027120: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-00027130: 4964 7320 6f66 2076 6f6c 756d 6573 2074  Ids of volumes t
-00027140: 6f20 7768 6963 6820 696e 7075 7420 766f  o which input vo
-00027150: 6c75 6d65 7320 6172 6520 6d65 7267 6564  lumes are merged
-00027160: 2e0a 2020 2020 2020 2020 6572 726f 725f  ..        error_
-00027170: 636f 6465 3a20 4572 726f 7243 6f64 652c  code: ErrorCode,
-00027180: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-00027190: 2020 2020 2020 4572 726f 7220 636f 6465        Error code
-000271a0: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-000271b0: 2074 6865 2076 6f6c 756d 6520 6d65 7267   the volume merg
-000271c0: 6520 6f70 6572 6174 696f 6e2e 0a20 2020  e operation..   
-000271d0: 2020 2020 206a 736f 6e5f 6461 7461 3a20       json_data: 
-000271e0: 6469 6374 2c20 6f70 7469 6f6e 616c 0a20  dict, optional. 
-000271f0: 2020 2020 2020 2020 2020 204a 534f 4e20             JSON 
-00027200: 6469 6374 696f 6e61 7279 2074 6f20 6372  dictionary to cr
-00027210: 6561 7465 2061 204d 6572 6765 566f 6c75  eate a MergeVolu
-00027220: 6d65 7352 6573 756c 7473 206f 626a 6563  mesResults objec
-00027230: 7420 7769 7468 2070 726f 7669 6465 6420  t with provided 
-00027240: 7061 7261 6d65 7465 7273 2e0a 0a20 2020  parameters...   
-00027250: 2020 2020 2045 7861 6d70 6c65 730a 2020       Examples.  
-00027260: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20        --------. 
-00027270: 2020 2020 2020 203e 3e3e 206d 6572 6765         >>> merge
-00027280: 5f76 6f6c 756d 6573 5f72 6573 756c 7473  _volumes_results
-00027290: 203d 2070 7269 6d65 2e4d 6572 6765 566f   = prime.MergeVo
-000272a0: 6c75 6d65 7352 6573 756c 7473 286d 6f64  lumesResults(mod
-000272b0: 656c 203d 206d 6f64 656c 290a 2020 2020  el = model).    
-000272c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000272d0: 6966 206a 736f 6e5f 6461 7461 3a0a 2020  if json_data:.  
-000272e0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000272f0: 5f69 6e69 7469 616c 697a 6528 0a20 2020  _initialize(.   
-00027300: 2020 2020 2020 2020 2020 2020 206a 736f               jso
-00027310: 6e5f 6461 7461 5b22 6d65 7267 6564 566f  n_data["mergedVo
-00027320: 6c75 6d65 7322 5d20 6966 2022 6d65 7267  lumes"] if "merg
-00027330: 6564 566f 6c75 6d65 7322 2069 6e20 6a73  edVolumes" in js
-00027340: 6f6e 5f64 6174 6120 656c 7365 204e 6f6e  on_data else Non
-00027350: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00027360: 2020 2045 7272 6f72 436f 6465 286a 736f     ErrorCode(jso
-00027370: 6e5f 6461 7461 5b22 6572 726f 7243 6f64  n_data["errorCod
-00027380: 6522 5d20 6966 2022 6572 726f 7243 6f64  e"] if "errorCod
-00027390: 6522 2069 6e20 6a73 6f6e 5f64 6174 6120  e" in json_data 
-000273a0: 656c 7365 204e 6f6e 6529 290a 2020 2020  else None)).    
-000273b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000273c0: 2020 2020 2020 616c 6c5f 6669 656c 645f        all_field_
-000273d0: 7370 6563 6966 6965 6420 3d20 616c 6c28  specified = all(
-000273e0: 6172 6720 6973 206e 6f74 204e 6f6e 6520  arg is not None 
-000273f0: 666f 7220 6172 6720 696e 205b 6d65 7267  for arg in [merg
-00027400: 6564 5f76 6f6c 756d 6573 2c20 6572 726f  ed_volumes, erro
-00027410: 725f 636f 6465 5d29 0a20 2020 2020 2020  r_code]).       
-00027420: 2020 2020 2069 6620 616c 6c5f 6669 656c       if all_fiel
-00027430: 645f 7370 6563 6966 6965 643a 0a20 2020  d_specified:.   
-00027440: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00027450: 662e 5f5f 696e 6974 6961 6c69 7a65 280a  f.__initialize(.
-00027460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027470: 2020 2020 6d65 7267 6564 5f76 6f6c 756d      merged_volum
-00027480: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00027490: 2020 2020 2020 2020 6572 726f 725f 636f          error_co
-000274a0: 6465 290a 2020 2020 2020 2020 2020 2020  de).            
-000274b0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000274c0: 2020 2020 2020 6966 206d 6f64 656c 2069        if model i
-000274d0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-000274e0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000274f0: 6520 5661 6c75 6545 7272 6f72 2822 496e  e ValueError("In
-00027500: 7661 6c69 6420 6173 7369 676e 6d65 6e74  valid assignment
-00027510: 2e20 4569 7468 6572 2070 6173 7320 6d6f  . Either pass mo
-00027520: 6465 6c20 6f72 2073 7065 6369 6679 2061  del or specify a
-00027530: 6c6c 2070 726f 7065 7274 6965 7322 290a  ll properties").
-00027540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027550: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00027560: 2020 2020 2020 2020 2020 7061 7261 6d5f            param_
-00027570: 6a73 6f6e 203d 206d 6f64 656c 2e5f 636f  json = model._co
-00027580: 6d6d 756e 6963 6174 6f72 2e69 6e69 7469  mmunicator.initi
-00027590: 616c 697a 655f 7061 7261 6d73 286d 6f64  alize_params(mod
-000275a0: 656c 2c20 224d 6572 6765 566f 6c75 6d65  el, "MergeVolume
-000275b0: 7352 6573 756c 7473 2229 0a20 2020 2020  sResults").     
-000275c0: 2020 2020 2020 2020 2020 2020 2020 206a                 j
-000275d0: 736f 6e5f 6461 7461 203d 2070 6172 616d  son_data = param
-000275e0: 5f6a 736f 6e5b 224d 6572 6765 566f 6c75  _json["MergeVolu
-000275f0: 6d65 7352 6573 756c 7473 225d 2069 6620  mesResults"] if 
-00027600: 224d 6572 6765 566f 6c75 6d65 7352 6573  "MergeVolumesRes
-00027610: 756c 7473 2220 696e 2070 6172 616d 5f6a  ults" in param_j
-00027620: 736f 6e20 656c 7365 207b 7d0a 2020 2020  son else {}.    
-00027630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027640: 7365 6c66 2e5f 5f69 6e69 7469 616c 697a  self.__initializ
-00027650: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00027660: 2020 2020 2020 2020 2020 206d 6572 6765             merge
-00027670: 645f 766f 6c75 6d65 7320 6966 206d 6572  d_volumes if mer
-00027680: 6765 645f 766f 6c75 6d65 7320 6973 206e  ged_volumes is n
-00027690: 6f74 204e 6f6e 6520 656c 7365 2028 204d  ot None else ( M
-000276a0: 6572 6765 566f 6c75 6d65 7352 6573 756c  ergeVolumesResul
-000276b0: 7473 2e5f 6465 6661 756c 745f 7061 7261  ts._default_para
-000276c0: 6d73 5b22 6d65 7267 6564 5f76 6f6c 756d  ms["merged_volum
-000276d0: 6573 225d 2069 6620 226d 6572 6765 645f  es"] if "merged_
-000276e0: 766f 6c75 6d65 7322 2069 6e20 4d65 7267  volumes" in Merg
-000276f0: 6556 6f6c 756d 6573 5265 7375 6c74 732e  eVolumesResults.
-00027700: 5f64 6566 6175 6c74 5f70 6172 616d 7320  _default_params 
-00027710: 656c 7365 2028 6a73 6f6e 5f64 6174 615b  else (json_data[
-00027720: 226d 6572 6765 6456 6f6c 756d 6573 225d  "mergedVolumes"]
-00027730: 2069 6620 226d 6572 6765 6456 6f6c 756d   if "mergedVolum
-00027740: 6573 2220 696e 206a 736f 6e5f 6461 7461  es" in json_data
-00027750: 2065 6c73 6520 4e6f 6e65 2929 2c0a 2020   else None)),.  
-00027760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027770: 2020 2020 2020 6572 726f 725f 636f 6465        error_code
-00027780: 2069 6620 6572 726f 725f 636f 6465 2069   if error_code i
-00027790: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
-000277a0: 2820 4d65 7267 6556 6f6c 756d 6573 5265  ( MergeVolumesRe
-000277b0: 7375 6c74 732e 5f64 6566 6175 6c74 5f70  sults._default_p
-000277c0: 6172 616d 735b 2265 7272 6f72 5f63 6f64  arams["error_cod
-000277d0: 6522 5d20 6966 2022 6572 726f 725f 636f  e"] if "error_co
-000277e0: 6465 2220 696e 204d 6572 6765 566f 6c75  de" in MergeVolu
-000277f0: 6d65 7352 6573 756c 7473 2e5f 6465 6661  mesResults._defa
-00027800: 756c 745f 7061 7261 6d73 2065 6c73 6520  ult_params else 
-00027810: 4572 726f 7243 6f64 6528 6a73 6f6e 5f64  ErrorCode(json_d
-00027820: 6174 615b 2265 7272 6f72 436f 6465 225d  ata["errorCode"]
-00027830: 2069 6620 2265 7272 6f72 436f 6465 2220   if "errorCode" 
-00027840: 696e 206a 736f 6e5f 6461 7461 2065 6c73  in json_data els
-00027850: 6520 4e6f 6e65 2929 290a 2020 2020 2020  e None))).      
-00027860: 2020 7365 6c66 2e5f 6375 7374 6f6d 5f70    self._custom_p
-00027870: 6172 616d 7320 3d20 6b77 6172 6773 0a20  arams = kwargs. 
-00027880: 2020 2020 2020 2069 6620 6d6f 6465 6c20         if model 
-00027890: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000278a0: 2020 2020 2020 2020 205b 206d 6f64 656c           [ model
-000278b0: 2e5f 6c6f 6767 6572 2e77 6172 6e69 6e67  ._logger.warning
-000278c0: 2866 2755 6e73 7570 706f 7274 6564 2061  (f'Unsupported a
-000278d0: 7267 756d 656e 7420 3a20 7b6b 6579 7d27  rgument : {key}'
-000278e0: 2920 666f 7220 6b65 7920 696e 206b 7761  ) for key in kwa
-000278f0: 7267 7320 5d0a 2020 2020 2020 2020 5b73  rgs ].        [s
-00027900: 6574 6174 7472 2874 7970 6528 7365 6c66  etattr(type(self
-00027910: 292c 206b 6579 2c20 7072 6f70 6572 7479  ), key, property
-00027920: 286c 616d 6264 6120 7365 6c66 2c20 6b65  (lambda self, ke
-00027930: 7920 3d20 6b65 793a 2020 7365 6c66 2e5f  y = key:  self._
-00027940: 6375 7374 6f6d 5f70 6172 616d 735b 6b65  custom_params[ke
-00027950: 795d 2069 6620 6b65 7920 696e 2073 656c  y] if key in sel
-00027960: 662e 5f63 7573 746f 6d5f 7061 7261 6d73  f._custom_params
-00027970: 2065 6c73 6520 4e6f 6e65 2c0a 2020 2020   else None,.    
-00027980: 2020 2020 6c61 6d62 6461 2073 656c 662c      lambda self,
-00027990: 2076 616c 7565 2c20 6b65 7920 3d20 6b65   value, key = ke
-000279a0: 7920 3a20 7365 6c66 2e5f 6375 7374 6f6d  y : self._custom
-000279b0: 5f70 6172 616d 732e 7570 6461 7465 287b  _params.update({
-000279c0: 206b 6579 3a20 7661 6c75 6520 7d29 2929   key: value })))
-000279d0: 2066 6f72 206b 6579 2069 6e20 6b77 6172   for key in kwar
-000279e0: 6773 5d0a 2020 2020 2020 2020 7365 6c66  gs].        self
-000279f0: 2e5f 6672 6565 7a65 2829 0a0a 2020 2020  ._freeze()..    
-00027a00: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
-00027a10: 2020 6465 6620 7365 745f 6465 6661 756c    def set_defaul
-00027a20: 7428 0a20 2020 2020 2020 2020 2020 206d  t(.            m
-00027a30: 6572 6765 645f 766f 6c75 6d65 733a 2049  erged_volumes: I
-00027a40: 7465 7261 626c 655b 696e 745d 203d 204e  terable[int] = N
-00027a50: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00027a60: 2065 7272 6f72 5f63 6f64 653a 2045 7272   error_code: Err
-00027a70: 6f72 436f 6465 203d 204e 6f6e 6529 3a0a  orCode = None):.
-00027a80: 2020 2020 2020 2020 2222 2253 6574 2074          """Set t
-00027a90: 6865 2064 6566 6175 6c74 2076 616c 7565  he default value
-00027aa0: 7320 6f66 204d 6572 6765 566f 6c75 6d65  s of MergeVolume
-00027ab0: 7352 6573 756c 7473 2e0a 0a20 2020 2020  sResults...     
-00027ac0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00027ad0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00027ae0: 0a20 2020 2020 2020 206d 6572 6765 645f  .        merged_
-00027af0: 766f 6c75 6d65 733a 2049 7465 7261 626c  volumes: Iterabl
-00027b00: 655b 696e 745d 2c20 6f70 7469 6f6e 616c  e[int], optional
-00027b10: 0a20 2020 2020 2020 2020 2020 2049 6473  .            Ids
-00027b20: 206f 6620 766f 6c75 6d65 7320 746f 2077   of volumes to w
-00027b30: 6869 6368 2069 6e70 7574 2076 6f6c 756d  hich input volum
-00027b40: 6573 2061 7265 206d 6572 6765 642e 0a20  es are merged.. 
-00027b50: 2020 2020 2020 2065 7272 6f72 5f63 6f64         error_cod
-00027b60: 653a 2045 7272 6f72 436f 6465 2c20 6f70  e: ErrorCode, op
-00027b70: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-00027b80: 2020 2045 7272 6f72 2063 6f64 6520 6173     Error code as
-00027b90: 736f 6369 6174 6564 2077 6974 6820 7468  sociated with th
-00027ba0: 6520 766f 6c75 6d65 206d 6572 6765 206f  e volume merge o
-00027bb0: 7065 7261 7469 6f6e 2e0a 2020 2020 2020  peration..      
-00027bc0: 2020 2222 220a 2020 2020 2020 2020 6172    """.        ar
-00027bd0: 6773 203d 206c 6f63 616c 7328 290a 2020  gs = locals().  
-00027be0: 2020 2020 2020 5b4d 6572 6765 566f 6c75        [MergeVolu
-00027bf0: 6d65 7352 6573 756c 7473 2e5f 6465 6661  mesResults._defa
-00027c00: 756c 745f 7061 7261 6d73 2e75 7064 6174  ult_params.updat
-00027c10: 6528 7b20 6b65 793a 2076 616c 7565 207d  e({ key: value }
-00027c20: 2920 666f 7220 6b65 792c 2076 616c 7565  ) for key, value
-00027c30: 2069 6e20 6172 6773 2e69 7465 6d73 2829   in args.items()
-00027c40: 2069 6620 7661 6c75 6520 6973 206e 6f74   if value is not
-00027c50: 204e 6f6e 655d 0a0a 2020 2020 4073 7461   None]..    @sta
-00027c60: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
-00027c70: 6620 7072 696e 745f 6465 6661 756c 7428  f print_default(
-00027c80: 293a 0a20 2020 2020 2020 2022 2222 5072  ):.        """Pr
-00027c90: 696e 7420 7468 6520 6465 6661 756c 7420  int the default 
-00027ca0: 7661 6c75 6573 206f 6620 4d65 7267 6556  values of MergeV
-00027cb0: 6f6c 756d 6573 5265 7375 6c74 732e 0a0a  olumesResults...
-00027cc0: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
-00027cd0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00027ce0: 2d0a 2020 2020 2020 2020 3e3e 3e20 4d65  -.        >>> Me
-00027cf0: 7267 6556 6f6c 756d 6573 5265 7375 6c74  rgeVolumesResult
-00027d00: 732e 7072 696e 745f 6465 6661 756c 7428  s.print_default(
-00027d10: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
-00027d20: 2020 2020 2020 6d65 7373 6167 6520 3d20        message = 
-00027d30: 2222 0a20 2020 2020 2020 206d 6573 7361  "".        messa
-00027d40: 6765 202b 3d20 2727 2e6a 6f69 6e28 7374  ge += ''.join(st
-00027d50: 7228 6b65 7929 202b 2027 203a 2027 202b  r(key) + ' : ' +
-00027d60: 2073 7472 2876 616c 7565 2920 2b20 275c   str(value) + '\
-00027d70: 6e27 2066 6f72 206b 6579 2c20 7661 6c75  n' for key, valu
-00027d80: 6520 696e 204d 6572 6765 566f 6c75 6d65  e in MergeVolume
-00027d90: 7352 6573 756c 7473 2e5f 6465 6661 756c  sResults._defaul
-00027da0: 745f 7061 7261 6d73 2e69 7465 6d73 2829  t_params.items()
-00027db0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-00027dc0: 6d65 7373 6167 6529 0a0a 2020 2020 6465  message)..    de
-00027dd0: 6620 5f6a 736f 6e69 6679 2873 656c 6629  f _jsonify(self)
-00027de0: 202d 3e20 4469 6374 5b73 7472 2c20 416e   -> Dict[str, An
-00027df0: 795d 3a0a 2020 2020 2020 2020 6a73 6f6e  y]:.        json
-00027e00: 5f64 6174 6120 3d20 7b7d 0a20 2020 2020  _data = {}.     
-00027e10: 2020 2069 6620 7365 6c66 2e5f 6d65 7267     if self._merg
-00027e20: 6564 5f76 6f6c 756d 6573 2069 7320 6e6f  ed_volumes is no
-00027e30: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00027e40: 2020 2020 6a73 6f6e 5f64 6174 615b 226d      json_data["m
-00027e50: 6572 6765 6456 6f6c 756d 6573 225d 203d  ergedVolumes"] =
-00027e60: 2073 656c 662e 5f6d 6572 6765 645f 766f   self._merged_vo
-00027e70: 6c75 6d65 730a 2020 2020 2020 2020 6966  lumes.        if
-00027e80: 2073 656c 662e 5f65 7272 6f72 5f63 6f64   self._error_cod
-00027e90: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-00027ea0: 2020 2020 2020 2020 2020 206a 736f 6e5f             json_
-00027eb0: 6461 7461 5b22 6572 726f 7243 6f64 6522  data["errorCode"
-00027ec0: 5d20 3d20 7365 6c66 2e5f 6572 726f 725f  ] = self._error_
-00027ed0: 636f 6465 0a20 2020 2020 2020 205b 206a  code.        [ j
-00027ee0: 736f 6e5f 6461 7461 2e75 7064 6174 6528  son_data.update(
-00027ef0: 7b20 7574 696c 732e 746f 5f63 616d 656c  { utils.to_camel
-00027f00: 5f63 6173 6528 6b65 7929 203a 2076 616c  _case(key) : val
-00027f10: 7565 207d 2920 666f 7220 6b65 792c 2076  ue }) for key, v
-00027f20: 616c 7565 2069 6e20 7365 6c66 2e5f 6375  alue in self._cu
-00027f30: 7374 6f6d 5f70 6172 616d 732e 6974 656d  stom_params.item
-00027f40: 7328 295d 0a20 2020 2020 2020 2072 6574  s()].        ret
-00027f50: 7572 6e20 6a73 6f6e 5f64 6174 610a 0a20  urn json_data.. 
-00027f60: 2020 2064 6566 205f 5f73 7472 5f5f 2873     def __str__(s
-00027f70: 656c 6629 202d 3e20 7374 723a 0a20 2020  elf) -> str:.   
-00027f80: 2020 2020 206d 6573 7361 6765 203d 2022       message = "
-00027f90: 6d65 7267 6564 5f76 6f6c 756d 6573 203a  merged_volumes :
-00027fa0: 2020 2573 5c6e 6572 726f 725f 636f 6465    %s\nerror_code
-00027fb0: 203a 2020 2573 2220 2520 2873 656c 662e   :  %s" % (self.
-00027fc0: 5f6d 6572 6765 645f 766f 6c75 6d65 732c  _merged_volumes,
-00027fd0: 2073 656c 662e 5f65 7272 6f72 5f63 6f64   self._error_cod
-00027fe0: 6529 0a20 2020 2020 2020 206d 6573 7361  e).        messa
-00027ff0: 6765 202b 3d20 2727 2e6a 6f69 6e28 275c  ge += ''.join('\
-00028000: 6e27 202b 2073 7472 286b 6579 2920 2b20  n' + str(key) + 
-00028010: 2720 3a20 2720 2b20 7374 7228 7661 6c75  ' : ' + str(valu
-00028020: 6529 2066 6f72 206b 6579 2c20 7661 6c75  e) for key, valu
-00028030: 6520 696e 2073 656c 662e 5f63 7573 746f  e in self._custo
-00028040: 6d5f 7061 7261 6d73 2e69 7465 6d73 2829  m_params.items()
-00028050: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00028060: 206d 6573 7361 6765 0a0a 2020 2020 4070   message..    @p
-00028070: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00028080: 6d65 7267 6564 5f76 6f6c 756d 6573 2873  merged_volumes(s
-00028090: 656c 6629 202d 3e20 4974 6572 6162 6c65  elf) -> Iterable
-000280a0: 5b69 6e74 5d3a 0a20 2020 2020 2020 2022  [int]:.        "
-000280b0: 2222 4964 7320 6f66 2076 6f6c 756d 6573  ""Ids of volumes
-000280c0: 2074 6f20 7768 6963 6820 696e 7075 7420   to which input 
-000280d0: 766f 6c75 6d65 7320 6172 6520 6d65 7267  volumes are merg
-000280e0: 6564 2e0a 2020 2020 2020 2020 2222 220a  ed..        """.
-000280f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00028100: 656c 662e 5f6d 6572 6765 645f 766f 6c75  elf._merged_volu
-00028110: 6d65 730a 0a20 2020 2040 6d65 7267 6564  mes..    @merged
-00028120: 5f76 6f6c 756d 6573 2e73 6574 7465 720a  _volumes.setter.
-00028130: 2020 2020 6465 6620 6d65 7267 6564 5f76      def merged_v
-00028140: 6f6c 756d 6573 2873 656c 662c 2076 616c  olumes(self, val
-00028150: 7565 3a20 4974 6572 6162 6c65 5b69 6e74  ue: Iterable[int
-00028160: 5d29 3a0a 2020 2020 2020 2020 7365 6c66  ]):.        self
-00028170: 2e5f 6d65 7267 6564 5f76 6f6c 756d 6573  ._merged_volumes
-00028180: 203d 2076 616c 7565 0a0a 2020 2020 4070   = value..    @p
-00028190: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-000281a0: 6572 726f 725f 636f 6465 2873 656c 6629  error_code(self)
-000281b0: 202d 3e20 4572 726f 7243 6f64 653a 0a20   -> ErrorCode:. 
-000281c0: 2020 2020 2020 2022 2222 4572 726f 7220         """Error 
-000281d0: 636f 6465 2061 7373 6f63 6961 7465 6420  code associated 
-000281e0: 7769 7468 2074 6865 2076 6f6c 756d 6520  with the volume 
-000281f0: 6d65 7267 6520 6f70 6572 6174 696f 6e2e  merge operation.
-00028200: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00028210: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00028220: 2e5f 6572 726f 725f 636f 6465 0a0a 2020  ._error_code..  
-00028230: 2020 4065 7272 6f72 5f63 6f64 652e 7365    @error_code.se
-00028240: 7474 6572 0a20 2020 2064 6566 2065 7272  tter.    def err
-00028250: 6f72 5f63 6f64 6528 7365 6c66 2c20 7661  or_code(self, va
-00028260: 6c75 653a 2045 7272 6f72 436f 6465 293a  lue: ErrorCode):
-00028270: 0a20 2020 2020 2020 2073 656c 662e 5f65  .        self._e
-00028280: 7272 6f72 5f63 6f64 6520 3d20 7661 6c75  rror_code = valu
-00028290: 650a                                     e.
+00026b20: 7322 290a 2020 2020 2020 2020 2020 2020  s").            
+00026b30: 2020 2020 2020 2020 6a73 6f6e 5f64 6174          json_dat
+00026b40: 6120 3d20 7061 7261 6d5f 6a73 6f6e 5b22  a = param_json["
+00026b50: 4d65 7267 6556 6f6c 756d 6573 5061 7261  MergeVolumesPara
+00026b60: 6d73 225d 2069 6620 224d 6572 6765 566f  ms"] if "MergeVo
+00026b70: 6c75 6d65 7350 6172 616d 7322 2069 6e20  lumesParams" in 
+00026b80: 7061 7261 6d5f 6a73 6f6e 2065 6c73 6520  param_json else 
+00026b90: 7b7d 0a20 2020 2020 2020 2020 2020 2020  {}.             
+00026ba0: 2020 2020 2020 2073 656c 662e 5f5f 696e         self.__in
+00026bb0: 6974 6961 6c69 7a65 280a 2020 2020 2020  itialize(.      
+00026bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026bd0: 2020 6d65 7267 655f 746f 5f6e 6569 6768    merge_to_neigh
+00026be0: 626f 725f 766f 6c75 6d65 2069 6620 6d65  bor_volume if me
+00026bf0: 7267 655f 746f 5f6e 6569 6768 626f 725f  rge_to_neighbor_
+00026c00: 766f 6c75 6d65 2069 7320 6e6f 7420 4e6f  volume is not No
+00026c10: 6e65 2065 6c73 6520 2820 4d65 7267 6556  ne else ( MergeV
+00026c20: 6f6c 756d 6573 5061 7261 6d73 2e5f 6465  olumesParams._de
+00026c30: 6661 756c 745f 7061 7261 6d73 5b22 6d65  fault_params["me
+00026c40: 7267 655f 746f 5f6e 6569 6768 626f 725f  rge_to_neighbor_
+00026c50: 766f 6c75 6d65 225d 2069 6620 226d 6572  volume"] if "mer
+00026c60: 6765 5f74 6f5f 6e65 6967 6862 6f72 5f76  ge_to_neighbor_v
+00026c70: 6f6c 756d 6522 2069 6e20 4d65 7267 6556  olume" in MergeV
+00026c80: 6f6c 756d 6573 5061 7261 6d73 2e5f 6465  olumesParams._de
+00026c90: 6661 756c 745f 7061 7261 6d73 2065 6c73  fault_params els
+00026ca0: 6520 286a 736f 6e5f 6461 7461 5b22 6d65  e (json_data["me
+00026cb0: 7267 6554 6f4e 6569 6768 626f 7256 6f6c  rgeToNeighborVol
+00026cc0: 756d 6522 5d20 6966 2022 6d65 7267 6554  ume"] if "mergeT
+00026cd0: 6f4e 6569 6768 626f 7256 6f6c 756d 6522  oNeighborVolume"
+00026ce0: 2069 6e20 6a73 6f6e 5f64 6174 6120 656c   in json_data el
+00026cf0: 7365 204e 6f6e 6529 292c 0a20 2020 2020  se None)),.     
+00026d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026d10: 2020 206e 6569 6768 626f 725f 766f 6c75     neighbor_volu
+00026d20: 6d65 7320 6966 206e 6569 6768 626f 725f  mes if neighbor_
+00026d30: 766f 6c75 6d65 7320 6973 206e 6f74 204e  volumes is not N
+00026d40: 6f6e 6520 656c 7365 2028 204d 6572 6765  one else ( Merge
+00026d50: 566f 6c75 6d65 7350 6172 616d 732e 5f64  VolumesParams._d
+00026d60: 6566 6175 6c74 5f70 6172 616d 735b 226e  efault_params["n
+00026d70: 6569 6768 626f 725f 766f 6c75 6d65 7322  eighbor_volumes"
+00026d80: 5d20 6966 2022 6e65 6967 6862 6f72 5f76  ] if "neighbor_v
+00026d90: 6f6c 756d 6573 2220 696e 204d 6572 6765  olumes" in Merge
+00026da0: 566f 6c75 6d65 7350 6172 616d 732e 5f64  VolumesParams._d
+00026db0: 6566 6175 6c74 5f70 6172 616d 7320 656c  efault_params el
+00026dc0: 7365 2028 6a73 6f6e 5f64 6174 615b 226e  se (json_data["n
+00026dd0: 6569 6768 626f 7256 6f6c 756d 6573 225d  eighborVolumes"]
+00026de0: 2069 6620 226e 6569 6768 626f 7256 6f6c   if "neighborVol
+00026df0: 756d 6573 2220 696e 206a 736f 6e5f 6461  umes" in json_da
+00026e00: 7461 2065 6c73 6520 4e6f 6e65 2929 290a  ta else None))).
+00026e10: 2020 2020 2020 2020 7365 6c66 2e5f 6375          self._cu
+00026e20: 7374 6f6d 5f70 6172 616d 7320 3d20 6b77  stom_params = kw
+00026e30: 6172 6773 0a20 2020 2020 2020 2069 6620  args.        if 
+00026e40: 6d6f 6465 6c20 6973 206e 6f74 204e 6f6e  model is not Non
+00026e50: 653a 0a20 2020 2020 2020 2020 2020 205b  e:.            [
+00026e60: 206d 6f64 656c 2e5f 6c6f 6767 6572 2e77   model._logger.w
+00026e70: 6172 6e69 6e67 2866 2755 6e73 7570 706f  arning(f'Unsuppo
+00026e80: 7274 6564 2061 7267 756d 656e 7420 3a20  rted argument : 
+00026e90: 7b6b 6579 7d27 2920 666f 7220 6b65 7920  {key}') for key 
+00026ea0: 696e 206b 7761 7267 7320 5d0a 2020 2020  in kwargs ].    
+00026eb0: 2020 2020 5b73 6574 6174 7472 2874 7970      [setattr(typ
+00026ec0: 6528 7365 6c66 292c 206b 6579 2c20 7072  e(self), key, pr
+00026ed0: 6f70 6572 7479 286c 616d 6264 6120 7365  operty(lambda se
+00026ee0: 6c66 2c20 6b65 7920 3d20 6b65 793a 2020  lf, key = key:  
+00026ef0: 7365 6c66 2e5f 6375 7374 6f6d 5f70 6172  self._custom_par
+00026f00: 616d 735b 6b65 795d 2069 6620 6b65 7920  ams[key] if key 
+00026f10: 696e 2073 656c 662e 5f63 7573 746f 6d5f  in self._custom_
+00026f20: 7061 7261 6d73 2065 6c73 6520 4e6f 6e65  params else None
+00026f30: 2c0a 2020 2020 2020 2020 6c61 6d62 6461  ,.        lambda
+00026f40: 2073 656c 662c 2076 616c 7565 2c20 6b65   self, value, ke
+00026f50: 7920 3d20 6b65 7920 3a20 7365 6c66 2e5f  y = key : self._
+00026f60: 6375 7374 6f6d 5f70 6172 616d 732e 7570  custom_params.up
+00026f70: 6461 7465 287b 206b 6579 3a20 7661 6c75  date({ key: valu
+00026f80: 6520 7d29 2929 2066 6f72 206b 6579 2069  e }))) for key i
+00026f90: 6e20 6b77 6172 6773 5d0a 2020 2020 2020  n kwargs].      
+00026fa0: 2020 7365 6c66 2e5f 6672 6565 7a65 2829    self._freeze()
+00026fb0: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+00026fc0: 686f 640a 2020 2020 6465 6620 7365 745f  hod.    def set_
+00026fd0: 6465 6661 756c 7428 0a20 2020 2020 2020  default(.       
+00026fe0: 2020 2020 206d 6572 6765 5f74 6f5f 6e65       merge_to_ne
+00026ff0: 6967 6862 6f72 5f76 6f6c 756d 653a 2062  ighbor_volume: b
+00027000: 6f6f 6c20 3d20 4e6f 6e65 2c0a 2020 2020  ool = None,.    
+00027010: 2020 2020 2020 2020 6e65 6967 6862 6f72          neighbor
+00027020: 5f76 6f6c 756d 6573 3a20 4974 6572 6162  _volumes: Iterab
+00027030: 6c65 5b69 6e74 5d20 3d20 4e6f 6e65 293a  le[int] = None):
+00027040: 0a20 2020 2020 2020 2022 2222 5365 7420  .        """Set 
+00027050: 7468 6520 6465 6661 756c 7420 7661 6c75  the default valu
+00027060: 6573 206f 6620 4d65 7267 6556 6f6c 756d  es of MergeVolum
+00027070: 6573 5061 7261 6d73 2e0a 0a20 2020 2020  esParams...     
+00027080: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00027090: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+000270a0: 0a20 2020 2020 2020 206d 6572 6765 5f74  .        merge_t
+000270b0: 6f5f 6e65 6967 6862 6f72 5f76 6f6c 756d  o_neighbor_volum
+000270c0: 653a 2062 6f6f 6c2c 206f 7074 696f 6e61  e: bool, optiona
+000270d0: 6c0a 2020 2020 2020 2020 2020 2020 4f70  l.            Op
+000270e0: 7469 6f6e 2074 6f20 6d65 7267 6520 6769  tion to merge gi
+000270f0: 7665 6e20 766f 6c75 6d65 7320 746f 2074  ven volumes to t
+00027100: 6865 6972 206e 6569 6768 626f 7220 766f  heir neighbor vo
+00027110: 6c75 6d65 2e0a 2020 2020 2020 2020 6e65  lume..        ne
+00027120: 6967 6862 6f72 5f76 6f6c 756d 6573 3a20  ighbor_volumes: 
+00027130: 4974 6572 6162 6c65 5b69 6e74 5d2c 206f  Iterable[int], o
+00027140: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00027150: 2020 2020 4964 73c2 a06f 66c2 a076 6f6c      Ids..of..vol
+00027160: 756d 6520 7468 6174 2061 7265 c2a0 6e65  ume that are..ne
+00027170: 6967 6862 6f72 73c2 a074 6fc2 a067 6976  ighbors..to..giv
+00027180: 656e c2a0 766f 6c75 6d65 73c2 a066 6f72  en..volumes..for
+00027190: c2a0 6d65 7267 696e 672e 0a20 2020 2020  ..merging..     
+000271a0: 2020 2022 2222 0a20 2020 2020 2020 2061     """.        a
+000271b0: 7267 7320 3d20 6c6f 6361 6c73 2829 0a20  rgs = locals(). 
+000271c0: 2020 2020 2020 205b 4d65 7267 6556 6f6c         [MergeVol
+000271d0: 756d 6573 5061 7261 6d73 2e5f 6465 6661  umesParams._defa
+000271e0: 756c 745f 7061 7261 6d73 2e75 7064 6174  ult_params.updat
+000271f0: 6528 7b20 6b65 793a 2076 616c 7565 207d  e({ key: value }
+00027200: 2920 666f 7220 6b65 792c 2076 616c 7565  ) for key, value
+00027210: 2069 6e20 6172 6773 2e69 7465 6d73 2829   in args.items()
+00027220: 2069 6620 7661 6c75 6520 6973 206e 6f74   if value is not
+00027230: 204e 6f6e 655d 0a0a 2020 2020 4073 7461   None]..    @sta
+00027240: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
+00027250: 6620 7072 696e 745f 6465 6661 756c 7428  f print_default(
+00027260: 293a 0a20 2020 2020 2020 2022 2222 5072  ):.        """Pr
+00027270: 696e 7420 7468 6520 6465 6661 756c 7420  int the default 
+00027280: 7661 6c75 6573 206f 6620 4d65 7267 6556  values of MergeV
+00027290: 6f6c 756d 6573 5061 7261 6d73 2e0a 0a20  olumesParams... 
+000272a0: 2020 2020 2020 2045 7861 6d70 6c65 730a         Examples.
+000272b0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+000272c0: 0a20 2020 2020 2020 203e 3e3e 204d 6572  .        >>> Mer
+000272d0: 6765 566f 6c75 6d65 7350 6172 616d 732e  geVolumesParams.
+000272e0: 7072 696e 745f 6465 6661 756c 7428 290a  print_default().
+000272f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00027300: 2020 2020 6d65 7373 6167 6520 3d20 2222      message = ""
+00027310: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
+00027320: 202b 3d20 2727 2e6a 6f69 6e28 7374 7228   += ''.join(str(
+00027330: 6b65 7929 202b 2027 203a 2027 202b 2073  key) + ' : ' + s
+00027340: 7472 2876 616c 7565 2920 2b20 275c 6e27  tr(value) + '\n'
+00027350: 2066 6f72 206b 6579 2c20 7661 6c75 6520   for key, value 
+00027360: 696e 204d 6572 6765 566f 6c75 6d65 7350  in MergeVolumesP
+00027370: 6172 616d 732e 5f64 6566 6175 6c74 5f70  arams._default_p
+00027380: 6172 616d 732e 6974 656d 7328 2929 0a20  arams.items()). 
+00027390: 2020 2020 2020 2070 7269 6e74 286d 6573         print(mes
+000273a0: 7361 6765 290a 0a20 2020 2064 6566 205f  sage)..    def _
+000273b0: 6a73 6f6e 6966 7928 7365 6c66 2920 2d3e  jsonify(self) ->
+000273c0: 2044 6963 745b 7374 722c 2041 6e79 5d3a   Dict[str, Any]:
+000273d0: 0a20 2020 2020 2020 206a 736f 6e5f 6461  .        json_da
+000273e0: 7461 203d 207b 7d0a 2020 2020 2020 2020  ta = {}.        
+000273f0: 6966 2073 656c 662e 5f6d 6572 6765 5f74  if self._merge_t
+00027400: 6f5f 6e65 6967 6862 6f72 5f76 6f6c 756d  o_neighbor_volum
+00027410: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00027420: 2020 2020 2020 2020 2020 206a 736f 6e5f             json_
+00027430: 6461 7461 5b22 6d65 7267 6554 6f4e 6569  data["mergeToNei
+00027440: 6768 626f 7256 6f6c 756d 6522 5d20 3d20  ghborVolume"] = 
+00027450: 7365 6c66 2e5f 6d65 7267 655f 746f 5f6e  self._merge_to_n
+00027460: 6569 6768 626f 725f 766f 6c75 6d65 0a20  eighbor_volume. 
+00027470: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+00027480: 6e65 6967 6862 6f72 5f76 6f6c 756d 6573  neighbor_volumes
+00027490: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000274a0: 2020 2020 2020 2020 2020 6a73 6f6e 5f64            json_d
+000274b0: 6174 615b 226e 6569 6768 626f 7256 6f6c  ata["neighborVol
+000274c0: 756d 6573 225d 203d 2073 656c 662e 5f6e  umes"] = self._n
+000274d0: 6569 6768 626f 725f 766f 6c75 6d65 730a  eighbor_volumes.
+000274e0: 2020 2020 2020 2020 5b20 6a73 6f6e 5f64          [ json_d
+000274f0: 6174 612e 7570 6461 7465 287b 2075 7469  ata.update({ uti
+00027500: 6c73 2e74 6f5f 6361 6d65 6c5f 6361 7365  ls.to_camel_case
+00027510: 286b 6579 2920 3a20 7661 6c75 6520 7d29  (key) : value })
+00027520: 2066 6f72 206b 6579 2c20 7661 6c75 6520   for key, value 
+00027530: 696e 2073 656c 662e 5f63 7573 746f 6d5f  in self._custom_
+00027540: 7061 7261 6d73 2e69 7465 6d73 2829 5d0a  params.items()].
+00027550: 2020 2020 2020 2020 7265 7475 726e 206a          return j
+00027560: 736f 6e5f 6461 7461 0a0a 2020 2020 6465  son_data..    de
+00027570: 6620 5f5f 7374 725f 5f28 7365 6c66 2920  f __str__(self) 
+00027580: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
+00027590: 6d65 7373 6167 6520 3d20 226d 6572 6765  message = "merge
+000275a0: 5f74 6f5f 6e65 6967 6862 6f72 5f76 6f6c  _to_neighbor_vol
+000275b0: 756d 6520 3a20 2025 735c 6e6e 6569 6768  ume :  %s\nneigh
+000275c0: 626f 725f 766f 6c75 6d65 7320 3a20 2025  bor_volumes :  %
+000275d0: 7322 2025 2028 7365 6c66 2e5f 6d65 7267  s" % (self._merg
+000275e0: 655f 746f 5f6e 6569 6768 626f 725f 766f  e_to_neighbor_vo
+000275f0: 6c75 6d65 2c20 7365 6c66 2e5f 6e65 6967  lume, self._neig
+00027600: 6862 6f72 5f76 6f6c 756d 6573 290a 2020  hbor_volumes).  
+00027610: 2020 2020 2020 6d65 7373 6167 6520 2b3d        message +=
+00027620: 2027 272e 6a6f 696e 2827 5c6e 2720 2b20   ''.join('\n' + 
+00027630: 7374 7228 6b65 7929 202b 2027 203a 2027  str(key) + ' : '
+00027640: 202b 2073 7472 2876 616c 7565 2920 666f   + str(value) fo
+00027650: 7220 6b65 792c 2076 616c 7565 2069 6e20  r key, value in 
+00027660: 7365 6c66 2e5f 6375 7374 6f6d 5f70 6172  self._custom_par
+00027670: 616d 732e 6974 656d 7328 2929 0a20 2020  ams.items()).   
+00027680: 2020 2020 2072 6574 7572 6e20 6d65 7373       return mess
+00027690: 6167 650a 0a20 2020 2040 7072 6f70 6572  age..    @proper
+000276a0: 7479 0a20 2020 2064 6566 206d 6572 6765  ty.    def merge
+000276b0: 5f74 6f5f 6e65 6967 6862 6f72 5f76 6f6c  _to_neighbor_vol
+000276c0: 756d 6528 7365 6c66 2920 2d3e 2062 6f6f  ume(self) -> boo
+000276d0: 6c3a 0a20 2020 2020 2020 2022 2222 4f70  l:.        """Op
+000276e0: 7469 6f6e 2074 6f20 6d65 7267 6520 6769  tion to merge gi
+000276f0: 7665 6e20 766f 6c75 6d65 7320 746f 2074  ven volumes to t
+00027700: 6865 6972 206e 6569 6768 626f 7220 766f  heir neighbor vo
+00027710: 6c75 6d65 2e0a 2020 2020 2020 2020 2222  lume..        ""
+00027720: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+00027730: 2073 656c 662e 5f6d 6572 6765 5f74 6f5f   self._merge_to_
+00027740: 6e65 6967 6862 6f72 5f76 6f6c 756d 650a  neighbor_volume.
+00027750: 0a20 2020 2040 6d65 7267 655f 746f 5f6e  .    @merge_to_n
+00027760: 6569 6768 626f 725f 766f 6c75 6d65 2e73  eighbor_volume.s
+00027770: 6574 7465 720a 2020 2020 6465 6620 6d65  etter.    def me
+00027780: 7267 655f 746f 5f6e 6569 6768 626f 725f  rge_to_neighbor_
+00027790: 766f 6c75 6d65 2873 656c 662c 2076 616c  volume(self, val
+000277a0: 7565 3a20 626f 6f6c 293a 0a20 2020 2020  ue: bool):.     
+000277b0: 2020 2073 656c 662e 5f6d 6572 6765 5f74     self._merge_t
+000277c0: 6f5f 6e65 6967 6862 6f72 5f76 6f6c 756d  o_neighbor_volum
+000277d0: 6520 3d20 7661 6c75 650a 0a20 2020 2040  e = value..    @
+000277e0: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+000277f0: 206e 6569 6768 626f 725f 766f 6c75 6d65   neighbor_volume
+00027800: 7328 7365 6c66 2920 2d3e 2049 7465 7261  s(self) -> Itera
+00027810: 626c 655b 696e 745d 3a0a 2020 2020 2020  ble[int]:.      
+00027820: 2020 2222 2249 6473 c2a0 6f66 c2a0 766f    """Ids..of..vo
+00027830: 6c75 6d65 2074 6861 7420 6172 65c2 a06e  lume that are..n
+00027840: 6569 6768 626f 7273 c2a0 746f c2a0 6769  eighbors..to..gi
+00027850: 7665 6ec2 a076 6f6c 756d 6573 c2a0 666f  ven..volumes..fo
+00027860: 72c2 a06d 6572 6769 6e67 2e0a 2020 2020  r..merging..    
+00027870: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00027880: 7265 7475 726e 2073 656c 662e 5f6e 6569  return self._nei
+00027890: 6768 626f 725f 766f 6c75 6d65 730a 0a20  ghbor_volumes.. 
+000278a0: 2020 2040 6e65 6967 6862 6f72 5f76 6f6c     @neighbor_vol
+000278b0: 756d 6573 2e73 6574 7465 720a 2020 2020  umes.setter.    
+000278c0: 6465 6620 6e65 6967 6862 6f72 5f76 6f6c  def neighbor_vol
+000278d0: 756d 6573 2873 656c 662c 2076 616c 7565  umes(self, value
+000278e0: 3a20 4974 6572 6162 6c65 5b69 6e74 5d29  : Iterable[int])
+000278f0: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00027900: 6e65 6967 6862 6f72 5f76 6f6c 756d 6573  neighbor_volumes
+00027910: 203d 2076 616c 7565 0a0a 636c 6173 7320   = value..class 
+00027920: 4d65 7267 6556 6f6c 756d 6573 5265 7375  MergeVolumesResu
+00027930: 6c74 7328 436f 7265 4f62 6a65 6374 293a  lts(CoreObject):
+00027940: 0a20 2020 2022 2222 5265 7375 6c74 7320  .    """Results 
+00027950: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
+00027960: 6d65 7267 6520 766f 6c75 6d65 7320 6f70  merge volumes op
+00027970: 6572 6174 696f 6e2e 0a20 2020 2022 2222  eration..    """
+00027980: 0a20 2020 205f 6465 6661 756c 745f 7061  .    _default_pa
+00027990: 7261 6d73 203d 207b 7d0a 0a20 2020 2064  rams = {}..    d
+000279a0: 6566 205f 5f69 6e69 7469 616c 697a 6528  ef __initialize(
+000279b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000279c0: 662c 0a20 2020 2020 2020 2020 2020 206d  f,.            m
+000279d0: 6572 6765 645f 766f 6c75 6d65 733a 2049  erged_volumes: I
+000279e0: 7465 7261 626c 655b 696e 745d 2c0a 2020  terable[int],.  
+000279f0: 2020 2020 2020 2020 2020 6572 726f 725f            error_
+00027a00: 636f 6465 3a20 4572 726f 7243 6f64 6529  code: ErrorCode)
+00027a10: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00027a20: 6d65 7267 6564 5f76 6f6c 756d 6573 203d  merged_volumes =
+00027a30: 206d 6572 6765 645f 766f 6c75 6d65 7320   merged_volumes 
+00027a40: 6966 2069 7369 6e73 7461 6e63 6528 6d65  if isinstance(me
+00027a50: 7267 6564 5f76 6f6c 756d 6573 2c20 6e70  rged_volumes, np
+00027a60: 2e6e 6461 7272 6179 2920 656c 7365 206e  .ndarray) else n
+00027a70: 702e 6172 7261 7928 6d65 7267 6564 5f76  p.array(merged_v
+00027a80: 6f6c 756d 6573 2c20 6474 7970 653d 6e70  olumes, dtype=np
+00027a90: 2e69 6e74 3332 2920 6966 206d 6572 6765  .int32) if merge
+00027aa0: 645f 766f 6c75 6d65 7320 6973 206e 6f74  d_volumes is not
+00027ab0: 204e 6f6e 6520 656c 7365 204e 6f6e 650a   None else None.
+00027ac0: 2020 2020 2020 2020 7365 6c66 2e5f 6572          self._er
+00027ad0: 726f 725f 636f 6465 203d 2045 7272 6f72  ror_code = Error
+00027ae0: 436f 6465 2865 7272 6f72 5f63 6f64 6529  Code(error_code)
+00027af0: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00027b00: 5f5f 280a 2020 2020 2020 2020 2020 2020  __(.            
+00027b10: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00027b20: 2020 6d6f 6465 6c3a 2043 6f6d 6d75 6e69    model: Communi
+00027b30: 6361 7469 6f6e 4d61 6e61 6765 723d 4e6f  cationManager=No
+00027b40: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00027b50: 6d65 7267 6564 5f76 6f6c 756d 6573 3a20  merged_volumes: 
+00027b60: 4974 6572 6162 6c65 5b69 6e74 5d20 3d20  Iterable[int] = 
+00027b70: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00027b80: 2020 6572 726f 725f 636f 6465 3a20 4572    error_code: Er
+00027b90: 726f 7243 6f64 6520 3d20 4e6f 6e65 2c0a  rorCode = None,.
+00027ba0: 2020 2020 2020 2020 2020 2020 6a73 6f6e              json
+00027bb0: 5f64 6174 6120 3a20 6469 6374 203d 204e  _data : dict = N
+00027bc0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00027bd0: 2020 2a2a 6b77 6172 6773 293a 0a20 2020    **kwargs):.   
+00027be0: 2020 2020 2022 2222 496e 6974 6961 6c69       """Initiali
+00027bf0: 7a65 7320 7468 6520 4d65 7267 6556 6f6c  zes the MergeVol
+00027c00: 756d 6573 5265 7375 6c74 732e 0a0a 2020  umesResults...  
+00027c10: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00027c20: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00027c30: 2d2d 2d0a 2020 2020 2020 2020 6d6f 6465  ---.        mode
+00027c40: 6c3a 204d 6f64 656c 0a20 2020 2020 2020  l: Model.       
+00027c50: 2020 2020 204d 6f64 656c 2074 6f20 6372       Model to cr
+00027c60: 6561 7465 2061 204d 6572 6765 566f 6c75  eate a MergeVolu
+00027c70: 6d65 7352 6573 756c 7473 206f 626a 6563  mesResults objec
+00027c80: 7420 7769 7468 2064 6566 6175 6c74 2070  t with default p
+00027c90: 6172 616d 6574 6572 732e 0a20 2020 2020  arameters..     
+00027ca0: 2020 206d 6572 6765 645f 766f 6c75 6d65     merged_volume
+00027cb0: 733a 2049 7465 7261 626c 655b 696e 745d  s: Iterable[int]
+00027cc0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+00027cd0: 2020 2020 2020 2049 6473 206f 6620 766f         Ids of vo
+00027ce0: 6c75 6d65 7320 746f 2077 6869 6368 2069  lumes to which i
+00027cf0: 6e70 7574 2076 6f6c 756d 6573 2061 7265  nput volumes are
+00027d00: 206d 6572 6765 642e 0a20 2020 2020 2020   merged..       
+00027d10: 2065 7272 6f72 5f63 6f64 653a 2045 7272   error_code: Err
+00027d20: 6f72 436f 6465 2c20 6f70 7469 6f6e 616c  orCode, optional
+00027d30: 0a20 2020 2020 2020 2020 2020 2045 7272  .            Err
+00027d40: 6f72 2063 6f64 6520 6173 736f 6369 6174  or code associat
+00027d50: 6564 2077 6974 6820 7468 6520 766f 6c75  ed with the volu
+00027d60: 6d65 206d 6572 6765 206f 7065 7261 7469  me merge operati
+00027d70: 6f6e 2e0a 2020 2020 2020 2020 6a73 6f6e  on..        json
+00027d80: 5f64 6174 613a 2064 6963 742c 206f 7074  _data: dict, opt
+00027d90: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+00027da0: 2020 4a53 4f4e 2064 6963 7469 6f6e 6172    JSON dictionar
+00027db0: 7920 746f 2063 7265 6174 6520 6120 4d65  y to create a Me
+00027dc0: 7267 6556 6f6c 756d 6573 5265 7375 6c74  rgeVolumesResult
+00027dd0: 7320 6f62 6a65 6374 2077 6974 6820 7072  s object with pr
+00027de0: 6f76 6964 6564 2070 6172 616d 6574 6572  ovided parameter
+00027df0: 732e 0a0a 2020 2020 2020 2020 4578 616d  s...        Exam
+00027e00: 706c 6573 0a20 2020 2020 2020 202d 2d2d  ples.        ---
+00027e10: 2d2d 2d2d 2d0a 2020 2020 2020 2020 3e3e  -----.        >>
+00027e20: 3e20 6d65 7267 655f 766f 6c75 6d65 735f  > merge_volumes_
+00027e30: 7265 7375 6c74 7320 3d20 7072 696d 652e  results = prime.
+00027e40: 4d65 7267 6556 6f6c 756d 6573 5265 7375  MergeVolumesResu
+00027e50: 6c74 7328 6d6f 6465 6c20 3d20 6d6f 6465  lts(model = mode
+00027e60: 6c29 0a20 2020 2020 2020 2022 2222 0a20  l).        """. 
+00027e70: 2020 2020 2020 2069 6620 6a73 6f6e 5f64         if json_d
+00027e80: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
+00027e90: 2073 656c 662e 5f5f 696e 6974 6961 6c69   self.__initiali
+00027ea0: 7a65 280a 2020 2020 2020 2020 2020 2020  ze(.            
+00027eb0: 2020 2020 6a73 6f6e 5f64 6174 615b 226d      json_data["m
+00027ec0: 6572 6765 6456 6f6c 756d 6573 225d 2069  ergedVolumes"] i
+00027ed0: 6620 226d 6572 6765 6456 6f6c 756d 6573  f "mergedVolumes
+00027ee0: 2220 696e 206a 736f 6e5f 6461 7461 2065  " in json_data e
+00027ef0: 6c73 6520 4e6f 6e65 2c0a 2020 2020 2020  lse None,.      
+00027f00: 2020 2020 2020 2020 2020 4572 726f 7243            ErrorC
+00027f10: 6f64 6528 6a73 6f6e 5f64 6174 615b 2265  ode(json_data["e
+00027f20: 7272 6f72 436f 6465 225d 2069 6620 2265  rrorCode"] if "e
+00027f30: 7272 6f72 436f 6465 2220 696e 206a 736f  rrorCode" in jso
+00027f40: 6e5f 6461 7461 2065 6c73 6520 4e6f 6e65  n_data else None
+00027f50: 2929 0a20 2020 2020 2020 2065 6c73 653a  )).        else:
+00027f60: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
+00027f70: 5f66 6965 6c64 5f73 7065 6369 6669 6564  _field_specified
+00027f80: 203d 2061 6c6c 2861 7267 2069 7320 6e6f   = all(arg is no
+00027f90: 7420 4e6f 6e65 2066 6f72 2061 7267 2069  t None for arg i
+00027fa0: 6e20 5b6d 6572 6765 645f 766f 6c75 6d65  n [merged_volume
+00027fb0: 732c 2065 7272 6f72 5f63 6f64 655d 290a  s, error_code]).
+00027fc0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+00027fd0: 6c6c 5f66 6965 6c64 5f73 7065 6369 6669  ll_field_specifi
+00027fe0: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+00027ff0: 2020 2020 7365 6c66 2e5f 5f69 6e69 7469      self.__initi
+00028000: 616c 697a 6528 0a20 2020 2020 2020 2020  alize(.         
+00028010: 2020 2020 2020 2020 2020 206d 6572 6765             merge
+00028020: 645f 766f 6c75 6d65 732c 0a20 2020 2020  d_volumes,.     
+00028030: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00028040: 7272 6f72 5f63 6f64 6529 0a20 2020 2020  rror_code).     
+00028050: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00028060: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00028070: 6d6f 6465 6c20 6973 204e 6f6e 653a 0a20  model is None:. 
+00028080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028090: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+000280a0: 726f 7228 2249 6e76 616c 6964 2061 7373  ror("Invalid ass
+000280b0: 6967 6e6d 656e 742e 2045 6974 6865 7220  ignment. Either 
+000280c0: 7061 7373 206d 6f64 656c 206f 7220 7370  pass model or sp
+000280d0: 6563 6966 7920 616c 6c20 7072 6f70 6572  ecify all proper
+000280e0: 7469 6573 2229 0a20 2020 2020 2020 2020  ties").         
+000280f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00028100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028110: 2070 6172 616d 5f6a 736f 6e20 3d20 6d6f   param_json = mo
+00028120: 6465 6c2e 5f63 6f6d 6d75 6e69 6361 746f  del._communicato
+00028130: 722e 696e 6974 6961 6c69 7a65 5f70 6172  r.initialize_par
+00028140: 616d 7328 6d6f 6465 6c2c 2022 4d65 7267  ams(model, "Merg
+00028150: 6556 6f6c 756d 6573 5265 7375 6c74 7322  eVolumesResults"
+00028160: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00028170: 2020 2020 2020 6a73 6f6e 5f64 6174 6120        json_data 
+00028180: 3d20 7061 7261 6d5f 6a73 6f6e 5b22 4d65  = param_json["Me
+00028190: 7267 6556 6f6c 756d 6573 5265 7375 6c74  rgeVolumesResult
+000281a0: 7322 5d20 6966 2022 4d65 7267 6556 6f6c  s"] if "MergeVol
+000281b0: 756d 6573 5265 7375 6c74 7322 2069 6e20  umesResults" in 
+000281c0: 7061 7261 6d5f 6a73 6f6e 2065 6c73 6520  param_json else 
+000281d0: 7b7d 0a20 2020 2020 2020 2020 2020 2020  {}.             
+000281e0: 2020 2020 2020 2073 656c 662e 5f5f 696e         self.__in
+000281f0: 6974 6961 6c69 7a65 280a 2020 2020 2020  itialize(.      
+00028200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028210: 2020 6d65 7267 6564 5f76 6f6c 756d 6573    merged_volumes
+00028220: 2069 6620 6d65 7267 6564 5f76 6f6c 756d   if merged_volum
+00028230: 6573 2069 7320 6e6f 7420 4e6f 6e65 2065  es is not None e
+00028240: 6c73 6520 2820 4d65 7267 6556 6f6c 756d  lse ( MergeVolum
+00028250: 6573 5265 7375 6c74 732e 5f64 6566 6175  esResults._defau
+00028260: 6c74 5f70 6172 616d 735b 226d 6572 6765  lt_params["merge
+00028270: 645f 766f 6c75 6d65 7322 5d20 6966 2022  d_volumes"] if "
+00028280: 6d65 7267 6564 5f76 6f6c 756d 6573 2220  merged_volumes" 
+00028290: 696e 204d 6572 6765 566f 6c75 6d65 7352  in MergeVolumesR
+000282a0: 6573 756c 7473 2e5f 6465 6661 756c 745f  esults._default_
+000282b0: 7061 7261 6d73 2065 6c73 6520 286a 736f  params else (jso
+000282c0: 6e5f 6461 7461 5b22 6d65 7267 6564 566f  n_data["mergedVo
+000282d0: 6c75 6d65 7322 5d20 6966 2022 6d65 7267  lumes"] if "merg
+000282e0: 6564 566f 6c75 6d65 7322 2069 6e20 6a73  edVolumes" in js
+000282f0: 6f6e 5f64 6174 6120 656c 7365 204e 6f6e  on_data else Non
+00028300: 6529 292c 0a20 2020 2020 2020 2020 2020  e)),.           
+00028310: 2020 2020 2020 2020 2020 2020 2065 7272               err
+00028320: 6f72 5f63 6f64 6520 6966 2065 7272 6f72  or_code if error
+00028330: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
+00028340: 6520 656c 7365 2028 204d 6572 6765 566f  e else ( MergeVo
+00028350: 6c75 6d65 7352 6573 756c 7473 2e5f 6465  lumesResults._de
+00028360: 6661 756c 745f 7061 7261 6d73 5b22 6572  fault_params["er
+00028370: 726f 725f 636f 6465 225d 2069 6620 2265  ror_code"] if "e
+00028380: 7272 6f72 5f63 6f64 6522 2069 6e20 4d65  rror_code" in Me
+00028390: 7267 6556 6f6c 756d 6573 5265 7375 6c74  rgeVolumesResult
+000283a0: 732e 5f64 6566 6175 6c74 5f70 6172 616d  s._default_param
+000283b0: 7320 656c 7365 2045 7272 6f72 436f 6465  s else ErrorCode
+000283c0: 286a 736f 6e5f 6461 7461 5b22 6572 726f  (json_data["erro
+000283d0: 7243 6f64 6522 5d20 6966 2022 6572 726f  rCode"] if "erro
+000283e0: 7243 6f64 6522 2069 6e20 6a73 6f6e 5f64  rCode" in json_d
+000283f0: 6174 6120 656c 7365 204e 6f6e 6529 2929  ata else None)))
+00028400: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
+00028410: 7573 746f 6d5f 7061 7261 6d73 203d 206b  ustom_params = k
+00028420: 7761 7267 730a 2020 2020 2020 2020 6966  wargs.        if
+00028430: 206d 6f64 656c 2069 7320 6e6f 7420 4e6f   model is not No
+00028440: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00028450: 5b20 6d6f 6465 6c2e 5f6c 6f67 6765 722e  [ model._logger.
+00028460: 7761 726e 696e 6728 6627 556e 7375 7070  warning(f'Unsupp
+00028470: 6f72 7465 6420 6172 6775 6d65 6e74 203a  orted argument :
+00028480: 207b 6b65 797d 2729 2066 6f72 206b 6579   {key}') for key
+00028490: 2069 6e20 6b77 6172 6773 205d 0a20 2020   in kwargs ].   
+000284a0: 2020 2020 205b 7365 7461 7474 7228 7479       [setattr(ty
+000284b0: 7065 2873 656c 6629 2c20 6b65 792c 2070  pe(self), key, p
+000284c0: 726f 7065 7274 7928 6c61 6d62 6461 2073  roperty(lambda s
+000284d0: 656c 662c 206b 6579 203d 206b 6579 3a20  elf, key = key: 
+000284e0: 2073 656c 662e 5f63 7573 746f 6d5f 7061   self._custom_pa
+000284f0: 7261 6d73 5b6b 6579 5d20 6966 206b 6579  rams[key] if key
+00028500: 2069 6e20 7365 6c66 2e5f 6375 7374 6f6d   in self._custom
+00028510: 5f70 6172 616d 7320 656c 7365 204e 6f6e  _params else Non
+00028520: 652c 0a20 2020 2020 2020 206c 616d 6264  e,.        lambd
+00028530: 6120 7365 6c66 2c20 7661 6c75 652c 206b  a self, value, k
+00028540: 6579 203d 206b 6579 203a 2073 656c 662e  ey = key : self.
+00028550: 5f63 7573 746f 6d5f 7061 7261 6d73 2e75  _custom_params.u
+00028560: 7064 6174 6528 7b20 6b65 793a 2076 616c  pdate({ key: val
+00028570: 7565 207d 2929 2920 666f 7220 6b65 7920  ue }))) for key 
+00028580: 696e 206b 7761 7267 735d 0a20 2020 2020  in kwargs].     
+00028590: 2020 2073 656c 662e 5f66 7265 657a 6528     self._freeze(
+000285a0: 290a 0a20 2020 2040 7374 6174 6963 6d65  )..    @staticme
+000285b0: 7468 6f64 0a20 2020 2064 6566 2073 6574  thod.    def set
+000285c0: 5f64 6566 6175 6c74 280a 2020 2020 2020  _default(.      
+000285d0: 2020 2020 2020 6d65 7267 6564 5f76 6f6c        merged_vol
+000285e0: 756d 6573 3a20 4974 6572 6162 6c65 5b69  umes: Iterable[i
+000285f0: 6e74 5d20 3d20 4e6f 6e65 2c0a 2020 2020  nt] = None,.    
+00028600: 2020 2020 2020 2020 6572 726f 725f 636f          error_co
+00028610: 6465 3a20 4572 726f 7243 6f64 6520 3d20  de: ErrorCode = 
+00028620: 4e6f 6e65 293a 0a20 2020 2020 2020 2022  None):.        "
+00028630: 2222 5365 7420 7468 6520 6465 6661 756c  ""Set the defaul
+00028640: 7420 7661 6c75 6573 206f 6620 4d65 7267  t values of Merg
+00028650: 6556 6f6c 756d 6573 5265 7375 6c74 732e  eVolumesResults.
+00028660: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00028670: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00028680: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00028690: 6d65 7267 6564 5f76 6f6c 756d 6573 3a20  merged_volumes: 
+000286a0: 4974 6572 6162 6c65 5b69 6e74 5d2c 206f  Iterable[int], o
+000286b0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+000286c0: 2020 2020 4964 7320 6f66 2076 6f6c 756d      Ids of volum
+000286d0: 6573 2074 6f20 7768 6963 6820 696e 7075  es to which inpu
+000286e0: 7420 766f 6c75 6d65 7320 6172 6520 6d65  t volumes are me
+000286f0: 7267 6564 2e0a 2020 2020 2020 2020 6572  rged..        er
+00028700: 726f 725f 636f 6465 3a20 4572 726f 7243  ror_code: ErrorC
+00028710: 6f64 652c 206f 7074 696f 6e61 6c0a 2020  ode, optional.  
+00028720: 2020 2020 2020 2020 2020 4572 726f 7220            Error 
+00028730: 636f 6465 2061 7373 6f63 6961 7465 6420  code associated 
+00028740: 7769 7468 2074 6865 2076 6f6c 756d 6520  with the volume 
+00028750: 6d65 7267 6520 6f70 6572 6174 696f 6e2e  merge operation.
+00028760: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00028770: 2020 2020 2061 7267 7320 3d20 6c6f 6361       args = loca
+00028780: 6c73 2829 0a20 2020 2020 2020 205b 4d65  ls().        [Me
+00028790: 7267 6556 6f6c 756d 6573 5265 7375 6c74  rgeVolumesResult
+000287a0: 732e 5f64 6566 6175 6c74 5f70 6172 616d  s._default_param
+000287b0: 732e 7570 6461 7465 287b 206b 6579 3a20  s.update({ key: 
+000287c0: 7661 6c75 6520 7d29 2066 6f72 206b 6579  value }) for key
+000287d0: 2c20 7661 6c75 6520 696e 2061 7267 732e  , value in args.
+000287e0: 6974 656d 7328 2920 6966 2076 616c 7565  items() if value
+000287f0: 2069 7320 6e6f 7420 4e6f 6e65 5d0a 0a20   is not None].. 
+00028800: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+00028810: 0a20 2020 2064 6566 2070 7269 6e74 5f64  .    def print_d
+00028820: 6566 6175 6c74 2829 3a0a 2020 2020 2020  efault():.      
+00028830: 2020 2222 2250 7269 6e74 2074 6865 2064    """Print the d
+00028840: 6566 6175 6c74 2076 616c 7565 7320 6f66  efault values of
+00028850: 204d 6572 6765 566f 6c75 6d65 7352 6573   MergeVolumesRes
+00028860: 756c 7473 2e0a 0a20 2020 2020 2020 2045  ults...        E
+00028870: 7861 6d70 6c65 730a 2020 2020 2020 2020  xamples.        
+00028880: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00028890: 203e 3e3e 204d 6572 6765 566f 6c75 6d65   >>> MergeVolume
+000288a0: 7352 6573 756c 7473 2e70 7269 6e74 5f64  sResults.print_d
+000288b0: 6566 6175 6c74 2829 0a20 2020 2020 2020  efault().       
+000288c0: 2022 2222 0a20 2020 2020 2020 206d 6573   """.        mes
+000288d0: 7361 6765 203d 2022 220a 2020 2020 2020  sage = "".      
+000288e0: 2020 6d65 7373 6167 6520 2b3d 2027 272e    message += ''.
+000288f0: 6a6f 696e 2873 7472 286b 6579 2920 2b20  join(str(key) + 
+00028900: 2720 3a20 2720 2b20 7374 7228 7661 6c75  ' : ' + str(valu
+00028910: 6529 202b 2027 5c6e 2720 666f 7220 6b65  e) + '\n' for ke
+00028920: 792c 2076 616c 7565 2069 6e20 4d65 7267  y, value in Merg
+00028930: 6556 6f6c 756d 6573 5265 7375 6c74 732e  eVolumesResults.
+00028940: 5f64 6566 6175 6c74 5f70 6172 616d 732e  _default_params.
+00028950: 6974 656d 7328 2929 0a20 2020 2020 2020  items()).       
+00028960: 2070 7269 6e74 286d 6573 7361 6765 290a   print(message).
+00028970: 0a20 2020 2064 6566 205f 6a73 6f6e 6966  .    def _jsonif
+00028980: 7928 7365 6c66 2920 2d3e 2044 6963 745b  y(self) -> Dict[
+00028990: 7374 722c 2041 6e79 5d3a 0a20 2020 2020  str, Any]:.     
+000289a0: 2020 206a 736f 6e5f 6461 7461 203d 207b     json_data = {
+000289b0: 7d0a 2020 2020 2020 2020 6966 2073 656c  }.        if sel
+000289c0: 662e 5f6d 6572 6765 645f 766f 6c75 6d65  f._merged_volume
+000289d0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+000289e0: 2020 2020 2020 2020 2020 206a 736f 6e5f             json_
+000289f0: 6461 7461 5b22 6d65 7267 6564 566f 6c75  data["mergedVolu
+00028a00: 6d65 7322 5d20 3d20 7365 6c66 2e5f 6d65  mes"] = self._me
+00028a10: 7267 6564 5f76 6f6c 756d 6573 0a20 2020  rged_volumes.   
+00028a20: 2020 2020 2069 6620 7365 6c66 2e5f 6572       if self._er
+00028a30: 726f 725f 636f 6465 2069 7320 6e6f 7420  ror_code is not 
+00028a40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00028a50: 2020 6a73 6f6e 5f64 6174 615b 2265 7272    json_data["err
+00028a60: 6f72 436f 6465 225d 203d 2073 656c 662e  orCode"] = self.
+00028a70: 5f65 7272 6f72 5f63 6f64 650a 2020 2020  _error_code.    
+00028a80: 2020 2020 5b20 6a73 6f6e 5f64 6174 612e      [ json_data.
+00028a90: 7570 6461 7465 287b 2075 7469 6c73 2e74  update({ utils.t
+00028aa0: 6f5f 6361 6d65 6c5f 6361 7365 286b 6579  o_camel_case(key
+00028ab0: 2920 3a20 7661 6c75 6520 7d29 2066 6f72  ) : value }) for
+00028ac0: 206b 6579 2c20 7661 6c75 6520 696e 2073   key, value in s
+00028ad0: 656c 662e 5f63 7573 746f 6d5f 7061 7261  elf._custom_para
+00028ae0: 6d73 2e69 7465 6d73 2829 5d0a 2020 2020  ms.items()].    
+00028af0: 2020 2020 7265 7475 726e 206a 736f 6e5f      return json_
+00028b00: 6461 7461 0a0a 2020 2020 6465 6620 5f5f  data..    def __
+00028b10: 7374 725f 5f28 7365 6c66 2920 2d3e 2073  str__(self) -> s
+00028b20: 7472 3a0a 2020 2020 2020 2020 6d65 7373  tr:.        mess
+00028b30: 6167 6520 3d20 226d 6572 6765 645f 766f  age = "merged_vo
+00028b40: 6c75 6d65 7320 3a20 2025 735c 6e65 7272  lumes :  %s\nerr
+00028b50: 6f72 5f63 6f64 6520 3a20 2025 7322 2025  or_code :  %s" %
+00028b60: 2028 7365 6c66 2e5f 6d65 7267 6564 5f76   (self._merged_v
+00028b70: 6f6c 756d 6573 2c20 7365 6c66 2e5f 6572  olumes, self._er
+00028b80: 726f 725f 636f 6465 290a 2020 2020 2020  ror_code).      
+00028b90: 2020 6d65 7373 6167 6520 2b3d 2027 272e    message += ''.
+00028ba0: 6a6f 696e 2827 5c6e 2720 2b20 7374 7228  join('\n' + str(
+00028bb0: 6b65 7929 202b 2027 203a 2027 202b 2073  key) + ' : ' + s
+00028bc0: 7472 2876 616c 7565 2920 666f 7220 6b65  tr(value) for ke
+00028bd0: 792c 2076 616c 7565 2069 6e20 7365 6c66  y, value in self
+00028be0: 2e5f 6375 7374 6f6d 5f70 6172 616d 732e  ._custom_params.
+00028bf0: 6974 656d 7328 2929 0a20 2020 2020 2020  items()).       
+00028c00: 2072 6574 7572 6e20 6d65 7373 6167 650a   return message.
+00028c10: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00028c20: 2020 2064 6566 206d 6572 6765 645f 766f     def merged_vo
+00028c30: 6c75 6d65 7328 7365 6c66 2920 2d3e 2049  lumes(self) -> I
+00028c40: 7465 7261 626c 655b 696e 745d 3a0a 2020  terable[int]:.  
+00028c50: 2020 2020 2020 2222 2249 6473 206f 6620        """Ids of 
+00028c60: 766f 6c75 6d65 7320 746f 2077 6869 6368  volumes to which
+00028c70: 2069 6e70 7574 2076 6f6c 756d 6573 2061   input volumes a
+00028c80: 7265 206d 6572 6765 642e 0a20 2020 2020  re merged..     
+00028c90: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00028ca0: 6574 7572 6e20 7365 6c66 2e5f 6d65 7267  eturn self._merg
+00028cb0: 6564 5f76 6f6c 756d 6573 0a0a 2020 2020  ed_volumes..    
+00028cc0: 406d 6572 6765 645f 766f 6c75 6d65 732e  @merged_volumes.
+00028cd0: 7365 7474 6572 0a20 2020 2064 6566 206d  setter.    def m
+00028ce0: 6572 6765 645f 766f 6c75 6d65 7328 7365  erged_volumes(se
+00028cf0: 6c66 2c20 7661 6c75 653a 2049 7465 7261  lf, value: Itera
+00028d00: 626c 655b 696e 745d 293a 0a20 2020 2020  ble[int]):.     
+00028d10: 2020 2073 656c 662e 5f6d 6572 6765 645f     self._merged_
+00028d20: 766f 6c75 6d65 7320 3d20 7661 6c75 650a  volumes = value.
+00028d30: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+00028d40: 2020 2064 6566 2065 7272 6f72 5f63 6f64     def error_cod
+00028d50: 6528 7365 6c66 2920 2d3e 2045 7272 6f72  e(self) -> Error
+00028d60: 436f 6465 3a0a 2020 2020 2020 2020 2222  Code:.        ""
+00028d70: 2245 7272 6f72 2063 6f64 6520 6173 736f  "Error code asso
+00028d80: 6369 6174 6564 2077 6974 6820 7468 6520  ciated with the 
+00028d90: 766f 6c75 6d65 206d 6572 6765 206f 7065  volume merge ope
+00028da0: 7261 7469 6f6e 2e0a 2020 2020 2020 2020  ration..        
+00028db0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00028dc0: 726e 2073 656c 662e 5f65 7272 6f72 5f63  rn self._error_c
+00028dd0: 6f64 650a 0a20 2020 2040 6572 726f 725f  ode..    @error_
+00028de0: 636f 6465 2e73 6574 7465 720a 2020 2020  code.setter.    
+00028df0: 6465 6620 6572 726f 725f 636f 6465 2873  def error_code(s
+00028e00: 656c 662c 2076 616c 7565 3a20 4572 726f  elf, value: Erro
+00028e10: 7243 6f64 6529 3a0a 2020 2020 2020 2020  rCode):.        
+00028e20: 7365 6c66 2e5f 6572 726f 725f 636f 6465  self._error_code
+00028e30: 203d 2076 616c 7565 0a                    = value.
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/periodiccontrol.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/periodiccontrol.py`

 * *Files 15% similar despite different names*

```diff
@@ -54,14 +54,16 @@
         Examples
         --------
         >>> periodic_control.set_params(
         >>>                  PeriodicControlParams(model=model,
         >>>                     center=[0,0,0], axis=[0,1,0], angle=180))
 
         """
+        if not isinstance(periodic_control_params, PeriodicControlParams):
+            raise TypeError("Invalid argument type passed for periodic_control_params, valid argument type is PeriodicControlParams.")
         args = {"periodic_control_params" : periodic_control_params._jsonify()}
         command_name = "PrimeMesh::PeriodicControl/SetParams"
         self._model._print_logs_before_command("set_params", args)
         self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("set_params")
 
     def set_suggested_name(self, name : str) -> SetNameResults:
@@ -80,14 +82,16 @@
 
 
         Examples
         --------
         >>> periodic_control.set_suggested_name("control1")
 
         """
+        if not isinstance(name, str):
+            raise TypeError("Invalid argument type passed for name, valid argument type is str.")
         args = {"name" : name}
         command_name = "PrimeMesh::PeriodicControl/SetSuggestedName"
         self._model._print_logs_before_command("set_suggested_name", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("set_suggested_name", SetNameResults(model = self._model, json_data = result))
         return SetNameResults(model = self._model, json_data = result)
 
@@ -134,14 +138,16 @@
         >>> surface_scope = prime.ScopeDefinition(model=model,
         >>>                     entity_type=prime.ScopeEntity.FACEZONELETS,
         >>>                     evaluation_type=prime.ScopeEvaluationType.LABELS,
         >>>                     label_expression="periodic-1")
         >>> periodic_control.set_scope(surface_scope)
 
         """
+        if not isinstance(scope, ScopeDefinition):
+            raise TypeError("Invalid argument type passed for scope, valid argument type is ScopeDefinition.")
         args = {"scope" : scope._jsonify()}
         command_name = "PrimeMesh::PeriodicControl/SetScope"
         self._model._print_logs_before_command("set_scope", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("set_scope", SetScopeResults(model = self._model, json_data = result))
         return SetScopeResults(model = self._model, json_data = result)
 
@@ -160,14 +166,16 @@
             Return the PeriodicControlSummaryResult.
 
         Examples
         --------
         >>> results = periodic_control.get_summary(prime.PeriodicControlSummaryParams(model=model))
 
         """
+        if not isinstance(params, PeriodicControlSummaryParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is PeriodicControlSummaryParams.")
         args = {"params" : params._jsonify()}
         command_name = "PrimeMesh::PeriodicControl/GetSummary"
         self._model._print_logs_before_command("get_summary", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("get_summary", PeriodicControlSummaryResult(model = self._model, json_data = result))
         return PeriodicControlSummaryResult(model = self._model, json_data = result)
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/periodiccontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/primeconfig.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/primeconfig.py`

 * *Files 19% similar despite different names*

```diff
@@ -114,16 +114,22 @@
     """Compute volumes failed."""
     QUADRATICTETNOTSUPPORTEDINPARALLEL = 130
     """Quadratic tetrahedal meshing is not supported in parallel mode."""
     QUADRATICTETNOTSUPPORTEDWITHPRISMS = 131
     """Quadratic tetrahedral meshing is not supported with prism."""
     EXTRACTVOLUMESFAILED = 132
     """Extract volumes failed."""
+    MERGEVOLUMESFAILED = 133
+    """Merge volumes failed."""
+    DELETEVOLUMESFAILED = 134
+    """Delete volumes failed."""
     PERIODICSURFACESNOTSUPPORTEDFORPRISMS = 135
     """Periodic surfaces selected for prism generation are not supported."""
+    INVALIDNEIGHBORVOLUMES = 136
+    """Invalid neighbor volumes selected to merge volumes."""
     OUTOFMEMORY = 200
     """Out of memory."""
     INTERRUPTED = 201
     """Method call interrupted."""
     GETSTATISTICSFAILED = 250
     """Failed to get mesh statistics."""
     GETELEMENTCOUNTFAILED = 251
@@ -170,21 +176,23 @@
     """BOI creation failed. Invalid flow or wake direction."""
     CREATEBOI_IVALIDWRAPMESHSIZE = 384
     """BOI creation failed. Wrap cannot be performed with invalid mesh size."""
     CREATEBOI_INVALIDWAKELEVELS = 385
     """BOI creation failed. Invalid wake levels input."""
     CREATEBOI_INVALIDTYPEFORWRAP = 386
     """BOI creation failed. Wrapping is invalid for this BOI type."""
-    CREATECONTACTPATCH_INVALIDOFFSETDISTANCE = 387
+    CREATEBOI_INVALIDSCOPE = 387
+    """BOI creation failed. Invalid face zonelets as input."""
+    CREATECONTACTPATCH_INVALIDOFFSETDISTANCE = 388
     """Contact patch creation process failed. Scale factors should not be less than zero."""
-    CREATECONTACTPATCH_INVALIDTOLERANCEVALUE = 390
+    CREATECONTACTPATCH_INVALIDTOLERANCEVALUE = 389
     """Contact patch creation process failed. Tolerance value should not be less than zero."""
-    CREATECONTACTPATCH_INVALIDCONTACTPATCHAXIS = 388
+    CREATECONTACTPATCH_INVALIDCONTACTPATCHAXIS = 390
     """Contact patch creation process failed. Invalid contact patch creation axis."""
-    CONTACTPATCHRESULTSFAILED = 389
+    CONTACTPATCHRESULTSFAILED = 391
     """Contact patch creation process failed. Check the inputs."""
     SIZEFIELDCOMPUTATIONFAILED = 400
     """Size field computation failed."""
     INVALIDSIZECONTROLS = 401
     """Invalid size controls."""
     REFRESHSIZEFIELDSFAILED = 402
     """Refreshing size field failed."""
@@ -230,14 +238,26 @@
     """Failed to write PMDAT file."""
     EXPORTFLUENTMESHINGMSHFAILED = 531
     """Export fluent meshing mesh failed."""
     WRITESIZEFIELDFAILED = 532
     """Writing size field failed."""
     MESHNOTFOUNDTOEXPORTFLUENTMESHINGMESH = 533
     """Mesh not found to export fluent meshing mesh."""
+    EXPORTSTLFAILEDWITHTOPOLOGY = 553
+    """Export STL not supported for part with topology data."""
+    EXPORTSTLFAILEDWITHQUADFACES = 554
+    """Export STL not supported for mesh with quad faces."""
+    EXPORTSTLFAILEDWITHPOLYFACES = 555
+    """Export STL not supported for mesh with poly faces."""
+    EXPORTSTLFAILEDWITHHIGHERORDERMESH = 556
+    """Export STL not supported for higher order mesh."""
+    EXPORTSTLFAILEDWITHEMPTYPARTIDLIST = 557
+    """Export STL failed. List of part ids is empty."""
+    EXPORTSTLFAILEDWITHINCORRECTPARTID = 558
+    """Export STL failed. Part id is incorrect."""
     MATCHEDMESHOPTIONINVALID = 850
     """Invalid option chosen to connect two different parts."""
     COLOCATEMATCHEDNODESFAILED = 851
     """Colocation of matched nodes failed."""
     IMPRINTBOUNDARYNODESFAILED = 852
     """Imprint of boundary nodes failed."""
     IMPRINTBOUNDARYEDGESFAILED = 853
@@ -278,14 +298,20 @@
     """Invalid input zonelets."""
     MERGEZONELETSFAILED = 1310
     """Merge zonelets failed."""
     MERGESMALLZONELETSSUPPORTEDFORFACEZONELETS = 1311
     """Merge small zonelets option is supported for only face zonelets."""
     INVALIDINPUTVOLUMES = 1312
     """Invalid input volumes."""
+    MORPHER_COMPUTEBCS = 1410
+    """Failed to compute boundary conditions."""
+    MORPHER_MATCHMORPHINVALIDSOURCEINPUT = 1450
+    """Invalid source input for match morphing."""
+    MORPHER_BCPAIRINPUTTYPEMISMATCH = 1451
+    """Entity type does not match with input for defined boundary condition pair."""
     INVALIDGLOBALMINMAX = 1500
     """Invalid global min and max value."""
     INVALIDSIZECONTROLINPUTS = 1501
     """Invalid size control input."""
     INVALIDSIZECONTROLSCOPE = 1502
     """Invalid size control scope."""
     INVALIDCURVATURESIZINGINPUT = 1503
@@ -340,14 +366,16 @@
     """Edge path computation failed."""
     IGA_INCORRECTDEGREE = 2415
     """Incorrect degree."""
     IGA_QUADRATICMESHINPUT = 2416
     """Quadratic mesh is not supported for solid spline creation."""
     IGA_UNIFORMTRIMMEDNURBSFAILED = 2417
     """Uniform trimmed spline creation failed."""
+    IGA_QUADTOSPLINEBASISFAILED = 2421
+    """Quad to spline operation failed."""
     PARTHASTOPOLOGY = 2800
     """Part has a topology."""
     SURFACESEARCHFAILED = 2802
     """Surface search failed."""
     SURFACESEARCHPARTWITHMESHNOTFOUND = 2803
     """Part with mesh not found for surface quality check."""
     INVALIDPLANEPOINTS = 2804
@@ -486,14 +514,52 @@
     """Target zonelets form a self intersecting volume."""
     TARGETZONELETS_NOTWATERTIGHT = 10003
     """Target zonelets do not form a watertight volume."""
     TOOLZONELETS_SELFINTERSECTING = 10004
     """Tool zonelets form a self intersecting volume."""
     TOOLZONELETS_NOTWATERTIGHT = 10005
     """Tool zonelets do not form a watertight volume."""
+    STACKER_INVALIDINPUTVOLUMES = 10101
+    """Invalid input volumes provided to stacker."""
+    STACKER_INVALIDPARAMS = 10102
+    """Invalid parameters provided to stacker."""
+    STACKER_FACESEPARATIONFAILED = 10103
+    """Stacker failed to separate base face."""
+    STACKER_FAILED = 10104
+    """Stacker failed to mesh the model."""
+    STACKER_NOFACEFOUNDINVOLUMES = 10105
+    """No faces are found in the specified volumes."""
+    STACKER_MESHEDFACESFOUND = 10106
+    """Some faces in the input model have existing mesh."""
+    STACKER_INVALIDBASEFACEINPUT = 10107
+    """Base face list input is invalid."""
+    STACKER_NONSTACKABLEVOLUMESFOUND = 10109
+    """Some volumes are not aligned in the stacking direction."""
+    STACKER_INCORRECTBODYDEFINITION = 10110
+    """Some bodies are intersecting or incorrectly defined."""
+    STACKER_BASEFACEUNMESHED = 10111
+    """Base face list input has unmeshed topofaces."""
+    INVALIDTHINVOLUMECONTROLS = 12010
+    """Invalid input provided. Invalid thin volume control."""
+    THINVOLUMECONTROLINVALIDSOURCESCOPE = 12020
+    """Invalid input provided. Source scope not found."""
+    THINVOLUMECONTROLINVALIDTARGETSCOPE = 12040
+    """Invalid input provided. Target scope not found."""
+    THINVOLUMECONTROLINVALIDSCOPE = 12060
+    """Invalid input provided. Source scope and target scope cannot be same."""
+    THINVOLUMECONTROLINVALIDSOURCESCOPEENTITY = 12080
+    """Invalid input provided. Invalid source scope entity."""
+    THINVOLUMECONTROLINVALIDTARGETSCOPEENTITY = 12100
+    """Invalid input provided. Invalid target scope entity."""
+    THINVOLUMECONTROLINVALIDNUMBEROFLAYER = 12120
+    """Invalid input provided. Number of layer in thin volume mesh should be greater than 0."""
+    THINVOLUMECONTROLTOPOLOGYNOTSUPPORTED = 12140
+    """Thin volume mesh controls not supported for part with topology data."""
+    MICROSTRUCTUREINVALIDELEMENTTYPE = 13000
+    """Invalid input provided. Invalid Element Type."""
 
 class WarningCode(enum.IntEnum):
     """Warning codes associated with the PyPrimeMesh operation.
     """
     NOWARNING = 0
     """No warnings."""
     UNKNOWN = 1
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/prismcontrol.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/prismcontrol.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,16 @@
             Parameters to set prism control growth.
 
         Examples
         --------
         >>> results = prism_control.set_growth_params(PrismControlGrowthParams(model=model))
 
         """
+        if not isinstance(prism_control_growth_params, PrismControlGrowthParams):
+            raise TypeError("Invalid argument type passed for prism_control_growth_params, valid argument type is PrismControlGrowthParams.")
         args = {"prism_control_growth_params" : prism_control_growth_params._jsonify()}
         command_name = "PrimeMesh::PrismControl/SetGrowthParams"
         self._model._print_logs_before_command("set_growth_params", args)
         self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("set_growth_params")
 
     def set_surface_scope(self, entities : ScopeDefinition) -> SetScopeResults:
@@ -56,14 +58,16 @@
 
 
         Examples
         --------
         >>> results = prism_control.set_surface_scope(entities)
 
         """
+        if not isinstance(entities, ScopeDefinition):
+            raise TypeError("Invalid argument type passed for entities, valid argument type is ScopeDefinition.")
         args = {"entities" : entities._jsonify()}
         command_name = "PrimeMesh::PrismControl/SetSurfaceScope"
         self._model._print_logs_before_command("set_surface_scope", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("set_surface_scope", SetScopeResults(model = self._model, json_data = result))
         return SetScopeResults(model = self._model, json_data = result)
 
@@ -83,14 +87,16 @@
 
 
         Examples
         --------
         >>> results = prism_control.set_volume_scope(entities)
 
         """
+        if not isinstance(entities, ScopeDefinition):
+            raise TypeError("Invalid argument type passed for entities, valid argument type is ScopeDefinition.")
         args = {"entities" : entities._jsonify()}
         command_name = "PrimeMesh::PrismControl/SetVolumeScope"
         self._model._print_logs_before_command("set_volume_scope", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("set_volume_scope", SetScopeResults(model = self._model, json_data = result))
         return SetScopeResults(model = self._model, json_data = result)
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/prismcontrolstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/prismcontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/scaffolder.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumecontrol.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,150 +1,160 @@
 """ Auto-generated file. DO NOT MODIFY """
 from __future__ import annotations
 from ansys.meshing.prime.internals.comm_manager import CommunicationManager
 from ansys.meshing.prime.params.primestructs import *
 from ansys.meshing.prime.autogen.coreobject import *
 from typing import List, Any, Union
 
-class Scaffolder(CoreObject):
-    """Scaffolder is used for achieving connections in structures made of sheets and beams. Solid bodies should be suppressed before applying scaffolding.
+class VolumeControl(CoreObject):
+    """Volume controls provide volume specific settings on volumes specified by scope and settings specified by parameters.
 
     """
 
-    def __init__(self, model: CommunicationManager, part_id: int):
-        """ Initialize Scaffolder  """
+    def __init__(self, model: CommunicationManager, id: int, object_id: int, name: str):
+        """ Initialize VolumeControl """
         self._model = model
         self._comm = model._communicator
-        command_name = "PrimeMesh::Scaffolder/Construct"
-        args = {"ModelID" : model._object_id , "PartID" : part_id, "MaxID" : -1}
-        result = self._comm.serve(model, command_name, args=args)
-        self._object_id = result["ObjectIndex"]
+        self._id = id
+        self._object_id = object_id
+        self._name = name
         self._freeze()
 
-    def __enter__(self):
-        """ Enter context for Scaffolder. """
-        return self
-
-    def __exit__(self, type, value, traceback) :
-        """ Exit context for Scaffolder. """
-        command_name = "PrimeMesh::Scaffolder/Destruct"
-        self._comm.serve(self._model, command_name, self._object_id, args={})
+    def set_params(self, volume_control_params : VolumeControlParams):
+        """ Sets the volume control parameters.
 
-    def scaffold_topo_faces_and_beams(self, topo_faces : Iterable[int], topo_beams : Iterable[int], params : ScaffolderParams) -> ScaffolderResults:
-        """ Scaffold faces and beams with provided parameters.
 
+        Parameters
+        ----------
+        volume_control_params : VolumeControlParams
+            Parameters to control volume.
+
+        Examples
+        --------
+        >>> volume_control.set_params(
+        >>>                  prime.VolumeControlParams(model=model,
+        >>>                  cell_zonelet_type = prime.CellZoneletType.FLUID))
+
+        """
+        if not isinstance(volume_control_params, VolumeControlParams):
+            raise TypeError("Invalid argument type passed for volume_control_params, valid argument type is VolumeControlParams.")
+        args = {"volume_control_params" : volume_control_params._jsonify()}
+        command_name = "PrimeMesh::VolumeControl/SetParams"
+        self._model._print_logs_before_command("set_params", args)
+        self._comm.serve(self._model, command_name, self._object_id, args=args)
+        self._model._print_logs_after_command("set_params")
+
+    def set_scope(self, scope : ScopeDefinition) -> SetScopeResults:
+        """ Sets the scope for volume control to evaluate.
+
+        Volume control uses scope to evaluate entities for which volume mesh needs to be generated.
 
         Parameters
         ----------
-        topo_faces : Iterable[int]
-            Ids of topology faces.
-        topo_beams : Iterable[int]
-            Ids of topology edges for beams.
-        params : ScaffolderParams
-            Scaffolding parameters.
+        scope : ScopeDefinition
+            ScopeDefinition to scope entities for volume mesh generation.
 
         Returns
         -------
-        ScaffolderResults
-            Return results in ScaffolderResults structure.
+        SetScopeResults
+            Returns a SetScopeResults.
 
 
         Examples
         --------
-        >>> results = scaffolder.ScaffoldTopoFacesAndBeams([1,2], [7,8], params)
+        >>> volume_control.set_scope(prime.ScopeDefinition(model=model,
+        >>>                        entity_type = ScopeEntity.VOLUMES,
+        >>>                        evaluation_type = ScopeEvaluationType.ZONES,
+        >>>                        zone_expression = "vol_in"))
 
         """
-        args = {"topo_faces" : topo_faces,
-        "topo_beams" : topo_beams,
-        "params" : params._jsonify()}
-        command_name = "PrimeMesh::Scaffolder/ScaffoldTopoFacesAndBeams"
-        self._model._print_logs_before_command("scaffold_topo_faces_and_beams", args)
+        if not isinstance(scope, ScopeDefinition):
+            raise TypeError("Invalid argument type passed for scope, valid argument type is ScopeDefinition.")
+        args = {"scope" : scope._jsonify()}
+        command_name = "PrimeMesh::VolumeControl/SetScope"
+        self._model._print_logs_before_command("set_scope", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("scaffold_topo_faces_and_beams", ScaffolderResults(model = self._model, json_data = result))
-        return ScaffolderResults(model = self._model, json_data = result)
+        self._model._print_logs_after_command("set_scope", SetScopeResults(model = self._model, json_data = result))
+        return SetScopeResults(model = self._model, json_data = result)
 
-    def split_topo_faces_by_mesh_region(self, topo_faces : Iterable[int]) -> ScaffolderSplitResults:
-        """ Split input topofaces by mesh region.
+    def set_suggested_name(self, name : str) -> SetNameResults:
+        """ Sets the unique name for the volume control based on the given suggested name.
 
 
         Parameters
         ----------
-        topo_faces : Iterable[int]
-            Ids of topology faces.
+        name : str
+            Suggested name for the volume control.
 
         Returns
         -------
-        ScaffolderSplitResults
-            Return results in ScaffolderSplitResults type.
+        SetNameResults
+            Returns a name of the volume control.
 
 
         Examples
         --------
-        >>> results = scaffolder.split_topo_faces_by_mesh_region([1,2,7,8])
+        >>> volume_control.set_suggested_name("control1")
 
         """
-        args = {"topo_faces" : topo_faces}
-        command_name = "PrimeMesh::Scaffolder/SplitTopoFacesByMeshRegion"
-        self._model._print_logs_before_command("split_topo_faces_by_mesh_region", args)
+        if not isinstance(name, str):
+            raise TypeError("Invalid argument type passed for name, valid argument type is str.")
+        args = {"name" : name}
+        command_name = "PrimeMesh::VolumeControl/SetSuggestedName"
+        self._model._print_logs_before_command("set_suggested_name", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("split_topo_faces_by_mesh_region", ScaffolderSplitResults(model = self._model, json_data = result))
-        return ScaffolderSplitResults(model = self._model, json_data = result)
-
-    def merge_overlapping_topo_faces(self, topo_faces : Iterable[int], params : ScaffolderParams) -> ScaffolderMergeResults:
-        """ Merge overlapping topofaces.
+        self._model._print_logs_after_command("set_suggested_name", SetNameResults(model = self._model, json_data = result))
+        return SetNameResults(model = self._model, json_data = result)
 
+    def get_scope(self) -> ScopeDefinition:
+        """ Gets the scope for the volume control.
 
-        Parameters
-        ----------
-        topo_faces : Iterable[int]
-            Ids of topology faces.
-        params : ScaffolderParams
-            Scaffolder parameters.
 
         Returns
         -------
-        ScaffolderMergeResults
-            Return results in ScaffolderMergeResults.
+        ScopeDefinition
+            Returns scope of the volume control.
 
 
         Examples
         --------
-        >>> results = scaffolder.MergeOverlappingTopoFaces([1,2,7,8], params)
+        >>> scope_definition = volume_control.get_scope()
 
         """
-        args = {"topo_faces" : topo_faces,
-        "params" : params._jsonify()}
-        command_name = "PrimeMesh::Scaffolder/MergeOverlappingTopoFaces"
-        self._model._print_logs_before_command("merge_overlapping_topo_faces", args)
+        args = {}
+        command_name = "PrimeMesh::VolumeControl/GetScope"
+        self._model._print_logs_before_command("get_scope", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("merge_overlapping_topo_faces", ScaffolderMergeResults(model = self._model, json_data = result))
-        return ScaffolderMergeResults(model = self._model, json_data = result)
+        self._model._print_logs_after_command("get_scope", ScopeDefinition(model = self._model, json_data = result))
+        return ScopeDefinition(model = self._model, json_data = result)
 
-    def delete_shadowed_topo_faces(self, topo_faces : Iterable[int], params : VolumetricScaffolderParams) -> ScaffolderMergeResults:
-        """ Delete fully shadowed topofaces.
+    def get_params(self) -> VolumeControlParams:
+        """ Get the parameters of the volume control.
 
 
-        Parameters
-        ----------
-        topo_faces : Iterable[int]
-            Ids of input topofaces.
-        params : VolumetricScaffolderParams
-            Volumetric scaffolder parameters.
-
         Returns
         -------
-        ScaffolderMergeResults
-            Return results in ScaffolderMergeResults.
+        VolumeControlParams
+            Return parameters of the volume control.
 
 
         Examples
         --------
-        >>> results = scaffolder.delete_shadowed_topo_faces([1,2,3,4,5], params)
+        >>> params = volume_control.get_params()
 
         """
-        args = {"topo_faces" : topo_faces,
-        "params" : params._jsonify()}
-        command_name = "PrimeMesh::Scaffolder/DeleteShadowedTopoFaces"
-        self._model._print_logs_before_command("delete_shadowed_topo_faces", args)
+        args = {}
+        command_name = "PrimeMesh::VolumeControl/GetParams"
+        self._model._print_logs_before_command("get_params", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
-        self._model._print_logs_after_command("delete_shadowed_topo_faces", ScaffolderMergeResults(model = self._model, json_data = result))
-        return ScaffolderMergeResults(model = self._model, json_data = result)
+        self._model._print_logs_after_command("get_params", VolumeControlParams(model = self._model, json_data = result))
+        return VolumeControlParams(model = self._model, json_data = result)
+
+    @property
+    def id(self):
+        """ Get the id of VolumeControl."""
+        return self._id
+
+    @property
+    def name(self):
+        """ Get the name of VolumeControl."""
+        return self._name
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/scaffolderstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/scaffolderstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/sizecontrolstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/sizecontrolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/sizefield.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/sizefield.py`

 * *Files 17% similar despite different names*

```diff
@@ -41,14 +41,18 @@
 
         Examples
         --------
         >>> size_field.compute_volumetric(
         >>>           [size_control.id for size_control in model.control_data.size_controls], volumetric_sizefield_params))
 
         """
+        if not isinstance(size_control_ids, Iterable):
+            raise TypeError("Invalid argument type passed for size_control_ids, valid argument type is Iterable[int].")
+        if not isinstance(volumetric_sizefield_params, VolumetricSizeFieldComputeParams):
+            raise TypeError("Invalid argument type passed for volumetric_sizefield_params, valid argument type is VolumetricSizeFieldComputeParams.")
         args = {"size_control_ids" : size_control_ids,
         "volumetric_sizefield_params" : volumetric_sizefield_params._jsonify()}
         command_name = "PrimeMesh::SizeField/ComputeVolumetric"
         self._model._print_logs_before_command("compute_volumetric", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("compute_volumetric", VolumetricSizeFieldComputeResults(model = self._model, json_data = result))
         return VolumetricSizeFieldComputeResults(model = self._model, json_data = result)
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/sizefieldstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/sizefieldstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/splittoolstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/splittoolstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/surfacesearchstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfacesearchstructs.py`

 * *Files 6% similar despite different names*

```diff
@@ -968,90 +968,112 @@
     """
     _default_params = {}
 
     def __initialize(
             self,
             strip_height_limit: float,
             quality_limit: float,
-            face_quality_measure: FaceQualityMeasure):
+            face_quality_measure: FaceQualityMeasure,
+            feature_type: SurfaceFeatureType,
+            feature_angle: float):
         self._strip_height_limit = strip_height_limit
         self._quality_limit = quality_limit
         self._face_quality_measure = FaceQualityMeasure(face_quality_measure)
+        self._feature_type = SurfaceFeatureType(feature_type)
+        self._feature_angle = feature_angle
 
     def __init__(
             self,
             model: CommunicationManager=None,
             strip_height_limit: float = None,
             quality_limit: float = None,
             face_quality_measure: FaceQualityMeasure = None,
+            feature_type: SurfaceFeatureType = None,
+            feature_angle: float = None,
             json_data : dict = None,
              **kwargs):
         """Initializes the SearchByThinStripParams.
 
         Parameters
         ----------
         model: Model
             Model to create a SearchByThinStripParams object with default parameters.
         strip_height_limit: float, optional
             Absolute height limit to ignore strips with height more than provided limit.
         quality_limit: float, optional
             Quality limit used for search strip of face elements.
         face_quality_measure: FaceQualityMeasure, optional
             Quality measure used for search strip of face elements.
+        feature_type: SurfaceFeatureType, optional
+            Used to identify thin strip of face elements based on the provided feature type.
+        feature_angle: float, optional
+            Angle used to identify angle based features.
         json_data: dict, optional
             JSON dictionary to create a SearchByThinStripParams object with provided parameters.
 
         Examples
         --------
         >>> search_by_thin_strip_params = prime.SearchByThinStripParams(model = model)
         """
         if json_data:
             self.__initialize(
                 json_data["stripHeightLimit"] if "stripHeightLimit" in json_data else None,
                 json_data["qualityLimit"] if "qualityLimit" in json_data else None,
-                FaceQualityMeasure(json_data["faceQualityMeasure"] if "faceQualityMeasure" in json_data else None))
+                FaceQualityMeasure(json_data["faceQualityMeasure"] if "faceQualityMeasure" in json_data else None),
+                SurfaceFeatureType(json_data["featureType"] if "featureType" in json_data else None),
+                json_data["featureAngle"] if "featureAngle" in json_data else None)
         else:
-            all_field_specified = all(arg is not None for arg in [strip_height_limit, quality_limit, face_quality_measure])
+            all_field_specified = all(arg is not None for arg in [strip_height_limit, quality_limit, face_quality_measure, feature_type, feature_angle])
             if all_field_specified:
                 self.__initialize(
                     strip_height_limit,
                     quality_limit,
-                    face_quality_measure)
+                    face_quality_measure,
+                    feature_type,
+                    feature_angle)
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
                     param_json = model._communicator.initialize_params(model, "SearchByThinStripParams")
                     json_data = param_json["SearchByThinStripParams"] if "SearchByThinStripParams" in param_json else {}
                     self.__initialize(
                         strip_height_limit if strip_height_limit is not None else ( SearchByThinStripParams._default_params["strip_height_limit"] if "strip_height_limit" in SearchByThinStripParams._default_params else (json_data["stripHeightLimit"] if "stripHeightLimit" in json_data else None)),
                         quality_limit if quality_limit is not None else ( SearchByThinStripParams._default_params["quality_limit"] if "quality_limit" in SearchByThinStripParams._default_params else (json_data["qualityLimit"] if "qualityLimit" in json_data else None)),
-                        face_quality_measure if face_quality_measure is not None else ( SearchByThinStripParams._default_params["face_quality_measure"] if "face_quality_measure" in SearchByThinStripParams._default_params else FaceQualityMeasure(json_data["faceQualityMeasure"] if "faceQualityMeasure" in json_data else None)))
+                        face_quality_measure if face_quality_measure is not None else ( SearchByThinStripParams._default_params["face_quality_measure"] if "face_quality_measure" in SearchByThinStripParams._default_params else FaceQualityMeasure(json_data["faceQualityMeasure"] if "faceQualityMeasure" in json_data else None)),
+                        feature_type if feature_type is not None else ( SearchByThinStripParams._default_params["feature_type"] if "feature_type" in SearchByThinStripParams._default_params else SurfaceFeatureType(json_data["featureType"] if "featureType" in json_data else None)),
+                        feature_angle if feature_angle is not None else ( SearchByThinStripParams._default_params["feature_angle"] if "feature_angle" in SearchByThinStripParams._default_params else (json_data["featureAngle"] if "featureAngle" in json_data else None)))
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
     def set_default(
             strip_height_limit: float = None,
             quality_limit: float = None,
-            face_quality_measure: FaceQualityMeasure = None):
+            face_quality_measure: FaceQualityMeasure = None,
+            feature_type: SurfaceFeatureType = None,
+            feature_angle: float = None):
         """Set the default values of SearchByThinStripParams.
 
         Parameters
         ----------
         strip_height_limit: float, optional
             Absolute height limit to ignore strips with height more than provided limit.
         quality_limit: float, optional
             Quality limit used for search strip of face elements.
         face_quality_measure: FaceQualityMeasure, optional
             Quality measure used for search strip of face elements.
+        feature_type: SurfaceFeatureType, optional
+            Used to identify thin strip of face elements based on the provided feature type.
+        feature_angle: float, optional
+            Angle used to identify angle based features.
         """
         args = locals()
         [SearchByThinStripParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
     def print_default():
         """Print the default values of SearchByThinStripParams.
@@ -1068,19 +1090,23 @@
         json_data = {}
         if self._strip_height_limit is not None:
             json_data["stripHeightLimit"] = self._strip_height_limit
         if self._quality_limit is not None:
             json_data["qualityLimit"] = self._quality_limit
         if self._face_quality_measure is not None:
             json_data["faceQualityMeasure"] = self._face_quality_measure
+        if self._feature_type is not None:
+            json_data["featureType"] = self._feature_type
+        if self._feature_angle is not None:
+            json_data["featureAngle"] = self._feature_angle
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "strip_height_limit :  %s\nquality_limit :  %s\nface_quality_measure :  %s" % (self._strip_height_limit, self._quality_limit, self._face_quality_measure)
+        message = "strip_height_limit :  %s\nquality_limit :  %s\nface_quality_measure :  %s\nfeature_type :  %s\nfeature_angle :  %s" % (self._strip_height_limit, self._quality_limit, self._face_quality_measure, self._feature_type, self._feature_angle)
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
     @property
     def strip_height_limit(self) -> float:
         """Absolute height limit to ignore strips with height more than provided limit.
         """
@@ -1106,14 +1132,34 @@
         """
         return self._face_quality_measure
 
     @face_quality_measure.setter
     def face_quality_measure(self, value: FaceQualityMeasure):
         self._face_quality_measure = value
 
+    @property
+    def feature_type(self) -> SurfaceFeatureType:
+        """Used to identify thin strip of face elements based on the provided feature type.
+        """
+        return self._feature_type
+
+    @feature_type.setter
+    def feature_type(self, value: SurfaceFeatureType):
+        self._feature_type = value
+
+    @property
+    def feature_angle(self) -> float:
+        """Angle used to identify angle based features.
+        """
+        return self._feature_angle
+
+    @feature_angle.setter
+    def feature_angle(self, value: float):
+        self._feature_angle = value
+
 class SearchByThinStripResults(CoreObject):
     """Results associated with search by thin strip of face elements.
     """
     _default_params = {}
 
     def __initialize(
             self,
@@ -2372,7 +2418,232 @@
         """Ids of the face zonelets containing atleast one registered face element.
         """
         return self._face_zonelets_found
 
     @face_zonelets_found.setter
     def face_zonelets_found(self, value: Iterable[int]):
         self._face_zonelets_found = value
+
+class CheckFaceDeviationParams(CoreObject):
+    """Parameters used for check face deviation operations.
+    """
+    _default_params = {}
+
+    def __initialize(
+            self,
+            distance: float):
+        self._distance = distance
+
+    def __init__(
+            self,
+            model: CommunicationManager=None,
+            distance: float = None,
+            json_data : dict = None,
+             **kwargs):
+        """Initializes the CheckFaceDeviationParams.
+
+        Parameters
+        ----------
+        model: Model
+            Model to create a CheckFaceDeviationParams object with default parameters.
+        distance: float, optional
+            Distance above which deviated entities are collected.
+        json_data: dict, optional
+            JSON dictionary to create a CheckFaceDeviationParams object with provided parameters.
+
+        Examples
+        --------
+        >>> check_face_deviation_params = prime.CheckFaceDeviationParams(model = model)
+        """
+        if json_data:
+            self.__initialize(
+                json_data["distance"] if "distance" in json_data else None)
+        else:
+            all_field_specified = all(arg is not None for arg in [distance])
+            if all_field_specified:
+                self.__initialize(
+                    distance)
+            else:
+                if model is None:
+                    raise ValueError("Invalid assignment. Either pass model or specify all properties")
+                else:
+                    param_json = model._communicator.initialize_params(model, "CheckFaceDeviationParams")
+                    json_data = param_json["CheckFaceDeviationParams"] if "CheckFaceDeviationParams" in param_json else {}
+                    self.__initialize(
+                        distance if distance is not None else ( CheckFaceDeviationParams._default_params["distance"] if "distance" in CheckFaceDeviationParams._default_params else (json_data["distance"] if "distance" in json_data else None)))
+        self._custom_params = kwargs
+        if model is not None:
+            [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
+        [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
+        lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
+        self._freeze()
+
+    @staticmethod
+    def set_default(
+            distance: float = None):
+        """Set the default values of CheckFaceDeviationParams.
+
+        Parameters
+        ----------
+        distance: float, optional
+            Distance above which deviated entities are collected.
+        """
+        args = locals()
+        [CheckFaceDeviationParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+
+    @staticmethod
+    def print_default():
+        """Print the default values of CheckFaceDeviationParams.
+
+        Examples
+        --------
+        >>> CheckFaceDeviationParams.print_default()
+        """
+        message = ""
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in CheckFaceDeviationParams._default_params.items())
+        print(message)
+
+    def _jsonify(self) -> Dict[str, Any]:
+        json_data = {}
+        if self._distance is not None:
+            json_data["distance"] = self._distance
+        [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
+        return json_data
+
+    def __str__(self) -> str:
+        message = "distance :  %s" % (self._distance)
+        message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
+        return message
+
+    @property
+    def distance(self) -> float:
+        """Distance above which deviated entities are collected.
+        """
+        return self._distance
+
+    @distance.setter
+    def distance(self, value: float):
+        self._distance = value
+
+class CheckFaceDeviationResults(CoreObject):
+    """Result structure associated with the check face deviation operations.
+    """
+    _default_params = {}
+
+    def __initialize(
+            self,
+            n_deviated: int,
+            maximum_deviation: float):
+        self._n_deviated = n_deviated
+        self._maximum_deviation = maximum_deviation
+
+    def __init__(
+            self,
+            model: CommunicationManager=None,
+            n_deviated: int = None,
+            maximum_deviation: float = None,
+            json_data : dict = None,
+             **kwargs):
+        """Initializes the CheckFaceDeviationResults.
+
+        Parameters
+        ----------
+        model: Model
+            Model to create a CheckFaceDeviationResults object with default parameters.
+        n_deviated: int, optional
+            Number of faces with deviation.
+        maximum_deviation: float, optional
+            Maximum deviation found.
+        json_data: dict, optional
+            JSON dictionary to create a CheckFaceDeviationResults object with provided parameters.
+
+        Examples
+        --------
+        >>> check_face_deviation_results = prime.CheckFaceDeviationResults(model = model)
+        """
+        if json_data:
+            self.__initialize(
+                json_data["nDeviated"] if "nDeviated" in json_data else None,
+                json_data["maximumDeviation"] if "maximumDeviation" in json_data else None)
+        else:
+            all_field_specified = all(arg is not None for arg in [n_deviated, maximum_deviation])
+            if all_field_specified:
+                self.__initialize(
+                    n_deviated,
+                    maximum_deviation)
+            else:
+                if model is None:
+                    raise ValueError("Invalid assignment. Either pass model or specify all properties")
+                else:
+                    param_json = model._communicator.initialize_params(model, "CheckFaceDeviationResults")
+                    json_data = param_json["CheckFaceDeviationResults"] if "CheckFaceDeviationResults" in param_json else {}
+                    self.__initialize(
+                        n_deviated if n_deviated is not None else ( CheckFaceDeviationResults._default_params["n_deviated"] if "n_deviated" in CheckFaceDeviationResults._default_params else (json_data["nDeviated"] if "nDeviated" in json_data else None)),
+                        maximum_deviation if maximum_deviation is not None else ( CheckFaceDeviationResults._default_params["maximum_deviation"] if "maximum_deviation" in CheckFaceDeviationResults._default_params else (json_data["maximumDeviation"] if "maximumDeviation" in json_data else None)))
+        self._custom_params = kwargs
+        if model is not None:
+            [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
+        [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
+        lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
+        self._freeze()
+
+    @staticmethod
+    def set_default(
+            n_deviated: int = None,
+            maximum_deviation: float = None):
+        """Set the default values of CheckFaceDeviationResults.
+
+        Parameters
+        ----------
+        n_deviated: int, optional
+            Number of faces with deviation.
+        maximum_deviation: float, optional
+            Maximum deviation found.
+        """
+        args = locals()
+        [CheckFaceDeviationResults._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+
+    @staticmethod
+    def print_default():
+        """Print the default values of CheckFaceDeviationResults.
+
+        Examples
+        --------
+        >>> CheckFaceDeviationResults.print_default()
+        """
+        message = ""
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in CheckFaceDeviationResults._default_params.items())
+        print(message)
+
+    def _jsonify(self) -> Dict[str, Any]:
+        json_data = {}
+        if self._n_deviated is not None:
+            json_data["nDeviated"] = self._n_deviated
+        if self._maximum_deviation is not None:
+            json_data["maximumDeviation"] = self._maximum_deviation
+        [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
+        return json_data
+
+    def __str__(self) -> str:
+        message = "n_deviated :  %s\nmaximum_deviation :  %s" % (self._n_deviated, self._maximum_deviation)
+        message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
+        return message
+
+    @property
+    def n_deviated(self) -> int:
+        """Number of faces with deviation.
+        """
+        return self._n_deviated
+
+    @n_deviated.setter
+    def n_deviated(self, value: int):
+        self._n_deviated = value
+
+    @property
+    def maximum_deviation(self) -> float:
+        """Maximum deviation found.
+        """
+        return self._maximum_deviation
+
+    @maximum_deviation.setter
+    def maximum_deviation(self, value: float):
+        self._maximum_deviation = value
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surfaceutilitystructs.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,168 +40,262 @@
     """BOI type for BOI creation.
     """
     OFFSETBOX = 1
     """Box BOI type for BOI creation."""
     OFFSETSURFACE = 2
     """Surface BOI type for BOI creation."""
 
-class SphereAtInvalidNormalNodeParams(CoreObject):
-    """Parameters to create a sphere at nodes with invalid average face normal. The sphere creation is expected to correct the face normal at the node.
+class FixInvalidNormalNodeParams(CoreObject):
+    """Parameters to fix invalid average face normal at nodes by creating a nugget.
     """
     _default_params = {}
 
     def __initialize(
-            self):
-        pass
+            self,
+            nugget_size: float,
+            nugget_mesh_size: float,
+            label: str):
+        self._nugget_size = nugget_size
+        self._nugget_mesh_size = nugget_mesh_size
+        self._label = label
 
     def __init__(
             self,
             model: CommunicationManager=None,
+            nugget_size: float = None,
+            nugget_mesh_size: float = None,
+            label: str = None,
             json_data : dict = None,
              **kwargs):
-        """Initializes the SphereAtInvalidNormalNodeParams.
+        """Initializes the FixInvalidNormalNodeParams.
 
         Parameters
         ----------
         model: Model
-            Model to create a SphereAtInvalidNormalNodeParams object with default parameters.
+            Model to create a FixInvalidNormalNodeParams object with default parameters.
+        nugget_size: float, optional
+            Relative size used to create nugget at invalid normal node. The size is relative to mesh size at the node.
+        nugget_mesh_size: float, optional
+            Relative size used as max size to mesh nugget created at invalid normal node. The size is relative to mesh size at the node.
+        label: str, optional
+            Label to set on new face zonelets created.
         json_data: dict, optional
-            JSON dictionary to create a SphereAtInvalidNormalNodeParams object with provided parameters.
+            JSON dictionary to create a FixInvalidNormalNodeParams object with provided parameters.
 
         Examples
         --------
-        >>> sphere_at_invalid_normal_node_params = prime.SphereAtInvalidNormalNodeParams(model = model)
+        >>> fix_invalid_normal_node_params = prime.FixInvalidNormalNodeParams(model = model)
         """
         if json_data:
-            self.__initialize()
+            self.__initialize(
+                json_data["nuggetSize"] if "nuggetSize" in json_data else None,
+                json_data["nuggetMeshSize"] if "nuggetMeshSize" in json_data else None,
+                json_data["label"] if "label" in json_data else None)
         else:
-            all_field_specified = all(arg is not None for arg in [])
+            all_field_specified = all(arg is not None for arg in [nugget_size, nugget_mesh_size, label])
             if all_field_specified:
-                self.__initialize()
+                self.__initialize(
+                    nugget_size,
+                    nugget_mesh_size,
+                    label)
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
-                    param_json = model._communicator.initialize_params(model, "SphereAtInvalidNormalNodeParams")
-                    json_data = param_json["SphereAtInvalidNormalNodeParams"] if "SphereAtInvalidNormalNodeParams" in param_json else {}
-                    self.__initialize()
+                    param_json = model._communicator.initialize_params(model, "FixInvalidNormalNodeParams")
+                    json_data = param_json["FixInvalidNormalNodeParams"] if "FixInvalidNormalNodeParams" in param_json else {}
+                    self.__initialize(
+                        nugget_size if nugget_size is not None else ( FixInvalidNormalNodeParams._default_params["nugget_size"] if "nugget_size" in FixInvalidNormalNodeParams._default_params else (json_data["nuggetSize"] if "nuggetSize" in json_data else None)),
+                        nugget_mesh_size if nugget_mesh_size is not None else ( FixInvalidNormalNodeParams._default_params["nugget_mesh_size"] if "nugget_mesh_size" in FixInvalidNormalNodeParams._default_params else (json_data["nuggetMeshSize"] if "nuggetMeshSize" in json_data else None)),
+                        label if label is not None else ( FixInvalidNormalNodeParams._default_params["label"] if "label" in FixInvalidNormalNodeParams._default_params else (json_data["label"] if "label" in json_data else None)))
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
-    def set_default():
-        """Set the default values of SphereAtInvalidNormalNodeParams.
+    def set_default(
+            nugget_size: float = None,
+            nugget_mesh_size: float = None,
+            label: str = None):
+        """Set the default values of FixInvalidNormalNodeParams.
 
+        Parameters
+        ----------
+        nugget_size: float, optional
+            Relative size used to create nugget at invalid normal node. The size is relative to mesh size at the node.
+        nugget_mesh_size: float, optional
+            Relative size used as max size to mesh nugget created at invalid normal node. The size is relative to mesh size at the node.
+        label: str, optional
+            Label to set on new face zonelets created.
         """
         args = locals()
-        [SphereAtInvalidNormalNodeParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+        [FixInvalidNormalNodeParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
     def print_default():
-        """Print the default values of SphereAtInvalidNormalNodeParams.
+        """Print the default values of FixInvalidNormalNodeParams.
 
         Examples
         --------
-        >>> SphereAtInvalidNormalNodeParams.print_default()
+        >>> FixInvalidNormalNodeParams.print_default()
         """
         message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in SphereAtInvalidNormalNodeParams._default_params.items())
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in FixInvalidNormalNodeParams._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
+        if self._nugget_size is not None:
+            json_data["nuggetSize"] = self._nugget_size
+        if self._nugget_mesh_size is not None:
+            json_data["nuggetMeshSize"] = self._nugget_mesh_size
+        if self._label is not None:
+            json_data["label"] = self._label
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "" % ()
+        message = "nugget_size :  %s\nnugget_mesh_size :  %s\nlabel :  %s" % (self._nugget_size, self._nugget_mesh_size, self._label)
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
-class SphereAtInvalidNormalNodeResults(CoreObject):
-    """Results associated with create sphere at invalid normal nodes.
+    @property
+    def nugget_size(self) -> float:
+        """Relative size used to create nugget at invalid normal node. The size is relative to mesh size at the node.
+        """
+        return self._nugget_size
+
+    @nugget_size.setter
+    def nugget_size(self, value: float):
+        self._nugget_size = value
+
+    @property
+    def nugget_mesh_size(self) -> float:
+        """Relative size used as max size to mesh nugget created at invalid normal node. The size is relative to mesh size at the node.
+        """
+        return self._nugget_mesh_size
+
+    @nugget_mesh_size.setter
+    def nugget_mesh_size(self, value: float):
+        self._nugget_mesh_size = value
+
+    @property
+    def label(self) -> str:
+        """Label to set on new face zonelets created.
+        """
+        return self._label
+
+    @label.setter
+    def label(self, value: str):
+        self._label = value
+
+class FixInvalidNormalNodeResults(CoreObject):
+    """Results associated with fix invalid average face normal at nodes.
     """
     _default_params = {}
 
     def __initialize(
-            self):
-        pass
+            self,
+            error_code: ErrorCode):
+        self._error_code = ErrorCode(error_code)
 
     def __init__(
             self,
             model: CommunicationManager=None,
+            error_code: ErrorCode = None,
             json_data : dict = None,
              **kwargs):
-        """Initializes the SphereAtInvalidNormalNodeResults.
+        """Initializes the FixInvalidNormalNodeResults.
 
         Parameters
         ----------
         model: Model
-            Model to create a SphereAtInvalidNormalNodeResults object with default parameters.
+            Model to create a FixInvalidNormalNodeResults object with default parameters.
+        error_code: ErrorCode, optional
+            Error code associated with failure of operation.
         json_data: dict, optional
-            JSON dictionary to create a SphereAtInvalidNormalNodeResults object with provided parameters.
+            JSON dictionary to create a FixInvalidNormalNodeResults object with provided parameters.
 
         Examples
         --------
-        >>> sphere_at_invalid_normal_node_results = prime.SphereAtInvalidNormalNodeResults(model = model)
+        >>> fix_invalid_normal_node_results = prime.FixInvalidNormalNodeResults(model = model)
         """
         if json_data:
-            self.__initialize()
+            self.__initialize(
+                ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None))
         else:
-            all_field_specified = all(arg is not None for arg in [])
+            all_field_specified = all(arg is not None for arg in [error_code])
             if all_field_specified:
-                self.__initialize()
+                self.__initialize(
+                    error_code)
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
-                    param_json = model._communicator.initialize_params(model, "SphereAtInvalidNormalNodeResults")
-                    json_data = param_json["SphereAtInvalidNormalNodeResults"] if "SphereAtInvalidNormalNodeResults" in param_json else {}
-                    self.__initialize()
+                    param_json = model._communicator.initialize_params(model, "FixInvalidNormalNodeResults")
+                    json_data = param_json["FixInvalidNormalNodeResults"] if "FixInvalidNormalNodeResults" in param_json else {}
+                    self.__initialize(
+                        error_code if error_code is not None else ( FixInvalidNormalNodeResults._default_params["error_code"] if "error_code" in FixInvalidNormalNodeResults._default_params else ErrorCode(json_data["errorCode"] if "errorCode" in json_data else None)))
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
-    def set_default():
-        """Set the default values of SphereAtInvalidNormalNodeResults.
+    def set_default(
+            error_code: ErrorCode = None):
+        """Set the default values of FixInvalidNormalNodeResults.
 
+        Parameters
+        ----------
+        error_code: ErrorCode, optional
+            Error code associated with failure of operation.
         """
         args = locals()
-        [SphereAtInvalidNormalNodeResults._default_params.update({ key: value }) for key, value in args.items() if value is not None]
+        [FixInvalidNormalNodeResults._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
     def print_default():
-        """Print the default values of SphereAtInvalidNormalNodeResults.
+        """Print the default values of FixInvalidNormalNodeResults.
 
         Examples
         --------
-        >>> SphereAtInvalidNormalNodeResults.print_default()
+        >>> FixInvalidNormalNodeResults.print_default()
         """
         message = ""
-        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in SphereAtInvalidNormalNodeResults._default_params.items())
+        message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in FixInvalidNormalNodeResults._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
+        if self._error_code is not None:
+            json_data["errorCode"] = self._error_code
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "" % ()
+        message = "error_code :  %s" % (self._error_code)
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
+    @property
+    def error_code(self) -> ErrorCode:
+        """Error code associated with failure of operation.
+        """
+        return self._error_code
+
+    @error_code.setter
+    def error_code(self, value: ErrorCode):
+        self._error_code = value
+
 class CopyZoneletsParams(CoreObject):
     """Parameters to copy zonelets. This is for internal use only.
     """
     _default_params = {}
 
     def __initialize(
             self):
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/surferstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/surferstructs.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,68 +19,83 @@
 class SurferParams(CoreObject):
     """Parameters used to generate surface mesh.
     """
     _default_params = {}
 
     def __initialize(
             self,
+            max_angle: float,
             size_field_type: SizeFieldType,
             min_size: float,
             max_size: float,
             growth_rate: float,
             constant_size: float,
             generate_quads: bool,
+            check_non_manifolds: bool,
+            avoid_corner_triangles: bool,
             smooth_size_transition: bool,
             advanced_surfer_setup: AdvancedSurferSetup,
             project_on_geometry: bool,
             enable_multi_threading: bool):
+        self._max_angle = max_angle
         self._size_field_type = SizeFieldType(size_field_type)
         self._min_size = min_size
         self._max_size = max_size
         self._growth_rate = growth_rate
         self._constant_size = constant_size
         self._generate_quads = generate_quads
+        self._check_non_manifolds = check_non_manifolds
+        self._avoid_corner_triangles = avoid_corner_triangles
         self._smooth_size_transition = smooth_size_transition
         self._advanced_surfer_setup = AdvancedSurferSetup(advanced_surfer_setup)
         self._project_on_geometry = project_on_geometry
         self._enable_multi_threading = enable_multi_threading
 
     def __init__(
             self,
             model: CommunicationManager=None,
+            max_angle: float = None,
             size_field_type: SizeFieldType = None,
             min_size: float = None,
             max_size: float = None,
             growth_rate: float = None,
             constant_size: float = None,
             generate_quads: bool = None,
+            check_non_manifolds: bool = None,
+            avoid_corner_triangles: bool = None,
             smooth_size_transition: bool = None,
             advanced_surfer_setup: AdvancedSurferSetup = None,
             project_on_geometry: bool = None,
             enable_multi_threading: bool = None,
             json_data : dict = None,
              **kwargs):
         """Initializes the SurferParams.
 
         Parameters
         ----------
         model: Model
             Model to create a SurferParams object with default parameters.
+        max_angle: float, optional
+            Maximum feature angle limit to be used to identify and preserve features.
         size_field_type: SizeFieldType, optional
             Size field type used to generate surface mesh.
         min_size: float, optional
             Minimum size to be used in sizing for the surfer.
         max_size: float, optional
             Maximum size to be used in sizing for the surfer.
         growth_rate: float, optional
             Growth rate to be used to propagate sizes.
         constant_size: float, optional
             Size used in constant size surface meshing.
         generate_quads: bool, optional
             Option to generate quadrilateral surface mesh.
+        check_non_manifolds: bool, optional
+            Option to avoid new non-manifolds(multi-connection) if generated in surface mesh.
+        avoid_corner_triangles: bool, optional
+            Option to avoid corner triangles(with all three boundary nodes) generated.
         smooth_size_transition: bool, optional
             Option to generate mesh with smooth size transition from neighbors of selected surfaces. This includes neighboring face edge sizes in sizing provided for surface meshing to achieve smooth size transition.
         advanced_surfer_setup: AdvancedSurferSetup, optional
             Option to define advanced settings for remeshing operation.
         project_on_geometry: bool, optional
             Option to project on CAD geometry when meshing.
         enable_multi_threading: bool, optional
@@ -90,90 +105,108 @@
 
         Examples
         --------
         >>> surfer_params = prime.SurferParams(model = model)
         """
         if json_data:
             self.__initialize(
+                json_data["maxAngle"] if "maxAngle" in json_data else None,
                 SizeFieldType(json_data["sizeFieldType"] if "sizeFieldType" in json_data else None),
                 json_data["minSize"] if "minSize" in json_data else None,
                 json_data["maxSize"] if "maxSize" in json_data else None,
                 json_data["growthRate"] if "growthRate" in json_data else None,
                 json_data["constantSize"] if "constantSize" in json_data else None,
                 json_data["generateQuads"] if "generateQuads" in json_data else None,
+                json_data["checkNonManifolds"] if "checkNonManifolds" in json_data else None,
+                json_data["avoidCornerTriangles"] if "avoidCornerTriangles" in json_data else None,
                 json_data["smoothSizeTransition"] if "smoothSizeTransition" in json_data else None,
                 AdvancedSurferSetup(json_data["advancedSurferSetup"] if "advancedSurferSetup" in json_data else None),
                 json_data["projectOnGeometry"] if "projectOnGeometry" in json_data else None,
                 json_data["enableMultiThreading"] if "enableMultiThreading" in json_data else None)
         else:
-            all_field_specified = all(arg is not None for arg in [size_field_type, min_size, max_size, growth_rate, constant_size, generate_quads, smooth_size_transition, advanced_surfer_setup, project_on_geometry, enable_multi_threading])
+            all_field_specified = all(arg is not None for arg in [max_angle, size_field_type, min_size, max_size, growth_rate, constant_size, generate_quads, check_non_manifolds, avoid_corner_triangles, smooth_size_transition, advanced_surfer_setup, project_on_geometry, enable_multi_threading])
             if all_field_specified:
                 self.__initialize(
+                    max_angle,
                     size_field_type,
                     min_size,
                     max_size,
                     growth_rate,
                     constant_size,
                     generate_quads,
+                    check_non_manifolds,
+                    avoid_corner_triangles,
                     smooth_size_transition,
                     advanced_surfer_setup,
                     project_on_geometry,
                     enable_multi_threading)
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
                     param_json = model._communicator.initialize_params(model, "SurferParams")
                     json_data = param_json["SurferParams"] if "SurferParams" in param_json else {}
                     self.__initialize(
+                        max_angle if max_angle is not None else ( SurferParams._default_params["max_angle"] if "max_angle" in SurferParams._default_params else (json_data["maxAngle"] if "maxAngle" in json_data else None)),
                         size_field_type if size_field_type is not None else ( SurferParams._default_params["size_field_type"] if "size_field_type" in SurferParams._default_params else SizeFieldType(json_data["sizeFieldType"] if "sizeFieldType" in json_data else None)),
                         min_size if min_size is not None else ( SurferParams._default_params["min_size"] if "min_size" in SurferParams._default_params else (json_data["minSize"] if "minSize" in json_data else None)),
                         max_size if max_size is not None else ( SurferParams._default_params["max_size"] if "max_size" in SurferParams._default_params else (json_data["maxSize"] if "maxSize" in json_data else None)),
                         growth_rate if growth_rate is not None else ( SurferParams._default_params["growth_rate"] if "growth_rate" in SurferParams._default_params else (json_data["growthRate"] if "growthRate" in json_data else None)),
                         constant_size if constant_size is not None else ( SurferParams._default_params["constant_size"] if "constant_size" in SurferParams._default_params else (json_data["constantSize"] if "constantSize" in json_data else None)),
                         generate_quads if generate_quads is not None else ( SurferParams._default_params["generate_quads"] if "generate_quads" in SurferParams._default_params else (json_data["generateQuads"] if "generateQuads" in json_data else None)),
+                        check_non_manifolds if check_non_manifolds is not None else ( SurferParams._default_params["check_non_manifolds"] if "check_non_manifolds" in SurferParams._default_params else (json_data["checkNonManifolds"] if "checkNonManifolds" in json_data else None)),
+                        avoid_corner_triangles if avoid_corner_triangles is not None else ( SurferParams._default_params["avoid_corner_triangles"] if "avoid_corner_triangles" in SurferParams._default_params else (json_data["avoidCornerTriangles"] if "avoidCornerTriangles" in json_data else None)),
                         smooth_size_transition if smooth_size_transition is not None else ( SurferParams._default_params["smooth_size_transition"] if "smooth_size_transition" in SurferParams._default_params else (json_data["smoothSizeTransition"] if "smoothSizeTransition" in json_data else None)),
                         advanced_surfer_setup if advanced_surfer_setup is not None else ( SurferParams._default_params["advanced_surfer_setup"] if "advanced_surfer_setup" in SurferParams._default_params else AdvancedSurferSetup(json_data["advancedSurferSetup"] if "advancedSurferSetup" in json_data else None)),
                         project_on_geometry if project_on_geometry is not None else ( SurferParams._default_params["project_on_geometry"] if "project_on_geometry" in SurferParams._default_params else (json_data["projectOnGeometry"] if "projectOnGeometry" in json_data else None)),
                         enable_multi_threading if enable_multi_threading is not None else ( SurferParams._default_params["enable_multi_threading"] if "enable_multi_threading" in SurferParams._default_params else (json_data["enableMultiThreading"] if "enableMultiThreading" in json_data else None)))
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
     def set_default(
+            max_angle: float = None,
             size_field_type: SizeFieldType = None,
             min_size: float = None,
             max_size: float = None,
             growth_rate: float = None,
             constant_size: float = None,
             generate_quads: bool = None,
+            check_non_manifolds: bool = None,
+            avoid_corner_triangles: bool = None,
             smooth_size_transition: bool = None,
             advanced_surfer_setup: AdvancedSurferSetup = None,
             project_on_geometry: bool = None,
             enable_multi_threading: bool = None):
         """Set the default values of SurferParams.
 
         Parameters
         ----------
+        max_angle: float, optional
+            Maximum feature angle limit to be used to identify and preserve features.
         size_field_type: SizeFieldType, optional
             Size field type used to generate surface mesh.
         min_size: float, optional
             Minimum size to be used in sizing for the surfer.
         max_size: float, optional
             Maximum size to be used in sizing for the surfer.
         growth_rate: float, optional
             Growth rate to be used to propagate sizes.
         constant_size: float, optional
             Size used in constant size surface meshing.
         generate_quads: bool, optional
             Option to generate quadrilateral surface mesh.
+        check_non_manifolds: bool, optional
+            Option to avoid new non-manifolds(multi-connection) if generated in surface mesh.
+        avoid_corner_triangles: bool, optional
+            Option to avoid corner triangles(with all three boundary nodes) generated.
         smooth_size_transition: bool, optional
             Option to generate mesh with smooth size transition from neighbors of selected surfaces. This includes neighboring face edge sizes in sizing provided for surface meshing to achieve smooth size transition.
         advanced_surfer_setup: AdvancedSurferSetup, optional
             Option to define advanced settings for remeshing operation.
         project_on_geometry: bool, optional
             Option to project on CAD geometry when meshing.
         enable_multi_threading: bool, optional
@@ -192,43 +225,59 @@
         """
         message = ""
         message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in SurferParams._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
+        if self._max_angle is not None:
+            json_data["maxAngle"] = self._max_angle
         if self._size_field_type is not None:
             json_data["sizeFieldType"] = self._size_field_type
         if self._min_size is not None:
             json_data["minSize"] = self._min_size
         if self._max_size is not None:
             json_data["maxSize"] = self._max_size
         if self._growth_rate is not None:
             json_data["growthRate"] = self._growth_rate
         if self._constant_size is not None:
             json_data["constantSize"] = self._constant_size
         if self._generate_quads is not None:
             json_data["generateQuads"] = self._generate_quads
+        if self._check_non_manifolds is not None:
+            json_data["checkNonManifolds"] = self._check_non_manifolds
+        if self._avoid_corner_triangles is not None:
+            json_data["avoidCornerTriangles"] = self._avoid_corner_triangles
         if self._smooth_size_transition is not None:
             json_data["smoothSizeTransition"] = self._smooth_size_transition
         if self._advanced_surfer_setup is not None:
             json_data["advancedSurferSetup"] = self._advanced_surfer_setup
         if self._project_on_geometry is not None:
             json_data["projectOnGeometry"] = self._project_on_geometry
         if self._enable_multi_threading is not None:
             json_data["enableMultiThreading"] = self._enable_multi_threading
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "size_field_type :  %s\nmin_size :  %s\nmax_size :  %s\ngrowth_rate :  %s\nconstant_size :  %s\ngenerate_quads :  %s\nsmooth_size_transition :  %s\nadvanced_surfer_setup :  %s\nproject_on_geometry :  %s\nenable_multi_threading :  %s" % (self._size_field_type, self._min_size, self._max_size, self._growth_rate, self._constant_size, self._generate_quads, self._smooth_size_transition, self._advanced_surfer_setup, self._project_on_geometry, self._enable_multi_threading)
+        message = "max_angle :  %s\nsize_field_type :  %s\nmin_size :  %s\nmax_size :  %s\ngrowth_rate :  %s\nconstant_size :  %s\ngenerate_quads :  %s\ncheck_non_manifolds :  %s\navoid_corner_triangles :  %s\nsmooth_size_transition :  %s\nadvanced_surfer_setup :  %s\nproject_on_geometry :  %s\nenable_multi_threading :  %s" % (self._max_angle, self._size_field_type, self._min_size, self._max_size, self._growth_rate, self._constant_size, self._generate_quads, self._check_non_manifolds, self._avoid_corner_triangles, self._smooth_size_transition, self._advanced_surfer_setup, self._project_on_geometry, self._enable_multi_threading)
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
     @property
+    def max_angle(self) -> float:
+        """Maximum feature angle limit to be used to identify and preserve features.
+        """
+        return self._max_angle
+
+    @max_angle.setter
+    def max_angle(self, value: float):
+        self._max_angle = value
+
+    @property
     def size_field_type(self) -> SizeFieldType:
         """Size field type used to generate surface mesh.
         """
         return self._size_field_type
 
     @size_field_type.setter
     def size_field_type(self, value: SizeFieldType):
@@ -281,14 +330,34 @@
         return self._generate_quads
 
     @generate_quads.setter
     def generate_quads(self, value: bool):
         self._generate_quads = value
 
     @property
+    def check_non_manifolds(self) -> bool:
+        """Option to avoid new non-manifolds(multi-connection) if generated in surface mesh.
+        """
+        return self._check_non_manifolds
+
+    @check_non_manifolds.setter
+    def check_non_manifolds(self, value: bool):
+        self._check_non_manifolds = value
+
+    @property
+    def avoid_corner_triangles(self) -> bool:
+        """Option to avoid corner triangles(with all three boundary nodes) generated.
+        """
+        return self._avoid_corner_triangles
+
+    @avoid_corner_triangles.setter
+    def avoid_corner_triangles(self, value: bool):
+        self._avoid_corner_triangles = value
+
+    @property
     def smooth_size_transition(self) -> bool:
         """Option to generate mesh with smooth size transition from neighbors of selected surfaces. This includes neighboring face edge sizes in sizing provided for surface meshing to achieve smooth size transition.
 
         Notes
          -----
           - Input facets or mesh with finer sizes compared to neighboring face edge sizes are required for this option to work.
           - Valid min, max sizes and growth rate are required to include the neighboring face edges sizes in sizing.
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/topoutilities.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/topoutilities.py`

 * *Files 18% similar despite different names*

```diff
@@ -47,14 +47,18 @@
 
 
         Examples
         --------
         >>> results = topo_utils.fill_hole(topo_edges, params)
 
         """
+        if not isinstance(topo_edges, Iterable):
+            raise TypeError("Invalid argument type passed for topo_edges, valid argument type is Iterable[int].")
+        if not isinstance(params, TopoFillHoleParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is TopoFillHoleParams.")
         args = {"topo_edges" : topo_edges,
         "params" : params._jsonify()}
         command_name = "PrimeMesh::TopoUtilities/FillHole"
         self._model._print_logs_before_command("fill_hole", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("fill_hole", TopoFillHoleResult(model = self._model, json_data = result))
         return TopoFillHoleResult(model = self._model, json_data = result)
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/topoutilitystructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/topoutilitystructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/transformstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/transformstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/volumecontrolstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumecontrolstructs.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,70 +11,81 @@
 class VolumeControlParams(CoreObject):
     """Volume control parameters are used to define the volume type in the volume control.
     """
     _default_params = {}
 
     def __initialize(
             self,
-            cell_zonelet_type: CellZoneletType):
+            cell_zonelet_type: CellZoneletType,
+            skip_hexcore: bool):
         self._cell_zonelet_type = CellZoneletType(cell_zonelet_type)
+        self._skip_hexcore = skip_hexcore
 
     def __init__(
             self,
             model: CommunicationManager=None,
             cell_zonelet_type: CellZoneletType = None,
+            skip_hexcore: bool = None,
             json_data : dict = None,
              **kwargs):
         """Initializes the VolumeControlParams.
 
         Parameters
         ----------
         model: Model
             Model to create a VolumeControlParams object with default parameters.
         cell_zonelet_type: CellZoneletType, optional
             Cell zonelet type is used to define the type of the associated volume.
+        skip_hexcore: bool, optional
+            Check whether to skip hexahedral cells generation in the core for this volume or not. Applicable only for volumeFillType set to HexcoreTet or HexcorePoly in the AutoMeshParams structure.
         json_data: dict, optional
             JSON dictionary to create a VolumeControlParams object with provided parameters.
 
         Examples
         --------
         >>> volume_control_params = prime.VolumeControlParams(model = model)
         """
         if json_data:
             self.__initialize(
-                CellZoneletType(json_data["cellZoneletType"] if "cellZoneletType" in json_data else None))
+                CellZoneletType(json_data["cellZoneletType"] if "cellZoneletType" in json_data else None),
+                json_data["skipHexcore"] if "skipHexcore" in json_data else None)
         else:
-            all_field_specified = all(arg is not None for arg in [cell_zonelet_type])
+            all_field_specified = all(arg is not None for arg in [cell_zonelet_type, skip_hexcore])
             if all_field_specified:
                 self.__initialize(
-                    cell_zonelet_type)
+                    cell_zonelet_type,
+                    skip_hexcore)
             else:
                 if model is None:
                     raise ValueError("Invalid assignment. Either pass model or specify all properties")
                 else:
                     param_json = model._communicator.initialize_params(model, "VolumeControlParams")
                     json_data = param_json["VolumeControlParams"] if "VolumeControlParams" in param_json else {}
                     self.__initialize(
-                        cell_zonelet_type if cell_zonelet_type is not None else ( VolumeControlParams._default_params["cell_zonelet_type"] if "cell_zonelet_type" in VolumeControlParams._default_params else CellZoneletType(json_data["cellZoneletType"] if "cellZoneletType" in json_data else None)))
+                        cell_zonelet_type if cell_zonelet_type is not None else ( VolumeControlParams._default_params["cell_zonelet_type"] if "cell_zonelet_type" in VolumeControlParams._default_params else CellZoneletType(json_data["cellZoneletType"] if "cellZoneletType" in json_data else None)),
+                        skip_hexcore if skip_hexcore is not None else ( VolumeControlParams._default_params["skip_hexcore"] if "skip_hexcore" in VolumeControlParams._default_params else (json_data["skipHexcore"] if "skipHexcore" in json_data else None)))
         self._custom_params = kwargs
         if model is not None:
             [ model._logger.warning(f'Unsupported argument : {key}') for key in kwargs ]
         [setattr(type(self), key, property(lambda self, key = key:  self._custom_params[key] if key in self._custom_params else None,
         lambda self, value, key = key : self._custom_params.update({ key: value }))) for key in kwargs]
         self._freeze()
 
     @staticmethod
     def set_default(
-            cell_zonelet_type: CellZoneletType = None):
+            cell_zonelet_type: CellZoneletType = None,
+            skip_hexcore: bool = None):
         """Set the default values of VolumeControlParams.
 
         Parameters
         ----------
         cell_zonelet_type: CellZoneletType, optional
             Cell zonelet type is used to define the type of the associated volume.
+        skip_hexcore: bool, optional
+            Check whether to skip hexahedral cells generation in the core for this volume or not. Applicable only for volumeFillType set to HexcoreTet or HexcorePoly in the AutoMeshParams structure.
         """
         args = locals()
         [VolumeControlParams._default_params.update({ key: value }) for key, value in args.items() if value is not None]
 
     @staticmethod
     def print_default():
         """Print the default values of VolumeControlParams.
@@ -87,24 +98,36 @@
         message += ''.join(str(key) + ' : ' + str(value) + '\n' for key, value in VolumeControlParams._default_params.items())
         print(message)
 
     def _jsonify(self) -> Dict[str, Any]:
         json_data = {}
         if self._cell_zonelet_type is not None:
             json_data["cellZoneletType"] = self._cell_zonelet_type
+        if self._skip_hexcore is not None:
+            json_data["skipHexcore"] = self._skip_hexcore
         [ json_data.update({ utils.to_camel_case(key) : value }) for key, value in self._custom_params.items()]
         return json_data
 
     def __str__(self) -> str:
-        message = "cell_zonelet_type :  %s" % (self._cell_zonelet_type)
+        message = "cell_zonelet_type :  %s\nskip_hexcore :  %s" % (self._cell_zonelet_type, self._skip_hexcore)
         message += ''.join('\n' + str(key) + ' : ' + str(value) for key, value in self._custom_params.items())
         return message
 
     @property
     def cell_zonelet_type(self) -> CellZoneletType:
         """Cell zonelet type is used to define the type of the associated volume.
         """
         return self._cell_zonelet_type
 
     @cell_zonelet_type.setter
     def cell_zonelet_type(self, value: CellZoneletType):
         self._cell_zonelet_type = value
+
+    @property
+    def skip_hexcore(self) -> bool:
+        """Check whether to skip hexahedral cells generation in the core for this volume or not. Applicable only for volumeFillType set to HexcoreTet or HexcorePoly in the AutoMeshParams structure.
+        """
+        return self._skip_hexcore
+
+    @skip_hexcore.setter
+    def skip_hexcore(self, value: bool):
+        self._skip_hexcore = value
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/volumesearch.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumesearch.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,13 +48,15 @@
 
         Examples
         --------
         >>> vol_search = VolumeSearch(model=model)
         >>> results = vol_search.get_volume_quality_summary(VolumeQualitySummaryParams(model=model))
 
         """
+        if not isinstance(params, VolumeQualitySummaryParams):
+            raise TypeError("Invalid argument type passed for params, valid argument type is VolumeQualitySummaryParams.")
         args = {"params" : params._jsonify()}
         command_name = "PrimeMesh::VolumeSearch/GetVolumeQualitySummary"
         self._model._print_logs_before_command("get_volume_quality_summary", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("get_volume_quality_summary", VolumeQualitySummaryResults(model = self._model, json_data = result))
         return VolumeQualitySummaryResults(model = self._model, json_data = result)
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/volumesearchstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/volumesearchstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/wrappercontrol.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/wrappercontrol.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,16 @@
             ScopeDefinition to scope entities for wrapping.
 
         Examples
         --------
         >>> wrapper_control.set_geometry_scope(scope)
 
         """
+        if not isinstance(scope, ScopeDefinition):
+            raise TypeError("Invalid argument type passed for scope, valid argument type is ScopeDefinition.")
         args = {"scope" : scope._jsonify()}
         command_name = "PrimeMesh::WrapperControl/SetGeometryScope"
         self._model._print_logs_before_command("set_geometry_scope", args)
         self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("set_geometry_scope")
 
     def set_leak_preventions(self, params : List[LeakPreventionParams]) -> SetLeakPreventionsResults:
@@ -54,14 +56,16 @@
             Return the set leak prevention results.
 
         Examples
         --------
         >>> set_leak_prev_results = wrapper_control.set_leak_preventions([params])
 
         """
+        if not isinstance(params, List):
+            raise TypeError("Invalid argument type passed for params, valid argument type is List[LeakPreventionParams].")
         args = {"params" : [p._jsonify() for p in params]}
         command_name = "PrimeMesh::WrapperControl/SetLeakPreventions"
         self._model._print_logs_before_command("set_leak_preventions", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("set_leak_preventions", SetLeakPreventionsResults(model = self._model, json_data = result))
         return SetLeakPreventionsResults(model = self._model, json_data = result)
 
@@ -80,14 +84,16 @@
             Return the set contact prevention results.
 
         Examples
         --------
         >>> set_cont_prev_results = wrapper_control.set_contact_preventions([params])
 
         """
+        if not isinstance(params, List):
+            raise TypeError("Invalid argument type passed for params, valid argument type is List[ContactPreventionParams].")
         args = {"params" : [p._jsonify() for p in params]}
         command_name = "PrimeMesh::WrapperControl/SetContactPreventions"
         self._model._print_logs_before_command("set_contact_preventions", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("set_contact_preventions", SetContactPreventionsResults(model = self._model, json_data = result))
         return SetContactPreventionsResults(model = self._model, json_data = result)
 
@@ -101,14 +107,16 @@
             List of live material points.
 
         Examples
         --------
         >>> wrapper_control.set_live_material_points(["Fluid1"])
 
         """
+        if not isinstance(material_point_names, List):
+            raise TypeError("Invalid argument type passed for material_point_names, valid argument type is List[str].")
         args = {"material_point_names" : material_point_names}
         command_name = "PrimeMesh::WrapperControl/SetLiveMaterialPoints"
         self._model._print_logs_before_command("set_live_material_points", args)
         self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("set_live_material_points")
 
     def set_feature_recoveries(self, params : List[FeatureRecoveryParams]) -> SetFeatureRecoveriesResults:
@@ -126,14 +134,16 @@
             Return the set feature recoveries results.
 
         Examples
         --------
         >>> set_feat_rec_results = wrapper_control.set_feature_recoveries([params])
 
         """
+        if not isinstance(params, List):
+            raise TypeError("Invalid argument type passed for params, valid argument type is List[FeatureRecoveryParams].")
         args = {"params" : [p._jsonify() for p in params]}
         command_name = "PrimeMesh::WrapperControl/SetFeatureRecoveries"
         self._model._print_logs_before_command("set_feature_recoveries", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("set_feature_recoveries", SetFeatureRecoveriesResults(model = self._model, json_data = result))
         return SetFeatureRecoveriesResults(model = self._model, json_data = result)
 
@@ -147,14 +157,16 @@
             Suggested name of the wrapper part to be created.
 
         Examples
         --------
         >>> wrapper_control.set_suggested_wrapper_part_name("wrap")
 
         """
+        if not isinstance(name, str):
+            raise TypeError("Invalid argument type passed for name, valid argument type is str.")
         args = {"name" : name}
         command_name = "PrimeMesh::WrapperControl/SetSuggestedWrapperPartName"
         self._model._print_logs_before_command("set_suggested_wrapper_part_name", args)
         self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("set_suggested_wrapper_part_name")
 
     def set_suggested_name(self, name : str) -> SetNameResults:
@@ -173,14 +185,16 @@
 
 
         Examples
         --------
         >>> wrapper_control.set_suggested_name("wrapper_control1")
 
         """
+        if not isinstance(name, str):
+            raise TypeError("Invalid argument type passed for name, valid argument type is str.")
         args = {"name" : name}
         command_name = "PrimeMesh::WrapperControl/SetSuggestedName"
         self._model._print_logs_before_command("set_suggested_name", args)
         result = self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("set_suggested_name", SetNameResults(model = self._model, json_data = result))
         return SetNameResults(model = self._model, json_data = result)
 
@@ -238,14 +252,16 @@
             ScopeDefinition to scope shadow entities for wrapping.
 
         Examples
         --------
         >>> wrapper_control.set_shadow_geometry_scope(scope)
 
         """
+        if not isinstance(scope, ScopeDefinition):
+            raise TypeError("Invalid argument type passed for scope, valid argument type is ScopeDefinition.")
         args = {"scope" : scope._jsonify()}
         command_name = "PrimeMesh::WrapperControl/SetShadowGeometryScope"
         self._model._print_logs_before_command("set_shadow_geometry_scope", args)
         self._comm.serve(self._model, command_name, self._object_id, args=args)
         self._model._print_logs_after_command("set_shadow_geometry_scope")
 
     @property
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/autogen/wrapperstructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/autogen/wrapperstructs.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/controldata.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/controldata.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # isort: split
 from ansys.meshing.prime.autogen.controldata import ControlData as _ControlData
 
 # isort: split
 from ansys.meshing.prime.autogen.commonstructs import DeleteResults
 from ansys.meshing.prime.autogen.primeconfig import ErrorCode
 from ansys.meshing.prime.autogen.prismcontrol import PrismControl
+from ansys.meshing.prime.autogen.thinvolumecontrol import ThinVolumeControl
 from ansys.meshing.prime.core.periodiccontrol import PeriodicControl
 from ansys.meshing.prime.core.sizecontrol import SizeControl
 from ansys.meshing.prime.core.volumecontrol import VolumeControl
 from ansys.meshing.prime.core.wrappercontrol import WrapperControl
 from ansys.meshing.prime.internals.comm_manager import CommunicationManager
 from ansys.meshing.prime.params.primestructs import SizingType
 
@@ -23,14 +24,15 @@
 
     def __init__(self, model: CommunicationManager, id: int, object_id: int, name: str):
         """Initializes ControlData"""
         self._model = model
         self._wrapper_controls = []
         self._size_controls = []
         self._prism_controls = []
+        self._thin_volume_controls = []
         self._volume_controls = []
         self._periodic_controls = []
         _ControlData.__init__(self, model, id, object_id, name)
 
     def get_wrapper_control_by_name(self, name) -> WrapperControl:
         """Gets the wrapper control by name.
 
@@ -43,15 +45,15 @@
         Returns
         -------
         WrapperControl
             Returns the wrapper control.
 
         Examples
         --------
-        >>> wrapper_control = model.control_data.get_wrapper_control_by_name("wrappercontol-1")
+        >>> wrapper_control = model.control_data.get_wrapper_control_by_name("wrappercontrol-1")
 
         """
         for wc in self._wrapper_controls:
             if wc.name == name:
                 return wc
         return None
 
@@ -99,14 +101,34 @@
 
         """
         res = _ControlData.create_prism_control(self)
         new_prism_control = PrismControl(self._model, res[0], res[1], res[2])
         self._prism_controls.append(new_prism_control)
         return new_prism_control
 
+    def create_thin_volume_control(self) -> ThinVolumeControl:
+        """Creates a ThinVolumeControl.
+
+
+        Returns
+        -------
+        ThinVolumeControl
+            Returns ThinVolumeControl.
+
+
+        Examples
+        --------
+        >>> thin_volume_control = model.control_data.create_thin_volume_control()
+
+        """
+        res = _ControlData.create_thin_volume_control(self)
+        new_thin_volume_control = ThinVolumeControl(self._model, res[0], res[1], res[2])
+        self._thin_volume_controls.append(new_thin_volume_control)
+        return new_thin_volume_control
+
     def create_wrapper_control(self) -> WrapperControl:
         """Creates wrapper control with defaults.
 
 
         Returns
         -------
         WrapperControl
@@ -170,14 +192,39 @@
 
         """
         for prism_control in self._prism_controls:
             if prism_control.name == name:
                 return prism_control
         return None
 
+    def get_thin_volume_control_by_name(self, name: str) -> ThinVolumeControl:
+        """Gets the thin volume control with the given name.
+
+
+        Parameters
+        ----------
+        name : str
+            Name of the thin volume control.
+
+        Returns
+        -------
+        ThinVolumeControl
+            Returns the thin volume control.
+
+        Examples
+        --------
+        >>> contorl_data = model.control_data
+        >>> thin_volume_control = control_data.get_thin_volume_control_by_name(
+                                                     "ThinVolumeControl-1")
+        """
+        for thin_volume_control in self._thin_volume_controls:
+            if thin_volume_control.name == name:
+                return thin_volume_control
+        return None
+
     def delete_controls(self, control_ids: Iterable[int]) -> DeleteResults:
         """Deletes the control for the given id.
 
 
         Parameters
         ----------
         control_ids : Iterable[int]
@@ -204,41 +251,46 @@
                     if wrapper_control.id == id:
                         self._wrapper_controls.remove(wrapper_control)
                         break
                 for prism_control in self._prism_controls:
                     if prism_control.id == id:
                         self._prism_controls.remove(prism_control)
                         break
+                for thin_volume_control in self._thin_volume_controls:
+                    if thin_volume_control.id == id:
+                        self._thin_volume_controls.remove(thin_volume_control)
+                        break
                 for volume_control in self._volume_controls:
                     if volume_control.id == id:
                         self._volume_controls.remove(volume_control)
                         break
                 for periodic_control in self._periodic_controls:
                     if periodic_control.id == id:
                         self._periodic_controls.remove(periodic_control)
                         break
         return res
 
-    def _update_size_controls(self, sc_data: List):
-        self._size_controls = [SizeControl(self._model, sc[0], sc[1], sc[2]) for sc in sc_data]
+    def _update_size_controls(self, c_data: List):
+        self._size_controls = [SizeControl(self._model, c[0], c[1], c[2]) for c in c_data]
 
-    def _update_prism_controls(self, sc_data: List):
-        self._prism_controls = [PrismControl(self._model, sc[0], sc[1], sc[2]) for sc in sc_data]
+    def _update_prism_controls(self, c_data: List):
+        self._prism_controls = [PrismControl(self._model, c[0], c[1], c[2]) for c in c_data]
 
-    def _update_wrapper_controls(self, sc_data: List):
-        self._wrapper_controls = [
-            WrapperControl(self._model, sc[0], sc[1], sc[2]) for sc in sc_data
-        ]
+    def _update_wrapper_controls(self, c_data: List):
+        self._wrapper_controls = [WrapperControl(self._model, c[0], c[1], c[2]) for c in c_data]
 
-    def _update_volume_controls(self, sc_data: List):
-        self._volume_controls = [VolumeControl(self._model, sc[0], sc[1], sc[2]) for sc in sc_data]
+    def _update_volume_controls(self, c_data: List):
+        self._volume_controls = [VolumeControl(self._model, c[0], c[1], c[2]) for c in c_data]
 
-    def _update_periodic_controls(self, sc_data: List):
-        self._periodic_controls = [
-            PeriodicControl(self._model, sc[0], sc[1], sc[2]) for sc in sc_data
+    def _update_periodic_controls(self, c_data: List):
+        self._periodic_controls = [PeriodicControl(self._model, c[0], c[1], c[2]) for c in c_data]
+
+    def _update_thin_volume_controls(self, c_data: List):
+        self._thin_volume_controls = [
+            ThinVolumeControl(self._model, c[0], c[1], c[2]) for c in c_data
         ]
 
     def create_volume_control(self) -> VolumeControl:
         """Creates the volume control.
 
         Returns
         -------
@@ -322,14 +374,30 @@
         --------
         >>> prism_control = model.control_data.prism_controls
 
         """
         return self._prism_controls
 
     @property
+    def thin_volume_controls(self) -> List[ThinVolumeControl]:
+        """Get the thin volume controls.
+
+        Returns
+        -------
+        List[ThinVolumeControl]
+            Returns the list of thin volume controls.
+
+        Examples
+        --------
+        >>> thin_volume_control = model.control_data.thin_volume_controls
+
+        """
+        return self._thin_volume_controls
+
+    @property
     def wrapper_controls(self) -> List[WrapperControl]:
         """Get the wrapper controls.
 
         Returns
         -------
         List[WrapperControl]
             Returns the list of wrapper controls.
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/fileio.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/fileio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Module containing file input and output related classes and methods."""
 from typing import List
 
 # isort: split
 from ansys.meshing.prime.autogen.fileio import FileIO as _FileIO
 
 # isort: split
 import ansys.meshing.prime.internals.utils as utils
@@ -28,37 +29,45 @@
     WriteSizeFieldParams,
 )
 from ansys.meshing.prime.core.model import Model
 from ansys.meshing.prime.params.primestructs import ErrorCode
 
 
 class FileIO(_FileIO):
+    """Input and output managing class.
+
+    Parameters
+    ----------
+    model : Model
+        Server model where to create and modify WrapperControls from.
+    """
+
     __doc__ = _FileIO.__doc__
 
     def __init__(self, model: Model):
-        """__init__(FileIO self, Model model)"""
+        """Initialize model and parent class."""
         self._model = model
         _FileIO.__init__(self, model)
 
     def read_pmdat(self, file_name: str, file_read_params: FileReadParams) -> FileReadResults:
-        """Function that reads PyPrimeMesh data file.
+        """Read PyPrimeMesh data file.
 
         PyPrimeMesh data files have pmdat extension.
 
         Parameters
         ----------
         file_name : str
             Path to file on disk.
         file_read_params : FileReadParams
             Parameter to read a file.
 
         Returns
         -------
         FileReadResults
-            Returns FileReadResults.
+            Return FileReadResults.
 
         Notes
         -----
         This API does not support Unicode paths now.
 
         Examples
         --------
@@ -74,28 +83,27 @@
         with utils.file_read_context(self._model, file_name) as temp_file_name:
             result = _FileIO.read_pmdat(self, temp_file_name, file_read_params)
             if result.error_code == ErrorCode.NOERROR:
                 self._model._sync_up_model()
         return result
 
     def write_pmdat(self, file_name: str, file_write_params: FileWriteParams) -> FileWriteResults:
-        """Writes PyPrimeMesh data file. PyPrimeMesh data files have .pmdat extension.
-
+        """Write PyPrimeMesh data file. PyPrimeMesh data files have .pmdat extension.
 
         Parameters
         ----------
         file_name : str
             Path to write file on disk.
         file_write_params : FileWriteParams
             Parameters to write PyPrimeMesh data file.
 
         Returns
         -------
         FileWriteResults
-            Returns the FileWriteResults structure.
+            Return the FileWriteResults structure.
 
         Examples
         --------
         >>> results = file_io.write_pmdat("/tmp/prime_mesh_data.pmdat",
                                           prime.FileWriteParams(model=model))
         """
         with utils.file_write_context(self._model, file_name) as temp_file_name:
@@ -189,15 +197,15 @@
         >>> results = file_io.write_size_field("/tmp/my_prime_sizefield.psf", params)
         """
         with utils.file_write_context(self._model, file_name) as temp_file_name:
             result = super().write_size_field(temp_file_name, params)
         return result
 
     def import_cad(self, file_name: str, params: ImportCadParams) -> ImportCadResults:
-        """Function that imports CAD file.
+        r"""Open CAD file.
 
         Import CAD file from disk.
 
         Supported formats on Windows are:
 
         \*.scdoc \*.fmd \*.agdb \*.pmdb \*.meshdat \*.mechdat \*.dsdb \*.cmdb \*.sat \*.sab
         \*.dwg \*.dxf \*.model \*.exp \*.CATPart \*.CATProduct \*.cgr \*.3dxml \*.prt\* \*.asm\*
@@ -219,15 +227,15 @@
 
         params : ImportCadParams
              Parameters to control CAD import options
 
         Returns
         -------
         ImportCadResults
-             Returns ImportCadResults.
+             Return ImportCadResults.
 
         Examples
         --------
         >>> import ansys.meshing.prime as prime
         >>> #connect client to server and get model from it
         >>> client = prime.Client(ip="localhost", port=50060)
         >>> model = client.model
@@ -244,29 +252,29 @@
         return import_result
 
     def import_fluent_meshing_meshes(
         self,
         file_names: List[str],
         import_fluent_meshing_mesh_params: ImportFluentMeshingMeshParams,
     ) -> ImportFluentMeshingMeshResults:
-        """Imports Fluent Meshing meshes of given files on disk.
+        """Import Fluent Meshing meshes of given files on disk.
 
         Fluent Meshing mesh files have msh and msh.gz extension.
 
         Parameters
         ----------
         file_names : List[str]
             Full path of files to be imported.
         import_fluent_meshing_mesh_params : ImportFluentMeshingMeshParams
             Parameters to import Fluent Meshing mesh.
 
         Returns
         -------
         ImportFluentMeshingMeshResults
-            Returns the FileReadResults.
+            Return the FileReadResults.
 
 
         Notes
         -----
         This API does not support Unicode paths now.
 
         Examples
@@ -285,29 +293,29 @@
         if result.error_code == ErrorCode.NOERROR:
             self._model._sync_up_model()
         return result
 
     def import_fluent_case(
         self, file_name: str, import_fluent_case_params: ImportFluentCaseParams
     ) -> ImportFluentCaseResults:
-        """Imports Fluent case file on disk.
+        """Import Fluent case file on disk.
 
         Fluent case files have cas extension.
 
         Parameters
         ----------
         file_name : str
             Path to file on disk.
         import_fluent_case_params : ImportFluentCaseParams
             Parameters to import fluent case file.
 
         Returns
         -------
         ImportFluentCaseResults
-            Returns the ImportFluentCaseResults.
+            Return the ImportFluentCaseResults.
 
 
         Notes
         -----
         This API does not support Unicode paths now.
 
         Examples
@@ -322,27 +330,27 @@
             if result.error_code == ErrorCode.NOERROR:
                 self._model._sync_up_model()
         return result
 
     def export_fluent_case(
         self, file_name: str, export_fluent_case_params: ExportFluentCaseParams
     ) -> FileWriteResults:
-        """Exports Fluent case file. Fluent case files have cas extension.
+        """Export Fluent case file. Fluent case files have cas extension.
 
         Parameters
         ----------
         file_name : str
             Path to file on disk.
         export_fluent_case_params : ExportFluentCaseParams
             Parameters to export fluent case file.
 
         Returns
         -------
         FileWriteResults
-            Returns the FileWriteResults structure.
+            Return the FileWriteResults structure.
 
         Examples
         --------
         >>> file_io = FileIO(model=model)
         >>> results = file_io.export_fluent_case(
                         "/tmp/fluent.cas",
                         prime.ExportFluentCaseParams(model=model))
@@ -350,27 +358,27 @@
         with utils.file_write_context(self._model, file_name) as temp_file_name:
             result = super().export_fluent_case(temp_file_name, export_fluent_case_params)
         return result
 
     def import_mapdl_cdb(
         self, file_name: str, params: ImportMapdlCdbParams
     ) -> ImportMapdlCdbResults:
-        """Function that imports MAPDL CDB file(cdb).
+        """Open MAPDL CDB file(cdb).
 
         Parameters
         ----------
         file_name : str
             Path to file on disk.
         params : ImportMapdlCdbParams
             Parameter to import a CDB file.
 
         Returns
         -------
         ImportMapdlCdbResults
-            Returns ImportMapdlCdbResults.
+            Return ImportMapdlCdbResults.
 
         Notes
         -----
         This API does not support Unicode paths now.
 
         Examples
         --------
@@ -387,27 +395,27 @@
             if result.error_code == ErrorCode.NOERROR:
                 self._model._sync_up_model()
         return result
 
     def export_mapdl_cdb(
         self, file_name: str, params: ExportMapdlCdbParams
     ) -> ExportMapdlCdbResults:
-        """Function that exports MAPDL CDB file(cdb).
+        """Export MAPDL CDB file(cdb).
 
         Parameters
         ----------
         file_name : str
             Path to file on disk.
         params : ExportMapdlCdbParams
             Parameter to export a CDB file.
 
         Returns
         -------
         ExportMapdlCdbResults
-            Returns ExportMapdlCdbResults.
+            Return ExportMapdlCdbResults.
 
         Notes
         -----
         This API does not support Unicode paths now.
 
         Examples
         --------
@@ -422,27 +430,27 @@
         with utils.file_write_context(self._model, file_name) as temp_file_name:
             result = super().export_mapdl_cdb(temp_file_name, params)
         return result
 
     def export_fluent_case(
         self, file_name: str, export_fluent_case_params: ExportFluentCaseParams
     ) -> FileWriteResults:
-        """Exports Fluent case file. Fluent case files have cas extension.
+        """Export Fluent case file. Fluent case files have cas extension.
 
         Parameters
         ----------
         file_name : str
             Path to file on disk.
         export_fluent_case_params : ExportFluentCaseParams
             Parameters to export fluent case file.
 
         Returns
         -------
         FileWriteResults
-            Returns the FileWriteResults structure.
+            Return the FileWriteResults structure.
 
         Examples
         --------
         >>> file_io = FileIO(model=model)
         >>> results = file_io.export_fluent_case("/tmp/fluent.cas",
                                                  prime.ExportFluentCaseParams(model=model))
         """
@@ -461,15 +469,15 @@
             Path to file on disk.
         export_fluent_mesh_params : ExportFluentMeshingMeshParams
             Parameters to export Fluent Meshing mesh file.
 
         Returns
         -------
         FileWriteResults
-            Returns the FileWriteResults structure.
+            Return the FileWriteResults structure.
 
         Examples
         --------
         >>> results = file_io.export_fluent_meshing_mesh(
                         "/tmp/fluent_meshing.msh",
                         ExportFluentMeshingMeshParams(model=model))
         """
@@ -488,15 +496,15 @@
             Name of the file.
         export_params : ExportBoundaryFittedSplineParams
             Parameters for IGA LS-DYNA Keyword file export.
 
         Returns
         -------
         FileWriteResults
-            Returns FileWriteResults.
+            Return FileWriteResults.
 
         Examples
         --------
         >>> results = file_io.export_boundary_fitted_spline_k_file(
                         file_name,
                         ExportBoundaryFittedSplineParams(model=model))
         """
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/model.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Module containing managing logic of the Prime Model."""
 from typing import Iterable, List
 
 # isort: split
 from ansys.meshing.prime.autogen.model import Model as _Model
 
 # isort: split
 import ansys.meshing.prime.internals.json_utils as json
@@ -17,29 +18,47 @@
 from ansys.meshing.prime.core.controldata import ControlData
 from ansys.meshing.prime.core.part import Part
 from ansys.meshing.prime.internals.communicator import Communicator
 from ansys.meshing.prime.internals.error_handling import PrimeRuntimeError
 
 
 class Model(_Model):
+    """Model is the nucleus of Prime.
+
+    Model forms the base and contains all the information about Prime.
+    You can access any information in Prime only through Model.
+    Model allows you to query TopoData, ControlData, Parts, SizeFields and more.
+
+    Parameters
+    ----------
+    comm : Communicator
+        Communicator to connect with the server.
+    id : int
+        ID of the model.
+    object_id : int
+        Object ID of the model.
+    name : str
+        Name of the model.
+    """
+
     __doc__ = _Model.__doc__
 
     def __init__(self, comm: Communicator, id: int, object_id: int, name: str):
-        """Initialize Model"""
+        """Initialize the model and the parameters."""
         _Model.__init__(self, comm, id, object_id, name)
         self._parts = []
         self._global_sf_params = GlobalSizingParams(model=self)
         self._default_part = None
         self._topo_data = None
         self._control_data = None
         self._material_point_data = None
         self._freeze()
 
     def _sync_up_model(self):
-        """Synchronizes client model with the server model.
+        """Synchronize client model with the server model.
 
         Updates proxy child objects of the client model with the child objects of the server model.
 
         Examples
         --------
         >>> from ansys.meshing.prime import Model
         >>> model = client.model
@@ -68,30 +87,41 @@
         self._control_data._update_volume_controls(vc_data)
         self._topo_data = TopoData(self, -1, res["TopoData"], "")
         if "PeriodicControl" in res:
             self._control_data._update_periodic_controls(percon_data)
         self._material_point_data = MaterialPointManager(self, -1, res["MaterialPointData"], "")
 
     def _add_part(self, id: int):
-        """Add a part that is present on server."""
+        """Add a part that is present on server.
+
+        Parameters
+        ----------
+        id : int
+            ID of the part
+
+        Raises
+        ------
+        PrimeRuntimeError
+            Raise if unable to create the part.
+        """
         res = json.loads(
             self._comm.serve(self, "PrimeMesh::Model/GetChildObjectsJson", self._object_id, args={})
         )
         part_data = res["Parts"]
         new_part = None
         for part in part_data:
             if part[0] == id:
                 new_part = Part(self, part[0], part[1], part[2])
                 self._parts.append(new_part)
                 break
         if new_part == None:
             raise PrimeRuntimeError("Unable to create part", ErrorCode.PARTNOTFOUND)
 
     def get_part_by_name(self, name: str) -> Part:
-        """Gets the part by name. Returns None if part doesn't exist for the given name.
+        """Get the part by name. Returns None if part doesn't exist for the given name.
 
         Parameters
         ----------
         name : str
             Name of the part.
 
         Returns
@@ -107,52 +137,51 @@
         """
         for part in self._parts:
             if part.name == name:
                 return part
         return None
 
     def get_part(self, id: int) -> Part:
-        """Gets the part by id. Returns None if part doesn't exist for the given id.
+        """Get the part by id. Returns None if part doesn't exist for the given id.
 
         Parameters
         ----------
         id : int
             Id of the part.
 
         Returns
         -------
         Part
-            Returns the part.
+            Return the part.
 
         Examples
         --------
             >>> from ansys.meshing.prime import Model
             >>> model = client.model
             >>> part = model.get_part(2)
         """
         for part in self._parts:
             if part.id == id:
                 return part
         return None
 
     def merge_parts(self, part_ids: Iterable[int], params: MergePartsParams) -> MergePartsResults:
-        """Merges given parts into one.
-
+        """Merge given parts into one.
 
         Parameters
         ----------
         part_ids : Iterable[int]
             Ids of parts to be merged.
         params : MergePartsParams
             Parameters to merge parts.
 
         Returns
         -------
         MergePartsResults
-            Returns the MergePartsResults.
+            Return the MergePartsResults.
 
 
         Examples
         --------
         >>> params = prime.MergePartsParams(model = model)
         >>> results = model.merge_parts(part_ids, params)
 
@@ -165,26 +194,25 @@
             for id in part_ids:
                 part = self.get_part(id)
                 if part.id != merged_part.id:
                     self._parts.remove(part)
         return res
 
     def delete_parts(self, part_ids: Iterable[int]) -> DeleteResults:
-        """Deletes the parts and its contents.
-
+        """Delete the parts and its contents.
 
         Parameters
         ----------
         part_ids : Iterable[int]
             Ids of parts to be deleted.
 
         Returns
         -------
         DeleteResults
-            Returns DeleteResults.
+            Return DeleteResults.
 
 
         Examples
         --------
         >>> results = model.delete_parts(part_ids)
 
         """
@@ -193,59 +221,57 @@
             for id in part_ids:
                 for part in list(self._parts):
                     if part.id == id:
                         self._parts.remove(part)
         return res
 
     def get_global_sizing_params(self) -> GlobalSizingParams:
-        """Gets the GlobalSizingParams.
+        """Get the GlobalSizingParams.
 
         Returns
         -------
         GlobalSizingParams
-            Returns the GlobalSizingParams.
+            Return the GlobalSizingParams.
 
         Examples
         --------
             >>> model = client.model
             >>> sf_params = model.get_global_sizing_params()
         """
         return self._global_sf_params
 
     def set_global_sizing_params(self, params: GlobalSizingParams):
-        """Sets the global sizing parameters.
+        """Set the global sizing parameters.
 
-        Sets the global sizing params to initialize surfer parameters and various size control
+        Set the global sizing params to initialize surfer parameters and various size control
         parameters.
 
         Parameters
         ----------
         params : GlobalSizingParams
              Global sizing parameters.
 
         Examples
         --------
-
         >>> model = client.model
         >>> model.set_global_sizing_params(GlobalSizingParams(model=model,
         ...                                          min=0.1,
         ...                                          max=1.0,
         ...                                          growth_rate=1.2))
-
         """
         _Model.set_global_sizing_params(self, params)
         self._global_sf_params = params
 
     def __str__(self):
-        """Prints the summary of the model.
+        """Print the summary of the model.
 
         Returns
         -------
         str
-            Returns the summary of the model.
+            Return the summary of the model.
 
         Examples
         --------
         >>> from ansys.meshing.prime import Model
         >>> model = client.model
         >>> print(model)
         """
@@ -253,20 +279,20 @@
         result += "Part Summary:\n"
         for part in self._parts:
             result += part.__str__() + "\n"
         return result
 
     @property
     def parts(self) -> List[Part]:
-        """Gets the list of parts of a model.
+        """Get the list of parts of a model.
 
         Returns
         -------
         List[Part]
-            Returns the list of parts.
+            Return the list of parts.
 
         Examples
         --------
             >>> from ansys.meshing.prime import Model
             >>> model = client.model
             >>> parts = model.parts
         """
@@ -285,20 +311,20 @@
         --------
             >>> topo_data=model.topo_data
         """
         return self._topo_data
 
     @property
     def control_data(self) -> ControlData:
-        """Gets the control data of a model.
+        """Get the control data of a model.
 
         Returns
         -------
         ControlData
-            Returns the control data.
+            Return the control data.
 
         Examples
         --------
             >>> control_data = model.control_data
         """
         return self._control_data
 
@@ -307,15 +333,15 @@
         """Get Material Point Data.
 
         MaterialPointManager is used to create, delete and manage material points.
 
         Returns
         -------
         MaterialPointManager
-            Returns the material point manager.
+            Return the material point manager.
 
         Examples
         --------
             >>> mpt_data = model.material_point_data
         """
         return self._material_point_data
 
@@ -325,15 +351,15 @@
 
         PyPrimeMesh's Logger instance can be used to control the verbosity
         of messages printed by PyPrimeMesh.
 
         Returns
         -------
         Logger
-             Returns logging.Logger instance.
+             Return logging.Logger instance.
 
         Examples
         --------
         Set log level to debug.
 
         >>> model.python_logger.setLevel(logging.DEBUG)
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/part.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/part.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,38 @@
+"""Module containing Part class."""
 from typing import Any
 
 # isort: split
 from ansys.meshing.prime.autogen.part import Part as _Part
 
 # isort: split
 from ansys.meshing.prime.autogen.commonstructs import SetNameResults as SetNameResults
 from ansys.meshing.prime.autogen.partstructs import PartSummaryParams
 
 
 class Part(_Part):
+    """
+    Defines and modifies the parts of a model.
+
+    Parameters
+    ----------
+    model: ansys.meshing.prime.Model
+        Model in which part is created
+    id: int
+        Id of the part provided by server
+    object_id: int
+        Object id provided by the server
+    name: str
+        Part name
+    """
+
     __doc__ = _Part.__doc__
 
     def __init__(self, model, id: int, object_id: int, name: str):
-        """Initialize Part
-
-        Parameters
-        ----------
-        model: ansys.meshing.prime.Model
-            Model in which part is created
-        id: int
-            Id of the part provided by server
-        object_id: int
-            Object id provided by the server
-        name: str
-            Part name
-        """
+        """Initialize Part."""
         self._model = model
         self._print_mesh = False
         self._print_id = False
         _Part.__init__(self, model, id, object_id, name)
 
     def __call__(self, *args: Any, **kwds: Any) -> str:
         """Callable interface of the Part.
@@ -65,22 +69,22 @@
                 params.print_mesh = value
             if key == 'print_id':
                 params.print_id = value
         result = _Part.get_summary(self, params)
         return result.message
 
     def __str__(self) -> str:
-        """Prints the summary of a part.
+        """Print the summary of a part.
 
         Uses print_mesh and print_id properties to control the the summary of a part.
 
         Returns
         -------
         str
-            Returns the summary of a part.
+            Return the summary of a part.
 
         Examples
         --------
         >>> from ansys.meshing.prime import Model
         >>> model = client.model
         >>> part = model.get_part_by_name("Part.1")
         >>> print(part)
@@ -88,26 +92,25 @@
         params = PartSummaryParams(model=self._model)
         params.print_mesh = self._print_mesh
         params.print_id = self._print_id
         result = _Part.get_summary(self, params)
         return result.message
 
     def set_suggested_name(self, name: str) -> SetNameResults:
-        """Sets the unique name for the part based on the given suggested name.
-
+        """Set the unique name for the part based on the given suggested name.
 
         Parameters
         ----------
         name : str
             Suggested name for the part.
 
         Returns
         -------
         SetNameResults
-            Returns the results with assigned name of the part.
+            Return the results with assigned name of the part.
 
 
         Examples
         --------
         >>> part.set_suggested_name("part1")
 
         """
@@ -118,19 +121,28 @@
     @property
     def print_mesh(self) -> bool:
         """When True, prints the mesh summary along with part summary. The default is False."""
         return self._print_mesh
 
     @print_mesh.setter
     def print_mesh(self, value: bool):
+        """Print the mesh of the part.
+
+        Parameters
+        ----------
+        value : bool
+            _description_
+        """
         self._print_mesh = value
 
     @property
     def print_id(self) -> bool:
-        """When True, prints the id's of topoentities or zonelets along with part summary.
+        """Print the id's of topoentities.
+
+        When True, prints the id's of topoentities or zonelets along with part summary.
         The default is False.
         """
         return self._print_id
 
     @print_id.setter
     def print_id(self, value: bool):
         self._print_id = value
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/periodiccontrol.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/periodiccontrol.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,78 @@
+"""Module containing PeriodicControl related classes and methods."""
+
 from ansys.meshing.prime.autogen.periodiccontrol import (
     PeriodicControl as _PeriodicControl,
 )
 
 # isort: split
 from ansys.meshing.prime.autogen.commonstructs import SetNameResults
 from ansys.meshing.prime.autogen.periodiccontrolstructs import PeriodicControlParams
 
 
 class PeriodicControl(_PeriodicControl):
-    """Periodic control is used to define the scope and transformation for periodic surfaces."""
+    """Periodic control is used to define the scope and transformation for periodic surfaces.
+
+    Parameters
+    ----------
+    model : CommunicationManager
+        Server model where to create and modify PeriodicControls from.
+    id : int
+        ID of the control.
+    object_id : int
+        Object ID of the control.
+    name : str
+        Name of the PeriodicControl
+    local : bool, optional
+        Unused, by default False
+    """
 
     def __init__(self, model, id, object_id, name, local=False):
-        """__init__(Model self, int id, int object_id, char* name)"""
+        """Initialize class variables and superclass."""
         _PeriodicControl.__init__(self, model, id, object_id, name)
         self._model = model
         self._name = name
 
     def __str__(self) -> str:
+        """Representation of the class in string format.
+
+        Returns
+        -------
+        str
+            Class data in string format.
+        """
         params = PeriodicControlParams(model=self._model)
         result = _PeriodicControl.get_summary(self, params)
         return result.message
 
     def set_suggested_name(self, name: str) -> SetNameResults:
-        """Sets the unique name for the periodic control based on the given suggested name.
-
+        """Set the unique name for the periodic control based on the given suggested name.
 
         Parameters
         ----------
         name : str
             Suggested name for the periodic control.
 
         Returns
         -------
         SetNameResults
             Returns a name of the periodic control.
 
-
         Examples
         --------
         >>> periodic_control.set_suggested_name("control1")
 
         """
         result = _PeriodicControl.set_suggested_name(self, name)
         self._name = result.assigned_name
         return result
 
     @property
     def name(self):
-        """Gets the name of the periodic control.
+        """Get the name of the periodic control.
 
         Returns
         -------
         str
             Returns the name of the periodic control.
 
         Examples
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/sizecontrol.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/sizecontrol.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,52 @@
+"""Module containing SizeControl related classes and methods."""
 from ansys.meshing.prime.autogen.sizecontrol import SizeControl as _SizeControl
 
 # isort: split
 from ansys.meshing.prime.autogen.commonstructs import SetNameResults
 from ansys.meshing.prime.autogen.sizecontrolstructs import SizeControlSummaryParams
 
 
 class SizeControl(_SizeControl):
-    """Size control is used to compute size field for volumetric surface meshing."""
+    """Compute size field for volumetric surface meshing.
+
+    Parameters
+    ----------
+    model : CommunicationManager
+        Server model where to create and modify SizeControls from.
+    id : int
+        ID of the control.
+    object_id : int
+        Object ID of the control.
+    name : str
+        Name of the SizeControl
+    local : bool, optional
+        Unused, by default False
+    """
 
     def __init__(self, model, id, object_id, name, local=False):
-        """__init__(Model self, int id, int object_id, char* name)"""
+        """Initialize class variables and superclass."""
         _SizeControl.__init__(self, model, id, object_id, name)
         self._model = model
         self._name = name
 
     def __str__(self) -> str:
+        """Representation of the class in string format.
+
+        Returns
+        -------
+        str
+            Class data in string format.
+        """
         params = SizeControlSummaryParams(model=self._model)
         result = _SizeControl.get_summary(self, params)
         return result.message
 
     def set_suggested_name(self, name: str) -> SetNameResults:
-        """Sets the unique name for the size control based on the given suggested name.
-
+        """Set the unique name for the size control based on the given suggested name.
 
         Parameters
         ----------
         name : str
             Suggested name for the size control.
 
         Returns
@@ -41,15 +62,15 @@
         """
         result = _SizeControl.set_suggested_name(self, name)
         self._name = result.assigned_name
         return result
 
     @property
     def name(self):
-        """Gets the name of size control.
+        """Get the name of size control.
 
         Returns
         -------
         str
             Returns a name of the size control.
 
         Examples
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/surfaceutilities.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/surfaceutilities.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,55 @@
+"""Utilities module for surface operations."""
 from ansys.meshing.prime.autogen.surfaceutilities import (
     SurfaceUtilities as _SurfaceUtilities,
 )
 
 # isort: split
+from typing import Iterable
+
 from ansys.meshing.prime.autogen.surfaceutilitystructs import (
-    AddThicknessParams as AddParams,
+    AddThicknessParams as AddThicknessParams,
 )
 from ansys.meshing.prime.autogen.surfaceutilitystructs import (
-    AddThicknessResults as AddResults,
+    AddThicknessResults as AddThicknessResults,
 )
 from ansys.meshing.prime.autogen.surfaceutilitystructs import (
     CreateBOIParams as CreateBOIParams,
 )
 from ansys.meshing.prime.autogen.surfaceutilitystructs import (
     CreateBOIResults as CreateBOIResults,
 )
 from ansys.meshing.prime.autogen.surfaceutilitystructs import (
-    CreateContactPatchParams as CPP,
+    CreateContactPatchParams as CreateContactPatchParams,
 )
 from ansys.meshing.prime.autogen.surfaceutilitystructs import (
-    CreateContactPatchResults as CPR,
+    CreateContactPatchResults as CreateContactPatchResults,
 )
 from ansys.meshing.prime.core.model import Model
 from ansys.meshing.prime.params.primestructs import ErrorCode as ErrorCode
-from ansys.meshing.prime.params.primestructs import Iterable as Iterable
-from ansys.meshing.prime.params.primestructs import ScopeDefinition as SD
 
 
 class SurfaceUtilities(_SurfaceUtilities):
-    """Performs various general surface utilities algorithms. For example, add thickness."""
+    """Performs various general surface utilities algorithms. For example, add thickness.
+
+    Parameters
+    ----------
+    model : Model
+        Server model in which to perform the operations.
+    """
 
     def __init__(self, model: Model):
-        """__init__(Model self, int id, int object_id, char* name)"""
+        """Initialize the superclass and Model variable."""
         _SurfaceUtilities.__init__(self, model)
         self._model = model
 
-    def add_thickness(self, zonelets: Iterable[int], params: AddParams) -> AddResults:
-        """Adds thickness to the selected list of face zonelet ids.
-
+    def add_thickness(
+        self, zonelets: Iterable[int], params: AddThicknessParams
+    ) -> AddThicknessResults:
+        """Thickens the selected list of face zonelet ids.
 
         Parameters
         ----------
         zonelets : Iterable[int]
             List of input face zonelet ids.
         params : AddThicknessParams
             Parameters to control the add thickness operation.
@@ -58,62 +66,71 @@
 
         """
         result = _SurfaceUtilities.add_thickness(self, zonelets, params)
         if result.error_code == ErrorCode.NOERROR:
             self._model._sync_up_model()
         return result
 
-    def create_boi(self, scope: SD, params: CreateBOIParams) -> CreateBOIResults:
+    def create_boi(
+        self, face_zonelet_ids: Iterable[int], params: CreateBOIParams
+    ) -> CreateBOIResults:
         """Creates BOI to the selected list of face zonelet ids.
 
 
         Parameters
         ----------
-        scope : ScopeDefinition
-            Scope of zonelets.
+        face_zonelet_ids : Iterable[int]
+            List of input face zonelet ids.
         params : CreateBOIParams
             Parameters to control the BOI creation operation.
 
         Returns
         -------
         CreateBOIResults
             Returns the BOIResults.
 
 
         Examples
         --------
-        >>> result = surf_utils.create_surface_boi(zonelets, params)
+        >>> result = surf_utils.create_boi(zonelets, params)
 
         """
-        result = _SurfaceUtilities.create_boi(self, scope, params)
+        result = _SurfaceUtilities.create_boi(self, face_zonelet_ids, params)
         if result.error_code == ErrorCode.NOERROR:
             self._model._sync_up_model()
         return result
 
-    def create_contact_patch(self, source_scope: SD, target_scope: SD, params: CPP) -> CPR:
-        """Creates contact patches.
+    def create_contact_patch(
+        self,
+        source_zonelets: Iterable[int],
+        target_zonelets: Iterable[int],
+        params: CreateContactPatchParams,
+    ) -> CreateContactPatchResults:
+        """Creates contact patch by offsetting the target zonelets.
 
 
         Parameters
         ----------
-        source_scope : ScopeDefinition
-            Scope of source zonelets.
-        target_scope : ScopeDefinition
-            Scope of target zonelets which is to be offsetted for contact patch creation.
+        source_zonelets : Iterable[int]
+            Source face zonelet ids.
+        target_zonelets : Iterable[int]
+            Target face zonelet ids.
         params : CreateContactPatchParams
             Parameters to control the contact patch creation operation.
 
         Returns
         -------
         CreateContactPatchResults
             Returns the CreateContactPatchResults.
 
 
         Examples
         --------
         >>> result = surf_utils.create_contact_patch(zonelets, params)
 
         """
-        result = _SurfaceUtilities.create_contact_patch(self, source_scope, target_scope, params)
+        result = _SurfaceUtilities.create_contact_patch(
+            self, source_zonelets, target_zonelets, params
+        )
         if result.error_code == ErrorCode.NOERROR:
             self._model._sync_up_model()
         return result
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/surfer.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/surfer.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/wrapper.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/core/wrappercontrol.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/core/wrappercontrol.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,47 @@
+"""Module containing WrapperControl related classes and methods."""
 from ansys.meshing.prime.autogen.wrappercontrol import WrapperControl as _WrapperControl
 
 # isort: split
 from ansys.meshing.prime.autogen.commonstructs import SetNameResults as SetNameResults
 from ansys.meshing.prime.internals.comm_manager import CommunicationManager
 
 
 class WrapperControl(_WrapperControl):
-    """Wrapper Control to describe all parameters and controls used for wrapping."""
+    """Wrapper Control to describe all parameters and controls used for wrapping.
+
+    Parameters
+    ----------
+    model : CommunicationManager
+        Server model where to create and modify WrapperControls from.
+    id : int
+        ID of the control.
+    object_id : int
+        Object ID of the control.
+    name : str
+        Name of the WrapperControl
+    """
 
     def __init__(self, model: CommunicationManager, id: int, object_id: int, name: str):
-        """Initialize Part"""
+        """Initialize the superclass and Model variable."""
         self._model = model
         _WrapperControl.__init__(self, model, id, object_id, name)
 
     def __str__(self) -> str:
+        """Representation of the class in string format.
+
+        Returns
+        -------
+        str
+            Class data in string format.
+        """
         return "Not implemented yet"
 
     def set_suggested_name(self, name: str) -> SetNameResults:
-        """Sets the unique name for the wrapper control based on the given suggested name.
-
+        """Set the unique name for the wrapper control based on the given suggested name.
 
         Parameters
         ----------
         name : str
             Suggested name for the wrapper control.
 
         Returns
@@ -38,15 +57,15 @@
         """
         result = _WrapperControl.set_suggested_name(self, name)
         self._name = result.assigned_name
         return result
 
     @property
     def name(self):
-        """Gets the name of wrapper control.
+        """Get the name of wrapper control.
 
         Returns
         -------
         str
             Returns a name of the wrapper control.
 
         Examples
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/examples/__init__.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/examples/examples.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,84 @@
 """Examples module for PyPrimeMesh
 """
 import os
+from enum import Enum
 from typing import Optional, Union
 
-from .download import download_file
+from .download_utilities import download_file
+
+__all__ = ['clear_download_cache', 'get_file', 'Examples']
+
+
+class Examples(Enum):
+    """Contains the available PyPrimeMesh examples to download."""
+
+    ELBOW_PMDAT = {"filename": "mixing_elbow.pmdat", "git_folder": "mixing_elbow"}
+    ELBOW_FMD = {"filename": "mixing_elbow.fmd", "git_folder": "mixing_elbow"}
+    ELBOW_SCDOC = {"filename": "mixing_elbow.scdoc", "git_folder": "mixing_elbow"}
+    BRACKET_FMD = {"filename": "bracket_mid_surface.fmd", "git_folder": "bracket_scaffold"}
+    BRACKET_SCDOC = {"filename": "bracket_mid_surface.scdoc", "git_folder": "bracket_scaffold"}
+    TOY_CAR_PMDAT = {"filename": "toy_car.pmdat", "git_folder": "toy_car"}
+    TOY_CAR_FMD = {"filename": "toy_car.fmd", "git_folder": "toy_car"}
+    TOY_CAR_SCDOC = {"filename": "toy_car.scdoc", "git_folder": "toy_car"}
+    PIPE_TEE_PMDAT = {"filename": "pipe_tee.pmdat", "git_folder": "pipe_tee"}
+    PIPE_TEE_FMD = {"filename": "pipe_tee.fmd", "git_folder": "pipe_tee"}
+    PIPE_TEE_SCDOC = {"filename": "pipe_tee.scdoc", "git_folder": "pipe_tee"}
 
-__all__ = [
-    'clear_download_cache',
-    'download_file',
-    'download_elbow_pmdat',
-    'download_elbow_fmd',
-    'download_elbow_scdoc',
-    'download_bracket_fmd',
-    'download_bracket_scdoc',
-    'download_toy_car_pmdat',
-    'download_toy_car_fmd',
-    'download_toy_car_scdoc',
-    'download_pipe_tee_pmdat',
-    'download_pipe_tee_fmd',
-]
 
 _DOWNLOADS = []
 
 
+def clear_download_cache():
+    """Clears the cache of downloaded files"""
+    [os.remove(_file) for _file in _DOWNLOADS]
+    _DOWNLOADS.clear()
+
+
+def get_file(
+    example: Examples,
+    destination: Optional[str] = None,
+    force: bool = False,
+) -> Union[str, os.PathLike]:
+    """Downloads example files from git.
+
+    Parameters
+    ----------
+    example: Examples
+        Known example to download from database
+    destination: Optional[str]
+        Destination for the file to be downloaded.
+        The default is ``None`` in which case the default path in app data is used.
+    force: bool
+        If true, the file is always downloaded.
+        Otherwise, an existing file in the cache may be re-used.
+
+    Returns
+    -------
+    str
+        Local path to the downloaded file
+
+    Raises
+    ------
+    ValueError
+        When the provided destination path does not exist on file
+    """
+    if destination is not None and not os.path.isdir(destination):
+        raise ValueError('destination directory provided does not exist')
+    file = download_file(
+        example.value["filename"],
+        'pyprimemesh',
+        example.value["git_folder"],
+        destination=destination,
+        force=force,
+    )
+    _DOWNLOADS.append(file)
+    return file
+
+
 def download_elbow_pmdat(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download PMDAT file for the mixing elbow example
 
     Parameters
     ----------
@@ -55,21 +107,15 @@
     >>>     model = session.model
     >>>     elbow = prime_examples.download_elbow_pmdat()
     >>>     with prime.FileIO(model) as io:
     >>>         _ = io.read_pmdat(elbow, params=prime.FileReadParams(model))
     >>>     print(model)
 
     """
-    if destination is not None and not os.path.isdir(destination):
-        raise ValueError('destination directory provided does not exist')
-    file = download_file(
-        'mixing_elbow.pmdat', 'pyprimemesh', 'mixing_elbow', destination=destination, force=force
-    )
-    _DOWNLOADS.append(file)
-    return file
+    return get_file(Examples.ELBOW_PMDAT, destination, force)
 
 
 def download_elbow_fmd(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download FMD file for the mixing elbow example
 
@@ -100,21 +146,16 @@
     >>>     model = session.model
     >>>     elbow = prime_examples.download_elbow_fmd()
     >>>     with prime.FileIO(model) as io:
     >>>         _ = io.import_cad(elbow, params=prime.ImportCADParams(model))
     >>>     print(model)
 
     """
-    if destination is not None and not os.path.isdir(destination):
-        raise ValueError('destination directory provided does not exist')
-    file = download_file(
-        'mixing_elbow.fmd', 'pyprimemesh', 'mixing_elbow', destination=destination, force=force
-    )
-    _DOWNLOADS.append(file)
-    return file
+
+    return get_file(Examples.ELBOW_FMD, destination, force)
 
 
 def download_elbow_scdoc(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download SCDOC file for the mixing elbow example
 
@@ -145,21 +186,15 @@
     >>>     model = session.model
     >>>     elbow = prime_examples.download_elbow_scdoc()
     >>>     with prime.FileIO(model) as io:
     >>>         _ = io.import_cad(elbow, params=prime.ImportCADParams(model))
     >>>     print(model)
 
     """
-    if destination is not None and not os.path.isdir(destination):
-        raise ValueError('destination directory provided does not exist')
-    file = download_file(
-        'mixing_elbow.scdoc', 'pyprimemesh', 'mixing_elbow', destination=destination, force=force
-    )
-    _DOWNLOADS.append(file)
-    return file
+    return get_file(Examples.ELBOW_SCDOC, destination, force)
 
 
 def download_bracket_fmd(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download FMD file for the bracket scaffold example
 
@@ -190,25 +225,15 @@
     >>>     model = session.model
     >>>     bracket = prime_examples.download_bracket_fmd()
     >>>     with prime.FileIO(model) as io:
     >>>         _ = io.import_cad(bracket, params=prime.ImportCADParams(model))
     >>>     print(model)
 
     """
-    if destination is not None and not os.path.isdir(destination):
-        raise ValueError('destination directory provided does not exist')
-    file = download_file(
-        'bracket_mid_surface.fmd',
-        'pyprimemesh',
-        'bracket_scaffold',
-        destination=destination,
-        force=force,
-    )
-    _DOWNLOADS.append(file)
-    return file
+    return get_file(Examples.BRACKET_FMD, destination, force)
 
 
 def download_bracket_scdoc(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download SCDOC file for the bracket scaffold example
 
@@ -239,25 +264,15 @@
     >>>     model = session.model
     >>>     bracket = prime_examples.download_bracket_scdoc()
     >>>     with prime.FileIO(model) as io:
     >>>         _ = io.import_cad(bracket, params=prime.ImportCADParams(model))
     >>>     print(model)
 
     """
-    if destination is not None and not os.path.isdir(destination):
-        raise ValueError('destination directory provided does not exist')
-    file = download_file(
-        'bracket_mid_surface.scdoc',
-        'pyprimemesh',
-        'bracket_scaffold',
-        destination=destination,
-        force=force,
-    )
-    _DOWNLOADS.append(file)
-    return file
+    return get_file(Examples.BRACKET_SCDOC, destination, force)
 
 
 def download_toy_car_pmdat(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download PMDAT file for the toy car example
 
@@ -288,21 +303,15 @@
     >>>     model = session.model
     >>>     toy_car = prime_examples.download_toy_car_pmdat()
     >>>     with prime.FileIO(model) as io:
     >>>         _ = io.read_pmdat(toy_car, params=prime.FileReadParams(model))
     >>>     print(model)
 
     """
-    if destination is not None and not os.path.isdir(destination):
-        raise ValueError('destination directory provided does not exist')
-    file = download_file(
-        'toy_car.pmdat', 'pyprimemesh', 'toy_car', destination=destination, force=force
-    )
-    _DOWNLOADS.append(file)
-    return file
+    return get_file(Examples.TOY_CAR_PMDAT, destination, force)
 
 
 def download_toy_car_fmd(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download FMD file for the toy car example
 
@@ -333,21 +342,15 @@
     >>>     model = session.model
     >>>     toy_car = prime_examples.download_toy_car_fmd()
     >>>     with prime.FileIO(model) as io:
     >>>         _ = io.import_cad(toy_car, params=prime.ImportCADParams(model))
     >>>     print(model)
 
     """
-    if destination is not None and not os.path.isdir(destination):
-        raise ValueError('destination directory provided does not exist')
-    file = download_file(
-        'toy_car.fmd', 'pyprimemesh', 'toy_car', destination=destination, force=force
-    )
-    _DOWNLOADS.append(file)
-    return file
+    return get_file(Examples.TOY_CAR_FMD, destination, force)
 
 
 def download_toy_car_scdoc(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download SCDOC file for the toy car example
 
@@ -378,21 +381,15 @@
     >>>     model = session.model
     >>>     toy_car = prime_examples.download_toy_car_scdoc()
     >>>     with prime.FileIO(model) as io:
     >>>         _ = io.import_cad(toy_car, params=prime.ImportCADParams(model))
     >>>     print(model)
 
     """
-    if destination is not None and not os.path.isdir(destination):
-        raise ValueError('destination directory provided does not exist')
-    file = download_file(
-        'toy_car.scdoc', 'pyprimemesh', 'toy_car', destination=destination, force=force
-    )
-    _DOWNLOADS.append(file)
-    return file
+    return get_file(Examples.TOY_CAR_SCDOC, destination, force)
 
 
 def download_pipe_tee_pmdat(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download PMDAT file for the pipe tee example
 
@@ -423,21 +420,15 @@
     >>>     model = session.model
     >>>     pipe_tee = prime_examples.download_pipe_tee_pmdat()
     >>>     with prime.FileIO(model) as io:
     >>>         _ = io.read_pmdat(pipe_tee, params=prime.FileReadParams(model))
     >>>     print(model)
 
     """
-    if destination is not None and not os.path.isdir(destination):
-        raise ValueError('destination directory provided does not exist')
-    file = download_file(
-        'pipe_tee.pmdat', 'pyprimemesh', 'pipe_tee', destination=destination, force=force
-    )
-    _DOWNLOADS.append(file)
-    return file
+    return get_file(Examples.PIPE_TEE_PMDAT, destination, force)
 
 
 def download_pipe_tee_fmd(
     destination: Optional[str] = None, force: bool = False
 ) -> Union[str, os.PathLike]:
     """Download FMD file for the pipe tee example
 
@@ -468,20 +459,47 @@
     >>>     model = session.model
     >>>     pipe_tee = prime_examples.download_pipe_tee_fmd()
     >>>     with prime.FileIO(model) as io:
     >>>         _ = io.import_cad(pipe_tee, params=prime.ImportCADParams(model))
     >>>     print(model)
 
     """
-    if destination is not None and not os.path.isdir(destination):
-        raise ValueError('destination directory provided does not exist')
-    file = download_file(
-        'pipe_tee.fmd', 'pyprimemesh', 'pipe_tee', destination=destination, force=force
-    )
-    _DOWNLOADS.append(file)
-    return file
+    return get_file(Examples.PIPE_TEE_FMD, destination, force)
 
 
-def clear_download_cache():
-    """Clears the cache of downloaded files"""
-    [os.remove(_file) for _file in _DOWNLOADS]
-    _DOWNLOADS.clear()
+def download_pipe_tee_scdoc(
+    destination: Optional[str] = None, force: bool = False
+) -> Union[str, os.PathLike]:
+    """Download SCDOC file for the pipe tee example
+
+    Parameters
+    ----------
+    destination: Optional[str]
+        Destination for the file to be downloaded.
+        If nothing is provided, the default path in app data is used
+    force: bool
+        If true, the file is always downloaded.
+        If false, an existing file in the cache may be re-used.
+
+    Returns
+    -------
+    str
+        Local path to the downloaded file
+
+    Raises
+    ------
+    ValueError
+        When the provided destination path does not exist on file
+
+    Examples
+    --------
+    >>> import ansys.meshing.prime as prime
+    >>> import ansys.meshing.prime.examples as prime_examples
+    >>> with prime.launch_prime() as session:
+    >>>     model = session.model
+    >>>     pipe_tee = prime_examples.download_pipe_tee_scdoc()
+    >>>     with prime.FileIO(model) as io:
+    >>>         _ = io.import_cad(pipe_tee, params=prime.ImportCADParams(model))
+    >>>     print(model)
+
+    """
+    return get_file(Examples.PIPE_TEE_SCDOC, destination, force)
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/examples/download.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/examples/download_utilities.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/graphics/graphics.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/graphics.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/graphics/images/bin.png` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/bin.png`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/graphics/images/invert_visibility.png` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/invert_visibility.png`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/graphics/images/parts.png` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/parts.png`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/graphics/images/selectioninfo.png` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/selectioninfo.png`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/graphics/images/show_edges.png` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/show_edges.png`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/graphics/images/surface_body.png` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/graphics/images/surface_body.png`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/client.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/client.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/config.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/config.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/defaults.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/defaults.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/error_handling.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/error_handling.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,17 @@
     ErrorCode.EXTRACTFEATURESBYEDGESFAILED: "Feature extraction by edge tracing failed.",
     ErrorCode.CREATEEDGEZONELETFAILED: "Create edge zonelets by node path failed.",
     ErrorCode.VOLUMEMESH_MIDNODESNOTSUPPORTED: "Improve volume mesh error: meshes with mid nodes are not supported.",
     ErrorCode.VOLUMEMESHNOTFOUND: "Volume mesh not found.",
     ErrorCode.NOTSUPPORTEDFORNONTRIFACEZONE: "Only triangular faces are supported.",
     ErrorCode.NOTSUPPORTEDFORNONQUADFACEZONE: "Only quadrilateral faces zonelets are supported.",
     ErrorCode.PARTNOTMESHED: "Part has unmeshed topofaces.",
+    ErrorCode.MORPHER_COMPUTEBCS: "Failed to compute boundary conditions.",
+    ErrorCode.MORPHER_MATCHMORPHINVALIDSOURCEINPUT: "Invalid source input for match morphing.",
+    ErrorCode.MORPHER_BCPAIRINPUTTYPEMISMATCH: "Entity type does not match with input for defined boundary condition pair.",
     ErrorCode.INVALIDGLOBALMINMAX: "Invalid global min, max value.",
     ErrorCode.INVALIDSIZECONTROLINPUTS: "Invalid size control input. Verify sizing parameters of size control.",
     ErrorCode.INVALIDSIZECONTROLSCOPE: "Invalid size control scope. Failed to evaluate scope for the size control.",
     ErrorCode.INVALIDPROXIMITYSIZINGINPUT: "Invalid proximity sizing input. Elements per gap should be a positive value.",
     ErrorCode.INVALIDCURVATURESIZINGINPUT: "Invalid curvature sizing input. Normal angle should be a positive value.",
     ErrorCode.TRANSFORMATIONFAILED: "Failed to transform.",
     ErrorCode.SCALINGFAILED: "Failed to scale.",
@@ -117,14 +120,15 @@
     ErrorCode.IGA_INCORRECTCONTROLPOINTSIZEWRTINPUT: "Control Points size cannot be greater than input mesh nodes.",
     ErrorCode.IGA_NURBSFITTINGFAILED: "Failed to fit spline.",
     ErrorCode.IGA_NEGATIVEJACOBIAN: "Negative Jacobian found.",
     ErrorCode.IGA_NURBSOPFAILED: "Spline operation failed.",
     ErrorCode.IGA_PERIODICKNOTVECTORCONVERSIONFAILED: "Periodic knot vector conversion failed.",
     ErrorCode.IGA_HREFINEMENTFAILED: "H refinement failed.",
     ErrorCode.IGA_PREFINEMENTFAILED: "P refinement failed.",
+    ErrorCode.IGA_QUADTOSPLINEBASISFAILED: "Quad to spline operation failed.",
     ErrorCode.BOIRESULTSFAILED: "BOI creation failed.",
     ErrorCode.CREATEBOI_INVALIDSCALE: "BOI creation failed. Scale factors should not be less than one.",
     ErrorCode.CREATEBOI_INVALIDFLOWDIRECTION: "BOI creation failed. Invalid flow or wake direction.",
     ErrorCode.CREATEBOI_IVALIDWRAPMESHSIZE: "BOI creation failed. Wrap cannot be performed with invalid mesh size.",
     ErrorCode.CREATEBOI_INVALIDWAKELEVELS: "BOI creation failed. Invalid wake levels input.",
     ErrorCode.CREATEBOI_INVALIDTYPEFORWRAP: "BOI creation failed. Wrapping is invalid for this BOI type.",
     ErrorCode.CREATECONTACTPATCH_INVALIDOFFSETDISTANCE: "Contact patch creation process failed. Scale factors should not be less than zero.",
@@ -210,14 +214,24 @@
     ErrorCode.PARTHASTOPOLOGY: "Part has a topology.",
     ErrorCode.PARTDOESNOTHAVETOPOLOGY: "Part does not have a topology.",
     ErrorCode.ZONESARENOTSUPPORTEDFORCELLZONELETS: "Zones are not supported for cell zonelets.",
     ErrorCode.TARGETZONELETS_NOTWATERTIGHT: "Zonelets of target do not form a watertight volume.",
     ErrorCode.TARGETZONELETS_SELFINTERSECTING: "Zonelets of target form a self intersecting volume.",
     ErrorCode.TOOLZONELETS_NOTWATERTIGHT: "Zonelets of tool do not form a watertight volume.",
     ErrorCode.TOOLZONELETS_SELFINTERSECTING: "Zonelets of tool form a self intersecting volume.",
+    ErrorCode.STACKER_INVALIDINPUTVOLUMES: "Invalid input volumes provided to stacker.",
+    ErrorCode.STACKER_INVALIDPARAMS: "Invalid parameters provided to stacker.",
+    ErrorCode.STACKER_FACESEPARATIONFAILED: "Stacker failed to separate base face.",
+    ErrorCode.STACKER_FAILED: "Stacker failed to mesh the model.",
+    ErrorCode.STACKER_NOFACEFOUNDINVOLUMES: "No face found in specified volumes.",
+    ErrorCode.STACKER_MESHEDFACESFOUND: "Some faces have existing mesh.",
+    ErrorCode.STACKER_INVALIDBASEFACEINPUT: "Base face list input has invalid ids.",
+    ErrorCode.STACKER_NONSTACKABLEVOLUMESFOUND: "Some volumes are not aligned in the stacking direction.",
+    ErrorCode.STACKER_INCORRECTBODYDEFINITION: "Some bodies are intersecting or incorrectly defined.",
+    ErrorCode.STACKER_BASEFACEUNMESHED: "Base face list input has unmeshed topofaces.",
     ErrorCode.PLUGINLOADFAILURE: "Failed to load surface editor plugin.",
     ErrorCode.INPUTNOTCOMPLETE: "Input provided is incomplete.",
     ErrorCode.SURFERCANNOTREMESHPERIODICZONELETS: "Remesh is not supported for periodic face zonelets.",
     ErrorCode.EXTRACTVOLUMESFAILED: "Extract volumes failed.",
     ErrorCode.REFINEATCONTACTSFAILED: "Failed to refine at contacts.",
     ErrorCode.RECOVERPERIODICSURFACESFAILED: "Failed to recover periodic surfaces.",
     ErrorCode.RECOVERPERIODICSURFACESINVALIDSCOPE: "Source face zonelets are empty. Invalid scope input.",
@@ -226,23 +240,40 @@
     ErrorCode.CREATECAPONFACEZONELETSFAILED: "Failed to create cap on face zonelets.",
     ErrorCode.INTERSECTIONINTARGETVOLUMES: "Found overlapping or intersecting target volumes.",
     ErrorCode.INTERSECTIONINCUTTERVOLUMES: "Found overlapping or intersecting cutter volumes.",
     ErrorCode.SUBTRACTVOLUMEFAILED: "Failed to subtract volumes.",
     ErrorCode.ZONELETSARENOTOFSAMEDIMENSION: "Zonelets are not of same dimension.",
     ErrorCode.MERGEZONELETSFAILED: "Merge zonelets failed.",
     ErrorCode.MERGESMALLZONELETSSUPPORTEDFORFACEZONELETS: "Merge small zonelets option is supported for only face zonelets.",
+    ErrorCode.MERGEVOLUMESFAILED: "Merge volumes failed.",
+    ErrorCode.DELETEVOLUMESFAILED: "Delete volumes failed.",
+    ErrorCode.INVALIDNEIGHBORVOLUMES: "Invalid neighbor volumes selected to merge volumes.",
     ErrorCode.INVALIDINPUTVOLUMES: "Invalid input volumes.",
     ErrorCode.MATCHEDMESHOPTIONINVALID: "Invalid option chosen to connect two different parts.",
     ErrorCode.COLOCATEMATCHEDNODESFAILED: "Colocation of matched nodes failed.",
     ErrorCode.IMPRINTBOUNDARYNODESFAILED: "Imprint of boundary nodes failed.",
     ErrorCode.IMPRINTBOUNDARYEDGESFAILED: "Imprint of boundary edges failed.",
     ErrorCode.SPLITINTERSECTINGBOUNDARYEDGESFAILED: "Splitting of intersecting boundary edges failed.",
     ErrorCode.MATCHINTERIORFAILED: "Matching of interior region of overlap failed.",
     ErrorCode.TOLERANCEVALUEINVALID: "Invalid tolerance value specified.",
+    ErrorCode.INVALIDTHINVOLUMECONTROLS: "Invalid thin volume control.",
     ErrorCode.SOURCEORTARGETNOTSPECIFIED: "No target or source faces specified.",
+    ErrorCode.THINVOLUMECONTROLINVALIDSOURCESCOPE: "Source scope not found.",
+    ErrorCode.THINVOLUMECONTROLINVALIDTARGETSCOPE: "Target scope not found.",
+    ErrorCode.THINVOLUMECONTROLINVALIDSCOPE: "Source scope and target scope cannot be same.",
+    ErrorCode.THINVOLUMECONTROLINVALIDSOURCESCOPEENTITY: "Invalid source scope entity.",
+    ErrorCode.THINVOLUMECONTROLINVALIDTARGETSCOPEENTITY: "Invalid target scope entity.",
+    ErrorCode.THINVOLUMECONTROLINVALIDNUMBEROFLAYER: "Number of layer in thin volume mesh should be greater than 0.",
+    ErrorCode.THINVOLUMECONTROLTOPOLOGYNOTSUPPORTED: "Thin volume mesh controls not supported for part with topology data.",
+    ErrorCode.EXPORTSTLFAILEDWITHTOPOLOGY: "Export STL not supported for part with topology data.",
+    ErrorCode.EXPORTSTLFAILEDWITHQUADFACES: "Export STL not supported for mesh with quad faces.",
+    ErrorCode.EXPORTSTLFAILEDWITHPOLYFACES: "Export STL not supported for mesh with poly faces.",
+    ErrorCode.EXPORTSTLFAILEDWITHHIGHERORDERMESH: "Export STL not supported for higher order mesh.",
+    ErrorCode.EXPORTSTLFAILEDWITHEMPTYPARTIDLIST: "Export STL failed. List of part ids is empty.",
+    ErrorCode.EXPORTSTLFAILEDWITHINCORRECTPARTID: "Export STL failed. Part id is incorrect.",
 }
 
 prime_warning_messages = {
     WarningCode.NOWARNING: "Success.",
     WarningCode.UNKNOWN: "Unknown Warning.",
     WarningCode.SURFER_QUADCLEANUP_MULTITHREADINGNOTSUPPORTED: "Warning: Multithreading is skipped for quad cleanup.",
     WarningCode.SURFERLAYEREDQUADFAILED: "Surface Meshing Warning: Layered quad region has triangles.",
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/grpc_communicator.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/grpc_communicator.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/json_utils.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/json_utils.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/launcher.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/prime_communicator.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/prime_communicator.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/internals/utils.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/internals/utils.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/lucid/mesh_util.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/lucid/mesh_util.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/lucid/scope.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/lucid/scope.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/params/primestructs.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/params/primestructs.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,27 @@
 from ansys.meshing.prime.autogen.deletetoolstructs import *
 from ansys.meshing.prime.autogen.featureextractionstructs import *
 from ansys.meshing.prime.autogen.fileiostructs import *
 from ansys.meshing.prime.autogen.igastructs import *
 from ansys.meshing.prime.autogen.materialpointmanagerstructs import *
 from ansys.meshing.prime.autogen.meshinfostructs import *
 from ansys.meshing.prime.autogen.modelstructs import *
+from ansys.meshing.prime.autogen.morpherbcsstructs import *
+from ansys.meshing.prime.autogen.morpherstructs import *
 from ansys.meshing.prime.autogen.partstructs import *
 from ansys.meshing.prime.autogen.periodiccontrolstructs import *
 from ansys.meshing.prime.autogen.prismcontrolstructs import *
 from ansys.meshing.prime.autogen.scaffolderstructs import *
 from ansys.meshing.prime.autogen.sizecontrolstructs import *
 from ansys.meshing.prime.autogen.sizefieldstructs import *
 from ansys.meshing.prime.autogen.splittoolstructs import *
 from ansys.meshing.prime.autogen.surfacesearchstructs import *
 from ansys.meshing.prime.autogen.surfaceutilitystructs import *
 from ansys.meshing.prime.autogen.surferstructs import *
+from ansys.meshing.prime.autogen.thinvolumecontrolstructs import *
 from ansys.meshing.prime.autogen.topoutilitystructs import *
 from ansys.meshing.prime.autogen.transformstructs import *
 from ansys.meshing.prime.autogen.volumecontrolstructs import *
 from ansys.meshing.prime.autogen.volumemeshtoolstructs import *
 from ansys.meshing.prime.autogen.volumesearchstructs import *
+from ansys.meshing.prime.autogen.volumesweeperstructs import *
 from ansys.meshing.prime.autogen.wrapperstructs import *
```

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/relaxed_json/__init__.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/relaxed_json/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/relaxed_json/decoder.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/relaxed_json/decoder.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/relaxed_json/encoder.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/relaxed_json/encoder.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/src/ansys/meshing/prime/relaxed_json/scanner.py` & `ansys-meshing-prime-0.4.0.dev6/src/ansys/meshing/prime/relaxed_json/scanner.py`

 * *Files identical despite different names*

### Comparing `ansys-meshing-prime-0.4.0.dev3/PKG-INFO` & `ansys-meshing-prime-0.4.0.dev6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-meshing-prime
-Version: 0.4.0.dev3
+Version: 0.4.0.dev6
 Summary: PyPrimeMesh provides a python client to Ansys Prime Server. Ansys Prime Server delivers core Ansys meshing technology.
 Author-email: "ANSYS, Inc." <pyansys.support@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -15,26 +15,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ansys-api-meshing-prime==0.1.1
 Requires-Dist: numpy>=1.14.0
 Requires-Dist: appdirs>=1.4.0
 Requires-Dist: importlib-metadata>=4.0,<5; python_version<='3.8'
 Requires-Dist: pyvista>=0.32.0 ; extra == "all"
-Requires-Dist: ansys-sphinx-theme==0.9.3 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.7 ; extra == "doc"
 Requires-Dist: jupyter-sphinx==0.4.0 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
-Requires-Dist: pyvista==0.38.2 ; extra == "doc"
+Requires-Dist: pyvista==0.38.5 ; extra == "doc"
 Requires-Dist: Sphinx==5.3.0 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.22 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.1 ; extra == "doc"
-Requires-Dist: sphinx-gallery==0.11.1 ; extra == "doc"
+Requires-Dist: sphinx-gallery==0.12.2 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxemoji==0.2.0 ; extra == "doc"
 Requires-Dist: pyvista>=0.32.0 ; extra == "graphics"
-Requires-Dist: pytest==7.2.1 ; extra == "tests"
+Requires-Dist: pytest==7.3.1 ; extra == "tests"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
 Project-URL: Documentation, https://prime.docs.pyansys.com
 Project-URL: Source, https://github.com/pyansys/pyprimemesh
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: graphics
 Provides-Extra: tests
@@ -88,15 +88,15 @@
 
 ```bash
 pip install -e .
 ```
 
 ## Dependencies
 
-You must have a licensed copy of the latest version of Ansys 2023 R1 locally.
+You must have Ansys 2023 R1 or newer versions installed for Ansys Prime Server (optionally, CAD readers can be configured).  Ansys Prime Server requires a Preppost or CFD Preppost license to run.
 
 ## Get Started
 
 ### Launching PyPrimeMesh
 
 To launch PyPrimeMesh:
```


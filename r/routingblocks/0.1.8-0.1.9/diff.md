# Comparing `tmp/routingblocks-0.1.8.tar.gz` & `tmp/routingblocks-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routingblocks-0.1.8.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "routingblocks-0.1.9.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `routingblocks-0.1.8.tar` & `routingblocks-0.1.9.tar`

### file list

```diff
@@ -1,293 +1,294 @@
--rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 routingblocks-0.1.8/.clang-format
--rw-r--r--   0        0        0     1221 2022-11-09 12:37:21.000000 routingblocks-0.1.8/.cmake-format
--rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 routingblocks-0.1.8/.github/dependabot.yml
--rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.8/.github/workflows/wheels.yml
--rw-r--r--   0        0        0     2103 2022-11-09 12:37:21.000000 routingblocks-0.1.8/.gitignore
--rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 routingblocks-0.1.8/.readthedocs.yaml
--rw-r--r--   0        0        0      436 2022-11-09 12:37:21.000000 routingblocks-0.1.8/CMakeLists.txt
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 routingblocks-0.1.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     1968 2022-11-09 12:37:21.000000 routingblocks-0.1.8/README.md
--rw-r--r--   0        0        0     2858 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/CMakeLists.txt
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/Evaluation.h
--rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/Instance.hpp
--rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/Labeling.h
--rw-r--r--   0        0        0      409 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/LocalSearch.h
--rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/Operators.h
--rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/Solution.h
--rw-r--r--   0        0        0     4413 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/binding_helpers.hpp
--rw-r--r--   0        0        0      288 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/large_neighborhood.h
--rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/specializations/ADPTW.h
--rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/specializations/NIFTW.h
--rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/include/routingblocks_bindings/utility.h
--rw-r--r--   0        0        0    15827 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/Evaluation.cpp
--rw-r--r--   0        0        0     5098 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/Instance.cpp
--rw-r--r--   0        0        0     4915 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/Labeling.cpp
--rw-r--r--   0        0        0     5942 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/LocalSearch.cpp
--rw-r--r--   0        0        0    10884 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/Operators.cpp
--rw-r--r--   0        0        0    22684 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/Solution.cpp
--rw-r--r--   0        0        0     1372 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/bindings.cpp
--rw-r--r--   0        0        0    10720 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/large_neighborhood.cpp
--rw-r--r--   0        0        0     1879 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/specializations/ADPTW.cpp
--rw-r--r--   0        0        0     2104 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/specializations/NIFTW.cpp
--rw-r--r--   0        0        0     6155 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/src/utility.cpp
--rw-r--r--   0        0        0     3693 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_adptw.pyi
--rw-r--r--   0        0        0     1555 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_alns.pyi
--rw-r--r--   0        0        0      942 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_arc.pyi
--rw-r--r--   0        0        0     8809 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_evaluation.pyi
--rw-r--r--   0        0        0      857 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_frvcp.pyi
--rw-r--r--   0        0        0      926 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_insertion_cache.pyi
--rw-r--r--   0        0        0     4553 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_instance.pyi
--rw-r--r--   0        0        0     6016 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_local_search.pyi
--rw-r--r--   0        0        0     3834 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_niftw.pyi
--rw-r--r--   0        0        0     4184 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_node.pyi
--rw-r--r--   0        0        0      667 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_node_location.pyi
--rw-r--r--   0        0        0      364 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_random.pyi
--rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_removal_cache.pyi
--rw-r--r--   0        0        0     8771 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_route.pyi
--rw-r--r--   0        0        0    10819 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_solution.pyi
--rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_types.pyi
--rw-r--r--   0        0        0     1961 2022-11-09 12:37:21.000000 routingblocks-0.1.8/bindings/stubs/_vertex.pyi
--rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/make.bat
--rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/adptw.rst
--rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/alns.rst
--rw-r--r--   0        0        0      651 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/auxilliary.rst
--rw-r--r--   0        0        0     1804 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/conf.py
--rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/development.rst
--rw-r--r--   0        0        0     2690 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/evaluation.rst
--rw-r--r--   0        0        0      417 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/examples.rst
--rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/extension.rst
--rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/frvcp.rst
--rw-r--r--   0        0        0      316 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/full_api.rst
--rw-r--r--   0        0        0    28951 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/getting_started.rst
--rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/index.rst
--rw-r--r--   0        0        0     4006 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/instance.rst
--rw-r--r--   0        0        0     9539 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/localsearch.rst
--rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/niftw.rst
--rw-r--r--   0        0        0     1245 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/references.bib
--rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/references.rst
--rw-r--r--   0        0        0     1376 2022-11-09 12:37:21.000000 routingblocks-0.1.8/docs/source/solution.rst
--rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/README.md
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/alns/__init__.py
--rw-r--r--   0        0        0     1372 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/alns/__main__.py
--rw-r--r--   0        0        0     4797 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/alns/alns.py
--rw-r--r--   0        0        0     2929 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/alns/parsing.py
--rw-r--r--   0        0        0      508 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/README.md
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/__init__.py
--rw-r--r--   0        0        0     3503 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/__main__.py
--rw-r--r--   0        0        0    18920 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/alns.py
--rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/config.json
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instance/__init__.py
--rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instance/interface.py
--rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instance/models.py
--rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instance/parsing.py
--rw-r--r--   0        0        0     1677 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/c101C10.txt
--rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/c104C10.txt
--rw-r--r--   0        0        0     1675 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/c202C10.txt
--rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/c205C10.txt
--rw-r--r--   0        0        0     1577 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/r102C10.txt
--rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/r103C10.txt
--rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/r201C10.txt
--rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/r203C10.txt
--rw-r--r--   0        0        0     1587 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/rc102C10.txt
--rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/rc108C10.txt
--rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/rc201C10.txt
--rw-r--r--   0        0        0     1584 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/rc205C10.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c102_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c103_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c104_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c105_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c106_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c107_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c108_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c109_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c201_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c202_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c203_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c204_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c205_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c206_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c207_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c208_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r102_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r103_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r104_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r105_21.txt
--rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r106_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r107_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r108_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r109_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r110_21.txt
--rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r111_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r112_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r201_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r202_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r203_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r204_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r205_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r206_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r207_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r208_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r209_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r210_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r211_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc102_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc103_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc104_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc105_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc106_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc107_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc108_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc201_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc202_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc203_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc204_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc205_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc206_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc207_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc208_21.txt
--rw-r--r--   0        0        0     2127 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/c103C15.txt
--rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/c106C15.txt
--rw-r--r--   0        0        0     2123 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/c202C15.txt
--rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/c208C15.txt
--rw-r--r--   0        0        0     2401 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/r102C15.txt
--rw-r--r--   0        0        0     2205 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/r105C15.txt
--rw-r--r--   0        0        0     2209 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/r202C15.txt
--rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/r209C15.txt
--rw-r--r--   0        0        0     2129 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/rc103C15.txt
--rw-r--r--   0        0        0     2119 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/rc108C15.txt
--rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/rc202C15.txt
--rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/rc204C15.txt
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/c101C5.txt
--rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/c103C5.txt
--rw-r--r--   0        0        0     1149 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/c206C5.txt
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/c208C5.txt
--rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/r104C5.txt
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/r105C5.txt
--rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/r202C5.txt
--rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/r203C5.txt
--rw-r--r--   0        0        0     1139 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/rc105C5.txt
--rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/rc108C5.txt
--rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/rc204C5.txt
--rw-r--r--   0        0        0     1053 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/rc208C5.txt
--rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/instances/evrptw/README.txt
--rw-r--r--   0        0        0      913 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/operators/ShawMoveSelector.py
--rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/operators/ShawRelatedness.py
--rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/operators/SpatioTemporalRelatedness.py
--rw-r--r--   0        0        0     2069 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/operators/__init__.py
--rw-r--r--   0        0        0     1269 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/parameters.py
--rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/requirements.txt
--rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/utility/__init__.py
--rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/evrptw/utility/algorithms.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/ils/__init__.py
--rw-r--r--   0        0        0     1454 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/ils/__main__.py
--rw-r--r--   0        0        0     4236 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/ils/ils.py
--rw-r--r--   0        0        0     2974 2022-11-09 12:37:21.000000 routingblocks-0.1.8/examples/ils/parsing.py
--rw-r--r--   0        0        0     2693 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/CMakeLists.txt
--rw-r--r--   0        0        0    35623 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/cmake/CPM.cmake
--rw-r--r--   0        0        0     1739 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/cmake/tools.cmake
--rw-r--r--   0        0        0    22838 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/ADPTWEvaluation.h
--rw-r--r--   0        0        0    14819 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/FRVCP.h
--rw-r--r--   0        0        0     2827 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/Instance.h
--rw-r--r--   0        0        0    14652 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/LocalSearch.h
--rw-r--r--   0        0        0    10459 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/NIFTWEvaluation.h
--rw-r--r--   0        0        0    28881 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/Solution.h
--rw-r--r--   0        0        0     5120 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/adaptive_large_neighborhood.hpp
--rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/arc.h
--rw-r--r--   0        0        0     8674 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/evaluation.h
--rw-r--r--   0        0        0    11760 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/insertion_cache.h
--rw-r--r--   0        0        0     2101 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/lns_operators.h
--rw-r--r--   0        0        0     3008 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/node.h
--rw-r--r--   0        0        0     4085 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/operators/InsertStationOperator.h
--rw-r--r--   0        0        0      936 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/operators/InterRouteTwoOptOperator.h
--rw-r--r--   0        0        0     3126 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/operators/RemoveStationOperator.h
--rw-r--r--   0        0        0    15813 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/operators/SwapOperator.h
--rw-r--r--   0        0        0     1972 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/operators.h
--rw-r--r--   0        0        0     5054 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/removal_cache.h
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/types.h
--rw-r--r--   0        0        0     8032 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/utility/adaptive_priority_list.h
--rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/utility/algorithms.h
--rw-r--r--   0        0        0      992 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/utility/arc_set.h
--rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/utility/heap.h
--rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/utility/iterator_pair.h
--rw-r--r--   0        0        0     3727 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/utility/random.h
--rw-r--r--   0        0        0     1357 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/include/routingblocks/vertex.h
--rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/CMakeLists.txt
--rw-r--r--   0        0        0      317 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/dynamic_bitset/CMakeLists.txt
--rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/dynamic_bitset/LICENSE.txt
--rw-r--r--   0        0        0   117337 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp
--rw-r--r--   0        0        0    20974 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h
--rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/small_vector/CMakeLists.txt
--rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/small_vector/LICENSE.txt
--rw-r--r--   0        0        0   241472 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/small_vector/small_vector/small_vector.hpp
--rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/xoshiro/CMakeLists.txt
--rw-r--r--   0        0        0     1090 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/xoshiro/LICENSE.txt
--rw-r--r--   0        0        0    49824 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/lib/xoshiro/xoshiro/xoshiro.h
--rw-r--r--   0        0        0     3299 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/ADPTWEvaluation.cpp
--rw-r--r--   0        0        0        1 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/FRVCP.cpp
--rw-r--r--   0        0        0     3393 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/Instance.cpp
--rw-r--r--   0        0        0     2289 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/LocalSearch.cpp
--rw-r--r--   0        0        0     8321 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/NIFTWEvaluation.cpp
--rw-r--r--   0        0        0     3773 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/Solution.cpp
--rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/adaptive_large_neighborbood.cpp
--rw-r--r--   0        0        0     4504 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/lns_operators.cpp
--rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/node.cpp
--rw-r--r--   0        0        0     3420 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/operators/InsertStationOperator.cpp
--rw-r--r--   0        0        0     2051 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/src/operators/InterRouteTwoOptOperator.cpp
--rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/test/CMakeLists.txt
--rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 routingblocks-0.1.8/native/test/src/dummy.cpp
--rw-r--r--   0        0        0     1946 2022-11-09 12:37:21.000000 routingblocks-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/__init__.py
--rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/adptw/__init__.py
--rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/niftw/__init__.py
--rw-r--r--   0        0        0      630 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/operators/__init__.py
--rw-r--r--   0        0        0     1525 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/operators/best_insert.py
--rw-r--r--   0        0        0     4397 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/operators/cluster_removal.py
--rw-r--r--   0        0        0     1908 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/operators/move_selectors.py
--rw-r--r--   0        0        0     5530 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/operators/related_removal.py
--rw-r--r--   0        0        0     1022 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/operators/route_removal.py
--rw-r--r--   0        0        0     3842 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/operators/station_vicinity_removal.py
--rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/operators/worst_removal.py
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/utility/__init__.py
--rw-r--r--   0        0        0     5849 2022-11-09 12:37:21.000000 routingblocks-0.1.8/routingblocks/utility/instance_builder.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/benchmarks/__init__.py
--rw-r--r--   0        0        0     3285 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/benchmarks/reference/insertion_cache.py
--rw-r--r--   0        0        0     1986 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/benchmarks/reference/removal_cache.py
--rw-r--r--   0        0        0     1191 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/benchmarks/test_benchmark_frvcp.py
--rw-r--r--   0        0        0     2056 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/benchmarks/test_benchmark_local_search.py
--rw-r--r--   0        0        0     3118 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/benchmarks/test_benchmark_removal_cache.py
--rw-r--r--   0        0        0     9867 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/benchmarks/test_benchmark_route_update.py
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/conftest.py
--rw-r--r--   0        0        0     5570 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/fixtures/data/c101C5.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/fixtures/data/c101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/fixtures/data/r101_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/fixtures/data/r201_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/fixtures/data/rc101_21.txt
--rw-r--r--   0        0        0     4623 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/fixtures/mock_evaluation.py
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/helpers/__init__.py
--rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/helpers/interface.py
--rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/helpers/models.py
--rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/helpers/parsing.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/__init__.py
--rw-r--r--   0        0        0     7708 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/test_cluster_removal.py
--rw-r--r--   0        0        0     1645 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/test_random_insertion.py
--rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/test_random_removal.py
--rw-r--r--   0        0        0     3876 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/test_related_removal.py
--rw-r--r--   0        0        0     1821 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/test_station_insertion.py
--rw-r--r--   0        0        0     1165 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/test_station_removal.py
--rw-r--r--   0        0        0     2480 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/test_station_vicinity_removal.py
--rw-r--r--   0        0        0    20635 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/operators/test_swap.py
--rw-r--r--   0        0        0     1934 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_evaluation.py
--rw-r--r--   0        0        0     4629 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_frvcp.py
--rw-r--r--   0        0        0     6422 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_insertion_cache.py
--rw-r--r--   0        0        0     5154 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_large_neighborhood.py
--rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_lns_helpers.py
--rw-r--r--   0        0        0     6343 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_local_search.py
--rw-r--r--   0        0        0     1990 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_node.py
--rw-r--r--   0        0        0     3190 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_removal_cache.py
--rw-r--r--   0        0        0    14114 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_route.py
--rw-r--r--   0        0        0    20300 2022-11-09 12:37:21.000000 routingblocks-0.1.8/test/tests/test_solution.py
--rw-r--r--   0        0        0     3226 2022-11-09 12:37:21.000000 routingblocks-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 routingblocks-0.1.9/.clang-format
+-rw-r--r--   0        0        0     1221 2022-11-09 12:37:21.000000 routingblocks-0.1.9/.cmake-format
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 routingblocks-0.1.9/.github/dependabot.yml
+-rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.9/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0     2103 2022-11-09 12:37:21.000000 routingblocks-0.1.9/.gitignore
+-rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 routingblocks-0.1.9/.readthedocs.yaml
+-rw-r--r--   0        0        0      436 2022-11-09 12:37:21.000000 routingblocks-0.1.9/CMakeLists.txt
+-rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 routingblocks-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1968 2022-11-09 12:37:21.000000 routingblocks-0.1.9/README.md
+-rw-r--r--   0        0        0     3073 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/CMakeLists.txt
+-rw-r--r--   0        0        0    35623 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/cmake/CPM.cmake
+-rw-r--r--   0        0        0      334 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/include/routingblocks_bindings/Evaluation.h
+-rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/include/routingblocks_bindings/Instance.hpp
+-rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/include/routingblocks_bindings/Labeling.h
+-rw-r--r--   0        0        0      409 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/include/routingblocks_bindings/LocalSearch.h
+-rw-r--r--   0        0        0      384 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/include/routingblocks_bindings/Operators.h
+-rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/include/routingblocks_bindings/Solution.h
+-rw-r--r--   0        0        0     4413 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/include/routingblocks_bindings/binding_helpers.hpp
+-rw-r--r--   0        0        0      288 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/include/routingblocks_bindings/large_neighborhood.h
+-rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/include/routingblocks_bindings/specializations/ADPTW.h
+-rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/include/routingblocks_bindings/specializations/NIFTW.h
+-rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/include/routingblocks_bindings/utility.h
+-rw-r--r--   0        0        0    15612 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/src/Evaluation.cpp
+-rw-r--r--   0        0        0     5098 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/src/Instance.cpp
+-rw-r--r--   0        0        0     4797 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/src/Labeling.cpp
+-rw-r--r--   0        0        0     5974 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/src/LocalSearch.cpp
+-rw-r--r--   0        0        0    10302 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/src/Operators.cpp
+-rw-r--r--   0        0        0    23224 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/src/Solution.cpp
+-rw-r--r--   0        0        0     1372 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/src/bindings.cpp
+-rw-r--r--   0        0        0    10104 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/src/large_neighborhood.cpp
+-rw-r--r--   0        0        0     1828 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/src/specializations/ADPTW.cpp
+-rw-r--r--   0        0        0     2041 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/src/specializations/NIFTW.cpp
+-rw-r--r--   0        0        0     6155 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/src/utility.cpp
+-rw-r--r--   0        0        0     3667 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_adptw.pyi
+-rw-r--r--   0        0        0     1555 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_alns.pyi
+-rw-r--r--   0        0        0      903 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_arc.pyi
+-rw-r--r--   0        0        0     8809 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_evaluation.pyi
+-rw-r--r--   0        0        0      857 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_frvcp.pyi
+-rw-r--r--   0        0        0      926 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_insertion_cache.pyi
+-rw-r--r--   0        0        0     4971 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_instance.pyi
+-rw-r--r--   0        0        0     6016 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_local_search.pyi
+-rw-r--r--   0        0        0     3796 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_niftw.pyi
+-rw-r--r--   0        0        0     4144 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_node.pyi
+-rw-r--r--   0        0        0      704 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_node_location.pyi
+-rw-r--r--   0        0        0      364 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_random.pyi
+-rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_removal_cache.pyi
+-rw-r--r--   0        0        0     8767 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_route.pyi
+-rw-r--r--   0        0        0    10819 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_solution.pyi
+-rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_types.pyi
+-rw-r--r--   0        0        0     1725 2022-11-09 12:37:21.000000 routingblocks-0.1.9/bindings/stubs/_vertex.pyi
+-rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/make.bat
+-rw-r--r--   0        0        0      213 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/adptw.rst
+-rw-r--r--   0        0        0      834 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/alns.rst
+-rw-r--r--   0        0        0      651 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/auxilliary.rst
+-rw-r--r--   0        0        0     1803 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/conf.py
+-rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/development.rst
+-rw-r--r--   0        0        0     2690 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/evaluation.rst
+-rw-r--r--   0        0        0      417 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/examples.rst
+-rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/extension.rst
+-rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/frvcp.rst
+-rw-r--r--   0        0        0      316 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/full_api.rst
+-rw-r--r--   0        0        0    28951 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/getting_started.rst
+-rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/index.rst
+-rw-r--r--   0        0        0     4033 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/instance.rst
+-rw-r--r--   0        0        0    14010 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/localsearch.rst
+-rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/niftw.rst
+-rw-r--r--   0        0        0     1245 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/references.bib
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/references.rst
+-rw-r--r--   0        0        0     1403 2022-11-09 12:37:21.000000 routingblocks-0.1.9/docs/source/solution.rst
+-rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/README.md
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/alns/__init__.py
+-rw-r--r--   0        0        0     1372 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/alns/__main__.py
+-rw-r--r--   0        0        0     4797 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/alns/alns.py
+-rw-r--r--   0        0        0     2929 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/alns/parsing.py
+-rw-r--r--   0        0        0      508 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/README.md
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/__init__.py
+-rw-r--r--   0        0        0     3503 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/__main__.py
+-rw-r--r--   0        0        0    18920 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/alns.py
+-rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/config.json
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instance/__init__.py
+-rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instance/interface.py
+-rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instance/models.py
+-rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instance/parsing.py
+-rw-r--r--   0        0        0     1677 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/c101C10.txt
+-rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/c104C10.txt
+-rw-r--r--   0        0        0     1675 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/c202C10.txt
+-rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/c205C10.txt
+-rw-r--r--   0        0        0     1577 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/r102C10.txt
+-rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/r103C10.txt
+-rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/r201C10.txt
+-rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/r203C10.txt
+-rw-r--r--   0        0        0     1587 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/rc102C10.txt
+-rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/rc108C10.txt
+-rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/rc201C10.txt
+-rw-r--r--   0        0        0     1584 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/rc205C10.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c102_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c103_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c104_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c105_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c106_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c107_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c108_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c109_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c201_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c202_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c203_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c204_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c205_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c206_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c207_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c208_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r102_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r103_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r104_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r105_21.txt
+-rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r106_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r107_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r108_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r109_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r110_21.txt
+-rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r111_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r112_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r201_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r202_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r203_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r204_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r205_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r206_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r207_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r208_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r209_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r210_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r211_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc102_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc103_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc104_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc105_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc106_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc107_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc108_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc201_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc202_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc203_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc204_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc205_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc206_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc207_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc208_21.txt
+-rw-r--r--   0        0        0     2127 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/c103C15.txt
+-rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/c106C15.txt
+-rw-r--r--   0        0        0     2123 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/c202C15.txt
+-rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/c208C15.txt
+-rw-r--r--   0        0        0     2401 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/r102C15.txt
+-rw-r--r--   0        0        0     2205 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/r105C15.txt
+-rw-r--r--   0        0        0     2209 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/r202C15.txt
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/r209C15.txt
+-rw-r--r--   0        0        0     2129 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/rc103C15.txt
+-rw-r--r--   0        0        0     2119 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/rc108C15.txt
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/rc202C15.txt
+-rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/rc204C15.txt
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/c101C5.txt
+-rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/c103C5.txt
+-rw-r--r--   0        0        0     1149 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/c206C5.txt
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/c208C5.txt
+-rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/r104C5.txt
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/r105C5.txt
+-rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/r202C5.txt
+-rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/r203C5.txt
+-rw-r--r--   0        0        0     1139 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/rc105C5.txt
+-rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/rc108C5.txt
+-rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/rc204C5.txt
+-rw-r--r--   0        0        0     1053 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/rc208C5.txt
+-rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/instances/evrptw/README.txt
+-rw-r--r--   0        0        0      913 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/operators/ShawMoveSelector.py
+-rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/operators/ShawRelatedness.py
+-rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/operators/SpatioTemporalRelatedness.py
+-rw-r--r--   0        0        0     2069 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/operators/__init__.py
+-rw-r--r--   0        0        0     1269 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/parameters.py
+-rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/requirements.txt
+-rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/utility/__init__.py
+-rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/evrptw/utility/algorithms.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/ils/__init__.py
+-rw-r--r--   0        0        0     1454 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/ils/__main__.py
+-rw-r--r--   0        0        0     4236 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/ils/ils.py
+-rw-r--r--   0        0        0     2974 2022-11-09 12:37:21.000000 routingblocks-0.1.9/examples/ils/parsing.py
+-rw-r--r--   0        0        0     2693 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/CMakeLists.txt
+-rw-r--r--   0        0        0    35623 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/cmake/CPM.cmake
+-rw-r--r--   0        0        0     1739 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/cmake/tools.cmake
+-rw-r--r--   0        0        0    22838 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/ADPTWEvaluation.h
+-rw-r--r--   0        0        0    14819 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/FRVCP.h
+-rw-r--r--   0        0        0     2827 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/Instance.h
+-rw-r--r--   0        0        0    14696 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/LocalSearch.h
+-rw-r--r--   0        0        0    10459 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/NIFTWEvaluation.h
+-rw-r--r--   0        0        0    28881 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/Solution.h
+-rw-r--r--   0        0        0     5120 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/adaptive_large_neighborhood.hpp
+-rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/arc.h
+-rw-r--r--   0        0        0     8624 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/evaluation.h
+-rw-r--r--   0        0        0    11760 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/insertion_cache.h
+-rw-r--r--   0        0        0     2101 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/lns_operators.h
+-rw-r--r--   0        0        0     3008 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/node.h
+-rw-r--r--   0        0        0     4085 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/operators/InsertStationOperator.h
+-rw-r--r--   0        0        0      936 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/operators/InterRouteTwoOptOperator.h
+-rw-r--r--   0        0        0     3126 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/operators/RemoveStationOperator.h
+-rw-r--r--   0        0        0    15813 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/operators/SwapOperator.h
+-rw-r--r--   0        0        0     1861 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/operators.h
+-rw-r--r--   0        0        0     5054 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/removal_cache.h
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/types.h
+-rw-r--r--   0        0        0     8032 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/utility/adaptive_priority_list.h
+-rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/utility/algorithms.h
+-rw-r--r--   0        0        0      992 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/utility/arc_set.h
+-rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/utility/heap.h
+-rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/utility/iterator_pair.h
+-rw-r--r--   0        0        0     3727 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/utility/random.h
+-rw-r--r--   0        0        0     1357 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/include/routingblocks/vertex.h
+-rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/lib/CMakeLists.txt
+-rw-r--r--   0        0        0      317 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/lib/dynamic_bitset/CMakeLists.txt
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/lib/dynamic_bitset/LICENSE.txt
+-rw-r--r--   0        0        0   117337 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp
+-rw-r--r--   0        0        0    20974 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h
+-rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/lib/small_vector/CMakeLists.txt
+-rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/lib/small_vector/LICENSE.txt
+-rw-r--r--   0        0        0   241472 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/lib/small_vector/small_vector/small_vector.hpp
+-rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/lib/xoshiro/CMakeLists.txt
+-rw-r--r--   0        0        0     1090 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/lib/xoshiro/LICENSE.txt
+-rw-r--r--   0        0        0    49824 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/lib/xoshiro/xoshiro/xoshiro.h
+-rw-r--r--   0        0        0     3299 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/src/ADPTWEvaluation.cpp
+-rw-r--r--   0        0        0        1 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/src/FRVCP.cpp
+-rw-r--r--   0        0        0     3393 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/src/Instance.cpp
+-rw-r--r--   0        0        0     2289 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/src/LocalSearch.cpp
+-rw-r--r--   0        0        0     8321 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/src/NIFTWEvaluation.cpp
+-rw-r--r--   0        0        0     3773 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/src/Solution.cpp
+-rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/src/adaptive_large_neighborbood.cpp
+-rw-r--r--   0        0        0     4504 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/src/lns_operators.cpp
+-rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/src/node.cpp
+-rw-r--r--   0        0        0     3420 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/src/operators/InsertStationOperator.cpp
+-rw-r--r--   0        0        0     2051 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/src/operators/InterRouteTwoOptOperator.cpp
+-rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/test/CMakeLists.txt
+-rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 routingblocks-0.1.9/native/test/src/dummy.cpp
+-rw-r--r--   0        0        0     1934 2022-11-09 12:37:21.000000 routingblocks-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 routingblocks-0.1.9/routingblocks/__init__.py
+-rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 routingblocks-0.1.9/routingblocks/adptw/__init__.py
+-rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 routingblocks-0.1.9/routingblocks/niftw/__init__.py
+-rw-r--r--   0        0        0      630 2022-11-09 12:37:21.000000 routingblocks-0.1.9/routingblocks/operators/__init__.py
+-rw-r--r--   0        0        0     1525 2022-11-09 12:37:21.000000 routingblocks-0.1.9/routingblocks/operators/best_insert.py
+-rw-r--r--   0        0        0     4397 2022-11-09 12:37:21.000000 routingblocks-0.1.9/routingblocks/operators/cluster_removal.py
+-rw-r--r--   0        0        0     1908 2022-11-09 12:37:21.000000 routingblocks-0.1.9/routingblocks/operators/move_selectors.py
+-rw-r--r--   0        0        0     5530 2022-11-09 12:37:21.000000 routingblocks-0.1.9/routingblocks/operators/related_removal.py
+-rw-r--r--   0        0        0     1022 2022-11-09 12:37:21.000000 routingblocks-0.1.9/routingblocks/operators/route_removal.py
+-rw-r--r--   0        0        0     3842 2022-11-09 12:37:21.000000 routingblocks-0.1.9/routingblocks/operators/station_vicinity_removal.py
+-rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 routingblocks-0.1.9/routingblocks/operators/worst_removal.py
+-rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 routingblocks-0.1.9/routingblocks/utility/__init__.py
+-rw-r--r--   0        0        0     5849 2022-11-09 12:37:21.000000 routingblocks-0.1.9/routingblocks/utility/instance_builder.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/benchmarks/__init__.py
+-rw-r--r--   0        0        0     3285 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/benchmarks/reference/insertion_cache.py
+-rw-r--r--   0        0        0     1986 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/benchmarks/reference/removal_cache.py
+-rw-r--r--   0        0        0     1191 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/benchmarks/test_benchmark_frvcp.py
+-rw-r--r--   0        0        0     2056 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/benchmarks/test_benchmark_local_search.py
+-rw-r--r--   0        0        0     3118 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/benchmarks/test_benchmark_removal_cache.py
+-rw-r--r--   0        0        0     9867 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/benchmarks/test_benchmark_route_update.py
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/conftest.py
+-rw-r--r--   0        0        0     5570 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/fixtures/data/c101C5.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/fixtures/data/c101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/fixtures/data/r101_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/fixtures/data/r201_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/fixtures/data/rc101_21.txt
+-rw-r--r--   0        0        0     4623 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/fixtures/mock_evaluation.py
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     2076 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/helpers/interface.py
+-rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/helpers/models.py
+-rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/helpers/parsing.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/operators/__init__.py
+-rw-r--r--   0        0        0     7708 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/operators/test_cluster_removal.py
+-rw-r--r--   0        0        0     1645 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/operators/test_random_insertion.py
+-rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/operators/test_random_removal.py
+-rw-r--r--   0        0        0     3876 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/operators/test_related_removal.py
+-rw-r--r--   0        0        0     1821 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/operators/test_station_insertion.py
+-rw-r--r--   0        0        0     1165 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/operators/test_station_removal.py
+-rw-r--r--   0        0        0     2480 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/operators/test_station_vicinity_removal.py
+-rw-r--r--   0        0        0    20635 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/operators/test_swap.py
+-rw-r--r--   0        0        0     1934 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/test_evaluation.py
+-rw-r--r--   0        0        0     4629 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/test_frvcp.py
+-rw-r--r--   0        0        0     6422 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/test_insertion_cache.py
+-rw-r--r--   0        0        0     5245 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/test_large_neighborhood.py
+-rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/test_lns_helpers.py
+-rw-r--r--   0        0        0    11505 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/test_local_search.py
+-rw-r--r--   0        0        0     1990 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/test_node.py
+-rw-r--r--   0        0        0     3190 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/test_removal_cache.py
+-rw-r--r--   0        0        0    14566 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/test_route.py
+-rw-r--r--   0        0        0    20300 2022-11-09 12:37:21.000000 routingblocks-0.1.9/test/tests/test_solution.py
+-rw-r--r--   0        0        0     3226 2022-11-09 12:37:21.000000 routingblocks-0.1.9/PKG-INFO
```

### Comparing `routingblocks-0.1.8/.cmake-format` & `routingblocks-0.1.9/.cmake-format`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/.github/workflows/wheels.yml` & `routingblocks-0.1.9/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/.gitignore` & `routingblocks-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/CONTRIBUTING.md` & `routingblocks-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/README.md` & `routingblocks-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/bindings/CMakeLists.txt` & `routingblocks-0.1.9/bindings/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 cmake_minimum_required(VERSION 3.18)
 include(CheckIPOSupported)
+include(${CMAKE_CURRENT_SOURCE_DIR}/cmake/CPM.cmake)
 # To force building for a specific python version, set Python_ROOT_DIR to the respective path.
 # This can be a venv as well.
 # See the FIND_PACKAGE python cmake documentation for details.
 FIND_PACKAGE(Python COMPONENTS Interpreter Development.Module REQUIRED)
 
 message(STATUS "Found python binary: ${Python_EXECUTABLE} (Version ${Python_VERSION})")
 
 set(PYBIND11_PYTHON_VERSION ${Python_VERSION})
 set(PYTHON_EXECUTABLE ${Python_EXECUTABLE})
 set(PYTHON_LIBS ${Python_LIBS})
-FIND_PACKAGE(pybind11 CONFIG REQUIRED)
+
+CPMAddPackage(
+        NAME pybind11
+        GITHUB_REPOSITORY pybind/pybind11
+        GIT_TAG smart_holder
+)
 
 file(GLOB_RECURSE headers CONFIGURE_DEPENDS "${CMAKE_CURRENT_SOURCE_DIR}/include/routingblocks_bindings/*.h")
 file(GLOB_RECURSE sources CONFIGURE_DEPENDS "${CMAKE_CURRENT_SOURCE_DIR}/src/*.cpp")
 
 pybind11_add_module(${PROJECT_NAME} ${sources})
 
 target_include_directories(${PROJECT_NAME} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)
 target_compile_definitions(${PROJECT_NAME} PUBLIC "routingblocks_MODULE_NAME=${PROJECT_NAME}")
 target_compile_definitions(${PROJECT_NAME} PUBLIC "routingblocks_VERSION=${PROJECT_VERSION}")
+target_compile_definitions(${PROJECT_NAME} PUBLIC "PYBIND11_USE_SMART_HOLDER_AS_DEFAULT")
 
 # Configure optimization flags
 if (CMAKE_COMPILER_IS_GNUCC)
     target_compile_options(${PROJECT_NAME} PUBLIC "$<$<CONFIG:DEBUG>:-O0;-g3>")
     target_compile_options(${PROJECT_NAME} PUBLIC "$<$<CONFIG:RELEASE>:-O3;>")
     target_compile_options(${PROJECT_NAME} PUBLIC "$<$<CONFIG:PROFILE>:-O2;-pg;-fno-omit-frame-pointer;-fno-optimize-sibling-calls;>")
 endif ()
```

### Comparing `routingblocks-0.1.8/bindings/include/routingblocks_bindings/binding_helpers.hpp` & `routingblocks-0.1.9/bindings/include/routingblocks_bindings/binding_helpers.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/bindings/src/Evaluation.cpp` & `routingblocks-0.1.9/bindings/src/Evaluation.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #include <pybind11/stl.h>
-#include <routingblocks/ADPTWEvaluation.h>
-#include <routingblocks/NIFTWEvaluation.h>
 #include <routingblocks/evaluation.h>
 #include <routingblocks_bindings/Evaluation.h>
 
+#include <algorithm>
 #include <routingblocks_bindings/binding_helpers.hpp>
 
 namespace routingblocks::bindings {
 
     class PyEvaluation : public routingblocks::Evaluation {
       protected:
         using py_type = pybind11::object;
@@ -171,137 +170,134 @@
             const ConcatenationBasedEvaluation::label_holder_t& label) const final {
             return py_get_cost_components(label.get<py_type>());
         }
     };
 
 }  // namespace routingblocks::bindings
 
-BIND_LIFETIME_PYTHON(routingblocks::Evaluation, "Evaluation")
-BIND_LIFETIME_PYTHON(routingblocks::bindings::PyEvaluation, "PyEvaluation")
-
 namespace routingblocks::bindings {
 
     class PyConcatenationBasedEvaluationTramboline : public PyConcatenationBasedEvaluation {
         using PyConcatenationBasedEvaluation::PyConcatenationBasedEvaluation;
 
       public:
         cost_t py_concatenate(const py_type& fwd, const py_type& bwd,
                               const Vertex& vertex) override {
             PYBIND11_OVERRIDE_PURE_NAME(cost_t, PyConcatenationBasedEvaluation, "concatenate",
-                                        py_concatenate, fwd, bwd, vertex);
+                                        py_concatenate, &fwd, &bwd, &vertex);
         }
 
         bool py_is_feasible(const py_type& label) const override {
             PYBIND11_OVERRIDE_PURE_NAME(bool, PyConcatenationBasedEvaluation, "is_feasible",
-                                        is_feasible, label);
+                                        is_feasible, &label);
         }
 
         cost_t py_compute_cost(const py_type& label) const override {
             PYBIND11_OVERRIDE_PURE_NAME(cost_t, PyConcatenationBasedEvaluation, "compute_cost",
-                                        py_compute_cost, label);
+                                        py_compute_cost, &label);
         }
 
         py_type py_propagate_forward(const py_type& pred_label, const Vertex& pred_vertex,
                                      const Vertex& vertex, const Arc& arc) const override {
             PYBIND11_OVERRIDE_PURE_NAME(py_type, PyConcatenationBasedEvaluation,
-                                        "propagate_forward", py_propagate_forward, pred_label,
-                                        pred_vertex, vertex, arc);
+                                        "propagate_forward", py_propagate_ & forward, &pred_label,
+                                        &pred_vertex, &vertex, &arc);
         }
 
         py_type py_propagate_backward(const py_type& succ_label, const Vertex& succ_vertex,
                                       const Vertex& vertex, const Arc& arc) const override {
             PYBIND11_OVERRIDE_PURE_NAME(py_type, PyConcatenationBasedEvaluation,
-                                        "propagate_backward", py_propagate_backward, succ_label,
-                                        succ_vertex, vertex, arc);
+                                        "propagate_backward", py_propagate_backward, &succ_label,
+                                        &succ_vertex, &vertex, &arc);
         }
 
         py_type py_create_forward_label(const Vertex& vertex) override {
             PYBIND11_OVERRIDE_PURE_NAME(py_type, PyConcatenationBasedEvaluation,
-                                        "create_forward_label", py_create_forward_label, vertex);
+                                        "create_forward_label", py_create_forward_label, &vertex);
         }
 
         py_type py_create_backward_label(const Vertex& vertex) override {
             PYBIND11_OVERRIDE_PURE_NAME(py_type, PyConcatenationBasedEvaluation,
-                                        "create_backward_label", py_create_backward_label, vertex);
+                                        "create_backward_label", py_create_backward_label, &vertex);
         }
 
         std::vector<resource_t> py_get_cost_components(const py_type& label) const override {
             PYBIND11_OVERRIDE_PURE_NAME(std::vector<resource_t>, PyConcatenationBasedEvaluation,
-                                        "get_cost_components", get_cost_components, label);
+                                        "get_cost_components", get_cost_components, &label);
         }
     };
 
     class PyEvaluationTramboline : public PyEvaluation {
         using PyEvaluation::PyEvaluation;
 
       public:
         cost_t py_evaluate(const Instance& instance,
                            const std::vector<py_segment_type>& segments) override {
-            PYBIND11_OVERRIDE_PURE_NAME(cost_t, PyEvaluation, "evaluate", py_evaluate, instance);
+            PYBIND11_OVERRIDE_PURE_NAME(cost_t, PyEvaluation, "evaluate", py_evaluate, &instance);
         }
 
         bool py_is_feasible(const py_type& label) const override {
-            PYBIND11_OVERRIDE_PURE_NAME(bool, PyEvaluation, "is_feasible", is_feasible, label);
+            PYBIND11_OVERRIDE_PURE_NAME(bool, PyEvaluation, "is_feasible", is_feasible, &label);
         }
 
         cost_t py_compute_cost(const py_type& label) const override {
             PYBIND11_OVERRIDE_PURE_NAME(cost_t, PyEvaluation, "compute_cost", py_compute_cost,
-                                        label);
+                                        &label);
         }
 
         py_type py_propagate_forward(const py_type& pred_label, const Vertex& pred_vertex,
                                      const Vertex& vertex, const Arc& arc) const override {
             PYBIND11_OVERRIDE_PURE_NAME(py_type, PyEvaluation, "propagate_forward",
-                                        py_propagate_forward, pred_label, pred_vertex, vertex, arc);
+                                        py_propagate_forward, &pred_label, &pred_vertex, &vertex,
+                                        &arc);
         }
 
         py_type py_propagate_backward(const py_type& succ_label, const Vertex& succ_vertex,
                                       const Vertex& vertex, const Arc& arc) const override {
             PYBIND11_OVERRIDE_PURE_NAME(py_type, PyEvaluation, "propagate_backward",
-                                        py_propagate_backward, succ_label, succ_vertex, vertex,
-                                        arc);
+                                        py_propagate_backward, &succ_label, &succ_vertex, &vertex,
+                                        &arc);
         }
 
         py_type py_create_forward_label(const Vertex& vertex) override {
             PYBIND11_OVERRIDE_PURE_NAME(py_type, PyEvaluation, "create_forward_label",
-                                        py_create_forward_label, vertex);
+                                        py_create_forward_label, &vertex);
         }
 
         py_type py_create_backward_label(const Vertex& vertex) override {
             PYBIND11_OVERRIDE_PURE_NAME(py_type, PyEvaluation, "create_backward_label",
-                                        py_create_backward_label, vertex);
+                                        py_create_backward_label, &vertex);
         }
 
         std::vector<resource_t> py_get_cost_components(const py_type& label) const override {
             PYBIND11_OVERRIDE_PURE_NAME(std::vector<resource_t>, PyEvaluation,
-                                        "get_cost_components", get_cost_components, label);
+                                        "get_cost_components", get_cost_components, &label);
         }
     };
 
     auto bind_evaluation_interface(pybind11::module& m) {
-        return pybind11::class_<Evaluation, std::shared_ptr<Evaluation>>(m, "Evaluation");
+        return pybind11::class_<Evaluation>(m, "Evaluation");
     }
 
     void bind_py_evaluation(pybind11::module_& m, auto& evaluation_interface) {
-        pybind11::class_<PyConcatenationBasedEvaluation, PyConcatenationBasedEvaluationTramboline,
-                         std::shared_ptr<PyConcatenationBasedEvaluation>>(
+        pybind11::class_<PyConcatenationBasedEvaluation, PyConcatenationBasedEvaluationTramboline>(
             m, "PyConcatenationBasedEvaluation", evaluation_interface)
             .def(pybind11::init<>())
             .def("propagate_forward", &PyConcatenationBasedEvaluation::py_propagate_forward)
             .def("propagate_backward", &PyConcatenationBasedEvaluation::py_propagate_backward)
             .def("concatenate", &PyConcatenationBasedEvaluation::py_concatenate)
             .def("compute_cost", &PyConcatenationBasedEvaluation::py_compute_cost)
             .def("get_cost_components", &PyConcatenationBasedEvaluation::py_get_cost_components)
             .def("is_feasible", &PyConcatenationBasedEvaluation::py_is_feasible)
             .def("create_forward_label", &PyConcatenationBasedEvaluation::py_create_forward_label)
             .def("create_backward_label",
                  &PyConcatenationBasedEvaluation::py_create_backward_label);
 
-        pybind11::class_<PyEvaluation, PyEvaluationTramboline, std::shared_ptr<PyEvaluation>>(
-            m, "PyEvaluation", evaluation_interface)
+        pybind11::class_<PyEvaluation, PyEvaluationTramboline>(m, "PyEvaluation",
+                                                               evaluation_interface)
             .def(pybind11::init<>())
             .def("propagate_forward", &PyEvaluation::py_propagate_forward)
             .def("propagate_backward", &PyEvaluation::py_propagate_backward)
             .def("concatenate", &PyEvaluation::py_evaluate)
             .def("compute_cost", &PyEvaluation::py_compute_cost)
             .def("get_cost_components", &PyEvaluation::py_get_cost_components)
             .def("is_feasible", &PyEvaluation::py_is_feasible)
```

### Comparing `routingblocks-0.1.8/bindings/src/Instance.cpp` & `routingblocks-0.1.9/bindings/src/Instance.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/bindings/src/Labeling.cpp` & `routingblocks-0.1.9/bindings/src/Labeling.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -28,50 +28,48 @@
         virtual void prepare(const std::vector<VertexID>&) = 0;
 
         virtual value_type create_root_label() = 0;
     };
     using PyPropagator = Propagator<pybind11::object>;
 }  // namespace routingblocks
 
-BIND_LIFETIME_PYTHON(routingblocks::Propagator<pybind11::object>, "Propagator")
-
 namespace routingblocks::bindings {
     class PyPropagatorTramboline : public PyPropagator {
       public:
         using value_type = PyPropagator::value_type;
         using PyPropagator::PyPropagator;
 
         std::optional<value_type> propagate(const value_type& predecessor, const Vertex& origin,
                                             const Vertex& target, const Arc& arc) override {
-            PYBIND11_OVERRIDE_PURE(std::optional<value_type>, PyPropagator, propagate, predecessor,
-                                   origin, target, arc);
+            PYBIND11_OVERRIDE_PURE(std::optional<value_type>, PyPropagator, propagate, &predecessor,
+                                   &origin, &target, &arc);
         }
 
         bool dominates(const value_type& label, const value_type& other) override {
-            PYBIND11_OVERRIDE_PURE(bool, PyPropagator, dominates, label, other);
+            PYBIND11_OVERRIDE_PURE(bool, PyPropagator, dominates, &label, &other);
         }
 
         bool cheaper_than(const value_type& label, const value_type& other) override {
-            PYBIND11_OVERRIDE_PURE(bool, PyPropagator, cheaper_than, label, other);
+            PYBIND11_OVERRIDE_PURE(bool, PyPropagator, cheaper_than, &label, &other);
         }
 
         bool should_order_before(const value_type& label, const value_type& other) override {
-            PYBIND11_OVERRIDE_PURE(bool, PyPropagator, should_order_before, label, other);
+            PYBIND11_OVERRIDE_PURE(bool, PyPropagator, should_order_before, &label, &other);
         }
 
         std::vector<VertexID> extract_path(const value_type& sink_label) override {
-            PYBIND11_OVERRIDE_PURE(std::vector<VertexID>, PyPropagator, extract_path, sink_label);
+            PYBIND11_OVERRIDE_PURE(std::vector<VertexID>, PyPropagator, extract_path, &sink_label);
         }
 
         bool is_final_label(const value_type& _label) override {
-            PYBIND11_OVERRIDE_PURE(bool, PyPropagator, is_final_label, _label);
+            PYBIND11_OVERRIDE_PURE(bool, PyPropagator, is_final_label, &_label);
         }
 
         void prepare(const std::vector<VertexID>& vector) override {
-            PYBIND11_OVERRIDE_PURE(void, PyPropagator, prepare, vector);
+            PYBIND11_OVERRIDE_PURE(void, PyPropagator, prepare, &vector);
         }
 
         value_type create_root_label() override {
             PYBIND11_OVERRIDE_PURE(value_type, PyPropagator, create_root_label, );
         }
     };
 
@@ -91,16 +89,15 @@
             .def("prepare", &PropagatorClass::prepare, "Prepares the propagator for a new route.")
             .def("create_root_label", &PropagatorClass::create_root_label,
                  "Creates the root label for the propagator.");
     }
 
     void bind_labeling(pybind11::module_& m) {
         auto propagator_interface
-            = pybind11::class_<PyPropagator, PyPropagatorTramboline, std::shared_ptr<PyPropagator>>(
-                  m, "Propagator")
+            = pybind11::class_<PyPropagator, PyPropagatorTramboline>(m, "Propagator")
                   .def(pybind11::init<>());
         bind_propagator<PyPropagator>(propagator_interface);
 
         pybind11::class_<FRVCP<PyPropagator::value_type>>(m, "FRVCP")
             .def(pybind11::init<const Instance&, std::shared_ptr<PyPropagator>>())
             .def("optimize", &FRVCP<PyPropagator::value_type>::optimize,
                  "Solve FRVCP for the specified route.");
```

### Comparing `routingblocks-0.1.8/bindings/src/LocalSearch.cpp` & `routingblocks-0.1.9/bindings/src/LocalSearch.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 namespace routingblocks::bindings {
 
     class PivotingRuleTrampoline : public PivotingRule {
       public:
         using PivotingRule::PivotingRule;
 
         std::shared_ptr<Move> select_move(const Solution& solution) override {
-            PYBIND11_OVERLOAD_PURE(std::shared_ptr<Move>, PivotingRule, select_move, solution);
+            PYBIND11_OVERRIDE_PURE(std::shared_ptr<Move>, PivotingRule, select_move, &solution);
         }
 
         bool continue_search(const std::shared_ptr<Move>& move, cost_t cost,
                              const Solution& solution) override {
-            PYBIND11_OVERLOAD_PURE(bool, PivotingRule, continue_search, move, cost, solution);
+            PYBIND11_OVERRIDE_PURE(bool, PivotingRule, continue_search, move, cost, &solution);
         }
     };
 
     void bind_pivoting_rule(pybind11::module_& m) {
         pybind11::class_<PivotingRule, PivotingRuleTrampoline>(m, "PivotingRule")
             .def(pybind11::init<>())
             .def("select_move", &PivotingRule::select_move)
@@ -45,15 +45,15 @@
             .def("continue_search", &FirstImprovementPivotingRule::continue_search);
     }
 
     void bind_local_search(pybind11::module& m) {
         pybind11::class_<routingblocks::LocalSearch>(m, "LocalSearch")
             .def(pybind11::init<const routingblocks::Instance&, std::shared_ptr<Evaluation>,
                                 std::shared_ptr<Evaluation>, PivotingRule*>(),
-                 pybind11::keep_alive<1, 5>())
+                 pybind11::keep_alive<1, 2>(), pybind11::keep_alive<1, 5>())
             .def(
                 "optimize",
                 [](LocalSearch& ls, Solution& sol, std::vector<Operator*> operators) -> void {
                     ls.run(sol, operators.begin(), operators.end());
                 },
                 "Optimizes the passed solution inplace.");
     }
```

### Comparing `routingblocks-0.1.8/bindings/src/Operators.cpp` & `routingblocks-0.1.9/bindings/src/Operators.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -10,57 +10,55 @@
 namespace routingblocks::bindings {
 
     class PyOperator : public routingblocks::Operator {
         using routingblocks::Operator::Operator;
 
       public:
         void prepare_search(const Solution& solution) override {
-            PYBIND11_OVERLOAD_PURE(void, routingblocks::Operator, prepare_search, solution);
+            PYBIND11_OVERRIDE_PURE(void, routingblocks::Operator, prepare_search, &solution);
         }
         std::shared_ptr<Move> find_next_improving_move(eval_t& evaluation, const Solution& solution,
                                                        const Move* previous_move) override {
-            PYBIND11_OVERLOAD_PURE(std::shared_ptr<Move>, routingblocks::Operator,
-                                   find_next_improving_move, evaluation, solution, previous_move);
+            PYBIND11_OVERRIDE_PURE(std::shared_ptr<Move>, routingblocks::Operator,
+                                   find_next_improving_move, &evaluation, &solution, previous_move);
         }
         void finalize_search() override {
-            PYBIND11_OVERLOAD_PURE(void, routingblocks::Operator, finalize_search);
+            PYBIND11_OVERRIDE_PURE(void, routingblocks::Operator, finalize_search);
         }
     };
 
     class PyMove : public routingblocks::Move {
         using routingblocks::Move::Move;
 
       public:
         cost_t get_cost_delta(Evaluation& evaluation, const Instance& instance,
                               const Solution& solution) const override {
-            PYBIND11_OVERLOAD_PURE(cost_t, routingblocks::Move, get_cost_delta, evaluation,
-                                   instance, solution);
+            PYBIND11_OVERRIDE_PURE(cost_t, routingblocks::Move, get_cost_delta, &evaluation,
+                                   &instance, &solution);
         }
 
         void apply(const Instance& instance, Solution& solution) const override {
-            PYBIND11_OVERRIDE_PURE(void, routingblocks::Move, apply, instance, solution);
+            PYBIND11_OVERRIDE_PURE(void, routingblocks::Move, apply, &instance, &solution);
         }
     };
 
     auto bind_operator_interface(pybind11::module_& m) {
-        return pybind11::class_<routingblocks::Operator, PyOperator,
-                                std::shared_ptr<routingblocks::Operator>>(m, "LocalSearchOperator")
+        return pybind11::class_<routingblocks::Operator, PyOperator>(m, "LocalSearchOperator")
             .def(pybind11::init<>())
             .def("prepare_search", &routingblocks::Operator::prepare_search,
                  "Prepare the operator for "
                  "searching for a move.")
             .def("find_next_improving_move", &routingblocks::Operator::find_next_improving_move,
                  "Find the next improving move.")
             .def("finalize_search", &routingblocks::Operator::finalize_search,
                  "Finalize the search.");
     }
 
     auto bind_move_interface(pybind11::module_& m) {
-        return pybind11::class_<routingblocks::Move, PyMove, std::shared_ptr<routingblocks::Move>>(
-                   m, "Move")
+        return pybind11::class_<routingblocks::Move, PyMove>(m, "Move")
             .def(pybind11::init<>())
             .def("get_cost_delta", &routingblocks::Move::get_cost_delta,
                  "Get the cost of the move.")
             .def("apply", &routingblocks::Move::apply, "Apply the move to the solution.");
     }
 
     template <size_t OriginSegmentSize, size_t TargetSegmentSize>
@@ -69,98 +67,91 @@
         using operator_move_t = routingblocks::SwapMove<OriginSegmentSize, TargetSegmentSize>;
 
         std::stringstream base_name;
         base_name << "SwapOperator"
                   << "_" << OriginSegmentSize << "_" << TargetSegmentSize;
         auto base_name_str = base_name.str();
 
-        pybind11::class_<operator_t, std::shared_ptr<operator_t>>(
+        pybind11::class_<operator_t>(
             m, base_name_str.data(), operator_interface,
             "Swap operator. Swaps a segment of customers from a route to another route.")
             .def(pybind11::init<const Instance&, const utility::arc_set*>(),
-                 pybind11::keep_alive<1, 3>())
+                 pybind11::keep_alive<1, 2>(), pybind11::keep_alive<1, 3>())
             .def("prepare_search", &operator_t::prepare_search)
             .def("find_next_improving_move", &operator_t::find_next_improving_move)
             .def("finalize_search", &operator_t::finalize_search)
             .def("create_move", &operator_t::create_move,
                  "Create a move that represents a given generator arc.");
 
         std::stringstream move_name;
         move_name << "SwapOperatorMove"
                   << "_" << OriginSegmentSize << "_" << TargetSegmentSize;
         auto move_name_str = move_name.str();
 
-        pybind11::class_<operator_move_t, std::shared_ptr<operator_move_t>>(
+        pybind11::class_<operator_move_t>(
             m, move_name_str.data(), move_interface,
             "Relocate move. Moves a customer from a route to "
             "another route. Implemented for inter- and intra-route moves.")
             .def(pybind11::init<NodeLocation, NodeLocation>())
             .def("get_cost_delta", &operator_move_t::get_cost_delta)
             .def("apply", &operator_move_t::apply);
     }
 
     void bind_inter_route_two_opt(pybind11::module_& m, auto& operator_interface,
                                   auto& move_interface) {
-        pybind11::class_<routingblocks::InterRouteTwoOptOperator,
-                         std::shared_ptr<routingblocks::InterRouteTwoOptOperator>>(
+        pybind11::class_<routingblocks::InterRouteTwoOptOperator>(
             m, "InterRouteTwoOptOperator", operator_interface,
             "Considers two-opt moves between distinct routes. Tries to integrate the "
             "generator arc into the solution.")
             .def(pybind11::init<const Instance&, const utility::arc_set*>(),
-                 pybind11::keep_alive<1, 3>())
+                 pybind11::keep_alive<1, 3>(), pybind11::keep_alive<1, 3>())
             .def("prepare_search", &routingblocks::InterRouteTwoOptOperator::prepare_search)
             .def("find_next_improving_move",
                  &routingblocks::InterRouteTwoOptOperator::find_next_improving_move)
             .def("finalize_search", &routingblocks::InterRouteTwoOptOperator::finalize_search)
             .def("create_move", &routingblocks::InterRouteTwoOptOperator::create_move,
                  "Create a move that represents a given generator arc.");
 
-        pybind11::class_<routingblocks::InterRouteTwoOptMove,
-                         std::shared_ptr<routingblocks::InterRouteTwoOptMove>>(
-            m, "InterRouteTwoOptMove", move_interface)
+        pybind11::class_<routingblocks::InterRouteTwoOptMove>(m, "InterRouteTwoOptMove",
+                                                              move_interface)
             .def(pybind11::init<NodeLocation, NodeLocation>())
             .def("get_cost_delta", &routingblocks::InterRouteTwoOptMove::get_cost_delta)
             .def("apply", &routingblocks::InterRouteTwoOptMove::apply);
     }
 
     void bind_station_in_operator(pybind11::module_& m, auto& operator_interface,
                                   auto& move_interface) {
-        pybind11::class_<routingblocks::InsertStationOperator,
-                         std::shared_ptr<routingblocks::InsertStationOperator>>(
+        pybind11::class_<routingblocks::InsertStationOperator>(
             m, "InsertStationOperator", operator_interface,
             "Considers station insertions between consecutive vertices.")
             .def(pybind11::init<const Instance&>())
             .def("prepare_search", &routingblocks::InsertStationOperator::prepare_search)
             .def("find_next_improving_move",
                  &routingblocks::InsertStationOperator::find_next_improving_move)
             .def("finalize_search", &routingblocks::InsertStationOperator::finalize_search);
 
-        pybind11::class_<routingblocks::InsertStationMove,
-                         std::shared_ptr<routingblocks::InsertStationMove>>(
-            m, "StationInsertionMove", move_interface)
+        pybind11::class_<routingblocks::InsertStationMove>(m, "StationInsertionMove",
+                                                           move_interface)
             .def(pybind11::init<NodeLocation, VertexID>())
             .def("get_cost_delta", &routingblocks::InsertStationMove::get_cost_delta)
             .def("apply", &routingblocks::InsertStationMove::apply);
     }
 
     void bind_station_out_operator(pybind11::module_& m, auto& operator_interface,
                                    auto& move_interface) {
-        pybind11::class_<routingblocks::RemoveStationOperator,
-                         std::shared_ptr<routingblocks::RemoveStationOperator>>(
+        pybind11::class_<routingblocks::RemoveStationOperator>(
             m, "RemoveStationOperator", operator_interface,
             "Considers station removals between consecutive vertices.")
             .def(pybind11::init<const Instance&>())
             .def("prepare_search", &routingblocks::RemoveStationOperator::prepare_search)
             .def("find_next_improving_move",
                  &routingblocks::RemoveStationOperator::find_next_improving_move)
             .def("finalize_search", &routingblocks::RemoveStationOperator::finalize_search);
 
-        pybind11::class_<routingblocks::RemoveStationMove,
-                         std::shared_ptr<routingblocks::RemoveStationMove>>(m, "StationRemovalMove",
-                                                                            move_interface)
+        pybind11::class_<routingblocks::RemoveStationMove>(m, "StationRemovalMove", move_interface)
             .def(pybind11::init<NodeLocation>())
             .def("get_cost_delta", &routingblocks::RemoveStationMove::get_cost_delta)
             .def("apply", &routingblocks::RemoveStationMove::apply);
     }
 
     void bind_arc_set(pybind11::module_& m) {
         pybind11::class_<utility::arc_set>(m, "ArcSet", "A set of arcs.")
```

### Comparing `routingblocks-0.1.8/bindings/src/Solution.cpp` & `routingblocks-0.1.9/bindings/src/Solution.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,16 @@
                 "Backward label at the node", pybind11::return_value_policy::reference_internal)
             .def_property_readonly("__str__", &routingblocks::Node::vertex_strid);
     }
 
     void bind_route(pybind11::module& m) {
         pybind11::class_<routingblocks::Route>(m, "Route")
             .def(pybind11::init<std::shared_ptr<Evaluation>, const Instance&>(),
-                 pybind11::keep_alive<1, 2>(), "Creates an empty route.")
+                 pybind11::keep_alive<1, 2>(), pybind11::keep_alive<1, 3>(),
+                 "Creates an empty route.")
             .def_property_readonly("cost", &routingblocks::Route::cost, "The cost of the route.")
             .def_property_readonly("cost_components", &routingblocks::Route::cost_components,
                                    "The cost components of the route.")
             .def_property_readonly("feasible", &routingblocks::Route::feasible,
                                    "Whether the route is feasible.")
             .def_property_readonly("empty", &routingblocks::Route::empty,
                                    "Whether the route is empty.")
@@ -159,15 +160,15 @@
                  })
             .def("update", pybind11::overload_cast<>(&routingblocks::Route::update),
                  "Updates the route.")
             .def("__eq__", &routingblocks::Route::operator==, "Whether the routes are equal.")
             .def("__ne__", &routingblocks::Route::operator!=, "Whether the routes are not equal.");
 
         m.def("create_route", &routingblocks::create_route_from_vector,
-              "Creates a route from the given vertices.");
+              "Creates a route from the given vertices.", pybind11::keep_alive<0, 3>{});
     }
 
     void bind_node_location(pybind11::module_& m) {
         pybind11::class_<routingblocks::NodeLocation>(m, "NodeLocation")
             .def(pybind11::init<unsigned int, unsigned int>())
             .def("__getitem__",
                  [](const routingblocks::NodeLocation& location, size_t pos) {
@@ -187,26 +188,35 @@
             .def("__eq__", &routingblocks::NodeLocation::operator==,
                  "Whether the node locations are equal.")
             .def("__ne__", &routingblocks::NodeLocation::operator!=,
                  "Whether the node locations are not equal.")
             .def("__lt__", &routingblocks::NodeLocation::operator<,
                  "Whether the node locations compare lexicographically smaller. Route index is "
                  "ordered before node position.")
+            .def("__copy__",
+                 [](const routingblocks::NodeLocation& location) {
+                     return routingblocks::NodeLocation(location);
+                 })
+            .def("__deepcopy__",
+                 [](const routingblocks::NodeLocation& location, pybind11::dict) {
+                     return routingblocks::NodeLocation(location);
+                 })
             .def("__str__", ::bindings::helpers::ostream_to_string<routingblocks::NodeLocation>)
             .def("__repr__", ::bindings::helpers::ostream_to_string<routingblocks::NodeLocation>);
     }
 
     void bind_solution(pybind11::module_& m) {
         bind_node_location(m);
 
         pybind11::class_<routingblocks::Solution>(m, "Solution")
             .def(pybind11::init<std::shared_ptr<Evaluation>, const Instance&, size_t>(),
-                 "Creates an empty solution with the specified number of routes.")
+                 "Creates an empty solution with the specified number of routes.",
+                 pybind11::keep_alive<1, 3>())
             .def(pybind11::init<std::shared_ptr<Evaluation>, const Instance&, std::vector<Route>>(),
-                 "Creates a solution from the specified routes.")
+                 "Creates a solution from the specified routes.", pybind11::keep_alive<1, 3>())
             .def_property_readonly("cost", &routingblocks::Solution::cost,
                                    "The cost of the solution.")
             .def_property_readonly("cost_components", &routingblocks::Solution::cost_components,
                                    "The cost components of the solution.")
             .def_property_readonly("feasible", &routingblocks::Solution::feasible,
                                    "Whether the solution is "
                                    "feasible.")
```

### Comparing `routingblocks-0.1.8/bindings/src/bindings.cpp` & `routingblocks-0.1.9/bindings/src/bindings.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/bindings/src/large_neighborhood.cpp` & `routingblocks-0.1.9/bindings/src/large_neighborhood.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -7,41 +7,37 @@
 #include <routingblocks/adaptive_large_neighborhood.hpp>
 #include <routingblocks_bindings/binding_helpers.hpp>
 
 /*
  * Couple the lifetime of objects created in python to the shared_ptr lifetime in c++.
  */
 
-BIND_LIFETIME_PYTHON(routingblocks::repair_operator, "RepairOperator")
-BIND_LIFETIME_PYTHON(routingblocks::destroy_operator, "DestroyOperator")
-
 namespace routingblocks::bindings {
 
     class py_repair_operator : public routingblocks::repair_operator {
       public:
         using routingblocks::repair_operator::repair_operator;
 
         void apply(Evaluation& evaluation, Solution& sol,
                    const std::vector<routingblocks::VertexID>& missing_vertices) override {
-            PYBIND11_OVERRIDE_PURE(void, routingblocks::repair_operator, apply, evaluation, sol,
+            PYBIND11_OVERRIDE_PURE(void, routingblocks::repair_operator, apply, &evaluation, &sol,
                                    missing_vertices);
         }
         std::string_view name() const override {
             PYBIND11_OVERRIDE_PURE(std::string_view, routingblocks::repair_operator, name, );
         }
 
         bool can_apply_to(const routingblocks::Solution& sol) const override {
-            PYBIND11_OVERRIDE_PURE(bool, routingblocks::repair_operator, can_apply_to, sol);
+            PYBIND11_OVERRIDE_PURE(bool, routingblocks::repair_operator, can_apply_to, &sol);
         }
     };
 
     auto bind_repair_operator_interface(pybind11::module_& m) {
-        return pybind11::class_<routingblocks::repair_operator, py_repair_operator,
-                                std::shared_ptr<routingblocks::repair_operator>>(m,
-                                                                                 "RepairOperator")
+        return pybind11::class_<routingblocks::repair_operator, py_repair_operator>(
+                   m, "RepairOperator")
             .def(pybind11::init<>())
             .def("apply", &routingblocks::repair_operator::apply,
                  "Apply the repair operator to the passed solution.")
             .def("name", &routingblocks::repair_operator::name,
                  "Returns the name of the repair operator.")
             .def("can_apply_to", &routingblocks::repair_operator::can_apply_to,
                  "Returns true if the repair operator can be applied to the passed solution. False "
@@ -52,56 +48,53 @@
       public:
         using routingblocks::destroy_operator::destroy_operator;
 
         std::vector<routingblocks::VertexID> apply(Evaluation& evaluation,
                                                    routingblocks::Solution& sol,
                                                    size_t numberOfRemovedCustomers) override {
             PYBIND11_OVERRIDE_PURE(std::vector<routingblocks::VertexID>,
-                                   routingblocks::destroy_operator, apply, evaluation, sol,
+                                   routingblocks::destroy_operator, apply, &evaluation, &sol,
                                    numberOfRemovedCustomers);
         }
         std::string_view name() const override {
             PYBIND11_OVERRIDE_PURE(std::string_view, routingblocks::destroy_operator, name, );
         }
 
         bool can_apply_to(const routingblocks::Solution& sol) const override {
-            PYBIND11_OVERRIDE_PURE(bool, routingblocks::destroy_operator, can_apply_to, sol);
+            PYBIND11_OVERRIDE_PURE(bool, routingblocks::destroy_operator, can_apply_to, &sol);
         };
     };
 
     auto bind_destroy_operator_interface(pybind11::module_& m) {
-        return pybind11::class_<routingblocks::destroy_operator, py_destroy_operator,
-                                std::shared_ptr<routingblocks::destroy_operator>>(m,
-                                                                                  "DestroyOperator")
+        return pybind11::class_<routingblocks::destroy_operator, py_destroy_operator>(
+                   m, "DestroyOperator")
             .def(pybind11::init<>())
             .def("apply", &routingblocks::destroy_operator::apply,
                  "Apply the destroy operator to the passed solution and return the id's of any "
                  "removed vertices. May contain the same vertex several times.")
             .def("name", &routingblocks::destroy_operator::name,
                  "Returns the name of the destroy operator.")
             .def("can_apply_to", &routingblocks::destroy_operator::can_apply_to,
                  "Returns true if the destroy operator can be applied to the passed solution. "
                  "False otherwise.");
     }
 
     auto bind_random_destory_operator(pybind11::module_& m, auto& interface) {
         using _operator = routingblocks::lns::operators::RandomRemoval;
-        return pybind11::class_<_operator, std::shared_ptr<_operator>>(m, "RandomRemovalOperator",
-                                                                       interface)
+        return pybind11::class_<_operator>(m, "RandomRemovalOperator", interface)
             .def(pybind11::init<routingblocks::utility::random&>())
             .def("apply", &_operator::apply, "Remove random vertices from the solution.")
             .def("name", &_operator::name)
             .def("can_apply_to", &_operator::can_apply_to,
                  "Returns true. Random remove is always possible.");
     }
 
     void bind_random_insertion_operator(pybind11::module_& m, auto& interface) {
         using _operator = routingblocks::lns::operators::RandomInsertion;
-        pybind11::class_<_operator, std::shared_ptr<_operator>>(m, "RandomInsertionOperator",
-                                                                interface)
+        pybind11::class_<_operator>(m, "RandomInsertionOperator", interface)
             .def(pybind11::init<routingblocks::utility::random&>())
             .def("apply", &_operator ::apply,
                  "Inserts the passed vertices in order at random locations.")
             .def("name", &_operator ::name)
             .def("can_apply_to", &_operator ::can_apply_to,
                  "Return true: random insertion is always possible.");
     }
```

### Comparing `routingblocks-0.1.8/bindings/src/specializations/ADPTW.cpp` & `routingblocks-0.1.9/bindings/src/specializations/ADPTW.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 #include "routingblocks/ADPTWEvaluation.h"
 #include "routingblocks_bindings/binding_helpers.hpp"
 
 namespace routingblocks::bindings {
 
     void bind_adptw(pybind11::module_& m) {
         ::bindings::helpers::bind_concatenation_evaluation_specialization<ADPTWEvaluation>(
-            pybind11::class_<ADPTWEvaluation, std::shared_ptr<ADPTWEvaluation>, Evaluation>(
-                m, "ADPTWEvaluation")
+            pybind11::class_<ADPTWEvaluation, Evaluation>(m, "ADPTWEvaluation")
                 .def(pybind11::init<resource_t, resource_t>()))
             .def_readwrite("overload_penalty_factor", &ADPTWEvaluation::overload_penalty_factor)
             .def_readwrite("overcharge_penalty_factor", &ADPTWEvaluation::overcharge_penalty_factor)
             .def_readwrite("time_shift_penalty_factor",
                            &ADPTWEvaluation::time_shift_penalty_factor);
 
         pybind11::class_<routingblocks::ADPTWVertexData>(m, "ADPTWVertexData")
```

### Comparing `routingblocks-0.1.8/bindings/src/specializations/NIFTW.cpp` & `routingblocks-0.1.9/bindings/src/specializations/NIFTW.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 #include "routingblocks/NIFTWEvaluation.h"
 #include "routingblocks_bindings/binding_helpers.hpp"
 
 namespace routingblocks::bindings {
 
     void bind_niftw(pybind11::module_& m) {
         ::bindings::helpers::bind_concatenation_evaluation_specialization<NIFTWEvaluation>(
-            pybind11::class_<routingblocks::NIFTWEvaluation, std::shared_ptr<NIFTWEvaluation>,
-                             Evaluation>(m, "NIFTWEvaluation")
+            pybind11::class_<routingblocks::NIFTWEvaluation, Evaluation>(m, "NIFTWEvaluation")
                 .def(pybind11::init<resource_t, resource_t, resource_t>()))
             .def_readwrite("overload_penalty_factor", &NIFTWEvaluation::overload_penalty_factor)
             .def_readwrite("overcharge_penalty_factor", &NIFTWEvaluation::overcharge_penalty_factor)
             .def_readwrite("time_shift_penalty_factor",
                            &NIFTWEvaluation::time_shift_penalty_factor);
 
         pybind11::class_<routingblocks::NIFTWVertexData>(m, "NIFTWVertexData")
```

### Comparing `routingblocks-0.1.8/bindings/src/utility.cpp` & `routingblocks-0.1.9/bindings/src/utility.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/bindings/stubs/_adptw.pyi` & `routingblocks-0.1.9/bindings/stubs/_adptw.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -75,18 +75,16 @@
 
     overload_penalty_factor: float
     overcharge_penalty_factor: float
     time_shift_penalty_factor: float
 
     def __init__(self, vehicle_battery_capacity: float, vehicle_storage_capacity: float) -> None:
         """
-        Creates an ADPTW evaluation.
-
-        :param vehicle_battery_capacity: The vehicle's battery capacity expressed in units of time, that is, the time it takes to fully recharge an empty battery.
-        :param vehicle_storage_capacity: The vehicle's storage capacity. Determines how much demand can be served in a single route.
+        :param float vehicle_battery_capacity: The vehicle's battery capacity expressed in units of time, that is, the time it takes to fully recharge an empty battery.
+        :param float vehicle_storage_capacity: The vehicle's storage capacity. Determines how much demand can be served in a single route.
         """
         ...
 
 
 class ADPTWFRVCP:
     def __init__(self, instance: Instance, battery_capacity_time: float) -> None: ...
```

### Comparing `routingblocks-0.1.8/bindings/stubs/_alns.pyi` & `routingblocks-0.1.9/bindings/stubs/_alns.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/bindings/stubs/_arc.pyi` & `routingblocks-0.1.9/bindings/stubs/_arc.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -6,16 +6,14 @@
     A simple arc object that represents a connection between two vertices in a graph. The arc stores additional data
     transparent to the RoutingBlocks package. This data can be used to store additional information about the arc, such as
     distances, durations, or any other attributes relevant to the problem being modeled.
     """
 
     def __init__(self, data: Any) -> None:
         """
-        Initializes a new Arc object.
-
         :param data: Additional data associated with the arc.
         """
         ...
 
     @property
     def data(self) -> Any:
         """
```

### Comparing `routingblocks-0.1.8/bindings/stubs/_evaluation.pyi` & `routingblocks-0.1.9/bindings/stubs/_evaluation.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/bindings/stubs/_frvcp.pyi` & `routingblocks-0.1.9/bindings/stubs/_frvcp.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/bindings/stubs/_insertion_cache.pyi` & `routingblocks-0.1.9/bindings/stubs/_insertion_cache.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/bindings/stubs/_instance.pyi` & `routingblocks-0.1.9/bindings/stubs/_instance.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -11,28 +11,38 @@
         It is recommend to use the :ref:`InstanceBuilder <instance-builder>` to create instances.
 
     """
 
     @overload
     def __init__(self, depot: Vertex, stations: List[Vertex], customers: List[Vertex], arcs: List[List[Arc]],
                  fleet_size: int) -> None:
-        """Initialize an Instance with a depot, lists of stations and customers, a list of arcs, and a fleet size."""
+        """
+        :param Vertex depot: The depot vertex
+        :param List[Vertex] stations: A list of station vertices
+        :param List[Vertex] customers: A list of customer vertices
+        :param List[List[Arc]]] arcs: A matrix of Arc objects representing the connections between vertices
+        :param int fleet_size: The number of vehicles in the fleet
+        """
         ...
 
     @overload
     def __init__(self, vertices: List[Vertex], arcs: List[List[Arc]]) -> None:
-        """Initialize an Instance with a list of vertices and a list of arcs. Sets the fleet size to the number of customers.
-        Expects vertices to be in the order depot, stations, customers
-        ."""
+        """
+        :param List[Vertex] vertices: A list of vertices in the order depot, stations, customers
+        :param List[List[Arc]] arcs: A list of lists of Arc objects representing the connections between vertices
+        """
         ...
 
     @overload
     def __init__(self, vertices: List[Vertex], arcs: List[List[Arc]], fleet_size: int) -> None:
-        """Initialize an Instance with a list of vertices, a list of arcs, and a fleet size. Expects vertices to be in the
-        order depot, stations, customers."""
+        """
+        :param List[Vertex] vertices: A list of vertices in the order depot, stations, customers
+        :param List[List[Arc]] arcs: A list of lists of Arc objects representing the connections between vertices
+        :param int fleet_size: The number of vehicles in the fleet
+        """
         ...
 
     @property
     def fleet_size(self) -> int:
         """
         Retrieves the number of vehicles available.
```

### Comparing `routingblocks-0.1.8/bindings/stubs/_local_search.pyi` & `routingblocks-0.1.9/bindings/stubs/_local_search.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -71,23 +71,24 @@
     def finalize_search(self) -> None:
         """
         Called after the search for improving moves has been completed.
         """
         ...
 
     def find_next_improving_move(self, evaluation: Evaluation, solution: Solution,
-                                 last_evaluated_move: Move) -> Move:
+                                 last_evaluated_move: Optional[Move]) -> Optional[Move]:
         """
         Finds the next improving move. Returns None if no improving move is found.
         To avoid looping forever, this method should pick up the search where it left off, i.e., at last_evaluated_move.
 
         :param Evaluation evaluation: The evaluation function to use.
         :param Solution solution: The solution to be improved.
-        :param Move last_evaluated_move: The last move that was evaluated. Note that this corresponds to the last Move this operator returned. None if no move has been evaluated yet.
+        :param Optional[Move] last_evaluated_move: The last move that was evaluated. Note that this corresponds to the last Move this operator returned. None if no move has been evaluated yet.
         :return: The next improving move. None if no improving move is found.
+        :rtype: Optional[Move]
         """
         ...
 
     def prepare_search(self, solution: Solution) -> None:
         """
         Called before the search for improving moves is started.
 
@@ -134,19 +135,19 @@
     ...
 
 
 class KBestImprovementPivotingRule(PivotingRule):
     """
     The k - best improvement pivoting rule selects best out of the first k improving moves found during the search
     for improving moves. It terminates the search as soon as the k - th improving move is found.
+
     """
 
     def __init__(self, k: int) -> None:
         """
-        Configures the number of improving moves to consider.
         :param int k: The number of improving moves to consider.
         """
         ...
 
 
 class FirstImprovementPivotingRule(PivotingRule):
     """
```

### Comparing `routingblocks-0.1.8/bindings/stubs/_niftw.pyi` & `routingblocks-0.1.9/bindings/stubs/_niftw.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,14 @@
     overload_penalty_factor: float
     overcharge_penalty_factor: float
     time_shift_penalty_factor: float
 
     def __init__(self, vehicle_battery_capacity: float, vehicle_storage_capacity: float,
                  replenishment_time: float) -> None:
         """
-        Creates an NIFTW evaluation.
-
         :param vehicle_battery_capacity: The vehicle's battery capacity expressed in units of time, that is, the time it takes to fully recharge an empty battery.
         :param vehicle_storage_capacity: The vehicle's storage capacity. Determines how much demand can be served in a single route.
         :param replenishment_time: The time penalty incurred to replenish the vehicle's battery.
         """
         ...
```

### Comparing `routingblocks-0.1.8/bindings/stubs/_node.pyi` & `routingblocks-0.1.9/bindings/stubs/_node.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,14 @@
     A node represents a visit to a vertex.
     It carries forward and backward labels that are used for cost calculation, constraint checking, and efficient move evaluation.
     The data itself is opaque to the node class, and is only used by the evaluation object.
     """
 
     def __init__(self, vertex: Vertex, fwd_label: AnyForwardLabel, bwd_label: AnyBackwardLabel) -> None:
         """
-        Initializes a new Node object.
-
         :param Vertex vertex: The associated Vertex object.
         :param AnyForwardLabel fwd_label: The forward label for the node.
         :param AnyBackwardLabel bwd_label: The backward label for the node.
         """
         ...
 
     def cost(self, evaluation: Evaluation) -> float:
```

### Comparing `routingblocks-0.1.8/bindings/stubs/_node_location.pyi` & `routingblocks-0.1.9/bindings/stubs/_node_location.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 class NodeLocation:
     """
     A class representing the location of a node within a solution. Stores the route index and the position of the node within that route.
-    
-    :ivar int route: The index of the route in which the node is located.
-    :ivar int position: The position of the node within the route.
     """
     route: int
     position: int
 
-    def __init__(self, route: int, position: int) -> None: ...
+    def __init__(self, route: int, position: int) -> None:
+        """
+        :param int route: The index of the route in which the node is located.
+        :param int position: The position of the node within the route.
+        """
+        ...
 
     def __eq__(self, other: NodeLocation) -> bool: ...
 
     def __getitem__(self, i: int) -> int: ...
 
     def __len__(self) -> int: ...
```

### Comparing `routingblocks-0.1.8/bindings/stubs/_removal_cache.pyi` & `routingblocks-0.1.9/bindings/stubs/_removal_cache.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/bindings/stubs/_route.pyi` & `routingblocks-0.1.9/bindings/stubs/_route.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from typing import Iterable, Tuple
 
 
 class Route:
     """
     Routes represent a sequence of visits to vertices, represented by Node objects.
     A route starts and ends at the depot.
@@ -19,15 +18,15 @@
     Routes carry a globally unique modification timestamp which can be used to efficiently test two routes for equality:
     On each modification of the route, the modification timestamp is incremented, while copying a route preserves it's timestamp.
     Hence, two routes with the same modification timestamp are guaranteed to be equal, although the converse does not necessarily apply.
     """
 
     def __init__(self, evaluation: Evaluation, instance: Instance) -> None:
         """
-        Initializes a new Route object. The route is initially empty, that is, contains only start and end depots.
+        The route constructor creates an empty route, that is, a route that contains only start and end depots.
         Refer to create_route for a method to create a route from a sequence of vertex ids.
 
         :param Evaluation evaluation: The Evaluation object used for cost and feasibility calculations.
         :param Instance instance: The Instance object representing the problem instance.
         """
         ...
```

### Comparing `routingblocks-0.1.8/bindings/stubs/_solution.pyi` & `routingblocks-0.1.9/bindings/stubs/_solution.pyi`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/bindings/stubs/_vertex.pyi` & `routingblocks-0.1.9/bindings/stubs/_vertex.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -3,29 +3,22 @@
 
 class Vertex:
     """
     A simple vertex object that represents a location vehicles can visit. Vertices can be stations, depots or customers.
     Each vertex has a unique id and a human-readable string identifier. The vertex also stores additional data transparent
     to the RoutingBlocks package. This data can be used to store additional information about the vertex, such as time windows,
     demand, prizes, or any other attribute that is relevant to the problem.
-
-    :ivar vertex_id: The unique identifier of the vertex.
-    :ivar str_id: A human-readable string identifier for the vertex.
-    :ivar is_station: Whether the vertex is a station.
-    :ivar is_depot: Whether the vertex is a depot.
     """
-    vertex_id: int
+    vertex_id: int  # The unique identifier of the vertex.
     str_id: str
     is_station: bool
     is_depot: bool
 
     def __init__(self, vertex_id: int, str_id: str, is_station: bool, is_depot: bool, data: Any) -> None:
         """
-        Initializes a new Vertex object.
-
         :param vertex_id: The unique identifier of the vertex.
         :param str_id: A human-readable string identifier for the vertex.
         :param is_station: Whether the vertex is a station.
         :param is_depot: Whether the vertex is a depot.
         :param data: Additional data associated with the vertex.
         """
         ...
```

### Comparing `routingblocks-0.1.8/docs/make.bat` & `routingblocks-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/docs/source/alns.rst` & `routingblocks-0.1.9/docs/source/alns.rst`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/docs/source/auxilliary.rst` & `routingblocks-0.1.9/docs/source/auxilliary.rst`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/docs/source/conf.py` & `routingblocks-0.1.9/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 autoapi_dirs = [str(routingblocks_import_path)]
 autoapi_options = ["undoc-members", "members", "special-members"]
 
 autoapi_generate_api_docs = False
 autoapi_add_toctree_entry = False
 autoapi_add_objects_to_toctree = False
 
-autoapi_python_class_content = "class"
+autoapi_python_class_content = "both"
 autoapi_member_order = "bysource"
 autodoc_member_order = "bysource"
 
 autodoc_typehints = "both"
 
 # Bibtex
 bibtex_bibfiles = ['references.bib']
```

### Comparing `routingblocks-0.1.8/docs/source/development.rst` & `routingblocks-0.1.9/docs/source/development.rst`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/docs/source/evaluation.rst` & `routingblocks-0.1.9/docs/source/evaluation.rst`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/docs/source/getting_started.rst` & `routingblocks-0.1.9/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/docs/source/index.rst` & `routingblocks-0.1.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/docs/source/instance.rst` & `routingblocks-0.1.9/docs/source/instance.rst`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     :members:
     :undoc-members:
 
 .. autoapiclass:: routingblocks.Instance
     :members:
     :undoc-members:
     :special-members: __len__, __iter__
+    :class-doc-from: class
 
     .. py:method:: __init__(self, depot: Vertex, stations: List[Vertex], customers: List[Vertex], arcs: List[List[Arc]], fleet_size: int) -> None
 
           Initialize an Instance with a depot, lists of stations and customers, a list of arcs, and a fleet size.
 
           :param Vertex depot: The depot vertex
           :param List[Vertex] stations: A list of station vertices
```

### Comparing `routingblocks-0.1.8/docs/source/references.bib` & `routingblocks-0.1.9/docs/source/references.bib`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/docs/source/solution.rst` & `routingblocks-0.1.9/docs/source/solution.rst`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 .. autoapiclass:: routingblocks.Route
     :members:
     :undoc-members:
 
 .. autoapiclass:: routingblocks.Solution
     :members:
     :undoc-members:
+    :class-doc-from: class
     :special-members: __len__, __iter__, __getitem__, __delitem__
 
     .. py:method:: __init__(self, evaluation: Evaluation, instance: Instance, number_of_routes: int)
 
         Creates a new Solution object with the specified number of empty routes.
 
         :param Evaluation evaluation: The evaluation object for cost and feasibility calculations.
```

### Comparing `routingblocks-0.1.8/examples/README.md` & `routingblocks-0.1.9/examples/README.md`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/alns/__main__.py` & `routingblocks-0.1.9/examples/alns/__main__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/alns/alns.py` & `routingblocks-0.1.9/examples/alns/alns.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/alns/parsing.py` & `routingblocks-0.1.9/examples/alns/parsing.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/__main__.py` & `routingblocks-0.1.9/examples/evrptw/__main__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/alns.py` & `routingblocks-0.1.9/examples/evrptw/alns.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/config.json` & `routingblocks-0.1.9/examples/evrptw/config.json`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instance/interface.py` & `routingblocks-0.1.9/examples/evrptw/instance/interface.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instance/models.py` & `routingblocks-0.1.9/examples/evrptw/instance/models.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instance/parsing.py` & `routingblocks-0.1.9/examples/evrptw/instance/parsing.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/c101C10.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/c101C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/c104C10.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/c104C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/c202C10.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/c202C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/c205C10.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/c205C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/r102C10.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/r102C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/r103C10.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/r103C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/r201C10.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/r201C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/r203C10.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/r203C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/rc102C10.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/rc102C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/rc108C10.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/rc108C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/rc201C10.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/rc201C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/10/rc205C10.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/10/rc205C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c101_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c102_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c102_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c103_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c103_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c104_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c104_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c105_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c105_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c106_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c106_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c107_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c107_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c108_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c108_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c109_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c109_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c201_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c202_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c202_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c203_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c203_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c204_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c204_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c205_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c205_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c206_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c206_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c207_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c207_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/c208_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/c208_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r101_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r102_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r102_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r103_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r103_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r104_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r104_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r105_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r105_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r106_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r106_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r107_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r107_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r108_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r108_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r109_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r109_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r110_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r110_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r111_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r111_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r112_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r112_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r201_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r202_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r202_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r203_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r203_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r204_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r204_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r205_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r205_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r206_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r206_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r207_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r207_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r208_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r208_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r209_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r209_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r210_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r210_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/r211_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/r211_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc101_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc102_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc102_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc103_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc103_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc104_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc104_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc105_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc105_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc106_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc106_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc107_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc107_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc108_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc108_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc201_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc202_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc202_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc203_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc203_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc204_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc204_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc205_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc205_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc206_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc206_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc207_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc207_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/100/rc208_21.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/100/rc208_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/c103C15.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/c103C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/c106C15.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/c106C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/c202C15.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/c202C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/c208C15.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/c208C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/r102C15.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/r102C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/r105C15.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/r105C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/r202C15.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/r202C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/r209C15.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/r209C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/rc103C15.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/rc103C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/rc108C15.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/rc108C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/rc202C15.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/rc202C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/15/rc204C15.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/15/rc204C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/c101C5.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/c101C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/c103C5.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/c103C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/c206C5.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/c206C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/c208C5.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/c208C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/r104C5.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/r104C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/r105C5.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/r105C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/r202C5.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/r202C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/r203C5.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/r203C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/rc105C5.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/rc105C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/rc108C5.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/rc108C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/rc204C5.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/rc204C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/5/rc208C5.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/5/rc208C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/instances/evrptw/README.txt` & `routingblocks-0.1.9/examples/evrptw/instances/evrptw/README.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/operators/ShawMoveSelector.py` & `routingblocks-0.1.9/examples/evrptw/operators/ShawMoveSelector.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/operators/ShawRelatedness.py` & `routingblocks-0.1.9/examples/evrptw/operators/ShawRelatedness.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/operators/SpatioTemporalRelatedness.py` & `routingblocks-0.1.9/examples/evrptw/operators/SpatioTemporalRelatedness.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/operators/__init__.py` & `routingblocks-0.1.9/examples/evrptw/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/evrptw/parameters.py` & `routingblocks-0.1.9/examples/evrptw/parameters.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/ils/__main__.py` & `routingblocks-0.1.9/examples/ils/__main__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/ils/ils.py` & `routingblocks-0.1.9/examples/ils/ils.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/examples/ils/parsing.py` & `routingblocks-0.1.9/examples/ils/parsing.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/CMakeLists.txt` & `routingblocks-0.1.9/native/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/cmake/CPM.cmake` & `routingblocks-0.1.9/bindings/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/cmake/tools.cmake` & `routingblocks-0.1.9/native/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/ADPTWEvaluation.h` & `routingblocks-0.1.9/native/include/routingblocks/ADPTWEvaluation.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/FRVCP.h` & `routingblocks-0.1.9/native/include/routingblocks/FRVCP.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/Instance.h` & `routingblocks-0.1.9/native/include/routingblocks/Instance.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/LocalSearch.h` & `routingblocks-0.1.9/native/include/routingblocks/LocalSearch.h`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         Solution::const_iterator origin_route;
         Solution::route_t::const_iterator origin_node;
 
         Solution::const_iterator target_route;
         Solution::route_t::const_iterator target_node;
     };
 
-    class Move {
+    class Move : public std::enable_shared_from_this<Move> {
       public:
         [[nodiscard]] virtual cost_t get_cost_delta(Evaluation& evaluation,
                                                     const Instance& instance,
                                                     const Solution& solution) const
             = 0;
         virtual void apply(const Instance& instance, Solution& solution) const = 0;
         virtual ~Move() = default;
```

### Comparing `routingblocks-0.1.8/native/include/routingblocks/NIFTWEvaluation.h` & `routingblocks-0.1.9/native/include/routingblocks/NIFTWEvaluation.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/Solution.h` & `routingblocks-0.1.9/native/include/routingblocks/Solution.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/adaptive_large_neighborhood.hpp` & `routingblocks-0.1.9/native/include/routingblocks/adaptive_large_neighborhood.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/arc.h` & `routingblocks-0.1.9/native/include/routingblocks/arc.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/evaluation.h` & `routingblocks-0.1.9/native/include/routingblocks/evaluation.h`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #include <memory>
 #include <span>
 #include <vector>
 
 namespace routingblocks {
 
-    class Evaluation : public std::enable_shared_from_this<Evaluation> {
+    class Evaluation {
       public:
         using label_holder_t = Node::label_holder_t;
 
         virtual cost_t evaluate(const Instance& instance, std::span<const route_segment> segments)
             = 0;
 
         [[nodiscard]] virtual cost_t compute_cost(const label_holder_t& label) const = 0;
```

### Comparing `routingblocks-0.1.8/native/include/routingblocks/insertion_cache.h` & `routingblocks-0.1.9/native/include/routingblocks/insertion_cache.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/lns_operators.h` & `routingblocks-0.1.9/native/include/routingblocks/lns_operators.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/node.h` & `routingblocks-0.1.9/native/include/routingblocks/node.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/operators/InsertStationOperator.h` & `routingblocks-0.1.9/native/include/routingblocks/operators/InsertStationOperator.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/operators/InterRouteTwoOptOperator.h` & `routingblocks-0.1.9/native/include/routingblocks/operators/InterRouteTwoOptOperator.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/operators/RemoveStationOperator.h` & `routingblocks-0.1.9/native/include/routingblocks/operators/RemoveStationOperator.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/operators/SwapOperator.h` & `routingblocks-0.1.9/native/include/routingblocks/operators/SwapOperator.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/operators.h` & `routingblocks-0.1.9/native/include/routingblocks/operators.h`

 * *Files 19% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 namespace routingblocks {
 
     class Solution;
 
     /**
      * \brief Destory Operator interface
      */
-    class destroy_operator : public std::enable_shared_from_this<destroy_operator> {
+    class destroy_operator {
       public:
         /**
          * Applies the operator to the passed solution.
          */
         virtual std::vector<routingblocks::VertexID> apply(routingblocks::Evaluation& evaluation,
                                                            routingblocks::Solution& sol,
                                                            size_t numberOfRemovedCustomers)
@@ -35,15 +35,15 @@
 
         virtual ~destroy_operator() = default;
     };
 
     /**
      * \brief Destory Operator interface
      */
-    class repair_operator : public std::enable_shared_from_this<repair_operator> {
+    class repair_operator {
       public:
         /**
          * Applies the operator to the passed solution.
          */
         virtual void apply(routingblocks::Evaluation& evaluation, routingblocks::Solution& sol,
                            const std::vector<routingblocks::VertexID>& missing_vertices)
             = 0;
```

### Comparing `routingblocks-0.1.8/native/include/routingblocks/removal_cache.h` & `routingblocks-0.1.9/native/include/routingblocks/removal_cache.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/utility/adaptive_priority_list.h` & `routingblocks-0.1.9/native/include/routingblocks/utility/adaptive_priority_list.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/utility/algorithms.h` & `routingblocks-0.1.9/native/include/routingblocks/utility/algorithms.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/utility/arc_set.h` & `routingblocks-0.1.9/native/include/routingblocks/utility/arc_set.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/utility/heap.h` & `routingblocks-0.1.9/native/include/routingblocks/utility/heap.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/utility/iterator_pair.h` & `routingblocks-0.1.9/native/include/routingblocks/utility/iterator_pair.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/utility/random.h` & `routingblocks-0.1.9/native/include/routingblocks/utility/random.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/include/routingblocks/vertex.h` & `routingblocks-0.1.9/native/include/routingblocks/vertex.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/lib/dynamic_bitset/LICENSE.txt` & `routingblocks-0.1.9/native/lib/dynamic_bitset/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp` & `routingblocks-0.1.9/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h` & `routingblocks-0.1.9/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/lib/small_vector/LICENSE.txt` & `routingblocks-0.1.9/native/lib/small_vector/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/lib/small_vector/small_vector/small_vector.hpp` & `routingblocks-0.1.9/native/lib/small_vector/small_vector/small_vector.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/lib/xoshiro/LICENSE.txt` & `routingblocks-0.1.9/native/lib/xoshiro/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/lib/xoshiro/xoshiro/xoshiro.h` & `routingblocks-0.1.9/native/lib/xoshiro/xoshiro/xoshiro.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/src/ADPTWEvaluation.cpp` & `routingblocks-0.1.9/native/src/ADPTWEvaluation.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/src/Instance.cpp` & `routingblocks-0.1.9/native/src/Instance.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/src/LocalSearch.cpp` & `routingblocks-0.1.9/native/src/LocalSearch.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/src/NIFTWEvaluation.cpp` & `routingblocks-0.1.9/native/src/NIFTWEvaluation.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/src/Solution.cpp` & `routingblocks-0.1.9/native/src/Solution.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/src/lns_operators.cpp` & `routingblocks-0.1.9/native/src/lns_operators.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/src/node.cpp` & `routingblocks-0.1.9/native/src/node.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/src/operators/InsertStationOperator.cpp` & `routingblocks-0.1.9/native/src/operators/InsertStationOperator.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/src/operators/InterRouteTwoOptOperator.cpp` & `routingblocks-0.1.9/native/src/operators/InterRouteTwoOptOperator.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/native/test/CMakeLists.txt` & `routingblocks-0.1.9/native/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/pyproject.toml` & `routingblocks-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
-requires = ["scikit-build-core>=0.2.1", "pybind11"]
+requires = ["scikit-build-core>=0.2.1"]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "RoutingBlocks"
-version = "0.1.8"
+version = "0.1.9"
 description = "A package for the implementation of vehicle routing problems with intermediate stops"
 readme = "README.md"
 authors = [
     { name = "Patrick Sean Klein", email = "patrick.sean.klein@tum.de" },
 ]
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `routingblocks-0.1.8/routingblocks/operators/__init__.py` & `routingblocks-0.1.9/routingblocks/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/routingblocks/operators/best_insert.py` & `routingblocks-0.1.9/routingblocks/operators/best_insert.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/routingblocks/operators/cluster_removal.py` & `routingblocks-0.1.9/routingblocks/operators/cluster_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/routingblocks/operators/move_selectors.py` & `routingblocks-0.1.9/routingblocks/operators/move_selectors.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/routingblocks/operators/related_removal.py` & `routingblocks-0.1.9/routingblocks/operators/related_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/routingblocks/operators/route_removal.py` & `routingblocks-0.1.9/routingblocks/operators/route_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/routingblocks/operators/station_vicinity_removal.py` & `routingblocks-0.1.9/routingblocks/operators/station_vicinity_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/routingblocks/operators/worst_removal.py` & `routingblocks-0.1.9/routingblocks/operators/worst_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/routingblocks/utility/instance_builder.py` & `routingblocks-0.1.9/routingblocks/utility/instance_builder.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/benchmarks/reference/insertion_cache.py` & `routingblocks-0.1.9/test/tests/benchmarks/reference/insertion_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/benchmarks/reference/removal_cache.py` & `routingblocks-0.1.9/test/tests/benchmarks/reference/removal_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/benchmarks/test_benchmark_frvcp.py` & `routingblocks-0.1.9/test/tests/benchmarks/test_benchmark_frvcp.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/benchmarks/test_benchmark_local_search.py` & `routingblocks-0.1.9/test/tests/benchmarks/test_benchmark_local_search.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/benchmarks/test_benchmark_removal_cache.py` & `routingblocks-0.1.9/test/tests/benchmarks/test_benchmark_removal_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/benchmarks/test_benchmark_route_update.py` & `routingblocks-0.1.9/test/tests/benchmarks/test_benchmark_route_update.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/fixtures/__init__.py` & `routingblocks-0.1.9/test/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/fixtures/data/c101C5.txt` & `routingblocks-0.1.9/test/tests/fixtures/data/c101C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/fixtures/data/c101_21.txt` & `routingblocks-0.1.9/test/tests/fixtures/data/c101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/fixtures/data/r101_21.txt` & `routingblocks-0.1.9/test/tests/fixtures/data/r101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/fixtures/data/r201_21.txt` & `routingblocks-0.1.9/test/tests/fixtures/data/r201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/fixtures/data/rc101_21.txt` & `routingblocks-0.1.9/test/tests/fixtures/data/rc101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/fixtures/mock_evaluation.py` & `routingblocks-0.1.9/test/tests/fixtures/mock_evaluation.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/helpers/interface.py` & `routingblocks-0.1.9/test/tests/helpers/interface.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/helpers/models.py` & `routingblocks-0.1.9/test/tests/helpers/models.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/helpers/parsing.py` & `routingblocks-0.1.9/test/tests/helpers/parsing.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/operators/test_cluster_removal.py` & `routingblocks-0.1.9/test/tests/operators/test_cluster_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/operators/test_random_insertion.py` & `routingblocks-0.1.9/test/tests/operators/test_random_insertion.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/operators/test_random_removal.py` & `routingblocks-0.1.9/test/tests/operators/test_random_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/operators/test_related_removal.py` & `routingblocks-0.1.9/test/tests/operators/test_related_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/operators/test_station_insertion.py` & `routingblocks-0.1.9/test/tests/operators/test_station_insertion.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/operators/test_station_removal.py` & `routingblocks-0.1.9/test/tests/operators/test_station_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/operators/test_station_vicinity_removal.py` & `routingblocks-0.1.9/test/tests/operators/test_station_vicinity_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/operators/test_swap.py` & `routingblocks-0.1.9/test/tests/operators/test_swap.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/test_evaluation.py` & `routingblocks-0.1.9/test/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/test_frvcp.py` & `routingblocks-0.1.9/test/tests/test_frvcp.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/test_insertion_cache.py` & `routingblocks-0.1.9/test/tests/test_insertion_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/test_large_neighborhood.py` & `routingblocks-0.1.9/test/tests/test_large_neighborhood.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,20 @@
 def test_large_neighborhood_custom_operators_lifetime(instance, random_solution_factory, mock_evaluation,
                                                       randgen: evrptw.Random):
     py_instance, instance = instance
     solution = random_solution_factory(instance, mock_evaluation)
     large_neighborhood = evrptw.AdaptiveLargeNeighborhood(randgen, 0.2)
 
     # Python frees the reference to Mock operators
-    large_neighborhood.add_destroy_operator(MockDestroyOperator(0))
-    large_neighborhood.add_repair_operator(MockRepairOperator(0))
+    destroy_op = MockDestroyOperator(0)
+    large_neighborhood.add_destroy_operator(destroy_op)
+    repair_op = MockRepairOperator(0)
+    large_neighborhood.add_repair_operator(repair_op)
+    del destroy_op
+    del repair_op
     # This should still work - the custom python object should still be valid
     large_neighborhood.generate(mock_evaluation, solution, 1)
 
 
 def test_large_neighborhood_remove(randgen):
     large_neighborhood = evrptw.AdaptiveLargeNeighborhood(randgen, 0.2)
```

### Comparing `routingblocks-0.1.8/test/tests/test_lns_helpers.py` & `routingblocks-0.1.9/test/tests/test_lns_helpers.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/test_node.py` & `routingblocks-0.1.9/test/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/test_removal_cache.py` & `routingblocks-0.1.9/test/tests/test_removal_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/test/tests/test_route.py` & `routingblocks-0.1.9/test/tests/test_route.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,28 @@
     expected_vertex_ids = [instance.depot.vertex_id, *vertex_ids, instance.depot.vertex_id]
     assert len(route) == len(expected_vertex_ids)
     assert [x.vertex_id for x in route] == expected_vertex_ids
     # Is updated?
     assert_updated(mock_evaluation, instance, route)
 
 
+def test_route_create_route_evaluation_lifetime(adptw_instance: evrptw.Instance):
+    instance = adptw_instance
+    vertex_ids = [x.vertex_id for x in instance.customers] + [x.vertex_id for x in instance.stations]
+    random.shuffle(vertex_ids)
+
+    evaluation = MockEvaluation()
+    route = evrptw.create_route(evaluation, instance, vertex_ids)
+    route.update()
+    del evaluation
+    del adptw_instance
+    # Should still work
+    route.update()
+
+
 def test_route_iterator(random_route):
     *_, route = random_route
     for i, node in enumerate(route):
         # Should not copy
         assert id(route[i]) == id(node)
```

### Comparing `routingblocks-0.1.8/test/tests/test_solution.py` & `routingblocks-0.1.9/test/tests/test_solution.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.8/PKG-INFO` & `routingblocks-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routingblocks
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for the implementation of vehicle routing problems with intermediate stops
 Author-Email: Patrick Sean Klein <patrick.sean.klein@tum.de>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


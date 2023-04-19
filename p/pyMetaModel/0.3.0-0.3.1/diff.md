# Comparing `tmp/pymetamodel-0.3.0.tar.gz` & `tmp/pymetamodel-0.3.1.tar.gz`

## Comparing `pymetamodel-0.3.0.tar` & `pymetamodel-0.3.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/.pydevproject
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.mermaid
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.puml
--rw-r--r--   0        0        0    16059 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.py
--rw-r--r--   0        0        0     8899 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.sidif
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.xlsx
--rw-r--r--   0        0        0     8799 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.yaml
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/ceur-ws/ceur-ws_puml.txt
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/city/city.mermaid
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/city/city.puml
--rw-r--r--   0        0        0     7910 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/city/city.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/city/city.sidif
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/city/city.xlsx
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/city/city.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/city/city_puml.txt
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/family/FamilyContext.mermaid
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/family/FamilyContext.puml
--rw-r--r--   0        0        0    21685 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/family/FamilyContext.py
--rw-r--r--   0        0        0     9723 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/family/FamilyContext.sidif
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/family/FamilyContext.xlsx
--rw-r--r--   0        0        0    10664 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/family/FamilyContext.yaml
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/family/FamilyContext_puml.txt
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/metamodel/metamodel.mermaid
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/metamodel/metamodel.puml
--rw-r--r--   0        0        0    43565 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/metamodel/metamodel.py
--rw-r--r--   0        0        0    36709 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/metamodel/metamodel.sidif
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/metamodel/metamodel.xlsx
--rw-r--r--   0        0        0    35205 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/metamodel/metamodel.yaml
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/metamodel/metamodel_puml.txt
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/scientific-events/scientific-events.mermaid
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/scientific-events/scientific-events.puml
--rw-r--r--   0        0        0    30338 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/scientific-events/scientific-events.py
--rw-r--r--   0        0        0    22450 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/scientific-events/scientific-events.sidif
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/scientific-events/scientific-events.xlsx
--rw-r--r--   0        0        0    19579 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/scientific-events/scientific-events.yaml
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/scientific-events/scientific-events_puml.txt
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/teaching/TeachingSchema.mermaid
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/teaching/TeachingSchema.puml
--rw-r--r--   0        0        0    45997 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/teaching/TeachingSchema.py
--rw-r--r--   0        0        0    31307 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/teaching/TeachingSchema.sidif
--rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/teaching/TeachingSchema.xlsx
--rw-r--r--   0        0        0    25078 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/teaching/TeachingSchema.yaml
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/examples/teaching/TeachingSchema_puml.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/__init__.py
--rw-r--r--   0        0        0    19028 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/metamodel.py
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/metamodel_cmd.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/mw.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/profiler.py
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/sidif2linkml.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/smw_type.py
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/uml.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/meta/version.py
--rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/scripts/genexamples
--rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/scripts/install
--rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/tests/basemwtest.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/tests/basetest.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/tests/test_linkml.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/tests/test_metamodel.py
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/tests/test_mw.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/tests/test_plantuml.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/tests/test_sidif.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/LICENSE
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/README.md
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    15893 2020-02-02 00:00:00.000000 pymetamodel-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/.pydevproject
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/ceur-ws/ceur-ws.mermaid
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/ceur-ws/ceur-ws.puml
+-rw-r--r--   0        0        0    16059 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/ceur-ws/ceur-ws.py
+-rw-r--r--   0        0        0     8899 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/ceur-ws/ceur-ws.sidif
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/ceur-ws/ceur-ws.xlsx
+-rw-r--r--   0        0        0     8799 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/ceur-ws/ceur-ws.yaml
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/ceur-ws/ceur-ws_puml.txt
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/city/city.mermaid
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/city/city.puml
+-rw-r--r--   0        0        0     7910 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/city/city.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/city/city.sidif
+-rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/city/city.xlsx
+-rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/city/city.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/city/city_puml.txt
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/family/FamilyContext.mermaid
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/family/FamilyContext.puml
+-rw-r--r--   0        0        0    21685 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/family/FamilyContext.py
+-rw-r--r--   0        0        0     9723 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/family/FamilyContext.sidif
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/family/FamilyContext.xlsx
+-rw-r--r--   0        0        0    10664 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/family/FamilyContext.yaml
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/family/FamilyContext_puml.txt
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/metamodel/metamodel.mermaid
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/metamodel/metamodel.puml
+-rw-r--r--   0        0        0    43565 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/metamodel/metamodel.py
+-rw-r--r--   0        0        0    36709 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/metamodel/metamodel.sidif
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/metamodel/metamodel.xlsx
+-rw-r--r--   0        0        0    35205 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/metamodel/metamodel.yaml
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/metamodel/metamodel_puml.txt
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/scientific-events/scientific-events.mermaid
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/scientific-events/scientific-events.puml
+-rw-r--r--   0        0        0    30338 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/scientific-events/scientific-events.py
+-rw-r--r--   0        0        0    22450 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/scientific-events/scientific-events.sidif
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/scientific-events/scientific-events.xlsx
+-rw-r--r--   0        0        0    19579 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/scientific-events/scientific-events.yaml
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/scientific-events/scientific-events_puml.txt
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/teaching/TeachingSchema.mermaid
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/teaching/TeachingSchema.puml
+-rw-r--r--   0        0        0    45997 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/teaching/TeachingSchema.py
+-rw-r--r--   0        0        0    31307 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/teaching/TeachingSchema.sidif
+-rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/teaching/TeachingSchema.xlsx
+-rw-r--r--   0        0        0    25078 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/teaching/TeachingSchema.yaml
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/examples/teaching/TeachingSchema_puml.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/meta/__init__.py
+-rw-r--r--   0        0        0    19051 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/meta/metamodel.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/meta/metamodel_cmd.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/meta/mw.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/meta/profiler.py
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/meta/sidif2linkml.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/meta/smw_type.py
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/meta/uml.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/meta/version.py
+-rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/scripts/genexamples
+-rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/scripts/install
+-rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/tests/basemwtest.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/tests/basetest.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/tests/test_linkml.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/tests/test_metamodel.py
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/tests/test_mw.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/tests/test_plantuml.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/tests/test_sidif.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/README.md
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    15893 2020-02-02 00:00:00.000000 pymetamodel-0.3.1/PKG-INFO
```

### Comparing `pymetamodel-0.3.0/.github/workflows/build.yml` & `pymetamodel-0.3.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/.github/workflows/upload-to-pypi.yml` & `pymetamodel-0.3.1/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.puml` & `pymetamodel-0.3.1/examples/ceur-ws/ceur-ws.puml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.py` & `pymetamodel-0.3.1/examples/ceur-ws/ceur-ws.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.sidif` & `pymetamodel-0.3.1/examples/ceur-ws/ceur-ws.sidif`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.xlsx` & `pymetamodel-0.3.1/examples/ceur-ws/ceur-ws.xlsx`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/ceur-ws/ceur-ws.yaml` & `pymetamodel-0.3.1/examples/ceur-ws/ceur-ws.yaml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/ceur-ws/ceur-ws_puml.txt` & `pymetamodel-0.3.1/examples/ceur-ws/ceur-ws_puml.txt`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/city/city.py` & `pymetamodel-0.3.1/examples/city/city.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/city/city.sidif` & `pymetamodel-0.3.1/examples/city/city.sidif`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/city/city.xlsx` & `pymetamodel-0.3.1/examples/city/city.xlsx`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/city/city.yaml` & `pymetamodel-0.3.1/examples/city/city.yaml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/family/FamilyContext.mermaid` & `pymetamodel-0.3.1/examples/family/FamilyContext.mermaid`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/family/FamilyContext.puml` & `pymetamodel-0.3.1/examples/family/FamilyContext.puml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/family/FamilyContext.py` & `pymetamodel-0.3.1/examples/family/FamilyContext.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/family/FamilyContext.sidif` & `pymetamodel-0.3.1/examples/family/FamilyContext.sidif`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/family/FamilyContext.xlsx` & `pymetamodel-0.3.1/examples/family/FamilyContext.xlsx`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/family/FamilyContext.yaml` & `pymetamodel-0.3.1/examples/family/FamilyContext.yaml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/family/FamilyContext_puml.txt` & `pymetamodel-0.3.1/examples/family/FamilyContext_puml.txt`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/metamodel/metamodel.mermaid` & `pymetamodel-0.3.1/examples/metamodel/metamodel.mermaid`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/metamodel/metamodel.puml` & `pymetamodel-0.3.1/examples/metamodel/metamodel.puml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/metamodel/metamodel.py` & `pymetamodel-0.3.1/examples/metamodel/metamodel.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/metamodel/metamodel.sidif` & `pymetamodel-0.3.1/examples/metamodel/metamodel.sidif`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/metamodel/metamodel.xlsx` & `pymetamodel-0.3.1/examples/metamodel/metamodel.xlsx`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/metamodel/metamodel.yaml` & `pymetamodel-0.3.1/examples/metamodel/metamodel.yaml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/metamodel/metamodel_puml.txt` & `pymetamodel-0.3.1/examples/metamodel/metamodel_puml.txt`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/scientific-events/scientific-events.mermaid` & `pymetamodel-0.3.1/examples/scientific-events/scientific-events.mermaid`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/scientific-events/scientific-events.puml` & `pymetamodel-0.3.1/examples/scientific-events/scientific-events.puml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/scientific-events/scientific-events.py` & `pymetamodel-0.3.1/examples/scientific-events/scientific-events.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/scientific-events/scientific-events.sidif` & `pymetamodel-0.3.1/examples/scientific-events/scientific-events.sidif`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/scientific-events/scientific-events.xlsx` & `pymetamodel-0.3.1/examples/scientific-events/scientific-events.xlsx`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/scientific-events/scientific-events.yaml` & `pymetamodel-0.3.1/examples/scientific-events/scientific-events.yaml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/scientific-events/scientific-events_puml.txt` & `pymetamodel-0.3.1/examples/scientific-events/scientific-events_puml.txt`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/teaching/TeachingSchema.mermaid` & `pymetamodel-0.3.1/examples/teaching/TeachingSchema.mermaid`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/teaching/TeachingSchema.puml` & `pymetamodel-0.3.1/examples/teaching/TeachingSchema.puml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/teaching/TeachingSchema.py` & `pymetamodel-0.3.1/examples/teaching/TeachingSchema.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/teaching/TeachingSchema.sidif` & `pymetamodel-0.3.1/examples/teaching/TeachingSchema.sidif`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/teaching/TeachingSchema.xlsx` & `pymetamodel-0.3.1/examples/teaching/TeachingSchema.xlsx`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/teaching/TeachingSchema.yaml` & `pymetamodel-0.3.1/examples/teaching/TeachingSchema.yaml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/examples/teaching/TeachingSchema_puml.txt` & `pymetamodel-0.3.1/examples/teaching/TeachingSchema_puml.txt`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/meta/metamodel.py` & `pymetamodel-0.3.1/meta/metamodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,14 +279,15 @@
             debug(bool): if True handle debugging
             
         Returns:
             Tuple[Context,str,str]: context, error and errorMessage
             
         """
         errMsg = None
+        context = None
         sp = SiDIFParser(debug=debug)
         parsed, error = sp.parseText(sidif, title,depth=depth)
         if debug:
             sp.printResult(parsed)
         if error is None:
             dif = parsed[0]
             did = dif.toDictOfDicts()
```

### Comparing `pymetamodel-0.3.0/meta/metamodel_cmd.py` & `pymetamodel-0.3.1/meta/metamodel_cmd.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/meta/mw.py` & `pymetamodel-0.3.1/meta/mw.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/meta/profiler.py` & `pymetamodel-0.3.1/meta/profiler.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/meta/sidif2linkml.py` & `pymetamodel-0.3.1/meta/sidif2linkml.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/meta/smw_type.py` & `pymetamodel-0.3.1/meta/smw_type.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/meta/uml.py` & `pymetamodel-0.3.1/meta/uml.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/meta/version.py` & `pymetamodel-0.3.1/meta/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     '''
     Version handling for pyMetaModel
     '''
     name="pyMetaModel"
     description='pyMetaModel: MetaModel for Knowledge Graphs'
     version=meta.__version__
     date = '2022-11-30'
-    updated = '2023-04-09'
+    updated = '2023-04-19'
     authors='Wolfgang Fahl'
     doc_url="https://wiki.bitplan.com/index.php/pyMetaModel"
     chat_url="https://github.com/WolfgangFahl/pyMetaModel/discussions"
     cm_url="https://github.com/WolfgangFahl/pyMetaModel"
     license=f'''Copyright 2022 contributors. All rights reserved.
   Licensed under the Apache License 2.0
   http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pymetamodel-0.3.0/scripts/genexamples` & `pymetamodel-0.3.1/scripts/genexamples`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/scripts/test` & `pymetamodel-0.3.1/scripts/test`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/tests/basemwtest.py` & `pymetamodel-0.3.1/tests/basemwtest.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/tests/basetest.py` & `pymetamodel-0.3.1/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/tests/test_linkml.py` & `pymetamodel-0.3.1/tests/test_linkml.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/tests/test_metamodel.py` & `pymetamodel-0.3.1/tests/test_metamodel.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/tests/test_mw.py` & `pymetamodel-0.3.1/tests/test_mw.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/tests/test_plantuml.py` & `pymetamodel-0.3.1/tests/test_plantuml.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/tests/test_sidif.py` & `pymetamodel-0.3.1/tests/test_sidif.py`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/.gitignore` & `pymetamodel-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/LICENSE` & `pymetamodel-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/README.md` & `pymetamodel-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/pyproject.toml` & `pymetamodel-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymetamodel-0.3.0/PKG-INFO` & `pymetamodel-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyMetaModel
-Version: 0.3.0
+Version: 0.3.1
 Project-URL: Home, https://github.com/WolfgangFahl/pyMetaModel
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/PyMetaModel
 Project-URL: Source, https://github.com/WolfgangFahl/pyMetaModel
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
```

